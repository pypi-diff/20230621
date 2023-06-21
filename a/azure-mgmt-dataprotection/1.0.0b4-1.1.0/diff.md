# Comparing `tmp/azure-mgmt-dataprotection-1.0.0b4.zip` & `tmp/azure-mgmt-dataprotection-1.1.0.zip`

## zipinfo {}

```diff
@@ -1,86 +1,84 @@
-Zip file size: 199727 bytes, number of entries: 84
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/
--rw-rw-r--  2.0 unx     5890 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/PKG-INFO
--rw-rw-r--  2.0 unx     2146 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/README.md
--rw-rw-r--  2.0 unx     2835 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/setup.py
--rw-rw-r--  2.0 unx       38 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/setup.cfg
--rw-rw-r--  2.0 unx      220 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/MANIFEST.in
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/LICENSE
--rw-rw-r--  2.0 unx     1076 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/LICENSE.txt
--rw-rw-r--  2.0 unx      666 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/_meta.json
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/CHANGELOG.md
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/
--rw-rw-r--  2.0 unx       26 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/py.typed
--rw-rw-r--  2.0 unx    77872 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_serialization.py
--rw-rw-r--  2.0 unx    10669 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_data_protection_client.py
--rw-rw-r--  2.0 unx      488 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_version.py
--rw-rw-r--  2.0 unx      900 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/__init__.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_patch.py
--rw-rw-r--  2.0 unx     3746 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_configuration.py
--rw-rw-r--  2.0 unx     8578 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_data_protection_client_enums.py
--rw-rw-r--  2.0 unx   254478 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_models_py3.py
--rw-rw-r--  2.0 unx    14185 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/
--rw-rw-r--  2.0 unx    10872 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_data_protection_client.py
--rw-rw-r--  2.0 unx      847 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_patch.py
--rw-rw-r--  2.0 unx     3794 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_configuration.py
--rw-rw-r--  2.0 unx    25440 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_dpp_resource_guard_proxy_operations.py
--rw-rw-r--  2.0 unx     5434 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_result_operations.py
--rw-rw-r--  2.0 unx   127022 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_instances_operations.py
--rw-rw-r--  2.0 unx     5512 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_export_jobs_operation_result_operations.py
--rw-rw-r--  2.0 unx     6322 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_instances_extension_routing_operations.py
--rw-rw-r--  2.0 unx    19361 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_policies_operations.py
--rw-rw-r--  2.0 unx     5693 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_vault_operation_results_operations.py
--rw-rw-r--  2.0 unx     9536 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_jobs_operations.py
--rw-rw-r--  2.0 unx     4834 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_operations.py
--rw-rw-r--  2.0 unx    10588 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_recovery_points_operations.py
--rw-rw-r--  2.0 unx     6068 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_data_protection_operations_operations.py
--rw-rw-r--  2.0 unx     9253 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_restorable_time_ranges_operations.py
--rw-rw-r--  2.0 unx     5110 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_resource_group_context_operations.py
--rw-rw-r--  2.0 unx     5288 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_backup_vault_context_operations.py
--rw-rw-r--  2.0 unx     8215 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_export_jobs_operations.py
--rw-rw-r--  2.0 unx     2882 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    77013 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_resource_guards_operations.py
--rw-rw-r--  2.0 unx    44138 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_vaults_operations.py
--rw-rw-r--  2.0 unx    15656 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_deleted_backup_instances_operations.py
--rw-rw-r--  2.0 unx     7871 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_data_protection_operations.py
--rw-rw-r--  2.0 unx    33275 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_dpp_resource_guard_proxy_operations.py
--rw-rw-r--  2.0 unx     6766 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_result_operations.py
--rw-rw-r--  2.0 unx   149511 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_instances_operations.py
--rw-rw-r--  2.0 unx     7012 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_export_jobs_operation_result_operations.py
--rw-rw-r--  2.0 unx     7283 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_instances_extension_routing_operations.py
--rw-rw-r--  2.0 unx    25303 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_policies_operations.py
--rw-rw-r--  2.0 unx     7186 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_vault_operation_results_operations.py
--rw-rw-r--  2.0 unx    12241 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_jobs_operations.py
--rw-rw-r--  2.0 unx     6165 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_operations.py
--rw-rw-r--  2.0 unx    14014 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_recovery_points_operations.py
--rw-rw-r--  2.0 unx     6795 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_data_protection_operations_operations.py
--rw-rw-r--  2.0 unx    11026 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_restorable_time_ranges_operations.py
--rw-rw-r--  2.0 unx     6474 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_resource_group_context_operations.py
--rw-rw-r--  2.0 unx     6773 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_backup_vault_context_operations.py
--rw-rw-r--  2.0 unx     9515 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_export_jobs_operations.py
--rw-rw-r--  2.0 unx     2882 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_patch.py
--rw-rw-r--  2.0 unx   102514 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_resource_guards_operations.py
--rw-rw-r--  2.0 unx    53212 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_vaults_operations.py
--rw-rw-r--  2.0 unx    19841 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_deleted_backup_instances_operations.py
--rw-rw-r--  2.0 unx     9307 b- defN 23-Jan-17 07:39 azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_data_protection_operations.py
--rw-rw-r--  2.0 unx     5890 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      116 b- defN 23-Jan-17 07:40 azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/requires.txt
-84 files, 1316439 bytes uncompressed, 178859 bytes compressed:  86.4%
+Zip file size: 193582 bytes, number of entries: 82
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure/
+-rw-rw-r--  2.0 unx     3624 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx      220 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/MANIFEST.in
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/LICENSE
+-rw-rw-r--  2.0 unx     2855 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/setup.py
+-rw-rw-r--  2.0 unx     2175 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/README.md
+-rw-rw-r--  2.0 unx     6727 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/PKG-INFO
+-rw-rw-r--  2.0 unx      660 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/_meta.json
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/setup.cfg
+-rw-rw-r--  2.0 unx     1076 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/LICENSE.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx      124 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     4048 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     6727 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/not-zip-safe
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/
+-rw-rw-r--  2.0 unx      913 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/__init__.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_serialization.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_patch.py
+-rw-rw-r--  2.0 unx      486 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_version.py
+-rw-rw-r--  2.0 unx    10285 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_data_protection_mgmt_client.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/py.typed
+-rw-rw-r--  2.0 unx     3526 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_configuration.py
+-rw-rw-r--  2.0 unx    19502 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_deleted_backup_instances_operations.py
+-rw-rw-r--  2.0 unx     2731 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/__init__.py
+-rw-rw-r--  2.0 unx   148926 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_instances_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_patch.py
+-rw-rw-r--  2.0 unx     6503 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_data_protection_operations_operations.py
+-rw-rw-r--  2.0 unx    11973 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_jobs_operations.py
+-rw-rw-r--  2.0 unx   102126 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_resource_guards_operations.py
+-rw-rw-r--  2.0 unx    25035 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_policies_operations.py
+-rw-rw-r--  2.0 unx    13746 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_recovery_points_operations.py
+-rw-rw-r--  2.0 unx     6524 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_backup_vault_context_operations.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_result_operations.py
+-rw-rw-r--  2.0 unx     9218 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_export_jobs_operations.py
+-rw-rw-r--  2.0 unx     6763 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_export_jobs_operation_result_operations.py
+-rw-rw-r--  2.0 unx     6225 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_resource_group_context_operations.py
+-rw-rw-r--  2.0 unx    10841 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_restorable_time_ranges_operations.py
+-rw-rw-r--  2.0 unx     9060 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_data_protection_operations.py
+-rw-rw-r--  2.0 unx     5869 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_operations.py
+-rw-rw-r--  2.0 unx    34708 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_dpp_resource_guard_proxy_operations.py
+-rw-rw-r--  2.0 unx    55479 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_vaults_operations.py
+-rw-rw-r--  2.0 unx     6937 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_vault_operation_results_operations.py
+-rw-rw-r--  2.0 unx    14648 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_patch.py
+-rw-rw-r--  2.0 unx     8604 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_data_protection_mgmt_client_enums.py
+-rw-rw-r--  2.0 unx   263192 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 03:09 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/
+-rw-rw-r--  2.0 unx      860 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_patch.py
+-rw-rw-r--  2.0 unx    10489 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_data_protection_mgmt_client.py
+-rw-rw-r--  2.0 unx     3574 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_configuration.py
+-rw-rw-r--  2.0 unx    15308 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_deleted_backup_instances_operations.py
+-rw-rw-r--  2.0 unx     2731 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   126392 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_instances_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     5824 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_data_protection_operations_operations.py
+-rw-rw-r--  2.0 unx     9262 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_jobs_operations.py
+-rw-rw-r--  2.0 unx    76622 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_resource_guards_operations.py
+-rw-rw-r--  2.0 unx    19081 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_policies_operations.py
+-rw-rw-r--  2.0 unx    10314 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_recovery_points_operations.py
+-rw-rw-r--  2.0 unx     5036 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_backup_vault_context_operations.py
+-rw-rw-r--  2.0 unx     5186 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_result_operations.py
+-rw-rw-r--  2.0 unx     7915 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_export_jobs_operations.py
+-rw-rw-r--  2.0 unx     5260 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_export_jobs_operation_result_operations.py
+-rw-rw-r--  2.0 unx     4858 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_resource_group_context_operations.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_restorable_time_ranges_operations.py
+-rw-rw-r--  2.0 unx     7672 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_data_protection_operations.py
+-rw-rw-r--  2.0 unx     4586 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_operations.py
+-rw-rw-r--  2.0 unx    26662 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_dpp_resource_guard_proxy_operations.py
+-rw-rw-r--  2.0 unx    46512 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_vaults_operations.py
+-rw-rw-r--  2.0 unx     5441 b- defN 23-Jun-21 03:08 azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_vault_operation_results_operations.py
+82 files, 1311960 bytes uncompressed, 173652 bytes compressed:  86.8%
```

## zipnote {}

```diff
@@ -1,253 +1,247 @@
-Filename: azure-mgmt-dataprotection-1.0.0b4/
+Filename: azure-mgmt-dataprotection-1.1.0/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/
+Filename: azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/
+Filename: azure-mgmt-dataprotection-1.1.0/azure/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/PKG-INFO
+Filename: azure-mgmt-dataprotection-1.1.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/README.md
+Filename: azure-mgmt-dataprotection-1.1.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/setup.py
+Filename: azure-mgmt-dataprotection-1.1.0/LICENSE
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/setup.cfg
+Filename: azure-mgmt-dataprotection-1.1.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/MANIFEST.in
+Filename: azure-mgmt-dataprotection-1.1.0/README.md
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/LICENSE
+Filename: azure-mgmt-dataprotection-1.1.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/LICENSE.txt
+Filename: azure-mgmt-dataprotection-1.1.0/_meta.json
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/_meta.json
+Filename: azure-mgmt-dataprotection-1.1.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/CHANGELOG.md
+Filename: azure-mgmt-dataprotection-1.1.0/LICENSE.txt
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/
+Filename: azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/__init__.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/
+Filename: azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/__init__.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/
+Filename: azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/
+Filename: azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/py.typed
+Filename: azure-mgmt-dataprotection-1.1.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_serialization.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_data_protection_client.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_version.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/__init__.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_vendor.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_patch.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_configuration.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_data_protection_client_enums.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_models_py3.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/__init__.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_version.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_patch.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_data_protection_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/py.typed
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_data_protection_client.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/__init__.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_deleted_backup_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_patch.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_configuration.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_dpp_resource_guard_proxy_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_result_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_data_protection_operations_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_instances_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_jobs_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_export_jobs_operation_result_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_resource_guards_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_instances_extension_routing_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_policies_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_recovery_points_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_vault_operation_results_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_backup_vault_context_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_jobs_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_export_jobs_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_recovery_points_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_export_jobs_operation_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_data_protection_operations_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_resource_group_context_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_restorable_time_ranges_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_restorable_time_ranges_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_resource_group_context_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_data_protection_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_backup_vault_context_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_export_jobs_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_dpp_resource_guard_proxy_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/__init__.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_vaults_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_patch.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_vault_operation_results_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_resource_guards_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_vaults_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_deleted_backup_instances_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_data_protection_mgmt_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_data_protection_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_dpp_resource_guard_proxy_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_result_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_instances_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_export_jobs_operation_result_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_data_protection_mgmt_client.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_instances_extension_routing_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_policies_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_deleted_backup_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_vault_operation_results_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_jobs_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_instances_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_recovery_points_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_data_protection_operations_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_data_protection_operations_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_jobs_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_restorable_time_ranges_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_resource_guards_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_resource_group_context_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_backup_vault_context_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_recovery_points_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_export_jobs_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_backup_vault_context_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/__init__.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_patch.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_export_jobs_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_resource_guards_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_export_jobs_operation_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_vaults_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_resource_group_context_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_deleted_backup_instances_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_restorable_time_ranges_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_data_protection_operations.py
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_data_protection_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/PKG-INFO
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/not-zip-safe
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_dpp_resource_guard_proxy_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/top_level.txt
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_vaults_operations.py
 Comment: 
 
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/dependency_links.txt
-Comment: 
-
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/SOURCES.txt
-Comment: 
-
-Filename: azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/requires.txt
+Filename: azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_vault_operation_results_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/PKG-INFO` & `azure-mgmt-dataprotection-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-dataprotection
-Version: 1.0.0b4
+Version: 1.1.0
 Summary: Microsoft Azure Data Protection Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -65,16 +65,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = DataProtectionClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Data Protection Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Data Protection Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -85,14 +86,37 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-dataprotection%2FREADME.png)
 
 
 # Release History
 
+## 1.1.0 (2023-06-16)
+
+### Features Added
+
+  - Added operation group DppResourceGuardProxyOperations
+
+## 1.0.0 (2023-02-15)
+
+### Features Added
+
+  - Model AzureBackupDiscreteRecoveryPoint has a new parameter expiry_time
+  - Model BackupVault has a new parameter feature_settings
+  - Model PatchBackupVaultInput has a new parameter feature_settings
+  - Model TargetDetails has a new parameter target_resource_arm_id
+
+### Breaking Changes
+
+  - Client name is changed from `DataProtectionClient` to `DataProtectionMgmtClient`
+  - Model ResourceGuardResource no longer has parameter identity
+  - Removed operation group BackupInstancesExtensionRoutingOperations
+  - Removed operation group DppResourceGuardProxyOperations
+  - Renamed operation BackupVaultsOperations.delete to BackupVaultsOperations.begin_delete
+
 ## 1.0.0b4 (2023-01-17)
 
 ### Features Added
 
   - Added operation group BackupInstancesExtensionRoutingOperations
   - Added operation group DppResourceGuardProxyOperations
   - Model PolicyParameters has a new parameter backup_datasource_parameters_list
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/README.md` & `azure-mgmt-dataprotection-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = DataProtectionClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Data Protection Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Data Protection Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/setup.py` & `azure-mgmt-dataprotection-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 #!/usr/bin/env python
 
-#-------------------------------------------------------------------------
+# -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
-#--------------------------------------------------------------------------
+# --------------------------------------------------------------------------
 
 import re
 import os.path
 from io import open
 from setuptools import find_packages, setup
 
 # Change the PACKAGE_NAME only to change folder and different name
 PACKAGE_NAME = "azure-mgmt-dataprotection"
 PACKAGE_PPRINT_NAME = "Data Protection Management"
 
 # a-b-c => a/b/c
-package_folder_path = PACKAGE_NAME.replace('-', '/')
+package_folder_path = PACKAGE_NAME.replace("-", "/")
 # a-b-c => a.b.c
-namespace_name = PACKAGE_NAME.replace('-', '.')
+namespace_name = PACKAGE_NAME.replace("-", ".")
 
 # Version extraction inspired from 'requests'
-with open(os.path.join(package_folder_path, 'version.py')
-          if os.path.exists(os.path.join(package_folder_path, 'version.py'))
-          else os.path.join(package_folder_path, '_version.py'), 'r') as fd:
-    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
-                        fd.read(), re.MULTILINE).group(1)
+with open(
+    os.path.join(package_folder_path, "version.py")
+    if os.path.exists(os.path.join(package_folder_path, "version.py"))
+    else os.path.join(package_folder_path, "_version.py"),
+    "r",
+) as fd:
+    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
 
 if not version:
-    raise RuntimeError('Cannot find version information')
+    raise RuntimeError("Cannot find version information")
 
-with open('README.md', encoding='utf-8') as f:
+with open("README.md", encoding="utf-8") as f:
     readme = f.read()
-with open('CHANGELOG.md', encoding='utf-8') as f:
+with open("CHANGELOG.md", encoding="utf-8") as f:
     changelog = f.read()
 
 setup(
     name=PACKAGE_NAME,
     version=version,
-    description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
-    long_description=readme + '\n\n' + changelog,
-    long_description_content_type='text/markdown',
-    license='MIT License',
-    author='Microsoft Corporation',
-    author_email='azpysdkhelp@microsoft.com',
-    url='https://github.com/Azure/azure-sdk-for-python',
+    description="Microsoft Azure {} Client Library for Python".format(PACKAGE_PPRINT_NAME),
+    long_description=readme + "\n\n" + changelog,
+    long_description_content_type="text/markdown",
+    license="MIT License",
+    author="Microsoft Corporation",
+    author_email="azpysdkhelp@microsoft.com",
+    url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'License :: OSI Approved :: MIT License',
+        "Development Status :: 4 - Beta",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
-    packages=find_packages(exclude=[
-        'tests',
-        # Exclude packages that will be covered by PEP420 or nspkg
-        'azure',
-        'azure.mgmt',
-    ]),
+    packages=find_packages(
+        exclude=[
+            "tests",
+            # Exclude packages that will be covered by PEP420 or nspkg
+            "azure",
+            "azure.mgmt",
+        ]
+    ),
     include_package_data=True,
     package_data={
-        'pytyped': ['py.typed'],
+        "pytyped": ["py.typed"],
     },
     install_requires=[
-        "msrest>=0.7.1",
+        "isodate<1.0.0,>=0.6.1",
         "azure-common~=1.1",
         "azure-mgmt-core>=1.3.2,<2.0.0",
         "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.7",
 )
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/LICENSE` & `azure-mgmt-dataprotection-1.1.0/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dataprotection-1.0.0b4/LICENSE.txt` & `azure-mgmt-dataprotection-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dataprotection-1.0.0b4/_meta.json` & `azure-mgmt-dataprotection-1.1.0/_meta.json`

 * *Files 7% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/dataprotection/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--tag=package-2023-01 --use=@autorest/python@6.4.12 '*

 * *                       '--use=@autorest/modelerfour@4.24.3 --version=3.9.2 '*

 * *                       "--version-tolerant=False'",*

 * * "'commit'": "'0cfd102 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/dataprotection/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --tag=package-preview-2022-11 --use=@autorest/python@6.2.7 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "24f2c762b5a3ce6bd476dfe204409bb6ed59ed3d",
+    "autorest_command": "autorest specification/dataprotection/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --tag=package-2023-01 --use=@autorest/python@6.4.12 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "0cfd102a6ecb172f04ec915732bd8ca6f6b2a7af",
     "readme": "specification/dataprotection/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.2.7",
+        "@autorest/python@6.4.12",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/CHANGELOG.md` & `azure-mgmt-dataprotection-1.1.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Release History
 
+## 1.1.0 (2023-06-16)
+
+### Features Added
+
+  - Added operation group DppResourceGuardProxyOperations
+
+## 1.0.0 (2023-02-15)
+
+### Features Added
+
+  - Model AzureBackupDiscreteRecoveryPoint has a new parameter expiry_time
+  - Model BackupVault has a new parameter feature_settings
+  - Model PatchBackupVaultInput has a new parameter feature_settings
+  - Model TargetDetails has a new parameter target_resource_arm_id
+
+### Breaking Changes
+
+  - Client name is changed from `DataProtectionClient` to `DataProtectionMgmtClient`
+  - Model ResourceGuardResource no longer has parameter identity
+  - Removed operation group BackupInstancesExtensionRoutingOperations
+  - Removed operation group DppResourceGuardProxyOperations
+  - Renamed operation BackupVaultsOperations.delete to BackupVaultsOperations.begin_delete
+
 ## 1.0.0b4 (2023-01-17)
 
 ### Features Added
 
   - Added operation group BackupInstancesExtensionRoutingOperations
   - Added operation group DppResourceGuardProxyOperations
   - Model PolicyParameters has a new parameter backup_datasource_parameters_list
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_serialization.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,47 @@
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
-from typing import Optional, Union, AnyStr, IO, Mapping
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from typing import Dict, Any, cast
-
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
+
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
@@ -273,43 +290,43 @@
     serialization and deserialization.
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
             cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
@@ -318,30 +335,35 @@
         try:
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -380,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -514,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -530,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -598,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -622,16 +649,15 @@
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
@@ -652,16 +678,16 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
@@ -773,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -1157,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1238,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1262,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1328,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1348,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1467,40 +1496,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_data_protection_client.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_data_protection_mgmt_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
 from . import models as _models
-from ._configuration import DataProtectionClientConfiguration
+from ._configuration import DataProtectionMgmtClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
-    BackupInstancesExtensionRoutingOperations,
     BackupInstancesOperations,
     BackupPoliciesOperations,
     BackupVaultOperationResultsOperations,
     BackupVaultsOperations,
     DataProtectionOperations,
     DataProtectionOperationsOperations,
     DeletedBackupInstancesOperations,
@@ -38,15 +37,15 @@
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class DataProtectionClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+class DataProtectionMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Open API 2.0 Specs for Azure Data Protection service.
 
     :ivar backup_vaults: BackupVaultsOperations operations
     :vartype backup_vaults: azure.mgmt.dataprotection.operations.BackupVaultsOperations
     :ivar operation_result: OperationResultOperations operations
     :vartype operation_result: azure.mgmt.dataprotection.operations.OperationResultOperations
     :ivar operation_status: OperationStatusOperations operations
@@ -67,17 +66,14 @@
     :ivar data_protection_operations: DataProtectionOperationsOperations operations
     :vartype data_protection_operations:
      azure.mgmt.dataprotection.operations.DataProtectionOperationsOperations
     :ivar backup_policies: BackupPoliciesOperations operations
     :vartype backup_policies: azure.mgmt.dataprotection.operations.BackupPoliciesOperations
     :ivar backup_instances: BackupInstancesOperations operations
     :vartype backup_instances: azure.mgmt.dataprotection.operations.BackupInstancesOperations
-    :ivar backup_instances_extension_routing: BackupInstancesExtensionRoutingOperations operations
-    :vartype backup_instances_extension_routing:
-     azure.mgmt.dataprotection.operations.BackupInstancesExtensionRoutingOperations
     :ivar recovery_points: RecoveryPointsOperations operations
     :vartype recovery_points: azure.mgmt.dataprotection.operations.RecoveryPointsOperations
     :ivar jobs: JobsOperations operations
     :vartype jobs: azure.mgmt.dataprotection.operations.JobsOperations
     :ivar restorable_time_ranges: RestorableTimeRangesOperations operations
     :vartype restorable_time_ranges:
      azure.mgmt.dataprotection.operations.RestorableTimeRangesOperations
@@ -92,36 +88,36 @@
     :ivar resource_guards: ResourceGuardsOperations operations
     :vartype resource_guards: azure.mgmt.dataprotection.operations.ResourceGuardsOperations
     :ivar dpp_resource_guard_proxy: DppResourceGuardProxyOperations operations
     :vartype dpp_resource_guard_proxy:
      azure.mgmt.dataprotection.operations.DppResourceGuardProxyOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The subscription Id. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = DataProtectionClientConfiguration(
+        self._config = DataProtectionMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.backup_vaults = BackupVaultsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operation_result = OperationResultOperations(
@@ -143,17 +139,14 @@
         self.data_protection_operations = DataProtectionOperationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.backup_policies = BackupPoliciesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.backup_instances = BackupInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.backup_instances_extension_routing = BackupInstancesExtensionRoutingOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.recovery_points = RecoveryPointsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.jobs = JobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.restorable_time_ranges = RestorableTimeRangesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.export_jobs = ExportJobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.export_jobs_operation_result = ExportJobsOperationResultOperations(
@@ -188,13 +181,13 @@
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
     def close(self) -> None:
         self._client.close()
 
-    def __enter__(self) -> "DataProtectionClient":
+    def __enter__(self) -> "DataProtectionMgmtClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/__init__.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._data_protection_client import DataProtectionClient
-from ._version import VERSION
-
-__version__ = VERSION
+from ._data_protection_mgmt_client import DataProtectionMgmtClient
 
 try:
     from ._patch import __all__ as _patch_all
     from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "DataProtectionClient",
+    "DataProtectionMgmtClient",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_vendor.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_vendor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from typing import List, cast
+
 from azure.core.pipeline.transport import HttpRequest
 
 
 def _convert_request(request, files=None):
     data = request.content if not files else None
     request = HttpRequest(method=request.method, url=request.url, headers=request.headers, data=data)
     if files:
@@ -18,10 +20,11 @@
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_patch.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/_configuration.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/_configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,51 +2,45 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class DataProtectionClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for DataProtectionClient.
+class DataProtectionMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for DataProtectionMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The subscription Id. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(DataProtectionClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop("api_version", "2022-11-01-preview")
+        super(DataProtectionMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2023-01-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_data_protection_client_enums.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_data_protection_mgmt_client_enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
 
 
+class CrossSubscriptionRestoreState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """CrossSubscriptionRestore state."""
+
+    DISABLED = "Disabled"
+    PERMANENTLY_DISABLED = "PermanentlyDisabled"
+    ENABLED = "Enabled"
+
+
 class CurrentProtectionState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Specifies the current protection state of the resource."""
 
     INVALID = "Invalid"
     NOT_PROTECTED = "NotProtected"
     CONFIGURING_PROTECTION = "ConfiguringProtection"
     PROTECTION_CONFIGURED = "ProtectionConfigured"
@@ -122,16 +130,16 @@
     MAY = "May"
     NOVEMBER = "November"
     OCTOBER = "October"
     SEPTEMBER = "September"
 
 
 class PersistentVolumeRestoreMode(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Gets or sets the PV Restore Mode property. This property sets whether volumes needs to be
-    restored.
+    """Gets or sets the PV (Persistent Volume) Restore Mode property. This property sets whether
+    volumes needs to be restored.
     """
 
     RESTORE_WITH_VOLUME_DATA = "RestoreWithVolumeData"
     RESTORE_WITHOUT_VOLUME_DATA = "RestoreWithoutVolumeData"
 
 
 class ProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
@@ -164,24 +172,14 @@
     CREATE_IN_PROGRESS = "CREATE_IN_PROGRESS"
     COMPLETED = "COMPLETED"
     DELETE_IN_PROGRESS = "DELETE_IN_PROGRESS"
     DELETED = "DELETED"
     FAILED = "FAILED"
 
 
-class ResourceGuardProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """Provisioning state of the BackupVault resource."""
-
-    FAILED = "Failed"
-    PROVISIONING = "Provisioning"
-    SUCCEEDED = "Succeeded"
-    UNKNOWN = "Unknown"
-    UPDATING = "Updating"
-
-
 class ResourceMoveState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Resource move state for backup vault."""
 
     UNKNOWN = "Unknown"
     IN_PROGRESS = "InProgress"
     PREPARE_FAILED = "PrepareFailed"
     COMMIT_FAILED = "CommitFailed"
@@ -218,27 +216,28 @@
     INVALID = "Invalid"
     AZURE_KEY_VAULT = "AzureKeyVault"
 
 
 class SoftDeleteState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """State of soft delete."""
 
-    #: Soft Delete is turned off for the BackupVault
     OFF = "Off"
-    #: Soft Delete is enabled for the BackupVault but can be turned off
+    """Soft Delete is turned off for the BackupVault"""
     ON = "On"
-    #: Soft Delete is permanently enabled for the BackupVault and the setting cannot be changed
+    """Soft Delete is enabled for the BackupVault but can be turned off"""
     ALWAYS_ON = "AlwaysOn"
+    """Soft Delete is permanently enabled for the BackupVault and the setting cannot be changed"""
 
 
 class SourceDataStoreType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Gets or sets the type of the source data store."""
 
     ARCHIVE_STORE = "ArchiveStore"
     SNAPSHOT_STORE = "SnapshotStore"
+    OPERATIONAL_STORE = "OperationalStore"
     VAULT_STORE = "VaultStore"
 
 
 class Status(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Specifies the protection status of the resource."""
 
     CONFIGURING_PROTECTION = "ConfiguringProtection"
@@ -249,15 +248,15 @@
     SOFT_DELETING = "SoftDeleting"
 
 
 class StorageSettingStoreTypes(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Gets or sets the type of the datastore."""
 
     ARCHIVE_STORE = "ArchiveStore"
-    SNAPSHOT_STORE = "SnapshotStore"
+    OPERATIONAL_STORE = "OperationalStore"
     VAULT_STORE = "VaultStore"
 
 
 class StorageSettingTypes(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Gets or sets the type."""
 
     GEO_REDUNDANT = "GeoRedundant"
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_models_py3.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_models_py3.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-from typing import Dict, List, Optional, TYPE_CHECKING, Union
+from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
@@ -39,15 +39,15 @@
     _attribute_map = {
         "duration": {"key": "duration", "type": "str"},
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"AbsoluteDeleteOption": "AbsoluteDeleteOption"}}
 
-    def __init__(self, *, duration: str, **kwargs):
+    def __init__(self, *, duration: str, **kwargs: Any) -> None:
         """
         :keyword duration: Duration of deletion after given timespan. Required.
         :paramtype duration: str
         """
         super().__init__(**kwargs)
         self.duration = duration
         self.object_type: Optional[str] = None
@@ -70,15 +70,15 @@
     }
 
     _attribute_map = {
         "duration": {"key": "duration", "type": "str"},
         "object_type": {"key": "objectType", "type": "str"},
     }
 
-    def __init__(self, *, duration: str, **kwargs):
+    def __init__(self, *, duration: str, **kwargs: Any) -> None:
         """
         :keyword duration: Duration of deletion after given timespan. Required.
         :paramtype duration: str
         """
         super().__init__(duration=duration, **kwargs)
         self.object_type: str = "AbsoluteDeleteOption"
 
@@ -100,15 +100,15 @@
     }
 
     _attribute_map = {
         "rule_name": {"key": "ruleName", "type": "str"},
         "trigger_option": {"key": "triggerOption", "type": "AdhocBackupTriggerOption"},
     }
 
-    def __init__(self, *, rule_name: str, trigger_option: "_models.AdhocBackupTriggerOption", **kwargs):
+    def __init__(self, *, rule_name: str, trigger_option: "_models.AdhocBackupTriggerOption", **kwargs: Any) -> None:
         """
         :keyword rule_name: Required.
         :paramtype rule_name: str
         :keyword trigger_option: Adhoc backup trigger option. Required.
         :paramtype trigger_option: ~azure.mgmt.dataprotection.models.AdhocBackupTriggerOption
         """
         super().__init__(**kwargs)
@@ -123,15 +123,15 @@
     :vartype retention_tag_override: str
     """
 
     _attribute_map = {
         "retention_tag_override": {"key": "retentionTagOverride", "type": "str"},
     }
 
-    def __init__(self, *, retention_tag_override: Optional[str] = None, **kwargs):
+    def __init__(self, *, retention_tag_override: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword retention_tag_override:
         :paramtype retention_tag_override: str
         """
         super().__init__(**kwargs)
         self.retention_tag_override = retention_tag_override
 
@@ -143,15 +143,15 @@
     :vartype tag_info: ~azure.mgmt.dataprotection.models.RetentionTag
     """
 
     _attribute_map = {
         "tag_info": {"key": "tagInfo", "type": "RetentionTag"},
     }
 
-    def __init__(self, *, tag_info: Optional["_models.RetentionTag"] = None, **kwargs):
+    def __init__(self, *, tag_info: Optional["_models.RetentionTag"] = None, **kwargs: Any) -> None:
         """
         :keyword tag_info: Retention tag information.
         :paramtype tag_info: ~azure.mgmt.dataprotection.models.RetentionTag
         """
         super().__init__(**kwargs)
         self.tag_info = tag_info
 
@@ -179,15 +179,15 @@
     _subtype_map = {
         "object_type": {
             "AdhocBasedTriggerContext": "AdhocBasedTriggerContext",
             "ScheduleBasedTriggerContext": "ScheduleBasedTriggerContext",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class AdhocBasedTriggerContext(TriggerContext):
     """Adhoc trigger context.
@@ -206,15 +206,15 @@
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "tagging_criteria": {"key": "taggingCriteria", "type": "AdhocBasedTaggingCriteria"},
     }
 
-    def __init__(self, *, tagging_criteria: "_models.AdhocBasedTaggingCriteria", **kwargs):
+    def __init__(self, *, tagging_criteria: "_models.AdhocBasedTaggingCriteria", **kwargs: Any) -> None:
         """
         :keyword tagging_criteria: Tagging Criteria containing retention tag for adhoc backup.
          Required.
         :paramtype tagging_criteria: ~azure.mgmt.dataprotection.models.AdhocBasedTaggingCriteria
         """
         super().__init__(**kwargs)
         self.object_type: str = "AdhocBasedTriggerContext"
@@ -239,15 +239,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"SecretStoreBasedAuthCredentials": "SecretStoreBasedAuthCredentials"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class AzureBackupRecoveryPoint(_serialization.Model):
     """Azure backup recoveryPoint.
@@ -267,23 +267,25 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"AzureBackupDiscreteRecoveryPoint": "AzureBackupDiscreteRecoveryPoint"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
-class AzureBackupDiscreteRecoveryPoint(AzureBackupRecoveryPoint):
+class AzureBackupDiscreteRecoveryPoint(AzureBackupRecoveryPoint):  # pylint: disable=too-many-instance-attributes
     """Azure backup discrete RecoveryPoint.
 
+    Variables are only populated by the server, and will be ignored when sending a request.
+
     All required parameters must be populated in order to send to Azure.
 
     :ivar object_type: Required.
     :vartype object_type: str
     :ivar friendly_name:
     :vartype friendly_name: str
     :ivar recovery_point_data_stores_details:
@@ -299,19 +301,22 @@
     :vartype recovery_point_id: str
     :ivar recovery_point_type:
     :vartype recovery_point_type: str
     :ivar retention_tag_name:
     :vartype retention_tag_name: str
     :ivar retention_tag_version:
     :vartype retention_tag_version: str
+    :ivar expiry_time:
+    :vartype expiry_time: ~datetime.datetime
     """
 
     _validation = {
         "object_type": {"required": True},
         "recovery_point_time": {"required": True},
+        "expiry_time": {"readonly": True},
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "friendly_name": {"key": "friendlyName", "type": "str"},
         "recovery_point_data_stores_details": {
             "key": "recoveryPointDataStoresDetails",
@@ -320,30 +325,31 @@
         "recovery_point_time": {"key": "recoveryPointTime", "type": "iso-8601"},
         "policy_name": {"key": "policyName", "type": "str"},
         "policy_version": {"key": "policyVersion", "type": "str"},
         "recovery_point_id": {"key": "recoveryPointId", "type": "str"},
         "recovery_point_type": {"key": "recoveryPointType", "type": "str"},
         "retention_tag_name": {"key": "retentionTagName", "type": "str"},
         "retention_tag_version": {"key": "retentionTagVersion", "type": "str"},
+        "expiry_time": {"key": "expiryTime", "type": "iso-8601"},
     }
 
     def __init__(
         self,
         *,
         recovery_point_time: datetime.datetime,
         friendly_name: Optional[str] = None,
         recovery_point_data_stores_details: Optional[List["_models.RecoveryPointDataStoreDetails"]] = None,
         policy_name: Optional[str] = None,
         policy_version: Optional[str] = None,
         recovery_point_id: Optional[str] = None,
         recovery_point_type: Optional[str] = None,
         retention_tag_name: Optional[str] = None,
         retention_tag_version: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword friendly_name:
         :paramtype friendly_name: str
         :keyword recovery_point_data_stores_details:
         :paramtype recovery_point_data_stores_details:
          list[~azure.mgmt.dataprotection.models.RecoveryPointDataStoreDetails]
         :keyword recovery_point_time: Required.
@@ -368,14 +374,15 @@
         self.recovery_point_time = recovery_point_time
         self.policy_name = policy_name
         self.policy_version = policy_version
         self.recovery_point_id = recovery_point_id
         self.recovery_point_type = recovery_point_type
         self.retention_tag_name = retention_tag_name
         self.retention_tag_version = retention_tag_version
+        self.expiry_time = None
 
 
 class AzureBackupFindRestorableTimeRangesRequest(_serialization.Model):
     """List Restore Ranges Request.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -401,16 +408,16 @@
 
     def __init__(
         self,
         *,
         source_data_store_type: Union[str, "_models.RestoreSourceDataStoreType"],
         start_time: Optional[str] = None,
         end_time: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword source_data_store_type: Gets or sets the type of the source data store. Required.
          Known values are: "OperationalStore", "VaultStore", and "ArchiveStore".
         :paramtype source_data_store_type: str or
          ~azure.mgmt.dataprotection.models.RestoreSourceDataStoreType
         :keyword start_time: Start time for the List Restore Ranges request. ISO 8601 format.
         :paramtype start_time: str
@@ -459,16 +466,16 @@
         subscription_id: Optional[str] = None,
         uri: Optional[str] = None,
         headers: Optional[Dict[str, List[str]]] = None,
         supported_group_versions: Optional[List[str]] = None,
         culture_info: Optional[str] = None,
         parameters: Optional[Dict[str, str]] = None,
         http_method: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword subscription_id:
         :paramtype subscription_id: str
         :keyword uri:
         :paramtype uri: str
         :keyword headers: Dictionary of
          <components·ikn5y4·schemas·dppworkerrequest·properties·headers·additionalproperties>.
@@ -532,16 +539,16 @@
         uri: Optional[str] = None,
         headers: Optional[Dict[str, List[str]]] = None,
         supported_group_versions: Optional[List[str]] = None,
         culture_info: Optional[str] = None,
         parameters: Optional[Dict[str, str]] = None,
         http_method: Optional[str] = None,
         content: Optional["_models.AzureBackupFindRestorableTimeRangesRequest"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword subscription_id:
         :paramtype subscription_id: str
         :keyword uri:
         :paramtype uri: str
         :keyword headers: Dictionary of
          <components·ikn5y4·schemas·dppworkerrequest·properties·headers·additionalproperties>.
@@ -586,16 +593,16 @@
     }
 
     def __init__(
         self,
         *,
         restorable_time_ranges: Optional[List["_models.RestorableTimeRange"]] = None,
         object_type: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword restorable_time_ranges: Returns the Restore Ranges available on the Backup Instance.
         :paramtype restorable_time_ranges: list[~azure.mgmt.dataprotection.models.RestorableTimeRange]
         :keyword object_type:
         :paramtype object_type: str
         """
         super().__init__(**kwargs)
@@ -629,15 +636,15 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.system_data = None
 
@@ -672,15 +679,17 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "AzureBackupFindRestorableTimeRangesResponse"},
     }
 
-    def __init__(self, *, properties: Optional["_models.AzureBackupFindRestorableTimeRangesResponse"] = None, **kwargs):
+    def __init__(
+        self, *, properties: Optional["_models.AzureBackupFindRestorableTimeRangesResponse"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword properties: AzureBackupFindRestorableTimeRangesResponseResource properties.
         :paramtype properties:
          ~azure.mgmt.dataprotection.models.AzureBackupFindRestorableTimeRangesResponse
         """
         super().__init__(**kwargs)
         self.properties = properties
@@ -842,16 +851,16 @@
         supported_actions: List[str],
         vault_name: str,
         data_source_set_name: Optional[str] = None,
         duration: Optional[str] = None,
         etag: Optional[str] = None,
         source_data_store_name: Optional[str] = None,
         destination_data_store_name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword activity_id: Job Activity Id. Required.
         :paramtype activity_id: str
         :keyword backup_instance_friendly_name: Name of the Backup Instance. Required.
         :paramtype backup_instance_friendly_name: str
         :keyword data_source_id: ARM ID of the DataSource. Required.
         :paramtype data_source_id: str
@@ -960,15 +969,15 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "AzureBackupJob"},
     }
 
-    def __init__(self, *, properties: Optional["_models.AzureBackupJob"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.AzureBackupJob"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: AzureBackupJobResource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.AzureBackupJob
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -981,15 +990,15 @@
     :vartype next_link: str
     """
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, next_link: Optional[str] = None, **kwargs):
+    def __init__(self, *, next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.next_link = next_link
@@ -1011,16 +1020,16 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.AzureBackupJobResource"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.AzureBackupJobResource]
         """
@@ -1046,15 +1055,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"AzureBackupParams": "AzureBackupParams"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class AzureBackupParams(BackupParameters):
     """Azure backup parameters.
@@ -1073,15 +1082,15 @@
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "backup_type": {"key": "backupType", "type": "str"},
     }
 
-    def __init__(self, *, backup_type: str, **kwargs):
+    def __init__(self, *, backup_type: str, **kwargs: Any) -> None:
         """
         :keyword backup_type: BackupType ; Full/Incremental etc. Required.
         :paramtype backup_type: str
         """
         super().__init__(**kwargs)
         self.object_type: str = "AzureBackupParams"
         self.backup_type = backup_type
@@ -1096,15 +1105,15 @@
     All required parameters must be populated in order to send to Azure.
 
     :ivar object_type: Required.
     :vartype object_type: str
     :ivar restore_target_info: Gets or sets the restore target information. Required.
     :vartype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
     :ivar source_data_store_type: Gets or sets the type of the source data store. Required. Known
-     values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+     values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
     :vartype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
     :ivar source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which is
      being recovered.
     :vartype source_resource_id: str
     """
 
     _validation = {
@@ -1129,21 +1138,21 @@
 
     def __init__(
         self,
         *,
         restore_target_info: "_models.RestoreTargetInfoBase",
         source_data_store_type: Union[str, "_models.SourceDataStoreType"],
         source_resource_id: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword restore_target_info: Gets or sets the restore target information. Required.
         :paramtype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
         :keyword source_data_store_type: Gets or sets the type of the source data store. Required.
-         Known values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+         Known values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
         :paramtype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
         :keyword source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which
          is being recovered.
         :paramtype source_resource_id: str
         """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
@@ -1161,15 +1170,15 @@
     All required parameters must be populated in order to send to Azure.
 
     :ivar object_type: Required.
     :vartype object_type: str
     :ivar restore_target_info: Gets or sets the restore target information. Required.
     :vartype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
     :ivar source_data_store_type: Gets or sets the type of the source data store. Required. Known
-     values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+     values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
     :vartype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
     :ivar source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which is
      being recovered.
     :vartype source_resource_id: str
     :ivar recovery_point_id: Required.
     :vartype recovery_point_id: str
     """
@@ -1196,21 +1205,21 @@
     def __init__(
         self,
         *,
         restore_target_info: "_models.RestoreTargetInfoBase",
         source_data_store_type: Union[str, "_models.SourceDataStoreType"],
         recovery_point_id: str,
         source_resource_id: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword restore_target_info: Gets or sets the restore target information. Required.
         :paramtype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
         :keyword source_data_store_type: Gets or sets the type of the source data store. Required.
-         Known values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+         Known values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
         :paramtype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
         :keyword source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which
          is being recovered.
         :paramtype source_resource_id: str
         :keyword recovery_point_id: Required.
         :paramtype recovery_point_id: str
         """
@@ -1253,15 +1262,15 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "AzureBackupRecoveryPoint"},
     }
 
-    def __init__(self, *, properties: Optional["_models.AzureBackupRecoveryPoint"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.AzureBackupRecoveryPoint"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: AzureBackupRecoveryPointResource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.AzureBackupRecoveryPoint
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -1282,16 +1291,16 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.AzureBackupRecoveryPointResource"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.AzureBackupRecoveryPointResource]
         """
@@ -1305,15 +1314,15 @@
     All required parameters must be populated in order to send to Azure.
 
     :ivar object_type: Required.
     :vartype object_type: str
     :ivar restore_target_info: Gets or sets the restore target information. Required.
     :vartype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
     :ivar source_data_store_type: Gets or sets the type of the source data store. Required. Known
-     values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+     values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
     :vartype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
     :ivar source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which is
      being recovered.
     :vartype source_resource_id: str
     :ivar recovery_point_time: The recovery time in ISO 8601 format example -
      2020-08-14T17:30:00.0000000Z. Required.
     :vartype recovery_point_time: str
@@ -1337,21 +1346,21 @@
     def __init__(
         self,
         *,
         restore_target_info: "_models.RestoreTargetInfoBase",
         source_data_store_type: Union[str, "_models.SourceDataStoreType"],
         recovery_point_time: str,
         source_resource_id: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword restore_target_info: Gets or sets the restore target information. Required.
         :paramtype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
         :keyword source_data_store_type: Gets or sets the type of the source data store. Required.
-         Known values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+         Known values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
         :paramtype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
         :keyword source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which
          is being recovered.
         :paramtype source_resource_id: str
         :keyword recovery_point_time: The recovery time in ISO 8601 format example -
          2020-08-14T17:30:00.0000000Z. Required.
         :paramtype recovery_point_time: str
@@ -1394,16 +1403,16 @@
 
     def __init__(
         self,
         *,
         recovery_point_id: str,
         rehydration_retention_duration: str,
         rehydration_priority: Optional[Union[str, "_models.RehydrationPriority"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword recovery_point_id: Id of the recovery point to be recovered. Required.
         :paramtype recovery_point_id: str
         :keyword rehydration_priority: Priority to be used for rehydration. Values High or Standard.
          Known values are: "Invalid", "High", and "Standard".
         :paramtype rehydration_priority: str or ~azure.mgmt.dataprotection.models.RehydrationPriority
         :keyword rehydration_retention_duration: Retention duration in ISO 8601 format i.e P10D .
@@ -1422,15 +1431,15 @@
     All required parameters must be populated in order to send to Azure.
 
     :ivar object_type: Required.
     :vartype object_type: str
     :ivar restore_target_info: Gets or sets the restore target information. Required.
     :vartype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
     :ivar source_data_store_type: Gets or sets the type of the source data store. Required. Known
-     values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+     values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
     :vartype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
     :ivar source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which is
      being recovered.
     :vartype source_resource_id: str
     :ivar recovery_point_id: Required.
     :vartype recovery_point_id: str
     :ivar rehydration_priority: Priority to be used for rehydration. Values High or Standard.
@@ -1465,21 +1474,21 @@
         *,
         restore_target_info: "_models.RestoreTargetInfoBase",
         source_data_store_type: Union[str, "_models.SourceDataStoreType"],
         recovery_point_id: str,
         rehydration_priority: Union[str, "_models.RehydrationPriority"],
         rehydration_retention_duration: str,
         source_resource_id: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword restore_target_info: Gets or sets the restore target information. Required.
         :paramtype restore_target_info: ~azure.mgmt.dataprotection.models.RestoreTargetInfoBase
         :keyword source_data_store_type: Gets or sets the type of the source data store. Required.
-         Known values are: "ArchiveStore", "SnapshotStore", and "VaultStore".
+         Known values are: "ArchiveStore", "SnapshotStore", "OperationalStore", and "VaultStore".
         :paramtype source_data_store_type: str or ~azure.mgmt.dataprotection.models.SourceDataStoreType
         :keyword source_resource_id: Fully qualified Azure Resource Manager ID of the datasource which
          is being recovered.
         :paramtype source_resource_id: str
         :keyword recovery_point_id: Required.
         :paramtype recovery_point_id: str
         :keyword rehydration_priority: Priority to be used for rehydration. Values High or Standard.
@@ -1523,15 +1532,15 @@
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"AzureBackupRule": "AzureBackupRule", "AzureRetentionRule": "AzureRetentionRule"}}
 
-    def __init__(self, *, name: str, **kwargs):
+    def __init__(self, *, name: str, **kwargs: Any) -> None:
         """
         :keyword name: Required.
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.name = name
         self.object_type: Optional[str] = None
@@ -1572,16 +1581,16 @@
     def __init__(
         self,
         *,
         name: str,
         data_store: "_models.DataStoreInfoBase",
         trigger: "_models.TriggerContext",
         backup_parameters: Optional["_models.BackupParameters"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Required.
         :paramtype name: str
         :keyword backup_parameters: BackupParameters base.
         :paramtype backup_parameters: ~azure.mgmt.dataprotection.models.BackupParameters
         :keyword data_store: DataStoreInfo base. Required.
         :paramtype data_store: ~azure.mgmt.dataprotection.models.DataStoreInfoBase
@@ -1602,15 +1611,17 @@
     :vartype alerts_for_all_job_failures: str or ~azure.mgmt.dataprotection.models.AlertsState
     """
 
     _attribute_map = {
         "alerts_for_all_job_failures": {"key": "alertsForAllJobFailures", "type": "str"},
     }
 
-    def __init__(self, *, alerts_for_all_job_failures: Optional[Union[str, "_models.AlertsState"]] = None, **kwargs):
+    def __init__(
+        self, *, alerts_for_all_job_failures: Optional[Union[str, "_models.AlertsState"]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword alerts_for_all_job_failures: Known values are: "Enabled" and "Disabled".
         :paramtype alerts_for_all_job_failures: str or ~azure.mgmt.dataprotection.models.AlertsState
         """
         super().__init__(**kwargs)
         self.alerts_for_all_job_failures = alerts_for_all_job_failures
 
@@ -1638,15 +1649,15 @@
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "data_store_type": {"key": "dataStoreType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"AzureOperationalStoreParameters": "AzureOperationalStoreParameters"}}
 
-    def __init__(self, *, data_store_type: Union[str, "_models.DataStoreTypes"], **kwargs):
+    def __init__(self, *, data_store_type: Union[str, "_models.DataStoreTypes"], **kwargs: Any) -> None:
         """
         :keyword data_store_type: type of datastore; Operational/Vault/Archive. Required. Known values
          are: "OperationalStore", "VaultStore", and "ArchiveStore".
         :paramtype data_store_type: str or ~azure.mgmt.dataprotection.models.DataStoreTypes
         """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
@@ -1679,16 +1690,16 @@
     }
 
     def __init__(
         self,
         *,
         data_store_type: Union[str, "_models.DataStoreTypes"],
         resource_group_id: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword data_store_type: type of datastore; Operational/Vault/Archive. Required. Known values
          are: "OperationalStore", "VaultStore", and "ArchiveStore".
         :paramtype data_store_type: str or ~azure.mgmt.dataprotection.models.DataStoreTypes
         :keyword resource_group_id: Gets or sets the Snapshot Resource Group Uri.
         :paramtype resource_group_id: str
         """
@@ -1722,16 +1733,21 @@
         "name": {"key": "name", "type": "str"},
         "object_type": {"key": "objectType", "type": "str"},
         "is_default": {"key": "isDefault", "type": "bool"},
         "lifecycles": {"key": "lifecycles", "type": "[SourceLifeCycle]"},
     }
 
     def __init__(
-        self, *, name: str, lifecycles: List["_models.SourceLifeCycle"], is_default: Optional[bool] = None, **kwargs
-    ):
+        self,
+        *,
+        name: str,
+        lifecycles: List["_models.SourceLifeCycle"],
+        is_default: Optional[bool] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Required.
         :paramtype name: str
         :keyword is_default:
         :paramtype is_default: bool
         :keyword lifecycles: Required.
         :paramtype lifecycles: list[~azure.mgmt.dataprotection.models.SourceLifeCycle]
@@ -1760,15 +1776,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"ScheduleBasedBackupCriteria": "ScheduleBasedBackupCriteria"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class BackupDatasourceParameters(_serialization.Model):
     """Parameters for Backup Datasource.
@@ -1793,15 +1809,15 @@
     _subtype_map = {
         "object_type": {
             "BlobBackupDatasourceParameters": "BlobBackupDatasourceParameters",
             "KubernetesClusterBackupDatasourceParameters": "KubernetesClusterBackupDatasourceParameters",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class BackupInstance(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """Backup Instance.
@@ -1873,16 +1889,16 @@
         data_source_info: "_models.Datasource",
         policy_info: "_models.PolicyInfo",
         object_type: str,
         friendly_name: Optional[str] = None,
         data_source_set_info: Optional["_models.DatasourceSet"] = None,
         datasource_auth_credentials: Optional["_models.AuthCredentials"] = None,
         validation_type: Optional[Union[str, "_models.ValidationType"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword friendly_name: Gets or sets the Backup Instance friendly name.
         :paramtype friendly_name: str
         :keyword data_source_info: Gets or sets the data source information. Required.
         :paramtype data_source_info: ~azure.mgmt.dataprotection.models.Datasource
         :keyword data_source_set_info: Gets or sets the data source set information.
         :paramtype data_source_set_info: ~azure.mgmt.dataprotection.models.DatasourceSet
@@ -1941,15 +1957,15 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "tags": {"key": "tags", "type": "{str}"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword tags: Proxy Resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
@@ -1991,16 +2007,20 @@
         "type": {"key": "type", "type": "str"},
         "tags": {"key": "tags", "type": "{str}"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "BackupInstance"},
     }
 
     def __init__(
-        self, *, tags: Optional[Dict[str, str]] = None, properties: Optional["_models.BackupInstance"] = None, **kwargs
-    ):
+        self,
+        *,
+        tags: Optional[Dict[str, str]] = None,
+        properties: Optional["_models.BackupInstance"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Proxy Resource tags.
         :paramtype tags: dict[str, str]
         :keyword properties: BackupInstanceResource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.BackupInstance
         """
         super().__init__(tags=tags, **kwargs)
@@ -2023,16 +2043,16 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.BackupInstanceResource"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.BackupInstanceResource]
         """
@@ -2062,15 +2082,15 @@
     _attribute_map = {
         "datasource_types": {"key": "datasourceTypes", "type": "[str]"},
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"BackupPolicy": "BackupPolicy"}}
 
-    def __init__(self, *, datasource_types: List[str], **kwargs):
+    def __init__(self, *, datasource_types: List[str], **kwargs: Any) -> None:
         """
         :keyword datasource_types: Type of datasource for the backup management. Required.
         :paramtype datasource_types: list[str]
         """
         super().__init__(**kwargs)
         self.datasource_types = datasource_types
         self.object_type: Optional[str] = None
@@ -2098,15 +2118,17 @@
 
     _attribute_map = {
         "datasource_types": {"key": "datasourceTypes", "type": "[str]"},
         "object_type": {"key": "objectType", "type": "str"},
         "policy_rules": {"key": "policyRules", "type": "[BasePolicyRule]"},
     }
 
-    def __init__(self, *, datasource_types: List[str], policy_rules: List["_models.BasePolicyRule"], **kwargs):
+    def __init__(
+        self, *, datasource_types: List[str], policy_rules: List["_models.BasePolicyRule"], **kwargs: Any
+    ) -> None:
         """
         :keyword datasource_types: Type of datasource for the backup management. Required.
         :paramtype datasource_types: list[str]
         :keyword policy_rules: Policy rule dictionary that contains rules for each backuptype i.e
          Full/Incremental/Logs etc. Required.
         :paramtype policy_rules: list[~azure.mgmt.dataprotection.models.BasePolicyRule]
         """
@@ -2131,15 +2153,15 @@
     }
 
     _attribute_map = {
         "repeating_time_intervals": {"key": "repeatingTimeIntervals", "type": "[str]"},
         "time_zone": {"key": "timeZone", "type": "str"},
     }
 
-    def __init__(self, *, repeating_time_intervals: List[str], time_zone: Optional[str] = None, **kwargs):
+    def __init__(self, *, repeating_time_intervals: List[str], time_zone: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword repeating_time_intervals: ISO 8601 repeating time interval format. Required.
         :paramtype repeating_time_intervals: list[str]
         :keyword time_zone: Time zone for a schedule. Example: Pacific Standard Time.
         :paramtype time_zone: str
         """
         super().__init__(**kwargs)
@@ -2167,14 +2189,16 @@
     :vartype resource_move_details: ~azure.mgmt.dataprotection.models.ResourceMoveDetails
     :ivar security_settings: Security Settings.
     :vartype security_settings: ~azure.mgmt.dataprotection.models.SecuritySettings
     :ivar storage_settings: Storage Settings. Required.
     :vartype storage_settings: list[~azure.mgmt.dataprotection.models.StorageSetting]
     :ivar is_vault_protected_by_resource_guard: Is vault protected by resource guard.
     :vartype is_vault_protected_by_resource_guard: bool
+    :ivar feature_settings: Feature Settings.
+    :vartype feature_settings: ~azure.mgmt.dataprotection.models.FeatureSettings
     """
 
     _validation = {
         "provisioning_state": {"readonly": True},
         "resource_move_state": {"readonly": True},
         "resource_move_details": {"readonly": True},
         "storage_settings": {"required": True},
@@ -2185,53 +2209,56 @@
         "monitoring_settings": {"key": "monitoringSettings", "type": "MonitoringSettings"},
         "provisioning_state": {"key": "provisioningState", "type": "str"},
         "resource_move_state": {"key": "resourceMoveState", "type": "str"},
         "resource_move_details": {"key": "resourceMoveDetails", "type": "ResourceMoveDetails"},
         "security_settings": {"key": "securitySettings", "type": "SecuritySettings"},
         "storage_settings": {"key": "storageSettings", "type": "[StorageSetting]"},
         "is_vault_protected_by_resource_guard": {"key": "isVaultProtectedByResourceGuard", "type": "bool"},
+        "feature_settings": {"key": "featureSettings", "type": "FeatureSettings"},
     }
 
     def __init__(
         self,
         *,
         storage_settings: List["_models.StorageSetting"],
         monitoring_settings: Optional["_models.MonitoringSettings"] = None,
         security_settings: Optional["_models.SecuritySettings"] = None,
-        **kwargs
-    ):
+        feature_settings: Optional["_models.FeatureSettings"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword monitoring_settings: Monitoring Settings.
         :paramtype monitoring_settings: ~azure.mgmt.dataprotection.models.MonitoringSettings
         :keyword security_settings: Security Settings.
         :paramtype security_settings: ~azure.mgmt.dataprotection.models.SecuritySettings
         :keyword storage_settings: Storage Settings. Required.
         :paramtype storage_settings: list[~azure.mgmt.dataprotection.models.StorageSetting]
+        :keyword feature_settings: Feature Settings.
+        :paramtype feature_settings: ~azure.mgmt.dataprotection.models.FeatureSettings
         """
         super().__init__(**kwargs)
         self.monitoring_settings = monitoring_settings
         self.provisioning_state = None
         self.resource_move_state = None
         self.resource_move_details = None
         self.security_settings = security_settings
         self.storage_settings = storage_settings
         self.is_vault_protected_by_resource_guard = None
+        self.feature_settings = feature_settings
 
 
-class DppTrackedResource(_serialization.Model):
-    """DppTrackedResource.
+class DppBaseTrackedResource(_serialization.Model):
+    """DppBaseTrackedResource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar e_tag: Optional ETag.
     :vartype e_tag: str
     :ivar id: Resource Id represents the complete path to the resource.
     :vartype id: str
-    :ivar identity: Input Managed Identity Details.
-    :vartype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
     :ivar location: Resource location.
     :vartype location: str
     :ivar name: Resource name associated with the resource.
     :vartype name: str
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar type: Resource type represents the complete path of the form
@@ -2247,76 +2274,136 @@
         "type": {"readonly": True},
         "system_data": {"readonly": True},
     }
 
     _attribute_map = {
         "e_tag": {"key": "eTag", "type": "str"},
         "id": {"key": "id", "type": "str"},
-        "identity": {"key": "identity", "type": "DppIdentityDetails"},
         "location": {"key": "location", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "tags": {"key": "tags", "type": "{str}"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
     def __init__(
         self,
         *,
         e_tag: Optional[str] = None,
-        identity: Optional["_models.DppIdentityDetails"] = None,
         location: Optional[str] = None,
         tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword e_tag: Optional ETag.
         :paramtype e_tag: str
-        :keyword identity: Input Managed Identity Details.
-        :paramtype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
         :keyword location: Resource location.
         :paramtype location: str
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.e_tag = e_tag
         self.id = None
-        self.identity = identity
         self.location = location
         self.name = None
         self.tags = tags
         self.type = None
         self.system_data = None
 
 
+class DppTrackedResource(DppBaseTrackedResource):
+    """DppTrackedResource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar e_tag: Optional ETag.
+    :vartype e_tag: str
+    :ivar id: Resource Id represents the complete path to the resource.
+    :vartype id: str
+    :ivar location: Resource location.
+    :vartype location: str
+    :ivar name: Resource name associated with the resource.
+    :vartype name: str
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar type: Resource type represents the complete path of the form
+     Namespace/ResourceType/ResourceType/...
+    :vartype type: str
+    :ivar system_data: Metadata pertaining to creation and last modification of the resource.
+    :vartype system_data: ~azure.mgmt.dataprotection.models.SystemData
+    :ivar identity: Input Managed Identity Details.
+    :vartype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "e_tag": {"key": "eTag", "type": "str"},
+        "id": {"key": "id", "type": "str"},
+        "location": {"key": "location", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "identity": {"key": "identity", "type": "DppIdentityDetails"},
+    }
+
+    def __init__(
+        self,
+        *,
+        e_tag: Optional[str] = None,
+        location: Optional[str] = None,
+        tags: Optional[Dict[str, str]] = None,
+        identity: Optional["_models.DppIdentityDetails"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword e_tag: Optional ETag.
+        :paramtype e_tag: str
+        :keyword location: Resource location.
+        :paramtype location: str
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword identity: Input Managed Identity Details.
+        :paramtype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
+        """
+        super().__init__(e_tag=e_tag, location=location, tags=tags, **kwargs)
+        self.identity = identity
+
+
 class BackupVaultResource(DppTrackedResource):
     """Backup Vault Resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar e_tag: Optional ETag.
     :vartype e_tag: str
     :ivar id: Resource Id represents the complete path to the resource.
     :vartype id: str
-    :ivar identity: Input Managed Identity Details.
-    :vartype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
     :ivar location: Resource location.
     :vartype location: str
     :ivar name: Resource name associated with the resource.
     :vartype name: str
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar type: Resource type represents the complete path of the form
      Namespace/ResourceType/ResourceType/...
     :vartype type: str
     :ivar system_data: Metadata pertaining to creation and last modification of the resource.
     :vartype system_data: ~azure.mgmt.dataprotection.models.SystemData
+    :ivar identity: Input Managed Identity Details.
+    :vartype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
     :ivar properties: BackupVaultResource properties. Required.
     :vartype properties: ~azure.mgmt.dataprotection.models.BackupVault
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
@@ -2324,46 +2411,46 @@
         "system_data": {"readonly": True},
         "properties": {"required": True},
     }
 
     _attribute_map = {
         "e_tag": {"key": "eTag", "type": "str"},
         "id": {"key": "id", "type": "str"},
-        "identity": {"key": "identity", "type": "DppIdentityDetails"},
         "location": {"key": "location", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "tags": {"key": "tags", "type": "{str}"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
+        "identity": {"key": "identity", "type": "DppIdentityDetails"},
         "properties": {"key": "properties", "type": "BackupVault"},
     }
 
     def __init__(
         self,
         *,
         properties: "_models.BackupVault",
         e_tag: Optional[str] = None,
-        identity: Optional["_models.DppIdentityDetails"] = None,
         location: Optional[str] = None,
         tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        identity: Optional["_models.DppIdentityDetails"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword e_tag: Optional ETag.
         :paramtype e_tag: str
-        :keyword identity: Input Managed Identity Details.
-        :paramtype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
         :keyword location: Resource location.
         :paramtype location: str
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
+        :keyword identity: Input Managed Identity Details.
+        :paramtype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
         :keyword properties: BackupVaultResource properties. Required.
         :paramtype properties: ~azure.mgmt.dataprotection.models.BackupVault
         """
-        super().__init__(e_tag=e_tag, identity=identity, location=location, tags=tags, **kwargs)
+        super().__init__(e_tag=e_tag, location=location, tags=tags, identity=identity, **kwargs)
         self.properties = properties
 
 
 class BackupVaultResourceList(DppResourceList):
     """List of BackupVault resources.
 
     :ivar next_link: The uri to fetch the next page of resources. Call ListNext() fetches next page
@@ -2375,16 +2462,20 @@
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
         "value": {"key": "value", "type": "[BackupVaultResource]"},
     }
 
     def __init__(
-        self, *, next_link: Optional[str] = None, value: Optional[List["_models.BackupVaultResource"]] = None, **kwargs
-    ):
+        self,
+        *,
+        next_link: Optional[str] = None,
+        value: Optional[List["_models.BackupVaultResource"]] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.BackupVaultResource]
         """
@@ -2421,15 +2512,15 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "BaseBackupPolicy"},
     }
 
-    def __init__(self, *, properties: Optional["_models.BaseBackupPolicy"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.BaseBackupPolicy"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: BaseBackupPolicyResource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.BaseBackupPolicy
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -2450,16 +2541,16 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.BaseBackupPolicyResource"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.BaseBackupPolicyResource]
         """
@@ -2485,15 +2576,15 @@
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "containers_list": {"key": "containersList", "type": "[str]"},
     }
 
-    def __init__(self, *, containers_list: List[str], **kwargs):
+    def __init__(self, *, containers_list: List[str], **kwargs: Any) -> None:
         """
         :keyword containers_list: List of containers to be backed up during configuration of backup of
          blobs. Required.
         :paramtype containers_list: list[str]
         """
         super().__init__(**kwargs)
         self.object_type: str = "BlobBackupDatasourceParameters"
@@ -2510,15 +2601,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, type: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, type: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Resource name for which availability needs to be checked.
         :paramtype name: str
         :keyword type: Describes the Resource type: Microsoft.DataProtection/BackupVaults.
         :paramtype type: str
         """
         super().__init__(**kwargs)
@@ -2545,16 +2636,16 @@
 
     def __init__(
         self,
         *,
         message: Optional[str] = None,
         name_available: Optional[bool] = None,
         reason: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword message: Gets or sets the message.
         :paramtype message: str
         :keyword name_available: Gets or sets a value indicating whether [name available].
         :paramtype name_available: bool
         :keyword reason: Gets or sets the reason.
         :paramtype reason: str
@@ -2588,16 +2679,16 @@
     def __init__(
         self,
         *,
         description: Optional[str] = None,
         operation: Optional[str] = None,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword description: Description of the operation having details of what operation is about.
         :paramtype description: str
         :keyword operation: Operations Name itself.
         :paramtype operation: str
         :keyword provider: Name of the provider for display purposes.
         :paramtype provider: str
@@ -2630,16 +2721,16 @@
 
     def __init__(
         self,
         *,
         blob_duration: Optional[str] = None,
         display_name: Optional[str] = None,
         name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword blob_duration: blob duration of shoebox log specification.
         :paramtype blob_duration: str
         :keyword display_name: Localized display name.
         :paramtype display_name: str
         :keyword name: Name for shoebox log specification.
         :paramtype name: str
@@ -2659,16 +2750,16 @@
     """
 
     _attribute_map = {
         "service_specification": {"key": "serviceSpecification", "type": "ClientDiscoveryForServiceSpecification"},
     }
 
     def __init__(
-        self, *, service_specification: Optional["_models.ClientDiscoveryForServiceSpecification"] = None, **kwargs
-    ):
+        self, *, service_specification: Optional["_models.ClientDiscoveryForServiceSpecification"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword service_specification: Operation properties.
         :paramtype service_specification:
          ~azure.mgmt.dataprotection.models.ClientDiscoveryForServiceSpecification
         """
         super().__init__(**kwargs)
         self.service_specification = service_specification
@@ -2683,16 +2774,16 @@
     """
 
     _attribute_map = {
         "log_specifications": {"key": "logSpecifications", "type": "[ClientDiscoveryForLogSpecification]"},
     }
 
     def __init__(
-        self, *, log_specifications: Optional[List["_models.ClientDiscoveryForLogSpecification"]] = None, **kwargs
-    ):
+        self, *, log_specifications: Optional[List["_models.ClientDiscoveryForLogSpecification"]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword log_specifications: List of log specifications of this operation.
         :paramtype log_specifications:
          list[~azure.mgmt.dataprotection.models.ClientDiscoveryForLogSpecification]
         """
         super().__init__(**kwargs)
         self.log_specifications = log_specifications
@@ -2713,16 +2804,16 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.ClientDiscoveryValueForSingleApi"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: Link to the next chunk of Response.
         :paramtype next_link: str
         :keyword value: List of available operations.
         :paramtype value: list[~azure.mgmt.dataprotection.models.ClientDiscoveryValueForSingleApi]
         """
         super().__init__(**kwargs)
@@ -2758,16 +2849,16 @@
         self,
         *,
         display: Optional["_models.ClientDiscoveryDisplay"] = None,
         name: Optional[str] = None,
         is_data_action: Optional[bool] = None,
         origin: Optional[str] = None,
         properties: Optional["_models.ClientDiscoveryForProperties"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword display: Contains the localized display information for this particular operation.
         :paramtype display: ~azure.mgmt.dataprotection.models.ClientDiscoveryDisplay
         :keyword name: Name of the Operation.
         :paramtype name: str
         :keyword is_data_action: Indicates whether the operation is a data action.
         :paramtype is_data_action: bool
@@ -2809,15 +2900,15 @@
         "object_type": {
             "CopyOnExpiryOption": "CopyOnExpiryOption",
             "CustomCopyOption": "CustomCopyOption",
             "ImmediateCopyOption": "ImmediateCopyOption",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class CopyOnExpiryOption(CopyOption):
     """Copy on Expiry Option.
@@ -2832,20 +2923,44 @@
         "object_type": {"required": True},
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: str = "CopyOnExpiryOption"
 
 
+class CrossSubscriptionRestoreSettings(_serialization.Model):
+    """CrossSubscriptionRestore Settings.
+
+    :ivar state: CrossSubscriptionRestore state. Known values are: "Disabled",
+     "PermanentlyDisabled", and "Enabled".
+    :vartype state: str or ~azure.mgmt.dataprotection.models.CrossSubscriptionRestoreState
+    """
+
+    _attribute_map = {
+        "state": {"key": "state", "type": "str"},
+    }
+
+    def __init__(
+        self, *, state: Optional[Union[str, "_models.CrossSubscriptionRestoreState"]] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword state: CrossSubscriptionRestore state. Known values are: "Disabled",
+         "PermanentlyDisabled", and "Enabled".
+        :paramtype state: str or ~azure.mgmt.dataprotection.models.CrossSubscriptionRestoreState
+        """
+        super().__init__(**kwargs)
+        self.state = state
+
+
 class CustomCopyOption(CopyOption):
     """Duration based custom options to copy.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar object_type: Type of the specific object - used for deserializing. Required.
     :vartype object_type: str
@@ -2858,15 +2973,15 @@
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "duration": {"key": "duration", "type": "str"},
     }
 
-    def __init__(self, *, duration: Optional[str] = None, **kwargs):
+    def __init__(self, *, duration: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword duration: Data copied after given timespan.
         :paramtype duration: str
         """
         super().__init__(**kwargs)
         self.object_type: str = "CustomCopyOption"
         self.duration = duration
@@ -2914,16 +3029,16 @@
         resource_id: str,
         datasource_type: Optional[str] = None,
         object_type: Optional[str] = None,
         resource_location: Optional[str] = None,
         resource_name: Optional[str] = None,
         resource_type: Optional[str] = None,
         resource_uri: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword datasource_type: DatasourceType of the resource.
         :paramtype datasource_type: str
         :keyword object_type: Type of Datasource object, used to initialize the right inherited type.
         :paramtype object_type: str
         :keyword resource_id: Full ARM ID of the resource. For azure resources, this is ARM ID. For non
          azure resources, this will be the ID created by backup service via Fabric/Vault. Required.
@@ -2989,16 +3104,16 @@
         resource_id: str,
         datasource_type: Optional[str] = None,
         object_type: Optional[str] = None,
         resource_location: Optional[str] = None,
         resource_name: Optional[str] = None,
         resource_type: Optional[str] = None,
         resource_uri: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword datasource_type: DatasourceType of the resource.
         :paramtype datasource_type: str
         :keyword object_type: Type of Datasource object, used to initialize the right inherited type.
         :paramtype object_type: str
         :keyword resource_id: Full ARM ID of the resource. For azure resources, this is ARM ID. For non
          azure resources, this will be the ID created by backup service via Fabric/Vault. Required.
@@ -3041,15 +3156,17 @@
     }
 
     _attribute_map = {
         "data_store_type": {"key": "dataStoreType", "type": "str"},
         "object_type": {"key": "objectType", "type": "str"},
     }
 
-    def __init__(self, *, data_store_type: Union[str, "_models.DataStoreTypes"], object_type: str, **kwargs):
+    def __init__(
+        self, *, data_store_type: Union[str, "_models.DataStoreTypes"], object_type: str, **kwargs: Any
+    ) -> None:
         """
         :keyword data_store_type: type of datastore; Operational/Vault/Archive. Required. Known values
          are: "OperationalStore", "VaultStore", and "ArchiveStore".
         :paramtype data_store_type: str or ~azure.mgmt.dataprotection.models.DataStoreTypes
         :keyword object_type: Type of Datasource object, used to initialize the right inherited type.
          Required.
         :paramtype object_type: str
@@ -3069,15 +3186,15 @@
     """
 
     _attribute_map = {
         "date": {"key": "date", "type": "int"},
         "is_last": {"key": "isLast", "type": "bool"},
     }
 
-    def __init__(self, *, date: Optional[int] = None, is_last: Optional[bool] = None, **kwargs):
+    def __init__(self, *, date: Optional[int] = None, is_last: Optional[bool] = None, **kwargs: Any) -> None:
         """
         :keyword date: Date of the month.
         :paramtype date: int
         :keyword is_last: Whether Date is last date of month.
         :paramtype is_last: bool
         """
         super().__init__(**kwargs)
@@ -3159,16 +3276,16 @@
         data_source_info: "_models.Datasource",
         policy_info: "_models.PolicyInfo",
         object_type: str,
         friendly_name: Optional[str] = None,
         data_source_set_info: Optional["_models.DatasourceSet"] = None,
         datasource_auth_credentials: Optional["_models.AuthCredentials"] = None,
         validation_type: Optional[Union[str, "_models.ValidationType"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword friendly_name: Gets or sets the Backup Instance friendly name.
         :paramtype friendly_name: str
         :keyword data_source_info: Gets or sets the data source information. Required.
         :paramtype data_source_info: ~azure.mgmt.dataprotection.models.Datasource
         :keyword data_source_set_info: Gets or sets the data source set information.
         :paramtype data_source_set_info: ~azure.mgmt.dataprotection.models.DatasourceSet
@@ -3226,15 +3343,15 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "DeletedBackupInstance"},
     }
 
-    def __init__(self, *, properties: Optional["_models.DeletedBackupInstance"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.DeletedBackupInstance"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: DeletedBackupInstanceResource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.DeletedBackupInstance
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -3255,16 +3372,16 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.DeletedBackupInstanceResource"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.DeletedBackupInstanceResource]
         """
@@ -3297,15 +3414,15 @@
     _attribute_map = {
         "deletion_time": {"key": "deletionTime", "type": "str"},
         "billing_end_date": {"key": "billingEndDate", "type": "str"},
         "scheduled_purge_time": {"key": "scheduledPurgeTime", "type": "str"},
         "delete_activity_id": {"key": "deleteActivityID", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.deletion_time = None
         self.billing_end_date = None
         self.scheduled_purge_time = None
         self.delete_activity_id = None
 
@@ -3332,15 +3449,15 @@
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
 
 
@@ -3356,16 +3473,16 @@
 
     _attribute_map = {
         "value": {"key": "value", "type": "[DppBaseResource]"},
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self, *, value: Optional[List["_models.DppBaseResource"]] = None, next_link: Optional[str] = None, **kwargs
-    ):
+        self, *, value: Optional[List["_models.DppBaseResource"]] = None, next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword value: List of Dpp resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.DppBaseResource]
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         """
@@ -3396,15 +3513,15 @@
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "tenant_id": {"key": "tenantId", "type": "str"},
         "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(self, *, type: Optional[str] = None, **kwargs):
+    def __init__(self, *, type: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword type: The identityType which can be either SystemAssigned or None.
         :paramtype type: str
         """
         super().__init__(**kwargs)
         self.principal_id = None
         self.tenant_id = None
@@ -3419,15 +3536,15 @@
     :vartype next_link: str
     """
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(self, *, next_link: Optional[str] = None, **kwargs):
+    def __init__(self, *, next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.next_link = next_link
@@ -3462,15 +3579,15 @@
         "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
         "code": {"key": "code", "type": "str"},
         "details": {"key": "details", "type": "[Error]"},
         "message": {"key": "message", "type": "str"},
         "target": {"key": "target", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.additional_info = None
         self.code = None
         self.details = None
         self.message = None
         self.target = None
@@ -3493,15 +3610,15 @@
     }
 
     _attribute_map = {
         "info": {"key": "info", "type": "object"},
         "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.info = None
         self.type = None
 
 
 class ExportJobsResult(_serialization.Model):
@@ -3529,23 +3646,53 @@
     _attribute_map = {
         "blob_url": {"key": "blobUrl", "type": "str"},
         "blob_sas_key": {"key": "blobSasKey", "type": "str"},
         "excel_file_blob_url": {"key": "excelFileBlobUrl", "type": "str"},
         "excel_file_blob_sas_key": {"key": "excelFileBlobSasKey", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.blob_url = None
         self.blob_sas_key = None
         self.excel_file_blob_url = None
         self.excel_file_blob_sas_key = None
 
 
+class FeatureSettings(_serialization.Model):
+    """Class containing feature settings of vault.
+
+    :ivar cross_subscription_restore_settings: CrossSubscriptionRestore Settings.
+    :vartype cross_subscription_restore_settings:
+     ~azure.mgmt.dataprotection.models.CrossSubscriptionRestoreSettings
+    """
+
+    _attribute_map = {
+        "cross_subscription_restore_settings": {
+            "key": "crossSubscriptionRestoreSettings",
+            "type": "CrossSubscriptionRestoreSettings",
+        },
+    }
+
+    def __init__(
+        self,
+        *,
+        cross_subscription_restore_settings: Optional["_models.CrossSubscriptionRestoreSettings"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword cross_subscription_restore_settings: CrossSubscriptionRestore Settings.
+        :paramtype cross_subscription_restore_settings:
+         ~azure.mgmt.dataprotection.models.CrossSubscriptionRestoreSettings
+        """
+        super().__init__(**kwargs)
+        self.cross_subscription_restore_settings = cross_subscription_restore_settings
+
+
 class FeatureValidationRequestBase(_serialization.Model):
     """Base class for Backup Feature support.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
     FeatureValidationRequest
 
     All required parameters must be populated in order to send to Azure.
@@ -3560,15 +3707,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"FeatureValidationRequest": "FeatureValidationRequest"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class FeatureValidationRequest(FeatureValidationRequestBase):
     """Base class for feature object.
@@ -3595,16 +3742,16 @@
     }
 
     def __init__(
         self,
         *,
         feature_type: Optional[Union[str, "_models.FeatureType"]] = None,
         feature_name: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword feature_type: backup support feature type. Known values are: "Invalid" and
          "DataSourceType".
         :paramtype feature_type: str or ~azure.mgmt.dataprotection.models.FeatureType
         :keyword feature_name: backup support feature name.
         :paramtype feature_name: str
         """
@@ -3632,15 +3779,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"FeatureValidationResponse": "FeatureValidationResponse"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class FeatureValidationResponse(FeatureValidationResponseBase):
     """Feature Validation Response.
@@ -3667,16 +3814,16 @@
     }
 
     def __init__(
         self,
         *,
         feature_type: Optional[Union[str, "_models.FeatureType"]] = None,
         features: Optional[List["_models.SupportedFeature"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword feature_type: backup support feature type. Known values are: "Invalid" and
          "DataSourceType".
         :paramtype feature_type: str or ~azure.mgmt.dataprotection.models.FeatureType
         :keyword features: Response features.
         :paramtype features: list[~azure.mgmt.dataprotection.models.SupportedFeature]
         """
@@ -3699,15 +3846,15 @@
         "object_type": {"required": True},
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: str = "ImmediateCopyOption"
 
 
 class ImmutabilitySettings(_serialization.Model):
     """Immutability Settings at vault level.
@@ -3716,15 +3863,15 @@
     :vartype state: str or ~azure.mgmt.dataprotection.models.ImmutabilityState
     """
 
     _attribute_map = {
         "state": {"key": "state", "type": "str"},
     }
 
-    def __init__(self, *, state: Optional[Union[str, "_models.ImmutabilityState"]] = None, **kwargs):
+    def __init__(self, *, state: Optional[Union[str, "_models.ImmutabilityState"]] = None, **kwargs: Any) -> None:
         """
         :keyword state: Immutability state. Known values are: "Disabled", "Unlocked", and "Locked".
         :paramtype state: str or ~azure.mgmt.dataprotection.models.ImmutabilityState
         """
         super().__init__(**kwargs)
         self.state = state
 
@@ -3749,16 +3896,16 @@
 
     def __init__(
         self,
         *,
         additional_info: Optional[Dict[str, str]] = None,
         code: Optional[str] = None,
         embedded_inner_error: Optional["_models.InnerError"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword additional_info: Any Key value pairs that can be provided to the client for additional
          verbose information.
         :paramtype additional_info: dict[str, str]
         :keyword code: Unique code for this error.
         :paramtype code: str
         :keyword embedded_inner_error: Child Inner Error, to allow Nesting.
@@ -3797,15 +3944,15 @@
             "KubernetesClusterRestoreCriteria": "KubernetesClusterRestoreCriteria",
             "KubernetesPVRestoreCriteria": "KubernetesPVRestoreCriteria",
             "KubernetesStorageClassRestoreCriteria": "KubernetesStorageClassRestoreCriteria",
             "RangeBasedItemLevelRestoreCriteria": "RangeBasedItemLevelRestoreCriteria",
         }
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class RestoreTargetInfoBase(_serialization.Model):
     """Base class common to RestoreTargetInfo and RestoreFilesTargetInfo.
@@ -3840,16 +3987,20 @@
             "ItemLevelRestoreTargetInfo": "ItemLevelRestoreTargetInfo",
             "RestoreFilesTargetInfo": "RestoreFilesTargetInfo",
             "RestoreTargetInfo": "RestoreTargetInfo",
         }
     }
 
     def __init__(
-        self, *, recovery_option: Union[str, "_models.RecoveryOption"], restore_location: Optional[str] = None, **kwargs
-    ):
+        self,
+        *,
+        recovery_option: Union[str, "_models.RecoveryOption"],
+        restore_location: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword recovery_option: Recovery Option. Required. "FailIfExists"
         :paramtype recovery_option: str or ~azure.mgmt.dataprotection.models.RecoveryOption
         :keyword restore_location: Target Restore region.
         :paramtype restore_location: str
         """
         super().__init__(**kwargs)
@@ -3903,16 +4054,16 @@
         *,
         recovery_option: Union[str, "_models.RecoveryOption"],
         restore_criteria: List["_models.ItemLevelRestoreCriteria"],
         datasource_info: "_models.Datasource",
         restore_location: Optional[str] = None,
         datasource_set_info: Optional["_models.DatasourceSet"] = None,
         datasource_auth_credentials: Optional["_models.AuthCredentials"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword recovery_option: Recovery Option. Required. "FailIfExists"
         :paramtype recovery_option: str or ~azure.mgmt.dataprotection.models.RecoveryOption
         :keyword restore_location: Target Restore region.
         :paramtype restore_location: str
         :keyword restore_criteria: Restore Criteria. Required.
         :paramtype restore_criteria: list[~azure.mgmt.dataprotection.models.ItemLevelRestoreCriteria]
@@ -3965,16 +4116,16 @@
 
     def __init__(
         self,
         *,
         item_path: str,
         is_path_relative_to_backup_item: bool,
         sub_item_path_prefix: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword item_path: The path of the item to be restored. It could be the full path of the item
          or the path relative to the backup item. Required.
         :paramtype item_path: str
         :keyword is_path_relative_to_backup_item: Flag to specify if the path is relative to backup
          item or full path. Required.
         :paramtype is_path_relative_to_backup_item: bool
@@ -4025,15 +4176,15 @@
         "data_transferred_in_bytes": {"key": "dataTransferredInBytes", "type": "float"},
         "recovery_destination": {"key": "recoveryDestination", "type": "str"},
         "source_recover_point": {"key": "sourceRecoverPoint", "type": "RestoreJobRecoveryPointDetails"},
         "sub_tasks": {"key": "subTasks", "type": "[JobSubTask]"},
         "target_recover_point": {"key": "targetRecoverPoint", "type": "RestoreJobRecoveryPointDetails"},
     }
 
-    def __init__(self, *, additional_details: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, additional_details: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword additional_details: Job's Additional Details.
         :paramtype additional_details: dict[str, str]
         """
         super().__init__(**kwargs)
         self.additional_details = additional_details
         self.backup_instance_state = None
@@ -4081,16 +4232,16 @@
     def __init__(
         self,
         *,
         task_id: int,
         task_name: str,
         task_status: str,
         additional_details: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword additional_details: Additional details of Sub Tasks.
         :paramtype additional_details: dict[str, str]
         :keyword task_id: Task Id of the Sub Task. Required.
         :paramtype task_id: int
         :keyword task_name: Name of the Sub Task. Required.
         :paramtype task_name: str
@@ -4158,16 +4309,16 @@
         snapshot_volumes: bool,
         include_cluster_scope_resources: bool,
         included_namespaces: Optional[List[str]] = None,
         excluded_namespaces: Optional[List[str]] = None,
         included_resource_types: Optional[List[str]] = None,
         excluded_resource_types: Optional[List[str]] = None,
         label_selectors: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword snapshot_volumes: Gets or sets the volume snapshot property. This property if enabled
          will take volume snapshots during restore. Required.
         :paramtype snapshot_volumes: bool
         :keyword include_cluster_scope_resources: Gets or sets the include cluster resources property.
          This property if enabled will include cluster scope resources during restore. Required.
         :paramtype include_cluster_scope_resources: bool
@@ -4219,17 +4370,17 @@
     :vartype included_resource_types: list[str]
     :ivar excluded_resource_types: Gets or sets the exclude resource types property. This property
      sets the resource types to be excluded during restore.
     :vartype excluded_resource_types: list[str]
     :ivar label_selectors: Gets or sets the LabelSelectors property. This property sets the
      resource with such label selectors to be included during restore.
     :vartype label_selectors: list[str]
-    :ivar persistent_volume_restore_mode: Gets or sets the PV Restore Mode property. This property
-     sets whether volumes needs to be restored. Known values are: "RestoreWithVolumeData" and
-     "RestoreWithoutVolumeData".
+    :ivar persistent_volume_restore_mode: Gets or sets the PV (Persistent Volume) Restore Mode
+     property. This property sets whether volumes needs to be restored. Known values are:
+     "RestoreWithVolumeData" and "RestoreWithoutVolumeData".
     :vartype persistent_volume_restore_mode: str or
      ~azure.mgmt.dataprotection.models.PersistentVolumeRestoreMode
     :ivar conflict_policy: Gets or sets the Conflict Policy property. This property sets policy
      during conflict of resources during restore. Known values are: "Skip" and "Patch".
     :vartype conflict_policy: str or ~azure.mgmt.dataprotection.models.ExistingResourcePolicy
     :ivar namespace_mappings: Gets or sets the Namespace Mappings property. This property sets if
      namespace needs to be change during restore.
@@ -4262,16 +4413,16 @@
         excluded_namespaces: Optional[List[str]] = None,
         included_resource_types: Optional[List[str]] = None,
         excluded_resource_types: Optional[List[str]] = None,
         label_selectors: Optional[List[str]] = None,
         persistent_volume_restore_mode: Optional[Union[str, "_models.PersistentVolumeRestoreMode"]] = None,
         conflict_policy: Optional[Union[str, "_models.ExistingResourcePolicy"]] = None,
         namespace_mappings: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword include_cluster_scope_resources: Gets or sets the include cluster resources property.
          This property if enabled will include cluster scope resources during restore. Required.
         :paramtype include_cluster_scope_resources: bool
         :keyword included_namespaces: Gets or sets the include namespaces property. This property sets
          the namespaces to be included during restore.
         :paramtype included_namespaces: list[str]
@@ -4283,17 +4434,17 @@
         :paramtype included_resource_types: list[str]
         :keyword excluded_resource_types: Gets or sets the exclude resource types property. This
          property sets the resource types to be excluded during restore.
         :paramtype excluded_resource_types: list[str]
         :keyword label_selectors: Gets or sets the LabelSelectors property. This property sets the
          resource with such label selectors to be included during restore.
         :paramtype label_selectors: list[str]
-        :keyword persistent_volume_restore_mode: Gets or sets the PV Restore Mode property. This
-         property sets whether volumes needs to be restored. Known values are: "RestoreWithVolumeData"
-         and "RestoreWithoutVolumeData".
+        :keyword persistent_volume_restore_mode: Gets or sets the PV (Persistent Volume) Restore Mode
+         property. This property sets whether volumes needs to be restored. Known values are:
+         "RestoreWithVolumeData" and "RestoreWithoutVolumeData".
         :paramtype persistent_volume_restore_mode: str or
          ~azure.mgmt.dataprotection.models.PersistentVolumeRestoreMode
         :keyword conflict_policy: Gets or sets the Conflict Policy property. This property sets policy
          during conflict of resources during restore. Known values are: "Skip" and "Patch".
         :paramtype conflict_policy: str or ~azure.mgmt.dataprotection.models.ExistingResourcePolicy
         :keyword namespace_mappings: Gets or sets the Namespace Mappings property. This property sets
          if namespace needs to be change during restore.
@@ -4331,15 +4482,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "storage_class_name": {"key": "storageClassName", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, storage_class_name: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, storage_class_name: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Selected persistent volume claim name.
         :paramtype name: str
         :keyword storage_class_name: Selected storage class name for restore operation.
         :paramtype storage_class_name: str
         """
         super().__init__(**kwargs)
@@ -4368,16 +4519,16 @@
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "selected_storage_class_name": {"key": "selectedStorageClassName", "type": "str"},
         "provisioner": {"key": "provisioner", "type": "str"},
     }
 
     def __init__(
-        self, *, selected_storage_class_name: Optional[str] = None, provisioner: Optional[str] = None, **kwargs
-    ):
+        self, *, selected_storage_class_name: Optional[str] = None, provisioner: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword selected_storage_class_name: Selected storage class name.
         :paramtype selected_storage_class_name: str
         :keyword provisioner: Provisioner of the storage class.
         :paramtype provisioner: str
         """
         super().__init__(**kwargs)
@@ -4394,15 +4545,17 @@
      ~azure.mgmt.dataprotection.models.AzureMonitorAlertSettings
     """
 
     _attribute_map = {
         "azure_monitor_alert_settings": {"key": "azureMonitorAlertSettings", "type": "AzureMonitorAlertSettings"},
     }
 
-    def __init__(self, *, azure_monitor_alert_settings: Optional["_models.AzureMonitorAlertSettings"] = None, **kwargs):
+    def __init__(
+        self, *, azure_monitor_alert_settings: Optional["_models.AzureMonitorAlertSettings"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword azure_monitor_alert_settings: Settings for Azure Monitor based alerts.
         :paramtype azure_monitor_alert_settings:
          ~azure.mgmt.dataprotection.models.AzureMonitorAlertSettings
         """
         super().__init__(**kwargs)
         self.azure_monitor_alert_settings = azure_monitor_alert_settings
@@ -4427,15 +4580,15 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
     }
 
     _subtype_map = {"object_type": {"OperationJobExtendedInfo": "OperationJobExtendedInfo"}}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.object_type: Optional[str] = None
 
 
 class OperationJobExtendedInfo(OperationExtendedInfo):
     """Operation Job Extended Info.
@@ -4454,15 +4607,15 @@
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "job_id": {"key": "jobId", "type": "str"},
     }
 
-    def __init__(self, *, job_id: Optional[str] = None, **kwargs):
+    def __init__(self, *, job_id: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword job_id: Arm Id of the job created for this operation.
         :paramtype job_id: str
         """
         super().__init__(**kwargs)
         self.object_type: str = "OperationJobExtendedInfo"
         self.job_id = job_id
@@ -4507,16 +4660,16 @@
         end_time: Optional[datetime.datetime] = None,
         error: Optional["_models.Error"] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
         properties: Optional["_models.OperationExtendedInfo"] = None,
         start_time: Optional[datetime.datetime] = None,
         status: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword end_time: End time of the operation.
         :paramtype end_time: ~datetime.datetime
         :keyword error: Required if status == failed or status == canceled. This is the OData v4 error
          format, used by the RPC and will go into the v2.2 Azure REST API guidelines.
          The full set of optional properties (e.g. inner errors / details) can be found in the "Error
          Response" section.
@@ -4546,37 +4699,64 @@
 class PatchBackupVaultInput(_serialization.Model):
     """Backup Vault Contract for Patch Backup Vault API.
 
     :ivar monitoring_settings: Monitoring Settings.
     :vartype monitoring_settings: ~azure.mgmt.dataprotection.models.MonitoringSettings
     :ivar security_settings: Security Settings.
     :vartype security_settings: ~azure.mgmt.dataprotection.models.SecuritySettings
+    :ivar feature_settings: Feature Settings.
+    :vartype feature_settings: ~azure.mgmt.dataprotection.models.FeatureSettings
     """
 
     _attribute_map = {
         "monitoring_settings": {"key": "monitoringSettings", "type": "MonitoringSettings"},
         "security_settings": {"key": "securitySettings", "type": "SecuritySettings"},
+        "feature_settings": {"key": "featureSettings", "type": "FeatureSettings"},
     }
 
     def __init__(
         self,
         *,
         monitoring_settings: Optional["_models.MonitoringSettings"] = None,
         security_settings: Optional["_models.SecuritySettings"] = None,
-        **kwargs
-    ):
+        feature_settings: Optional["_models.FeatureSettings"] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword monitoring_settings: Monitoring Settings.
         :paramtype monitoring_settings: ~azure.mgmt.dataprotection.models.MonitoringSettings
         :keyword security_settings: Security Settings.
         :paramtype security_settings: ~azure.mgmt.dataprotection.models.SecuritySettings
+        :keyword feature_settings: Feature Settings.
+        :paramtype feature_settings: ~azure.mgmt.dataprotection.models.FeatureSettings
         """
         super().__init__(**kwargs)
         self.monitoring_settings = monitoring_settings
         self.security_settings = security_settings
+        self.feature_settings = feature_settings
+
+
+class PatchResourceGuardInput(_serialization.Model):
+    """Patch Request content for Microsoft.DataProtection Resource Guard resources.
+
+    :ivar tags: Resource Guard tags.
+    :vartype tags: dict[str, str]
+    """
+
+    _attribute_map = {
+        "tags": {"key": "tags", "type": "{str}"},
+    }
+
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword tags: Resource Guard tags.
+        :paramtype tags: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
 
 
 class PatchResourceRequestInput(_serialization.Model):
     """Patch Request content for Microsoft.DataProtection resources.
 
     :ivar identity: Input Managed Identity Details.
     :vartype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
@@ -4594,16 +4774,16 @@
 
     def __init__(
         self,
         *,
         identity: Optional["_models.DppIdentityDetails"] = None,
         properties: Optional["_models.PatchBackupVaultInput"] = None,
         tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword identity: Input Managed Identity Details.
         :paramtype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
         :keyword properties: Resource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.PatchBackupVaultInput
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
@@ -4636,15 +4816,17 @@
 
     _attribute_map = {
         "policy_id": {"key": "policyId", "type": "str"},
         "policy_version": {"key": "policyVersion", "type": "str"},
         "policy_parameters": {"key": "policyParameters", "type": "PolicyParameters"},
     }
 
-    def __init__(self, *, policy_id: str, policy_parameters: Optional["_models.PolicyParameters"] = None, **kwargs):
+    def __init__(
+        self, *, policy_id: str, policy_parameters: Optional["_models.PolicyParameters"] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword policy_id: Required.
         :paramtype policy_id: str
         :keyword policy_parameters: Policy parameters for the backup instance.
         :paramtype policy_parameters: ~azure.mgmt.dataprotection.models.PolicyParameters
         """
         super().__init__(**kwargs)
@@ -4673,16 +4855,16 @@
     }
 
     def __init__(
         self,
         *,
         data_store_parameters_list: Optional[List["_models.DataStoreParameters"]] = None,
         backup_datasource_parameters_list: Optional[List["_models.BackupDatasourceParameters"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword data_store_parameters_list: Gets or sets the DataStore Parameters.
         :paramtype data_store_parameters_list:
          list[~azure.mgmt.dataprotection.models.DataStoreParameters]
         :keyword backup_datasource_parameters_list: Gets or sets the Backup Data Source Parameters.
         :paramtype backup_datasource_parameters_list:
          list[~azure.mgmt.dataprotection.models.BackupDatasourceParameters]
@@ -4709,16 +4891,16 @@
     }
 
     def __init__(
         self,
         *,
         error_details: Optional["_models.UserFacingError"] = None,
         status: Optional[Union[str, "_models.Status"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword error_details: Specifies the protection status error of the resource.
         :paramtype error_details: ~azure.mgmt.dataprotection.models.UserFacingError
         :keyword status: Specifies the protection status of the resource. Known values are:
          "ConfiguringProtection", "ConfiguringProtectionFailed", "ProtectionConfigured",
          "ProtectionStopped", "SoftDeleted", and "SoftDeleting".
         :paramtype status: str or ~azure.mgmt.dataprotection.models.Status
@@ -4747,15 +4929,17 @@
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "min_matching_value": {"key": "minMatchingValue", "type": "str"},
         "max_matching_value": {"key": "maxMatchingValue", "type": "str"},
     }
 
-    def __init__(self, *, min_matching_value: Optional[str] = None, max_matching_value: Optional[str] = None, **kwargs):
+    def __init__(
+        self, *, min_matching_value: Optional[str] = None, max_matching_value: Optional[str] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword min_matching_value: minimum value for range prefix match.
         :paramtype min_matching_value: str
         :keyword max_matching_value: maximum value for range prefix match.
         :paramtype max_matching_value: str
         """
         super().__init__(**kwargs)
@@ -4813,16 +4997,16 @@
         creation_time: Optional[datetime.datetime] = None,
         expiry_time: Optional[datetime.datetime] = None,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         meta_data: Optional[str] = None,
         state: Optional[str] = None,
         type: Optional[str] = None,
         visible: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword creation_time:
         :paramtype creation_time: ~datetime.datetime
         :keyword expiry_time:
         :paramtype expiry_time: ~datetime.datetime
         :keyword id:
         :paramtype id: str
@@ -4878,16 +5062,16 @@
         *,
         restore_point_data_store_id: Optional[str] = None,
         is_visible: Optional[bool] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         extended_info: Optional[bool] = None,
         restore_point_state: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword restore_point_data_store_id:
         :paramtype restore_point_data_store_id: str
         :keyword is_visible:
         :paramtype is_visible: bool
         :keyword start_date:
         :paramtype start_date: str
@@ -4910,16 +5094,15 @@
 class ResourceGuard(_serialization.Model):
     """ResourceGuard.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar provisioning_state: Provisioning state of the BackupVault resource. Known values are:
      "Failed", "Provisioning", "Succeeded", "Unknown", and "Updating".
-    :vartype provisioning_state: str or
-     ~azure.mgmt.dataprotection.models.ResourceGuardProvisioningState
+    :vartype provisioning_state: str or ~azure.mgmt.dataprotection.models.ProvisioningState
     :ivar allow_auto_approvals: This flag indicates whether auto approval is allowed or not.
     :vartype allow_auto_approvals: bool
     :ivar resource_guard_operations: {readonly} List of operation details those are protected by
      the ResourceGuard resource.
     :vartype resource_guard_operations:
      list[~azure.mgmt.dataprotection.models.ResourceGuardOperation]
     :ivar vault_critical_operation_exclusion_list: List of critical operations which are not
@@ -4940,15 +5123,15 @@
         "provisioning_state": {"key": "provisioningState", "type": "str"},
         "allow_auto_approvals": {"key": "allowAutoApprovals", "type": "bool"},
         "resource_guard_operations": {"key": "resourceGuardOperations", "type": "[ResourceGuardOperation]"},
         "vault_critical_operation_exclusion_list": {"key": "vaultCriticalOperationExclusionList", "type": "[str]"},
         "description": {"key": "description", "type": "str"},
     }
 
-    def __init__(self, *, vault_critical_operation_exclusion_list: Optional[List[str]] = None, **kwargs):
+    def __init__(self, *, vault_critical_operation_exclusion_list: Optional[List[str]] = None, **kwargs: Any) -> None:
         """
         :keyword vault_critical_operation_exclusion_list: List of critical operations which are not
          protected by this resourceGuard.
         :paramtype vault_critical_operation_exclusion_list: list[str]
         """
         super().__init__(**kwargs)
         self.provisioning_state = None
@@ -4975,23 +5158,23 @@
     }
 
     _attribute_map = {
         "vault_critical_operation": {"key": "vaultCriticalOperation", "type": "str"},
         "request_resource_type": {"key": "requestResourceType", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.vault_critical_operation = None
         self.request_resource_type = None
 
 
 class ResourceGuardOperationDetail(_serialization.Model):
-    """ResourceGuardOperationDetail.
+    """VaultCritical Operation protected by a resource guard.
 
     :ivar vault_critical_operation:
     :vartype vault_critical_operation: str
     :ivar default_resource_request:
     :vartype default_resource_request: str
     """
 
@@ -5001,29 +5184,29 @@
     }
 
     def __init__(
         self,
         *,
         vault_critical_operation: Optional[str] = None,
         default_resource_request: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword vault_critical_operation:
         :paramtype vault_critical_operation: str
         :keyword default_resource_request:
         :paramtype default_resource_request: str
         """
         super().__init__(**kwargs)
         self.vault_critical_operation = vault_critical_operation
         self.default_resource_request = default_resource_request
 
 
 class ResourceGuardProxyBase(_serialization.Model):
-    """ResourceGuardProxyBase.
+    """ResourceGuardProxyBase object, used in ResourceGuardProxyBaseResource.
 
     :ivar resource_guard_resource_id:
     :vartype resource_guard_resource_id: str
     :ivar resource_guard_operation_details:
     :vartype resource_guard_operation_details:
      list[~azure.mgmt.dataprotection.models.ResourceGuardOperationDetail]
     :ivar last_updated_time:
@@ -5045,16 +5228,16 @@
     def __init__(
         self,
         *,
         resource_guard_resource_id: Optional[str] = None,
         resource_guard_operation_details: Optional[List["_models.ResourceGuardOperationDetail"]] = None,
         last_updated_time: Optional[str] = None,
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword resource_guard_resource_id:
         :paramtype resource_guard_resource_id: str
         :keyword resource_guard_operation_details:
         :paramtype resource_guard_operation_details:
          list[~azure.mgmt.dataprotection.models.ResourceGuardOperationDetail]
         :keyword last_updated_time:
@@ -5066,15 +5249,16 @@
         self.resource_guard_resource_id = resource_guard_resource_id
         self.resource_guard_operation_details = resource_guard_operation_details
         self.last_updated_time = last_updated_time
         self.description = description
 
 
 class ResourceGuardProxyBaseResource(DppResource):
-    """ResourceGuardProxyBaseResource.
+    """ResourceGuardProxyBaseResource object, used for response and request bodies for
+    ResourceGuardProxy APIs.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Resource Id represents the complete path to the resource.
     :vartype id: str
     :ivar name: Resource name associated with the resource.
     :vartype name: str
@@ -5098,15 +5282,15 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "ResourceGuardProxyBase"},
     }
 
-    def __init__(self, *, properties: Optional["_models.ResourceGuardProxyBase"] = None, **kwargs):
+    def __init__(self, *, properties: Optional["_models.ResourceGuardProxyBase"] = None, **kwargs: Any) -> None:
         """
         :keyword properties: ResourceGuardProxyBaseResource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBase
         """
         super().__init__(**kwargs)
         self.properties = properties
 
@@ -5127,38 +5311,36 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.ResourceGuardProxyBaseResource"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource]
         """
         super().__init__(next_link=next_link, **kwargs)
         self.value = value
 
 
-class ResourceGuardResource(DppTrackedResource):
+class ResourceGuardResource(DppBaseTrackedResource):
     """ResourceGuardResource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar e_tag: Optional ETag.
     :vartype e_tag: str
     :ivar id: Resource Id represents the complete path to the resource.
     :vartype id: str
-    :ivar identity: Input Managed Identity Details.
-    :vartype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
     :ivar location: Resource location.
     :vartype location: str
     :ivar name: Resource name associated with the resource.
     :vartype name: str
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar type: Resource type represents the complete path of the form
@@ -5176,46 +5358,42 @@
         "type": {"readonly": True},
         "system_data": {"readonly": True},
     }
 
     _attribute_map = {
         "e_tag": {"key": "eTag", "type": "str"},
         "id": {"key": "id", "type": "str"},
-        "identity": {"key": "identity", "type": "DppIdentityDetails"},
         "location": {"key": "location", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "tags": {"key": "tags", "type": "{str}"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "properties": {"key": "properties", "type": "ResourceGuard"},
     }
 
     def __init__(
         self,
         *,
         e_tag: Optional[str] = None,
-        identity: Optional["_models.DppIdentityDetails"] = None,
         location: Optional[str] = None,
         tags: Optional[Dict[str, str]] = None,
         properties: Optional["_models.ResourceGuard"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword e_tag: Optional ETag.
         :paramtype e_tag: str
-        :keyword identity: Input Managed Identity Details.
-        :paramtype identity: ~azure.mgmt.dataprotection.models.DppIdentityDetails
         :keyword location: Resource location.
         :paramtype location: str
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword properties: ResourceGuardResource properties.
         :paramtype properties: ~azure.mgmt.dataprotection.models.ResourceGuard
         """
-        super().__init__(e_tag=e_tag, identity=identity, location=location, tags=tags, **kwargs)
+        super().__init__(e_tag=e_tag, location=location, tags=tags, **kwargs)
         self.properties = properties
 
 
 class ResourceGuardResourceList(DppTrackedResourceList):
     """List of ResourceGuard resources.
 
     :ivar next_link: The uri to fetch the next page of resources. Call ListNext() fetches next page
@@ -5231,16 +5409,16 @@
     }
 
     def __init__(
         self,
         *,
         next_link: Optional[str] = None,
         value: Optional[List["_models.ResourceGuardResource"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The uri to fetch the next page of resources. Call ListNext() fetches next
          page of resources.
         :paramtype next_link: str
         :keyword value: List of resources.
         :paramtype value: list[~azure.mgmt.dataprotection.models.ResourceGuardResource]
         """
@@ -5278,16 +5456,16 @@
         self,
         *,
         operation_id: Optional[str] = None,
         start_time_utc: Optional[str] = None,
         completion_time_utc: Optional[str] = None,
         source_resource_path: Optional[str] = None,
         target_resource_path: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword operation_id: CorrelationId of latest ResourceMove operation attempted.
         :paramtype operation_id: str
         :keyword start_time_utc: Start time in UTC of latest ResourceMove operation attempted. ISO 8601
          format.
         :paramtype start_time_utc: str
         :keyword completion_time_utc: Completion time in UTC of latest ResourceMove operation
@@ -5327,15 +5505,15 @@
 
     _attribute_map = {
         "start_time": {"key": "startTime", "type": "str"},
         "end_time": {"key": "endTime", "type": "str"},
         "object_type": {"key": "objectType", "type": "str"},
     }
 
-    def __init__(self, *, start_time: str, end_time: str, object_type: Optional[str] = None, **kwargs):
+    def __init__(self, *, start_time: str, end_time: str, object_type: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword start_time: Start time for the available restore range. Required.
         :paramtype start_time: str
         :keyword end_time: End time for the available restore range. Required.
         :paramtype end_time: str
         :keyword object_type:
         :paramtype object_type: str
@@ -5378,16 +5556,16 @@
 
     def __init__(
         self,
         *,
         recovery_option: Union[str, "_models.RecoveryOption"],
         target_details: "_models.TargetDetails",
         restore_location: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword recovery_option: Recovery Option. Required. "FailIfExists"
         :paramtype recovery_option: str or ~azure.mgmt.dataprotection.models.RecoveryOption
         :keyword restore_location: Target Restore region.
         :paramtype restore_location: str
         :keyword target_details: Destination of RestoreAsFiles operation, when destination is not a
          datasource. Required.
@@ -5413,16 +5591,16 @@
     }
 
     def __init__(
         self,
         *,
         recovery_point_id: Optional[str] = None,
         recovery_point_time: Optional[datetime.datetime] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword recovery_point_id:
         :paramtype recovery_point_id: str
         :keyword recovery_point_time:
         :paramtype recovery_point_time: ~datetime.datetime
         """
         super().__init__(**kwargs)
@@ -5470,16 +5648,16 @@
         self,
         *,
         recovery_option: Union[str, "_models.RecoveryOption"],
         datasource_info: "_models.Datasource",
         restore_location: Optional[str] = None,
         datasource_set_info: Optional["_models.DatasourceSet"] = None,
         datasource_auth_credentials: Optional["_models.AuthCredentials"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword recovery_option: Recovery Option. Required. "FailIfExists"
         :paramtype recovery_option: str or ~azure.mgmt.dataprotection.models.RecoveryOption
         :keyword restore_location: Target Restore region.
         :paramtype restore_location: str
         :keyword datasource_info: Information of target DS. Required.
         :paramtype datasource_info: ~azure.mgmt.dataprotection.models.Datasource
@@ -5519,15 +5697,15 @@
 
     _attribute_map = {
         "e_tag": {"key": "eTag", "type": "str"},
         "id": {"key": "id", "type": "str"},
         "tag_name": {"key": "tagName", "type": "str"},
     }
 
-    def __init__(self, *, tag_name: str, **kwargs):
+    def __init__(self, *, tag_name: str, **kwargs: Any) -> None:
         """
         :keyword tag_name: Retention Tag Name to relate it to retention rule. Required.
         :paramtype tag_name: str
         """
         super().__init__(**kwargs)
         self.e_tag = None
         self.id = None
@@ -5576,16 +5754,16 @@
         *,
         absolute_criteria: Optional[List[Union[str, "_models.AbsoluteMarker"]]] = None,
         days_of_month: Optional[List["_models.Day"]] = None,
         days_of_the_week: Optional[List[Union[str, "_models.DayOfWeek"]]] = None,
         months_of_year: Optional[List[Union[str, "_models.Month"]]] = None,
         schedule_times: Optional[List[datetime.datetime]] = None,
         weeks_of_the_month: Optional[List[Union[str, "_models.WeekNumber"]]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword absolute_criteria: it contains absolute values like "AllBackup" / "FirstOfDay" /
          "FirstOfWeek" / "FirstOfMonth"
          and should be part of AbsoluteMarker enum.
         :paramtype absolute_criteria: list[str or ~azure.mgmt.dataprotection.models.AbsoluteMarker]
         :keyword days_of_month: This is day of the month from 1 to 28 other wise last of month.
         :paramtype days_of_month: list[~azure.mgmt.dataprotection.models.Day]
@@ -5630,16 +5808,16 @@
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "schedule": {"key": "schedule", "type": "BackupSchedule"},
         "tagging_criteria": {"key": "taggingCriteria", "type": "[TaggingCriteria]"},
     }
 
     def __init__(
-        self, *, schedule: "_models.BackupSchedule", tagging_criteria: List["_models.TaggingCriteria"], **kwargs
-    ):
+        self, *, schedule: "_models.BackupSchedule", tagging_criteria: List["_models.TaggingCriteria"], **kwargs: Any
+    ) -> None:
         """
         :keyword schedule: Schedule for this backup. Required.
         :paramtype schedule: ~azure.mgmt.dataprotection.models.BackupSchedule
         :keyword tagging_criteria: List of tags that can be applicable for given schedule. Required.
         :paramtype tagging_criteria: list[~azure.mgmt.dataprotection.models.TaggingCriteria]
         """
         super().__init__(**kwargs)
@@ -5664,15 +5842,15 @@
     }
 
     _attribute_map = {
         "object_type": {"key": "objectType", "type": "str"},
         "secret_store_resource": {"key": "secretStoreResource", "type": "SecretStoreResource"},
     }
 
-    def __init__(self, *, secret_store_resource: Optional["_models.SecretStoreResource"] = None, **kwargs):
+    def __init__(self, *, secret_store_resource: Optional["_models.SecretStoreResource"] = None, **kwargs: Any) -> None:
         """
         :keyword secret_store_resource: Secret store resource.
         :paramtype secret_store_resource: ~azure.mgmt.dataprotection.models.SecretStoreResource
         """
         super().__init__(**kwargs)
         self.object_type: str = "SecretStoreBasedAuthCredentials"
         self.secret_store_resource = secret_store_resource
@@ -5704,16 +5882,16 @@
 
     def __init__(
         self,
         *,
         secret_store_type: Union[str, "_models.SecretStoreType"],
         uri: Optional[str] = None,
         value: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword uri: Uri to get to the resource.
         :paramtype uri: str
         :keyword secret_store_type: Gets or sets the type of secret store. Required. Known values are:
          "Invalid" and "AzureKeyVault".
         :paramtype secret_store_type: str or ~azure.mgmt.dataprotection.models.SecretStoreType
         :keyword value: Gets or sets value stored in secret store resource.
@@ -5740,16 +5918,16 @@
     }
 
     def __init__(
         self,
         *,
         soft_delete_settings: Optional["_models.SoftDeleteSettings"] = None,
         immutability_settings: Optional["_models.ImmutabilitySettings"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword soft_delete_settings: Soft delete related settings.
         :paramtype soft_delete_settings: ~azure.mgmt.dataprotection.models.SoftDeleteSettings
         :keyword immutability_settings: Immutability Settings at vault level.
         :paramtype immutability_settings: ~azure.mgmt.dataprotection.models.ImmutabilitySettings
         """
         super().__init__(**kwargs)
@@ -5772,16 +5950,16 @@
     }
 
     def __init__(
         self,
         *,
         state: Optional[Union[str, "_models.SoftDeleteState"]] = None,
         retention_duration_in_days: Optional[float] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword state: State of soft delete. Known values are: "Off", "On", and "AlwaysOn".
         :paramtype state: str or ~azure.mgmt.dataprotection.models.SoftDeleteState
         :keyword retention_duration_in_days: Soft delete retention duration.
         :paramtype retention_duration_in_days: float
         """
         super().__init__(**kwargs)
@@ -5816,16 +5994,16 @@
 
     def __init__(
         self,
         *,
         delete_after: "_models.DeleteOption",
         source_data_store: "_models.DataStoreInfoBase",
         target_data_store_copy_settings: Optional[List["_models.TargetCopySetting"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword delete_after: Delete Option. Required.
         :paramtype delete_after: ~azure.mgmt.dataprotection.models.DeleteOption
         :keyword source_data_store: DataStoreInfo base. Required.
         :paramtype source_data_store: ~azure.mgmt.dataprotection.models.DataStoreInfoBase
         :keyword target_data_store_copy_settings:
         :paramtype target_data_store_copy_settings:
@@ -5837,15 +6015,15 @@
         self.target_data_store_copy_settings = target_data_store_copy_settings
 
 
 class StorageSetting(_serialization.Model):
     """Storage setting.
 
     :ivar datastore_type: Gets or sets the type of the datastore. Known values are: "ArchiveStore",
-     "SnapshotStore", and "VaultStore".
+     "OperationalStore", and "VaultStore".
     :vartype datastore_type: str or ~azure.mgmt.dataprotection.models.StorageSettingStoreTypes
     :ivar type: Gets or sets the type. Known values are: "GeoRedundant", "LocallyRedundant", and
      "ZoneRedundant".
     :vartype type: str or ~azure.mgmt.dataprotection.models.StorageSettingTypes
     """
 
     _attribute_map = {
@@ -5854,19 +6032,19 @@
     }
 
     def __init__(
         self,
         *,
         datastore_type: Optional[Union[str, "_models.StorageSettingStoreTypes"]] = None,
         type: Optional[Union[str, "_models.StorageSettingTypes"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword datastore_type: Gets or sets the type of the datastore. Known values are:
-         "ArchiveStore", "SnapshotStore", and "VaultStore".
+         "ArchiveStore", "OperationalStore", and "VaultStore".
         :paramtype datastore_type: str or ~azure.mgmt.dataprotection.models.StorageSettingStoreTypes
         :keyword type: Gets or sets the type. Known values are: "GeoRedundant", "LocallyRedundant", and
          "ZoneRedundant".
         :paramtype type: str or ~azure.mgmt.dataprotection.models.StorageSettingTypes
         """
         super().__init__(**kwargs)
         self.datastore_type = datastore_type
@@ -5893,16 +6071,16 @@
 
     def __init__(
         self,
         *,
         feature_name: Optional[str] = None,
         support_status: Optional[Union[str, "_models.FeatureSupportStatus"]] = None,
         exposure_controlled_features: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword feature_name: support feature type.
         :paramtype feature_name: str
         :keyword support_status: feature support status. Known values are: "Invalid", "NotSupported",
          "AlphaPreview", "PrivatePreview", "PublicPreview", and "GenerallyAvailable".
         :paramtype support_status: str or ~azure.mgmt.dataprotection.models.FeatureSupportStatus
         :keyword exposure_controlled_features: support feature type.
@@ -5922,15 +6100,15 @@
     :vartype sync_type: str or ~azure.mgmt.dataprotection.models.SyncType
     """
 
     _attribute_map = {
         "sync_type": {"key": "syncType", "type": "str"},
     }
 
-    def __init__(self, *, sync_type: Optional[Union[str, "_models.SyncType"]] = None, **kwargs):
+    def __init__(self, *, sync_type: Optional[Union[str, "_models.SyncType"]] = None, **kwargs: Any) -> None:
         """
         :keyword sync_type: Field indicating sync type e.g. to sync only in case of failure or in all
          cases. Known values are: "Default" and "ForceResync".
         :paramtype sync_type: str or ~azure.mgmt.dataprotection.models.SyncType
         """
         super().__init__(**kwargs)
         self.sync_type = sync_type
@@ -5947,15 +6125,15 @@
     :ivar created_at: The timestamp of resource creation (UTC).
     :vartype created_at: ~datetime.datetime
     :ivar last_modified_by: The identity that last modified the resource.
     :vartype last_modified_by: str
     :ivar last_modified_by_type: The type of identity that last modified the resource. Known values
      are: "User", "Application", "ManagedIdentity", and "Key".
     :vartype last_modified_by_type: str or ~azure.mgmt.dataprotection.models.CreatedByType
-    :ivar last_modified_at: The type of identity that last modified the resource.
+    :ivar last_modified_at: The timestamp of resource last modification (UTC).
     :vartype last_modified_at: ~datetime.datetime
     """
 
     _attribute_map = {
         "created_by": {"key": "createdBy", "type": "str"},
         "created_by_type": {"key": "createdByType", "type": "str"},
         "created_at": {"key": "createdAt", "type": "iso-8601"},
@@ -5969,30 +6147,30 @@
         *,
         created_by: Optional[str] = None,
         created_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
         last_modified_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         last_modified_at: Optional[datetime.datetime] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
         :keyword created_by_type: The type of identity that created the resource. Known values are:
          "User", "Application", "ManagedIdentity", and "Key".
         :paramtype created_by_type: str or ~azure.mgmt.dataprotection.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: The identity that last modified the resource.
         :paramtype last_modified_by: str
         :keyword last_modified_by_type: The type of identity that last modified the resource. Known
          values are: "User", "Application", "ManagedIdentity", and "Key".
         :paramtype last_modified_by_type: str or ~azure.mgmt.dataprotection.models.CreatedByType
-        :keyword last_modified_at: The type of identity that last modified the resource.
+        :keyword last_modified_at: The timestamp of resource last modification (UTC).
         :paramtype last_modified_at: ~datetime.datetime
         """
         super().__init__(**kwargs)
         self.created_by = created_by
         self.created_by_type = created_by_type
         self.created_at = created_at
         self.last_modified_by = last_modified_by
@@ -6031,16 +6209,16 @@
     def __init__(
         self,
         *,
         is_default: bool,
         tagging_priority: int,
         tag_info: "_models.RetentionTag",
         criteria: Optional[List["_models.BackupCriteria"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword criteria: Criteria which decides whether the tag can be applied to a triggered backup.
         :paramtype criteria: list[~azure.mgmt.dataprotection.models.BackupCriteria]
         :keyword is_default: Specifies if tag is default. Required.
         :paramtype is_default: bool
         :keyword tagging_priority: Retention Tag priority. Required.
         :paramtype tagging_priority: int
@@ -6071,15 +6249,17 @@
     }
 
     _attribute_map = {
         "copy_after": {"key": "copyAfter", "type": "CopyOption"},
         "data_store": {"key": "dataStore", "type": "DataStoreInfoBase"},
     }
 
-    def __init__(self, *, copy_after: "_models.CopyOption", data_store: "_models.DataStoreInfoBase", **kwargs):
+    def __init__(
+        self, *, copy_after: "_models.CopyOption", data_store: "_models.DataStoreInfoBase", **kwargs: Any
+    ) -> None:
         """
         :keyword copy_after: It can be CustomCopyOption or ImmediateCopyOption. Required.
         :paramtype copy_after: ~azure.mgmt.dataprotection.models.CopyOption
         :keyword data_store: Info of target datastore. Required.
         :paramtype data_store: ~azure.mgmt.dataprotection.models.DataStoreInfoBase
         """
         super().__init__(**kwargs)
@@ -6101,36 +6281,44 @@
      {Microsoft.Internal.AzureBackup.DataProtection.Common.Interface.RestoreTargetLocationType}.
      Required. Known values are: "Invalid", "AzureBlobs", and "AzureFiles".
     :vartype restore_target_location_type: str or
      ~azure.mgmt.dataprotection.models.RestoreTargetLocationType
     :ivar url: Url denoting the restore destination. It can point to container / file share etc.
      Required.
     :vartype url: str
+    :ivar target_resource_arm_id: Full ARM Id denoting the restore destination. It is the ARM Id
+     pointing to container / file share
+     This is optional if the target subscription can be identified with the URL field. If not
+     then this is needed if CrossSubscriptionRestore field of BackupVault is in any of the disabled
+     states.
+    :vartype target_resource_arm_id: str
     """
 
     _validation = {
         "file_prefix": {"required": True},
         "restore_target_location_type": {"required": True},
         "url": {"required": True},
     }
 
     _attribute_map = {
         "file_prefix": {"key": "filePrefix", "type": "str"},
         "restore_target_location_type": {"key": "restoreTargetLocationType", "type": "str"},
         "url": {"key": "url", "type": "str"},
+        "target_resource_arm_id": {"key": "targetResourceArmId", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         file_prefix: str,
         restore_target_location_type: Union[str, "_models.RestoreTargetLocationType"],
         url: str,
-        **kwargs
-    ):
+        target_resource_arm_id: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword file_prefix: Restore operation may create multiple files inside location pointed by
          Url
          Below will be the common prefix for all of them. Required.
         :paramtype file_prefix: str
         :keyword restore_target_location_type: Denotes the target location where the data will be
          restored,
@@ -6138,19 +6326,26 @@
          {Microsoft.Internal.AzureBackup.DataProtection.Common.Interface.RestoreTargetLocationType}.
          Required. Known values are: "Invalid", "AzureBlobs", and "AzureFiles".
         :paramtype restore_target_location_type: str or
          ~azure.mgmt.dataprotection.models.RestoreTargetLocationType
         :keyword url: Url denoting the restore destination. It can point to container / file share etc.
          Required.
         :paramtype url: str
+        :keyword target_resource_arm_id: Full ARM Id denoting the restore destination. It is the ARM Id
+         pointing to container / file share
+         This is optional if the target subscription can be identified with the URL field. If not
+         then this is needed if CrossSubscriptionRestore field of BackupVault is in any of the disabled
+         states.
+        :paramtype target_resource_arm_id: str
         """
         super().__init__(**kwargs)
         self.file_prefix = file_prefix
         self.restore_target_location_type = restore_target_location_type
         self.url = url
+        self.target_resource_arm_id = target_resource_arm_id
 
 
 class TriggerBackupRequest(_serialization.Model):
     """Trigger backup request.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -6163,15 +6358,15 @@
         "backup_rule_options": {"required": True},
     }
 
     _attribute_map = {
         "backup_rule_options": {"key": "backupRuleOptions", "type": "AdHocBackupRuleOptions"},
     }
 
-    def __init__(self, *, backup_rule_options: "_models.AdHocBackupRuleOptions", **kwargs):
+    def __init__(self, *, backup_rule_options: "_models.AdHocBackupRuleOptions", **kwargs: Any) -> None:
         """
         :keyword backup_rule_options: Name for the Rule of the Policy which needs to be applied for
          this backup. Required.
         :paramtype backup_rule_options: ~azure.mgmt.dataprotection.models.AdHocBackupRuleOptions
         """
         super().__init__(**kwargs)
         self.backup_rule_options = backup_rule_options
@@ -6192,16 +6387,16 @@
     }
 
     def __init__(
         self,
         *,
         resource_guard_operation_requests: Optional[List[str]] = None,
         resource_to_be_deleted: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword resource_guard_operation_requests:
         :paramtype resource_guard_operation_requests: list[str]
         :keyword resource_to_be_deleted:
         :paramtype resource_to_be_deleted: str
         """
         super().__init__(**kwargs)
@@ -6217,15 +6412,15 @@
     :vartype unlock_delete_expiry_time: str
     """
 
     _attribute_map = {
         "unlock_delete_expiry_time": {"key": "unlockDeleteExpiryTime", "type": "str"},
     }
 
-    def __init__(self, *, unlock_delete_expiry_time: Optional[str] = None, **kwargs):
+    def __init__(self, *, unlock_delete_expiry_time: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword unlock_delete_expiry_time: This is the time when unlock delete privileges will get
          expired.
         :paramtype unlock_delete_expiry_time: str
         """
         super().__init__(**kwargs)
         self.unlock_delete_expiry_time = unlock_delete_expiry_time
@@ -6274,16 +6469,16 @@
         inner_error: Optional["_models.InnerError"] = None,
         is_retryable: Optional[bool] = None,
         is_user_error: Optional[bool] = None,
         properties: Optional[Dict[str, str]] = None,
         message: Optional[str] = None,
         recommended_action: Optional[List[str]] = None,
         target: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword code: Unique code for this error.
         :paramtype code: str
         :keyword details: Additional related Errors.
         :paramtype details: list[~azure.mgmt.dataprotection.models.UserFacingError]
         :keyword inner_error: Inner Error.
         :paramtype inner_error: ~azure.mgmt.dataprotection.models.InnerError
@@ -6325,15 +6520,15 @@
         "backup_instance": {"required": True},
     }
 
     _attribute_map = {
         "backup_instance": {"key": "backupInstance", "type": "BackupInstance"},
     }
 
-    def __init__(self, *, backup_instance: "_models.BackupInstance", **kwargs):
+    def __init__(self, *, backup_instance: "_models.BackupInstance", **kwargs: Any) -> None:
         """
         :keyword backup_instance: Backup Instance. Required.
         :paramtype backup_instance: ~azure.mgmt.dataprotection.models.BackupInstance
         """
         super().__init__(**kwargs)
         self.backup_instance = backup_instance
 
@@ -6351,14 +6546,14 @@
         "restore_request_object": {"required": True},
     }
 
     _attribute_map = {
         "restore_request_object": {"key": "restoreRequestObject", "type": "AzureBackupRestoreRequest"},
     }
 
-    def __init__(self, *, restore_request_object: "_models.AzureBackupRestoreRequest", **kwargs):
+    def __init__(self, *, restore_request_object: "_models.AzureBackupRestoreRequest", **kwargs: Any) -> None:
         """
         :keyword restore_request_object: Gets or sets the restore request object. Required.
         :paramtype restore_request_object: ~azure.mgmt.dataprotection.models.AzureBackupRestoreRequest
         """
         super().__init__(**kwargs)
         self.restore_request_object = restore_request_object
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/__init__.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,37 +55,40 @@
 from ._models_py3 import ClientDiscoveryForLogSpecification
 from ._models_py3 import ClientDiscoveryForProperties
 from ._models_py3 import ClientDiscoveryForServiceSpecification
 from ._models_py3 import ClientDiscoveryResponse
 from ._models_py3 import ClientDiscoveryValueForSingleApi
 from ._models_py3 import CopyOnExpiryOption
 from ._models_py3 import CopyOption
+from ._models_py3 import CrossSubscriptionRestoreSettings
 from ._models_py3 import CustomCopyOption
 from ._models_py3 import DataStoreInfoBase
 from ._models_py3 import DataStoreParameters
 from ._models_py3 import Datasource
 from ._models_py3 import DatasourceSet
 from ._models_py3 import Day
 from ._models_py3 import DeleteOption
 from ._models_py3 import DeletedBackupInstance
 from ._models_py3 import DeletedBackupInstanceResource
 from ._models_py3 import DeletedBackupInstanceResourceList
 from ._models_py3 import DeletionInfo
 from ._models_py3 import DppBaseResource
 from ._models_py3 import DppBaseResourceList
+from ._models_py3 import DppBaseTrackedResource
 from ._models_py3 import DppIdentityDetails
 from ._models_py3 import DppProxyResource
 from ._models_py3 import DppResource
 from ._models_py3 import DppResourceList
 from ._models_py3 import DppTrackedResource
 from ._models_py3 import DppTrackedResourceList
 from ._models_py3 import DppWorkerRequest
 from ._models_py3 import Error
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ExportJobsResult
+from ._models_py3 import FeatureSettings
 from ._models_py3 import FeatureValidationRequest
 from ._models_py3 import FeatureValidationRequestBase
 from ._models_py3 import FeatureValidationResponse
 from ._models_py3 import FeatureValidationResponseBase
 from ._models_py3 import ImmediateCopyOption
 from ._models_py3 import ImmutabilitySettings
 from ._models_py3 import InnerError
@@ -99,14 +102,15 @@
 from ._models_py3 import KubernetesPVRestoreCriteria
 from ._models_py3 import KubernetesStorageClassRestoreCriteria
 from ._models_py3 import MonitoringSettings
 from ._models_py3 import OperationExtendedInfo
 from ._models_py3 import OperationJobExtendedInfo
 from ._models_py3 import OperationResource
 from ._models_py3 import PatchBackupVaultInput
+from ._models_py3 import PatchResourceGuardInput
 from ._models_py3 import PatchResourceRequestInput
 from ._models_py3 import PolicyInfo
 from ._models_py3 import PolicyParameters
 from ._models_py3 import ProtectionStatusDetails
 from ._models_py3 import RangeBasedItemLevelRestoreCriteria
 from ._models_py3 import RecoveryPointDataStoreDetails
 from ._models_py3 import RecoveryPointsFilters
@@ -143,43 +147,43 @@
 from ._models_py3 import TriggerContext
 from ._models_py3 import UnlockDeleteRequest
 from ._models_py3 import UnlockDeleteResponse
 from ._models_py3 import UserFacingError
 from ._models_py3 import ValidateForBackupRequest
 from ._models_py3 import ValidateRestoreRequestObject
 
-from ._data_protection_client_enums import AbsoluteMarker
-from ._data_protection_client_enums import AlertsState
-from ._data_protection_client_enums import CreatedByType
-from ._data_protection_client_enums import CurrentProtectionState
-from ._data_protection_client_enums import DataStoreTypes
-from ._data_protection_client_enums import DayOfWeek
-from ._data_protection_client_enums import ExistingResourcePolicy
-from ._data_protection_client_enums import FeatureSupportStatus
-from ._data_protection_client_enums import FeatureType
-from ._data_protection_client_enums import ImmutabilityState
-from ._data_protection_client_enums import Month
-from ._data_protection_client_enums import PersistentVolumeRestoreMode
-from ._data_protection_client_enums import ProvisioningState
-from ._data_protection_client_enums import RecoveryOption
-from ._data_protection_client_enums import RehydrationPriority
-from ._data_protection_client_enums import RehydrationStatus
-from ._data_protection_client_enums import ResourceGuardProvisioningState
-from ._data_protection_client_enums import ResourceMoveState
-from ._data_protection_client_enums import RestoreSourceDataStoreType
-from ._data_protection_client_enums import RestoreTargetLocationType
-from ._data_protection_client_enums import SecretStoreType
-from ._data_protection_client_enums import SoftDeleteState
-from ._data_protection_client_enums import SourceDataStoreType
-from ._data_protection_client_enums import Status
-from ._data_protection_client_enums import StorageSettingStoreTypes
-from ._data_protection_client_enums import StorageSettingTypes
-from ._data_protection_client_enums import SyncType
-from ._data_protection_client_enums import ValidationType
-from ._data_protection_client_enums import WeekNumber
+from ._data_protection_mgmt_client_enums import AbsoluteMarker
+from ._data_protection_mgmt_client_enums import AlertsState
+from ._data_protection_mgmt_client_enums import CreatedByType
+from ._data_protection_mgmt_client_enums import CrossSubscriptionRestoreState
+from ._data_protection_mgmt_client_enums import CurrentProtectionState
+from ._data_protection_mgmt_client_enums import DataStoreTypes
+from ._data_protection_mgmt_client_enums import DayOfWeek
+from ._data_protection_mgmt_client_enums import ExistingResourcePolicy
+from ._data_protection_mgmt_client_enums import FeatureSupportStatus
+from ._data_protection_mgmt_client_enums import FeatureType
+from ._data_protection_mgmt_client_enums import ImmutabilityState
+from ._data_protection_mgmt_client_enums import Month
+from ._data_protection_mgmt_client_enums import PersistentVolumeRestoreMode
+from ._data_protection_mgmt_client_enums import ProvisioningState
+from ._data_protection_mgmt_client_enums import RecoveryOption
+from ._data_protection_mgmt_client_enums import RehydrationPriority
+from ._data_protection_mgmt_client_enums import RehydrationStatus
+from ._data_protection_mgmt_client_enums import ResourceMoveState
+from ._data_protection_mgmt_client_enums import RestoreSourceDataStoreType
+from ._data_protection_mgmt_client_enums import RestoreTargetLocationType
+from ._data_protection_mgmt_client_enums import SecretStoreType
+from ._data_protection_mgmt_client_enums import SoftDeleteState
+from ._data_protection_mgmt_client_enums import SourceDataStoreType
+from ._data_protection_mgmt_client_enums import Status
+from ._data_protection_mgmt_client_enums import StorageSettingStoreTypes
+from ._data_protection_mgmt_client_enums import StorageSettingTypes
+from ._data_protection_mgmt_client_enums import SyncType
+from ._data_protection_mgmt_client_enums import ValidationType
+from ._data_protection_mgmt_client_enums import WeekNumber
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AbsoluteDeleteOption",
     "AdHocBackupRuleOptions",
@@ -230,37 +234,40 @@
     "ClientDiscoveryForLogSpecification",
     "ClientDiscoveryForProperties",
     "ClientDiscoveryForServiceSpecification",
     "ClientDiscoveryResponse",
     "ClientDiscoveryValueForSingleApi",
     "CopyOnExpiryOption",
     "CopyOption",
+    "CrossSubscriptionRestoreSettings",
     "CustomCopyOption",
     "DataStoreInfoBase",
     "DataStoreParameters",
     "Datasource",
     "DatasourceSet",
     "Day",
     "DeleteOption",
     "DeletedBackupInstance",
     "DeletedBackupInstanceResource",
     "DeletedBackupInstanceResourceList",
     "DeletionInfo",
     "DppBaseResource",
     "DppBaseResourceList",
+    "DppBaseTrackedResource",
     "DppIdentityDetails",
     "DppProxyResource",
     "DppResource",
     "DppResourceList",
     "DppTrackedResource",
     "DppTrackedResourceList",
     "DppWorkerRequest",
     "Error",
     "ErrorAdditionalInfo",
     "ExportJobsResult",
+    "FeatureSettings",
     "FeatureValidationRequest",
     "FeatureValidationRequestBase",
     "FeatureValidationResponse",
     "FeatureValidationResponseBase",
     "ImmediateCopyOption",
     "ImmutabilitySettings",
     "InnerError",
@@ -274,14 +281,15 @@
     "KubernetesPVRestoreCriteria",
     "KubernetesStorageClassRestoreCriteria",
     "MonitoringSettings",
     "OperationExtendedInfo",
     "OperationJobExtendedInfo",
     "OperationResource",
     "PatchBackupVaultInput",
+    "PatchResourceGuardInput",
     "PatchResourceRequestInput",
     "PolicyInfo",
     "PolicyParameters",
     "ProtectionStatusDetails",
     "RangeBasedItemLevelRestoreCriteria",
     "RecoveryPointDataStoreDetails",
     "RecoveryPointsFilters",
@@ -320,28 +328,28 @@
     "UnlockDeleteResponse",
     "UserFacingError",
     "ValidateForBackupRequest",
     "ValidateRestoreRequestObject",
     "AbsoluteMarker",
     "AlertsState",
     "CreatedByType",
+    "CrossSubscriptionRestoreState",
     "CurrentProtectionState",
     "DataStoreTypes",
     "DayOfWeek",
     "ExistingResourcePolicy",
     "FeatureSupportStatus",
     "FeatureType",
     "ImmutabilityState",
     "Month",
     "PersistentVolumeRestoreMode",
     "ProvisioningState",
     "RecoveryOption",
     "RehydrationPriority",
     "RehydrationStatus",
-    "ResourceGuardProvisioningState",
     "ResourceMoveState",
     "RestoreSourceDataStoreType",
     "RestoreTargetLocationType",
     "SecretStoreType",
     "SoftDeleteState",
     "SourceDataStoreType",
     "Status",
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/models/_patch.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_data_protection_client.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_data_protection_mgmt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
-from ._configuration import DataProtectionClientConfiguration
+from ._configuration import DataProtectionMgmtClientConfiguration
 from .operations import (
-    BackupInstancesExtensionRoutingOperations,
     BackupInstancesOperations,
     BackupPoliciesOperations,
     BackupVaultOperationResultsOperations,
     BackupVaultsOperations,
     DataProtectionOperations,
     DataProtectionOperationsOperations,
     DeletedBackupInstancesOperations,
@@ -38,15 +37,15 @@
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class DataProtectionClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+class DataProtectionMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Open API 2.0 Specs for Azure Data Protection service.
 
     :ivar backup_vaults: BackupVaultsOperations operations
     :vartype backup_vaults: azure.mgmt.dataprotection.aio.operations.BackupVaultsOperations
     :ivar operation_result: OperationResultOperations operations
     :vartype operation_result: azure.mgmt.dataprotection.aio.operations.OperationResultOperations
     :ivar operation_status: OperationStatusOperations operations
@@ -67,17 +66,14 @@
     :ivar data_protection_operations: DataProtectionOperationsOperations operations
     :vartype data_protection_operations:
      azure.mgmt.dataprotection.aio.operations.DataProtectionOperationsOperations
     :ivar backup_policies: BackupPoliciesOperations operations
     :vartype backup_policies: azure.mgmt.dataprotection.aio.operations.BackupPoliciesOperations
     :ivar backup_instances: BackupInstancesOperations operations
     :vartype backup_instances: azure.mgmt.dataprotection.aio.operations.BackupInstancesOperations
-    :ivar backup_instances_extension_routing: BackupInstancesExtensionRoutingOperations operations
-    :vartype backup_instances_extension_routing:
-     azure.mgmt.dataprotection.aio.operations.BackupInstancesExtensionRoutingOperations
     :ivar recovery_points: RecoveryPointsOperations operations
     :vartype recovery_points: azure.mgmt.dataprotection.aio.operations.RecoveryPointsOperations
     :ivar jobs: JobsOperations operations
     :vartype jobs: azure.mgmt.dataprotection.aio.operations.JobsOperations
     :ivar restorable_time_ranges: RestorableTimeRangesOperations operations
     :vartype restorable_time_ranges:
      azure.mgmt.dataprotection.aio.operations.RestorableTimeRangesOperations
@@ -92,36 +88,36 @@
     :ivar resource_guards: ResourceGuardsOperations operations
     :vartype resource_guards: azure.mgmt.dataprotection.aio.operations.ResourceGuardsOperations
     :ivar dpp_resource_guard_proxy: DppResourceGuardProxyOperations operations
     :vartype dpp_resource_guard_proxy:
      azure.mgmt.dataprotection.aio.operations.DppResourceGuardProxyOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The subscription Id. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        self._config = DataProtectionClientConfiguration(
+        self._config = DataProtectionMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.backup_vaults = BackupVaultsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operation_result = OperationResultOperations(
@@ -143,17 +139,14 @@
         self.data_protection_operations = DataProtectionOperationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.backup_policies = BackupPoliciesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.backup_instances = BackupInstancesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.backup_instances_extension_routing = BackupInstancesExtensionRoutingOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.recovery_points = RecoveryPointsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.jobs = JobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.restorable_time_ranges = RestorableTimeRangesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.export_jobs = ExportJobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.export_jobs_operation_result = ExportJobsOperationResultOperations(
@@ -188,13 +181,13 @@
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, **kwargs)
 
     async def close(self) -> None:
         await self._client.close()
 
-    async def __aenter__(self) -> "DataProtectionClient":
+    async def __aenter__(self) -> "DataProtectionMgmtClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/__init__.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._data_protection_client import DataProtectionClient
+from ._data_protection_mgmt_client import DataProtectionMgmtClient
+from ._version import VERSION
+
+__version__ = VERSION
 
 try:
     from ._patch import __all__ as _patch_all
     from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "DataProtectionClient",
+    "DataProtectionMgmtClient",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_patch.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/_configuration.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,51 +2,45 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class DataProtectionClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
-    """Configuration for DataProtectionClient.
+class DataProtectionMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for DataProtectionMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The subscription Id. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-01-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(DataProtectionClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop("api_version", "2022-11-01-preview")
+        super(DataProtectionMgmtClientConfiguration, self).__init__(**kwargs)
+        api_version: str = kwargs.pop("api_version", "2023-01-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_dpp_resource_guard_proxy_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_dpp_resource_guard_proxy_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -26,36 +26,32 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._dpp_resource_guard_proxy_operations import (
+    build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
-    build_put_request,
     build_unlock_delete_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DppResourceGuardProxyOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`dpp_resource_guard_proxy` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -64,34 +60,34 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.ResourceGuardProxyBaseResource"]:
-        """list.
+        """Returns the list of ResourceGuardProxies associated with the vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        Returns the list of ResourceGuardProxies associated with the vault.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ResourceGuardProxyBaseResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardProxyBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -137,16 +133,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -158,22 +155,26 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies"
     }
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """get.
+        """Returns the ResourceGuardProxy object associated with the vault, and that matches the name in
+        the request.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        Returns the ResourceGuardProxy object associated with the vault, and that matches the name in
+        the request.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
@@ -183,17 +184,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardProxyBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             resource_guard_proxy_name=resource_guard_proxy_name,
             subscription_id=self._config.subscription_id,
@@ -201,16 +200,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -223,94 +223,101 @@
         return deserialized
 
     get.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}"
     }
 
     @overload
-    async def put(
+    async def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: _models.ResourceGuardProxyBaseResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """put.
+        """Creates or Updates a ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        Creates or Updates a ResourceGuardProxy.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def put(
+    async def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """put.
+        """Creates or Updates a ResourceGuardProxy.
+
+        Creates or Updates a ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
-    async def put(
+    async def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: Union[_models.ResourceGuardProxyBaseResource, IO],
         **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """put.
+        """Creates or Updates a ResourceGuardProxy.
+
+        Creates or Updates a ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ResourceGuardProxyBaseResource type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
@@ -323,46 +330,45 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ResourceGuardProxyBaseResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ResourceGuardProxyBaseResource")
 
-        request = build_put_request(
+        request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             resource_guard_proxy_name=resource_guard_proxy_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.put.metadata["url"],
+            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -370,30 +376,32 @@
         deserialized = self._deserialize("ResourceGuardProxyBaseResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    put.metadata = {
+    create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}"
     }
 
     @distributed_trace_async
     async def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, **kwargs: Any
     ) -> None:
-        """delete.
+        """Deletes the ResourceGuardProxy.
+
+        Deletes the ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
@@ -403,17 +411,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             resource_guard_proxy_name=resource_guard_proxy_name,
             subscription_id=self._config.subscription_id,
@@ -421,16 +427,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -449,22 +456,24 @@
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: _models.UnlockDeleteRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.UnlockDeleteResponse:
-        """unlock_delete.
+        """UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
+
+        UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.UnlockDeleteRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -480,22 +489,24 @@
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.UnlockDeleteResponse:
-        """unlock_delete.
+        """UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -509,24 +520,27 @@
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: Union[_models.UnlockDeleteRequest, IO],
         **kwargs: Any
     ) -> _models.UnlockDeleteResponse:
-        """unlock_delete.
+        """UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
+
+        UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a UnlockDeleteRequest type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.UnlockDeleteRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: UnlockDeleteResponse or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.UnlockDeleteResponse
@@ -539,24 +553,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.UnlockDeleteResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "UnlockDeleteRequest")
 
         request = build_unlock_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -569,16 +581,17 @@
             template_url=self.unlock_delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_result_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_result_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +23,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operation_result_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class OperationResultOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`operation_result` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -77,33 +72,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         request = build_get_request(
             operation_id=operation_id,
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_instances_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_instances_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -45,29 +45,25 @@
     build_sync_backup_instance_request,
     build_trigger_rehydrate_request,
     build_trigger_restore_request,
     build_validate_for_backup_request,
     build_validate_for_restore_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class BackupInstancesOperations:  # pylint: disable=too-many-public-methods
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`backup_instances` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -78,32 +74,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.BackupInstanceResource"]:
         """Gets a backup instances belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either BackupInstanceResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.BackupInstanceResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupInstanceResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -149,16 +143,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -172,15 +167,15 @@
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> _models.BackupInstanceResource:
         """Gets a backup instance with name in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -195,17 +190,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupInstanceResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -213,16 +206,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -253,24 +247,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.BackupInstanceResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "BackupInstanceResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -283,16 +275,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -329,15 +322,15 @@
         parameters: _models.BackupInstanceResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupInstanceResource]:
         """Create or update a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -369,15 +362,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupInstanceResource]:
         """Create or update a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -407,22 +400,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.BackupInstanceResource, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupInstanceResource]:
         """Create or update a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a BackupInstanceResource type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BackupInstanceResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -436,17 +430,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dataprotection.models.BackupInstanceResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupInstanceResource] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -498,17 +490,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -516,16 +506,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -547,15 +538,15 @@
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -569,17 +560,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -631,24 +620,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TriggerBackupRequest")
 
         request = build_adhoc_backup_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -661,16 +648,17 @@
             template_url=self._adhoc_backup_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -705,15 +693,15 @@
         parameters: _models.TriggerBackupRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Trigger adhoc backup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -745,15 +733,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Trigger adhoc backup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -783,22 +771,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.TriggerBackupRequest, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Trigger adhoc backup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a TriggerBackupRequest type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.TriggerBackupRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -812,17 +801,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._adhoc_backup_initial(
@@ -878,24 +865,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ValidateForBackupRequest")
 
         request = build_validate_for_backup_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -907,16 +892,17 @@
             template_url=self._validate_for_backup_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -950,15 +936,15 @@
         parameters: _models.ValidateForBackupRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Validate whether adhoc backup will be successful or not.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ValidateForBackupRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -987,15 +973,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Validate whether adhoc backup will be successful or not.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -1022,20 +1008,21 @@
         resource_group_name: str,
         vault_name: str,
         parameters: Union[_models.ValidateForBackupRequest, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Validate whether adhoc backup will be successful or not.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ValidateForBackupRequest type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ValidateForBackupRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1049,17 +1036,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._validate_for_backup_initial(
@@ -1102,20 +1087,20 @@
 
     @distributed_trace_async
     async def get_backup_instance_operation_result(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, operation_id: str, **kwargs: Any
     ) -> Optional[_models.BackupInstanceResource]:
         """Get result of backup instance creation operation.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param operation_id: Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: BackupInstanceResource or None or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.BackupInstanceResource or None
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1127,17 +1112,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.BackupInstanceResource]] = kwargs.pop("cls", None)
 
         request = build_get_backup_instance_operation_result_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             operation_id=operation_id,
@@ -1146,16 +1129,17 @@
             template_url=self.get_backup_instance_operation_result.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1188,24 +1172,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AzureBackupRehydrationRequest")
 
         request = build_trigger_rehydrate_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -1218,16 +1200,17 @@
             template_url=self._trigger_rehydrate_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1256,20 +1239,20 @@
         parameters: _models.AzureBackupRehydrationRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """rehydrate recovery point for restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupRehydrationRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1294,20 +1277,20 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """rehydrate recovery point for restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1330,22 +1313,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.AzureBackupRehydrationRequest, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """rehydrate recovery point for restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a AzureBackupRehydrationRequest type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupRehydrationRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1357,17 +1341,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._trigger_rehydrate_initial(  # type: ignore
@@ -1422,24 +1404,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AzureBackupRestoreRequest")
 
         request = build_trigger_restore_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -1452,16 +1432,17 @@
             template_url=self._trigger_restore_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1496,15 +1477,15 @@
         parameters: _models.AzureBackupRestoreRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Triggers restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -1536,15 +1517,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Triggers restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -1574,22 +1555,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.AzureBackupRestoreRequest, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Triggers restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a AzureBackupRestoreRequest type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupRestoreRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1603,17 +1585,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._trigger_restore_initial(
@@ -1665,17 +1645,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_resume_backups_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -1683,16 +1661,17 @@
             template_url=self._resume_backups_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1714,20 +1693,20 @@
 
     @distributed_trace_async
     async def begin_resume_backups(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """This operation will resume backups for backup instance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
@@ -1736,17 +1715,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._resume_backups_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1793,17 +1770,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_resume_protection_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -1811,16 +1786,17 @@
             template_url=self._resume_protection_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1842,20 +1818,20 @@
 
     @distributed_trace_async
     async def begin_resume_protection(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """This operation will resume protection for a stopped backup instance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
@@ -1864,17 +1840,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._resume_protection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1921,17 +1895,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_stop_protection_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -1939,16 +1911,17 @@
             template_url=self._stop_protection_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1970,20 +1943,20 @@
 
     @distributed_trace_async
     async def begin_stop_protection(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """This operation will stop protection of a backup instance and data will be held forever.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
@@ -1992,17 +1965,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._stop_protection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2049,17 +2020,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_suspend_backups_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -2067,16 +2036,17 @@
             template_url=self._suspend_backups_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2099,20 +2069,20 @@
     @distributed_trace_async
     async def begin_suspend_backups(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """This operation will stop backup for a backup instance and retains the backup data as per the
         policy (except latest Recovery point, which will be retained forever).
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
@@ -2121,17 +2091,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._suspend_backups_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2183,24 +2151,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SyncBackupInstanceRequest")
 
         request = build_sync_backup_instance_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -2213,16 +2179,17 @@
             template_url=self._sync_backup_instance_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2252,20 +2219,20 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Sync backup instance again in case of failure
         This action will retry last failed operation and will bring backup instance to valid state.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.SyncBackupInstanceRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2291,20 +2258,20 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Sync backup instance again in case of failure
         This action will retry last failed operation and will bring backup instance to valid state.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2328,22 +2295,23 @@
         backup_instance_name: str,
         parameters: Union[_models.SyncBackupInstanceRequest, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Sync backup instance again in case of failure
         This action will retry last failed operation and will bring backup instance to valid state.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a SyncBackupInstanceRequest type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.SyncBackupInstanceRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -2355,17 +2323,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._sync_backup_instance_initial(  # type: ignore
@@ -2420,24 +2386,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ValidateRestoreRequestObject")
 
         request = build_validate_for_restore_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -2450,16 +2414,17 @@
             template_url=self._validate_for_restore_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2494,15 +2459,15 @@
         parameters: _models.ValidateRestoreRequestObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Validates if Restore can be triggered for a DataSource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -2534,15 +2499,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Validates if Restore can be triggered for a DataSource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -2572,22 +2537,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.ValidateRestoreRequestObject, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.OperationJobExtendedInfo]:
         """Validates if Restore can be triggered for a DataSource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ValidateRestoreRequestObject type or
+         a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ValidateRestoreRequestObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -2601,17 +2567,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._validate_for_restore_initial(
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_export_jobs_operation_result_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_export_jobs_operation_result_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +23,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._export_jobs_operation_result_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ExportJobsOperationResultOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`export_jobs_operation_result` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -59,15 +54,15 @@
     async def get(
         self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
     ) -> Optional[_models.ExportJobsResult]:
         """Gets the operation result of operation triggered by Export Jobs API. If the operation is
         successful, then it also contains URL of a Blob and a SAS key to access the same. The blob
         contains exported jobs in JSON serialized format.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param operation_id: OperationID which represents the export job. Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -82,17 +77,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ExportJobsResult]] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
@@ -100,16 +93,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_instances_extension_routing_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_data_protection_operations_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -24,78 +23,68 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._backup_instances_extension_routing_operations import build_list_request
+from ...operations._data_protection_operations_operations import build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class BackupInstancesExtensionRoutingOperations:
+class DataProtectionOperationsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
-        :attr:`backup_instances_extension_routing` attribute.
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
+        :attr:`data_protection_operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, resource_id: str, **kwargs: Any) -> AsyncIterable["_models.BackupInstanceResource"]:
-        """Gets a list backup instances associated with a tracked resource.
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.ClientDiscoveryValueForSingleApi"]:
+        """Returns the list of available operations.
 
-        :param resource_id: ARM path of the resource to be protected using Microsoft.DataProtection.
-         Required.
-        :type resource_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either BackupInstanceResource or the result of
+        :return: An iterator like instance of either ClientDiscoveryValueForSingleApi or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.BackupInstanceResource]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.ClientDiscoveryValueForSingleApi]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.BackupInstanceResourceList] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ClientDiscoveryResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_list_request(
-                    resource_id=resource_id,
                     api_version=api_version,
                     template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
@@ -115,30 +104,31 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("BackupInstanceResourceList", pipeline_response)
+            deserialized = self._deserialize("ClientDiscoveryResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/{resourceId}/providers/Microsoft.DataProtection/backupInstances"}
+    list.metadata = {"url": "/providers/Microsoft.DataProtection/operations"}
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_policies_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_policies_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -32,29 +32,25 @@
 from ...operations._backup_policies_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class BackupPoliciesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`backup_policies` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -65,32 +61,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.BaseBackupPolicyResource"]:
         """Returns list of backup policies belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either BaseBackupPolicyResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.BaseBackupPolicyResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BaseBackupPolicyResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -136,16 +130,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -161,15 +156,15 @@
     async def get(
         self, resource_group_name: str, vault_name: str, backup_policy_name: str, **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Gets a backup policy belonging to a backup vault.
 
         Gets a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Required.
         :type backup_policy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -184,17 +179,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BaseBackupPolicyResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_policy_name=backup_policy_name,
             subscription_id=self._config.subscription_id,
@@ -202,16 +195,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -238,15 +232,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Creates or Updates a backup policy belonging to a backup vault.
 
         Creates or Updates a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Name of the policy. Required.
         :type backup_policy_name: str
         :param parameters: Request body for operation. Required.
@@ -271,15 +265,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Creates or Updates a backup policy belonging to a backup vault.
 
         Creates or Updates a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Name of the policy. Required.
         :type backup_policy_name: str
         :param parameters: Request body for operation. Required.
@@ -302,22 +296,23 @@
         parameters: Union[_models.BaseBackupPolicyResource, IO],
         **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Creates or Updates a backup policy belonging to a backup vault.
 
         Creates or Updates a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Name of the policy. Required.
         :type backup_policy_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a BaseBackupPolicyResource type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BaseBackupPolicyResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: BaseBackupPolicyResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.BaseBackupPolicyResource
@@ -330,24 +325,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BaseBackupPolicyResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "BaseBackupPolicyResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -360,16 +353,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -389,15 +383,15 @@
     async def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, backup_policy_name: str, **kwargs: Any
     ) -> None:
         """Deletes a backup policy belonging to a backup vault.
 
         Deletes a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Required.
         :type backup_policy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -412,17 +406,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_policy_name=backup_policy_name,
             subscription_id=self._config.subscription_id,
@@ -430,16 +422,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_vault_operation_results_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_vault_operation_results_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +23,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._backup_vault_operation_results_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class BackupVaultOperationResultsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`backup_vault_operation_results` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -57,15 +52,15 @@
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
     ) -> Optional[_models.BackupVaultResource]:
         """get.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -80,17 +75,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.BackupVaultResource]] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
@@ -98,16 +91,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_jobs_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_jobs_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -27,29 +26,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._jobs_operations import build_get_request, build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class JobsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`jobs` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -60,32 +55,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.AzureBackupJobResource"]:
         """Returns list of jobs belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either AzureBackupJobResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.AzureBackupJobResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupJobResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -131,16 +124,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -154,15 +148,15 @@
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, vault_name: str, job_id: str, **kwargs: Any
     ) -> _models.AzureBackupJobResource:
         """Gets a job with id in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param job_id: The Job ID. This is a GUID-formatted string (e.g.
          00000000-0000-0000-0000-000000000000). Required.
         :type job_id: str
@@ -178,17 +172,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupJobResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             job_id=job_id,
             subscription_id=self._config.subscription_id,
@@ -196,16 +188,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +23,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operation_status_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class OperationStatusOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`operation_status` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -77,33 +72,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             location=location,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_recovery_points_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_recovery_points_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -27,29 +26,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._recovery_points_operations import build_get_request, build_list_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class RecoveryPointsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`recovery_points` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -66,15 +61,15 @@
         backup_instance_name: str,
         filter: Optional[str] = None,
         skip_token: Optional[str] = None,
         **kwargs: Any
     ) -> AsyncIterable["_models.AzureBackupRecoveryPointResource"]:
         """Returns a list of Recovery Points for a DataSource in a vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param filter: OData filter options. Default value is None.
@@ -87,17 +82,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.AzureBackupRecoveryPointResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupRecoveryPointResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -146,16 +139,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -174,15 +168,15 @@
         vault_name: str,
         backup_instance_name: str,
         recovery_point_id: str,
         **kwargs: Any
     ) -> _models.AzureBackupRecoveryPointResource:
         """Gets a Recovery Point using recoveryPointId for a Datasource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param recovery_point_id: Required.
@@ -199,17 +193,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupRecoveryPointResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             recovery_point_id=recovery_point_id,
@@ -218,16 +210,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_data_protection_operations_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_data_protection_operations_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,82 +2,97 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._data_protection_operations_operations import build_list_request
-
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
+
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_list_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.DataProtection/operations")
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class DataProtectionOperationsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`data_protection_operations` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.ClientDiscoveryValueForSingleApi"]:
+    def list(self, **kwargs: Any) -> Iterable["_models.ClientDiscoveryValueForSingleApi"]:
         """Returns the list of available operations.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClientDiscoveryValueForSingleApi or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.ClientDiscoveryValueForSingleApi]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.ClientDiscoveryValueForSingleApi]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClientDiscoveryResponse] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -110,31 +125,32 @@
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("ClientDiscoveryResponse", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
+        def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
+        return ItemPaged(get_next, extract_data)
 
     list.metadata = {"url": "/providers/Microsoft.DataProtection/operations"}
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_restorable_time_ranges_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_restorable_time_ranges_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +24,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._restorable_time_ranges_operations import build_find_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class RestorableTimeRangesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`restorable_time_ranges` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -64,15 +60,15 @@
         parameters: _models.AzureBackupFindRestorableTimeRangesRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.AzureBackupFindRestorableTimeRangesResponseResource:
         """find.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -95,15 +91,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.AzureBackupFindRestorableTimeRangesResponseResource:
         """find.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -124,22 +120,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.AzureBackupFindRestorableTimeRangesRequest, IO],
         **kwargs: Any
     ) -> _models.AzureBackupFindRestorableTimeRangesResponseResource:
         """find.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a
+         AzureBackupFindRestorableTimeRangesRequest type or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupFindRestorableTimeRangesRequest
          or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AzureBackupFindRestorableTimeRangesResponseResource or the result of cls(response)
@@ -153,24 +150,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AzureBackupFindRestorableTimeRangesResponseResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AzureBackupFindRestorableTimeRangesRequest")
 
         request = build_find_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -183,16 +178,17 @@
             template_url=self.find.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_resource_group_context_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_resource_group_context_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +23,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operation_status_resource_group_context_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class OperationStatusResourceGroupContextOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`operation_status_resource_group_context` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -57,15 +52,15 @@
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, operation_id: str, **kwargs: Any) -> _models.OperationResource:
         """Gets the operation status for an operation over a ResourceGroup's context.
 
         Gets the operation status for an operation over a ResourceGroup's context.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param operation_id: Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.OperationResource
@@ -78,33 +73,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_operation_status_backup_vault_context_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_operation_status_backup_vault_context_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +23,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operation_status_backup_vault_context_operations import build_get_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class OperationStatusBackupVaultContextOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`operation_status_backup_vault_context` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -59,15 +54,15 @@
     async def get(
         self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
     ) -> _models.OperationResource:
         """Gets the operation status for an operation over a BackupVault's context.
 
         Gets the operation status for an operation over a BackupVault's context.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -82,17 +77,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
@@ -100,16 +93,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_export_jobs_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_export_jobs_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -26,29 +25,25 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._export_jobs_operations import build_trigger_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ExportJobsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`export_jobs` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -67,33 +62,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_trigger_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._trigger_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -110,15 +104,15 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/exportBackupJobs"
     }
 
     @distributed_trace_async
     async def begin_trigger(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Triggers export of jobs and returns an OperationID to track.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -130,17 +124,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._trigger_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/__init__.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from ._operation_status_backup_vault_context_operations import OperationStatusBackupVaultContextOperations
 from ._operation_status_resource_group_context_operations import OperationStatusResourceGroupContextOperations
 from ._backup_vault_operation_results_operations import BackupVaultOperationResultsOperations
 from ._data_protection_operations import DataProtectionOperations
 from ._data_protection_operations_operations import DataProtectionOperationsOperations
 from ._backup_policies_operations import BackupPoliciesOperations
 from ._backup_instances_operations import BackupInstancesOperations
-from ._backup_instances_extension_routing_operations import BackupInstancesExtensionRoutingOperations
 from ._recovery_points_operations import RecoveryPointsOperations
 from ._jobs_operations import JobsOperations
 from ._restorable_time_ranges_operations import RestorableTimeRangesOperations
 from ._export_jobs_operations import ExportJobsOperations
 from ._export_jobs_operation_result_operations import ExportJobsOperationResultOperations
 from ._deleted_backup_instances_operations import DeletedBackupInstancesOperations
 from ._resource_guards_operations import ResourceGuardsOperations
@@ -37,15 +36,14 @@
     "OperationStatusBackupVaultContextOperations",
     "OperationStatusResourceGroupContextOperations",
     "BackupVaultOperationResultsOperations",
     "DataProtectionOperations",
     "DataProtectionOperationsOperations",
     "BackupPoliciesOperations",
     "BackupInstancesOperations",
-    "BackupInstancesExtensionRoutingOperations",
     "RecoveryPointsOperations",
     "JobsOperations",
     "RestorableTimeRangesOperations",
     "ExportJobsOperations",
     "ExportJobsOperationResultOperations",
     "DeletedBackupInstancesOperations",
     "ResourceGuardsOperations",
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_patch.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_resource_guards_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_resource_guards_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -46,29 +46,25 @@
     build_get_resources_in_subscription_request,
     build_get_update_protected_item_requests_objects_request,
     build_get_update_protection_policy_requests_objects_request,
     build_patch_request,
     build_put_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ResourceGuardsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`resource_guards` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -89,17 +85,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.ResourceGuardResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -143,16 +137,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -168,30 +163,28 @@
     def get_resources_in_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.ResourceGuardResource"]:
         """Returns ResourceGuards collection belonging to a ResourceGroup.
 
         Returns ResourceGuards collection belonging to a ResourceGroup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ResourceGuardResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.ResourceGuardResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -236,16 +229,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -267,15 +261,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Creates or updates a ResourceGuard resource belonging to a resource group.
 
         Creates or updates a ResourceGuard resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -297,15 +291,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Creates or updates a ResourceGuard resource belonging to a resource group.
 
         Creates or updates a ResourceGuard resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -325,20 +319,21 @@
         parameters: Union[_models.ResourceGuardResource, IO],
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Creates or updates a ResourceGuard resource belonging to a resource group.
 
         Creates or updates a ResourceGuard resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ResourceGuardResource type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
@@ -351,24 +346,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ResourceGuardResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ResourceGuardResource")
 
         request = build_put_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
@@ -380,44 +373,49 @@
             template_url=self.put.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ResourceGuardResource", pipeline_response)
+        if response.status_code == 200:
+            deserialized = self._deserialize("ResourceGuardResource", pipeline_response)
+
+        if response.status_code == 201:
+            deserialized = self._deserialize("ResourceGuardResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     put.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}"
     }
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, resource_guards_name: str, **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Returns a ResourceGuard belonging to a resource group.
 
         Returns a ResourceGuard belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
@@ -430,33 +428,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -476,15 +473,15 @@
     async def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_guards_name: str, **kwargs: Any
     ) -> None:
         """Deletes a ResourceGuard resource from the resource group.
 
         Deletes a ResourceGuard resource from the resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
@@ -497,33 +494,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -536,32 +532,32 @@
     }
 
     @overload
     async def patch(
         self,
         resource_group_name: str,
         resource_guards_name: str,
-        parameters: _models.PatchResourceRequestInput,
+        parameters: _models.PatchResourceGuardInput,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
         Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
-        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput
+        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceGuardInput
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -579,15 +575,15 @@
     ) -> _models.ResourceGuardResource:
         """Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
         Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -600,30 +596,31 @@
         """
 
     @distributed_trace_async
     async def patch(
         self,
         resource_group_name: str,
         resource_guards_name: str,
-        parameters: Union[_models.PatchResourceRequestInput, IO],
+        parameters: Union[_models.PatchResourceGuardInput, IO],
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
         Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
-        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput or IO
+        :param parameters: Request body for operation. Is either a PatchResourceGuardInput type or a IO
+         type. Required.
+        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceGuardInput or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -635,27 +632,25 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ResourceGuardResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "PatchResourceRequestInput")
+            _json = self._serialize.body(parameters, "PatchResourceGuardInput")
 
         request = build_patch_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -664,16 +659,17 @@
             template_url=self.patch.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -695,31 +691,29 @@
     ) -> AsyncIterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -765,16 +759,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -792,31 +787,29 @@
     ) -> AsyncIterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -862,16 +855,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -889,31 +883,29 @@
     ) -> AsyncIterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -959,16 +951,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -986,31 +979,29 @@
     ) -> AsyncIterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1056,16 +1047,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1083,31 +1075,29 @@
     ) -> AsyncIterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1153,16 +1143,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1180,31 +1171,29 @@
     ) -> AsyncIterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1250,16 +1239,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1277,15 +1267,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1300,17 +1290,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_disable_soft_delete_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1318,16 +1306,17 @@
             template_url=self.get_default_disable_soft_delete_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1349,15 +1338,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1372,17 +1361,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_delete_resource_guard_proxy_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1390,16 +1377,17 @@
             template_url=self.get_default_delete_resource_guard_proxy_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1421,15 +1409,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1444,17 +1432,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_backup_security_pin_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1462,16 +1448,17 @@
             template_url=self.get_default_backup_security_pin_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1493,15 +1480,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1516,17 +1503,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_delete_protected_item_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1534,16 +1519,17 @@
             template_url=self.get_default_delete_protected_item_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1565,15 +1551,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1588,17 +1574,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_update_protection_policy_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1606,16 +1590,17 @@
             template_url=self.get_default_update_protection_policy_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1637,15 +1622,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1660,17 +1645,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_update_protected_item_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1678,16 +1661,17 @@
             template_url=self.get_default_update_protected_item_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_backup_vaults_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_backup_vaults_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -37,29 +37,25 @@
     build_delete_request,
     build_get_in_resource_group_request,
     build_get_in_subscription_request,
     build_get_request,
     build_update_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class BackupVaultsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`backup_vaults` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -77,17 +73,15 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupVaultResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -131,16 +125,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -154,29 +149,27 @@
 
     @distributed_trace
     def get_in_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.BackupVaultResource"]:
         """Returns resource collection belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either BackupVaultResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupVaultResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -221,16 +214,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -242,15 +236,15 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults"
     }
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> _models.BackupVaultResource:
         """Returns a resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: BackupVaultResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.BackupVaultResource
@@ -263,33 +257,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -319,24 +312,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "BackupVaultResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -348,16 +339,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -385,15 +377,15 @@
         parameters: _models.BackupVaultResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupVaultResource]:
         """Creates or updates a BackupVault resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BackupVaultResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -422,15 +414,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupVaultResource]:
         """Creates or updates a BackupVault resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -457,20 +449,21 @@
         resource_group_name: str,
         vault_name: str,
         parameters: Union[_models.BackupVaultResource, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupVaultResource]:
         """Creates or updates a BackupVault resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a BackupVaultResource type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BackupVaultResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -484,17 +477,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -531,72 +522,122 @@
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}"
     }
 
-    @distributed_trace_async
-    async def delete(  # pylint: disable=inconsistent-return-statements
+    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> None:
-        """Deletes a BackupVault resource from the resource group.
-
-        :param resource_group_name: The name of the resource group where the backup vault is present.
-         Required.
-        :type resource_group_name: str
-        :param vault_name: The name of the backup vault. Required.
-        :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
+            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}"
+    }
+
+    @distributed_trace_async
+    async def begin_delete(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
+        """Deletes a BackupVault resource from the resource group.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param vault_name: The name of the backup vault. Required.
+        :type vault_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._delete_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                vault_name=vault_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_delete.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}"
     }
 
     async def _update_initial(
         self,
         resource_group_name: str,
         vault_name: str,
@@ -610,24 +651,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.BackupVaultResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PatchResourceRequestInput")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -639,16 +678,17 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -675,15 +715,15 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupVaultResource]:
         """Updates a BackupVault resource belonging to a resource group. For example, updating tags for a
         resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -713,15 +753,15 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupVaultResource]:
         """Updates a BackupVault resource belonging to a resource group. For example, updating tags for a
         resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -749,20 +789,21 @@
         vault_name: str,
         parameters: Union[_models.PatchResourceRequestInput, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.BackupVaultResource]:
         """Updates a BackupVault resource belonging to a resource group. For example, updating tags for a
         resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a PatchResourceRequestInput type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -776,17 +817,15 @@
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -837,15 +876,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
 
         API to check for resource name availability.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: The location in which uniqueness will be verified. Required.
         :type location: str
         :param parameters: Check name availability request. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.CheckNameAvailabilityRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -867,15 +906,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
 
         API to check for resource name availability.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: The location in which uniqueness will be verified. Required.
         :type location: str
         :param parameters: Check name availability request. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -895,21 +934,21 @@
         parameters: Union[_models.CheckNameAvailabilityRequest, IO],
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
 
         API to check for resource name availability.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: The location in which uniqueness will be verified. Required.
         :type location: str
-        :param parameters: Check name availability request. Is either a model type or a IO type.
-         Required.
+        :param parameters: Check name availability request. Is either a CheckNameAvailabilityRequest
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.CheckNameAvailabilityRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.CheckNameAvailabilityResult
@@ -922,24 +961,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CheckNameAvailabilityResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "CheckNameAvailabilityRequest")
 
         request = build_check_name_availability_request(
             resource_group_name=resource_group_name,
             location=location,
@@ -951,16 +988,17 @@
             template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_deleted_backup_instances_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_deleted_backup_instances_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar, Union, cast
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,29 +32,25 @@
 from ..._vendor import _convert_request
 from ...operations._deleted_backup_instances_operations import (
     build_get_request,
     build_list_request,
     build_undelete_request,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DeletedBackupInstancesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`deleted_backup_instances` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -66,32 +61,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.DeletedBackupInstanceResource"]:
         """Gets deleted backup instances belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DeletedBackupInstanceResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dataprotection.models.DeletedBackupInstanceResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DeletedBackupInstanceResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -137,16 +130,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -160,15 +154,15 @@
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> _models.DeletedBackupInstanceResource:
         """Gets a deleted backup instance with name in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the deleted backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -183,17 +177,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DeletedBackupInstanceResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -201,16 +193,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -236,17 +229,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_undelete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -254,16 +245,17 @@
             template_url=self._undelete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -277,15 +269,15 @@
 
     @distributed_trace_async
     async def begin_undelete(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """undelete.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the deleted backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -299,17 +291,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._undelete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/aio/operations/_data_protection_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_data_protection_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,29 +24,25 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._data_protection_operations import build_check_feature_support_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DataProtectionOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.aio.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.aio.DataProtectionMgmtClient`'s
         :attr:`data_protection` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
@@ -108,16 +104,16 @@
     ) -> _models.FeatureValidationResponseBase:
         """Validates if a feature is supported.
 
         Validates if a feature is supported.
 
         :param location: Required.
         :type location: str
-        :param parameters: Feature support request object. Is either a model type or a IO type.
-         Required.
+        :param parameters: Feature support request object. Is either a FeatureValidationRequestBase
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.FeatureValidationRequestBase or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FeatureValidationResponseBase or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.FeatureValidationResponseBase
@@ -130,24 +126,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.FeatureValidationResponseBase] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "FeatureValidationRequestBase")
 
         request = build_check_feature_support_request(
             location=location,
             subscription_id=self._config.subscription_id,
@@ -158,16 +152,17 @@
             template_url=self.check_feature_support.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_dpp_resource_guard_proxy_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_dpp_resource_guard_proxy_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,42 +26,38 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,64 +70,68 @@
 
 def build_get_request(
     resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
-        "resourceGuardProxyName": _SERIALIZER.url("resource_guard_proxy_name", resource_guard_proxy_name, "str"),
+        "resourceGuardProxyName": _SERIALIZER.url(
+            "resource_guard_proxy_name", resource_guard_proxy_name, "str", pattern=r"^[A-Za-z0-9]*$"
+        ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_put_request(
+def build_create_or_update_request(
     resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
-        "resourceGuardProxyName": _SERIALIZER.url("resource_guard_proxy_name", resource_guard_proxy_name, "str"),
+        "resourceGuardProxyName": _SERIALIZER.url(
+            "resource_guard_proxy_name", resource_guard_proxy_name, "str", pattern=r"^[A-Za-z0-9]*$"
+        ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -145,29 +145,31 @@
 
 def build_delete_request(
     resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
-        "resourceGuardProxyName": _SERIALIZER.url("resource_guard_proxy_name", resource_guard_proxy_name, "str"),
+        "resourceGuardProxyName": _SERIALIZER.url(
+            "resource_guard_proxy_name", resource_guard_proxy_name, "str", pattern=r"^[A-Za-z0-9]*$"
+        ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -179,30 +181,32 @@
 
 def build_unlock_delete_request(
     resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}/unlockDelete",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
-        "resourceGuardProxyName": _SERIALIZER.url("resource_guard_proxy_name", resource_guard_proxy_name, "str"),
+        "resourceGuardProxyName": _SERIALIZER.url(
+            "resource_guard_proxy_name", resource_guard_proxy_name, "str", pattern=r"^[A-Za-z0-9]*$"
+        ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -216,15 +220,15 @@
 
 class DppResourceGuardProxyOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`dpp_resource_guard_proxy` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -233,34 +237,34 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> Iterable["_models.ResourceGuardProxyBaseResource"]:
-        """list.
+        """Returns the list of ResourceGuardProxies associated with the vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        Returns the list of ResourceGuardProxies associated with the vault.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ResourceGuardProxyBaseResource or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardProxyBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -306,16 +310,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -327,22 +332,26 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies"
     }
 
     @distributed_trace
     def get(
         self, resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """get.
+        """Returns the ResourceGuardProxy object associated with the vault, and that matches the name in
+        the request.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        Returns the ResourceGuardProxy object associated with the vault, and that matches the name in
+        the request.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
@@ -352,17 +361,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardProxyBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             resource_guard_proxy_name=resource_guard_proxy_name,
             subscription_id=self._config.subscription_id,
@@ -370,16 +377,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -392,94 +400,101 @@
         return deserialized
 
     get.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}"
     }
 
     @overload
-    def put(
+    def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: _models.ResourceGuardProxyBaseResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """put.
+        """Creates or Updates a ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        Creates or Updates a ResourceGuardProxy.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def put(
+    def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """put.
+        """Creates or Updates a ResourceGuardProxy.
+
+        Creates or Updates a ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
-    def put(
+    def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: Union[_models.ResourceGuardProxyBaseResource, IO],
         **kwargs: Any
     ) -> _models.ResourceGuardProxyBaseResource:
-        """put.
+        """Creates or Updates a ResourceGuardProxy.
+
+        Creates or Updates a ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ResourceGuardProxyBaseResource type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardProxyBaseResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardProxyBaseResource
@@ -492,46 +507,45 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ResourceGuardProxyBaseResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ResourceGuardProxyBaseResource")
 
-        request = build_put_request(
+        request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             resource_guard_proxy_name=resource_guard_proxy_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.put.metadata["url"],
+            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -539,30 +553,32 @@
         deserialized = self._deserialize("ResourceGuardProxyBaseResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    put.metadata = {
+    create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupResourceGuardProxies/{resourceGuardProxyName}"
     }
 
     @distributed_trace
     def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, resource_guard_proxy_name: str, **kwargs: Any
     ) -> None:
-        """delete.
+        """Deletes the ResourceGuardProxy.
+
+        Deletes the ResourceGuardProxy.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
@@ -572,17 +588,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             resource_guard_proxy_name=resource_guard_proxy_name,
             subscription_id=self._config.subscription_id,
@@ -590,16 +604,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -618,22 +633,24 @@
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: _models.UnlockDeleteRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.UnlockDeleteResponse:
-        """unlock_delete.
+        """UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
+
+        UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.UnlockDeleteRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -649,22 +666,24 @@
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.UnlockDeleteResponse:
-        """unlock_delete.
+        """UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -678,24 +697,27 @@
         self,
         resource_group_name: str,
         vault_name: str,
         resource_guard_proxy_name: str,
         parameters: Union[_models.UnlockDeleteRequest, IO],
         **kwargs: Any
     ) -> _models.UnlockDeleteResponse:
-        """unlock_delete.
+        """UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
+
+        UnlockDelete call for ResourceGuardProxy, executed before one can delete it.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param resource_guard_proxy_name: Required.
+        :param resource_guard_proxy_name: name of the resource guard proxy. Required.
         :type resource_guard_proxy_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a UnlockDeleteRequest type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.UnlockDeleteRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: UnlockDeleteResponse or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.UnlockDeleteResponse
@@ -708,24 +730,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.UnlockDeleteResponse] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "UnlockDeleteRequest")
 
         request = build_unlock_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -738,16 +758,17 @@
             template_url=self.unlock_delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_result_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_result_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +23,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(operation_id: str, location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.DataProtection/locations/{location}/operationResults/{operationId}",
     )  # pylint: disable=line-too-long
@@ -72,15 +65,15 @@
 
 class OperationResultOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`operation_result` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -111,33 +104,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         request = build_get_request(
             operation_id=operation_id,
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_instances_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_instances_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,42 +28,38 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -76,27 +72,27 @@
 
 def build_get_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -110,28 +106,28 @@
 
 def build_create_or_update_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -147,27 +143,27 @@
 
 def build_delete_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -181,28 +177,28 @@
 
 def build_adhoc_backup_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/backup",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -218,28 +214,28 @@
 
 def build_validate_for_backup_request(
     resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/validateForBackup",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -259,27 +255,27 @@
     operation_id: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/operationResults/{operationId}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
         "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -294,27 +290,27 @@
 
 def build_trigger_rehydrate_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/rehydrate",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -331,28 +327,28 @@
 
 def build_trigger_restore_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/restore",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -368,27 +364,27 @@
 
 def build_resume_backups_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/resumeBackups",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -402,27 +398,27 @@
 
 def build_resume_protection_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/resumeProtection",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -436,27 +432,27 @@
 
 def build_stop_protection_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/stopProtection",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -470,27 +466,27 @@
 
 def build_suspend_backups_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/suspendBackups",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -504,28 +500,28 @@
 
 def build_sync_backup_instance_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/sync",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -541,28 +537,28 @@
 
 def build_validate_for_restore_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/validateRestore",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -578,15 +574,15 @@
 
 class BackupInstancesOperations:  # pylint: disable=too-many-public-methods
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`backup_instances` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -597,31 +593,29 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> Iterable["_models.BackupInstanceResource"]:
         """Gets a backup instances belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either BackupInstanceResource or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.BackupInstanceResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupInstanceResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -667,16 +661,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -690,15 +685,15 @@
 
     @distributed_trace
     def get(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> _models.BackupInstanceResource:
         """Gets a backup instance with name in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -713,17 +708,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupInstanceResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -731,16 +724,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -771,24 +765,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.BackupInstanceResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "BackupInstanceResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -801,16 +793,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -847,15 +840,15 @@
         parameters: _models.BackupInstanceResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.BackupInstanceResource]:
         """Create or update a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -886,15 +879,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.BackupInstanceResource]:
         """Create or update a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -923,22 +916,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.BackupInstanceResource, IO],
         **kwargs: Any
     ) -> LROPoller[_models.BackupInstanceResource]:
         """Create or update a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a BackupInstanceResource type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BackupInstanceResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -951,17 +945,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.dataprotection.models.BackupInstanceResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupInstanceResource] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -1013,17 +1005,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -1031,16 +1021,17 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1062,15 +1053,15 @@
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Delete a backup instance in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1084,17 +1075,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1146,24 +1135,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "TriggerBackupRequest")
 
         request = build_adhoc_backup_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -1176,16 +1163,17 @@
             template_url=self._adhoc_backup_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1220,15 +1208,15 @@
         parameters: _models.TriggerBackupRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Trigger adhoc backup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -1260,15 +1248,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Trigger adhoc backup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -1298,22 +1286,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.TriggerBackupRequest, IO],
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Trigger adhoc backup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a TriggerBackupRequest type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.TriggerBackupRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1327,17 +1316,15 @@
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._adhoc_backup_initial(
@@ -1393,24 +1380,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ValidateForBackupRequest")
 
         request = build_validate_for_backup_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -1422,16 +1407,17 @@
             template_url=self._validate_for_backup_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1465,15 +1451,15 @@
         parameters: _models.ValidateForBackupRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Validate whether adhoc backup will be successful or not.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ValidateForBackupRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -1502,15 +1488,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Validate whether adhoc backup will be successful or not.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -1537,20 +1523,21 @@
         resource_group_name: str,
         vault_name: str,
         parameters: Union[_models.ValidateForBackupRequest, IO],
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Validate whether adhoc backup will be successful or not.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ValidateForBackupRequest type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ValidateForBackupRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1564,17 +1551,15 @@
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._validate_for_backup_initial(
@@ -1617,20 +1602,20 @@
 
     @distributed_trace
     def get_backup_instance_operation_result(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, operation_id: str, **kwargs: Any
     ) -> Optional[_models.BackupInstanceResource]:
         """Get result of backup instance creation operation.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param operation_id: Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: BackupInstanceResource or None or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.BackupInstanceResource or None
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1642,17 +1627,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.BackupInstanceResource]] = kwargs.pop("cls", None)
 
         request = build_get_backup_instance_operation_result_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             operation_id=operation_id,
@@ -1661,16 +1644,17 @@
             template_url=self.get_backup_instance_operation_result.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1703,24 +1687,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AzureBackupRehydrationRequest")
 
         request = build_trigger_rehydrate_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -1733,16 +1715,17 @@
             template_url=self._trigger_rehydrate_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1771,20 +1754,20 @@
         parameters: _models.AzureBackupRehydrationRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """rehydrate recovery point for restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupRehydrationRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1809,20 +1792,20 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """rehydrate recovery point for restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1845,22 +1828,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.AzureBackupRehydrationRequest, IO],
         **kwargs: Any
     ) -> LROPoller[None]:
         """rehydrate recovery point for restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a AzureBackupRehydrationRequest type
+         or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupRehydrationRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1872,17 +1856,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._trigger_rehydrate_initial(  # type: ignore
@@ -1937,24 +1919,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AzureBackupRestoreRequest")
 
         request = build_trigger_restore_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -1967,16 +1947,17 @@
             template_url=self._trigger_restore_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2011,15 +1992,15 @@
         parameters: _models.AzureBackupRestoreRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Triggers restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -2051,15 +2032,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Triggers restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -2089,22 +2070,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.AzureBackupRestoreRequest, IO],
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Triggers restore for a BackupInstance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a AzureBackupRestoreRequest type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupRestoreRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -2118,17 +2100,15 @@
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._trigger_restore_initial(
@@ -2180,17 +2160,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_resume_backups_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -2198,16 +2176,17 @@
             template_url=self._resume_backups_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2229,20 +2208,20 @@
 
     @distributed_trace
     def begin_resume_backups(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """This operation will resume backups for backup instance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
@@ -2251,17 +2230,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._resume_backups_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2308,17 +2285,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_resume_protection_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -2326,16 +2301,17 @@
             template_url=self._resume_protection_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2357,20 +2333,20 @@
 
     @distributed_trace
     def begin_resume_protection(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """This operation will resume protection for a stopped backup instance.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
@@ -2379,17 +2355,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._resume_protection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2436,17 +2410,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_stop_protection_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -2454,16 +2426,17 @@
             template_url=self._stop_protection_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2485,20 +2458,20 @@
 
     @distributed_trace
     def begin_stop_protection(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """This operation will stop protection of a backup instance and data will be held forever.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
@@ -2507,17 +2480,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._stop_protection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2564,17 +2535,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_suspend_backups_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -2582,16 +2551,17 @@
             template_url=self._suspend_backups_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2614,20 +2584,20 @@
     @distributed_trace
     def begin_suspend_backups(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """This operation will stop backup for a backup instance and retains the backup data as per the
         policy (except latest Recovery point, which will be retained forever).
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
@@ -2636,17 +2606,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._suspend_backups_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2698,24 +2666,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "SyncBackupInstanceRequest")
 
         request = build_sync_backup_instance_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -2728,16 +2694,17 @@
             template_url=self._sync_backup_instance_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2767,20 +2734,20 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Sync backup instance again in case of failure
         This action will retry last failed operation and will bring backup instance to valid state.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.SyncBackupInstanceRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2806,20 +2773,20 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Sync backup instance again in case of failure
         This action will retry last failed operation and will bring backup instance to valid state.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2843,22 +2810,23 @@
         backup_instance_name: str,
         parameters: Union[_models.SyncBackupInstanceRequest, IO],
         **kwargs: Any
     ) -> LROPoller[None]:
         """Sync backup instance again in case of failure
         This action will retry last failed operation and will bring backup instance to valid state.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param backup_instance_name: Required.
+        :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a SyncBackupInstanceRequest type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.SyncBackupInstanceRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -2870,17 +2838,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._sync_backup_instance_initial(  # type: ignore
@@ -2935,24 +2901,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.OperationJobExtendedInfo]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ValidateRestoreRequestObject")
 
         request = build_validate_for_restore_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -2965,16 +2929,17 @@
             template_url=self._validate_for_restore_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -3009,15 +2974,15 @@
         parameters: _models.ValidateRestoreRequestObject,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Validates if Restore can be triggered for a DataSource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -3049,15 +3014,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Validates if Restore can be triggered for a DataSource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -3087,22 +3052,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.ValidateRestoreRequestObject, IO],
         **kwargs: Any
     ) -> LROPoller[_models.OperationJobExtendedInfo]:
         """Validates if Restore can be triggered for a DataSource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ValidateRestoreRequestObject type or
+         a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ValidateRestoreRequestObject or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -3116,17 +3082,15 @@
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.dataprotection.models.OperationJobExtendedInfo]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.OperationJobExtendedInfo] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._validate_for_restore_initial(
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_export_jobs_operation_result_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_export_jobs_operation_result_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,44 +23,40 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(
     resource_group_name: str, vault_name: str, operation_id: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupJobs/operations/{operationId}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -75,15 +70,15 @@
 
 class ExportJobsOperationResultOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`export_jobs_operation_result` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -96,15 +91,15 @@
     def get(
         self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
     ) -> Optional[_models.ExportJobsResult]:
         """Gets the operation result of operation triggered by Export Jobs API. If the operation is
         successful, then it also contains URL of a Blob and a SAS key to access the same. The blob
         contains exported jobs in JSON serialized format.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param operation_id: OperationID which represents the export job. Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -119,17 +114,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ExportJobsResult]] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
@@ -137,16 +130,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_instances_extension_routing_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_vault_operation_results_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,171 +2,164 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
-import urllib.parse
+from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_request(resource_id: str, **kwargs: Any) -> HttpRequest:
+def build_get_request(
+    resource_group_name: str, vault_name: str, operation_id: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/{resourceId}/providers/Microsoft.DataProtection/backupInstances")
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationResults/{operationId}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceId": _SERIALIZER.url("resource_id", resource_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
+        "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class BackupInstancesExtensionRoutingOperations:
+class BackupVaultOperationResultsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
-        :attr:`backup_instances_extension_routing` attribute.
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
+        :attr:`backup_vault_operation_results` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, resource_id: str, **kwargs: Any) -> Iterable["_models.BackupInstanceResource"]:
-        """Gets a list backup instances associated with a tracked resource.
+    def get(
+        self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
+    ) -> Optional[_models.BackupVaultResource]:
+        """get.
 
-        :param resource_id: ARM path of the resource to be protected using Microsoft.DataProtection.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
-        :type resource_id: str
+        :type resource_group_name: str
+        :param vault_name: The name of the backup vault. Required.
+        :type vault_name: str
+        :param operation_id: Required.
+        :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either BackupInstanceResource or the result of
-         cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.BackupInstanceResource]
+        :return: BackupVaultResource or None or the result of cls(response)
+        :rtype: ~azure.mgmt.dataprotection.models.BackupVaultResource or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.BackupInstanceResourceList] = kwargs.pop("cls", None)
-
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        def prepare_request(next_link=None):
-            if not next_link:
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-                request = build_list_request(
-                    resource_id=resource_id,
-                    api_version=api_version,
-                    template_url=self.list.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize("BackupInstanceResourceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, iter(list_of_elem)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[Optional[_models.BackupVaultResource]] = kwargs.pop("cls", None)
 
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
+        request = build_get_request(
+            resource_group_name=resource_group_name,
+            vault_name=vault_name,
+            operation_id=operation_id,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
-            )
-            response = pipeline_response.http_response
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
 
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+        response = pipeline_response.http_response
 
-            return pipeline_response
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("BackupVaultResource", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)
 
-        return ItemPaged(get_next, extract_data)
+        return deserialized
 
-    list.metadata = {"url": "/{resourceId}/providers/Microsoft.DataProtection/backupInstances"}
+    get.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationResults/{operationId}"
+    }
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_policies_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_policies_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,42 +26,38 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupPolicies",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,27 +70,27 @@
 
 def build_get_request(
     resource_group_name: str, vault_name: str, backup_policy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupPolicies/{backupPolicyName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupPolicyName": _SERIALIZER.url("backup_policy_name", backup_policy_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -108,28 +104,28 @@
 
 def build_create_or_update_request(
     resource_group_name: str, vault_name: str, backup_policy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupPolicies/{backupPolicyName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupPolicyName": _SERIALIZER.url("backup_policy_name", backup_policy_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -145,27 +141,27 @@
 
 def build_delete_request(
     resource_group_name: str, vault_name: str, backup_policy_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupPolicies/{backupPolicyName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupPolicyName": _SERIALIZER.url("backup_policy_name", backup_policy_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -179,15 +175,15 @@
 
 class BackupPoliciesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`backup_policies` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -198,32 +194,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> Iterable["_models.BaseBackupPolicyResource"]:
         """Returns list of backup policies belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either BaseBackupPolicyResource or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.BaseBackupPolicyResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BaseBackupPolicyResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -269,16 +263,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -294,15 +289,15 @@
     def get(
         self, resource_group_name: str, vault_name: str, backup_policy_name: str, **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Gets a backup policy belonging to a backup vault.
 
         Gets a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Required.
         :type backup_policy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -317,17 +312,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BaseBackupPolicyResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_policy_name=backup_policy_name,
             subscription_id=self._config.subscription_id,
@@ -335,16 +328,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -371,15 +365,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Creates or Updates a backup policy belonging to a backup vault.
 
         Creates or Updates a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Name of the policy. Required.
         :type backup_policy_name: str
         :param parameters: Request body for operation. Required.
@@ -404,15 +398,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Creates or Updates a backup policy belonging to a backup vault.
 
         Creates or Updates a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Name of the policy. Required.
         :type backup_policy_name: str
         :param parameters: Request body for operation. Required.
@@ -435,22 +429,23 @@
         parameters: Union[_models.BaseBackupPolicyResource, IO],
         **kwargs: Any
     ) -> _models.BaseBackupPolicyResource:
         """Creates or Updates a backup policy belonging to a backup vault.
 
         Creates or Updates a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Name of the policy. Required.
         :type backup_policy_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a BaseBackupPolicyResource type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BaseBackupPolicyResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: BaseBackupPolicyResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.BaseBackupPolicyResource
@@ -463,24 +458,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BaseBackupPolicyResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "BaseBackupPolicyResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -493,16 +486,17 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -522,15 +516,15 @@
     def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, backup_policy_name: str, **kwargs: Any
     ) -> None:
         """Deletes a backup policy belonging to a backup vault.
 
         Deletes a backup policy belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_policy_name: Required.
         :type backup_policy_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -545,17 +539,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_policy_name=backup_policy_name,
             subscription_id=self._config.subscription_id,
@@ -563,16 +555,17 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_vault_operation_results_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_resource_group_context_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,148 +23,127 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_get_request(
-    resource_group_name: str, vault_name: str, operation_id: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
+def build_get_request(resource_group_name: str, operation_id: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationResults/{operationId}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/operationStatus/{operationId}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class BackupVaultOperationResultsOperations:
+class OperationStatusResourceGroupContextOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
-        :attr:`backup_vault_operation_results` attribute.
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
+        :attr:`operation_status_resource_group_context` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def get(
-        self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
-    ) -> Optional[_models.BackupVaultResource]:
-        """get.
+    def get(self, resource_group_name: str, operation_id: str, **kwargs: Any) -> _models.OperationResource:
+        """Gets the operation status for an operation over a ResourceGroup's context.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        Gets the operation status for an operation over a ResourceGroup's context.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param vault_name: The name of the backup vault. Required.
-        :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: BackupVaultResource or None or the result of cls(response)
-        :rtype: ~azure.mgmt.dataprotection.models.BackupVaultResource or None
+        :return: OperationResource or the result of cls(response)
+        :rtype: ~azure.mgmt.dataprotection.models.OperationResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[Optional[_models.BackupVaultResource]] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
-            vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = None
-        response_headers = {}
-        if response.status_code == 200:
-            deserialized = self._deserialize("BackupVaultResource", pipeline_response)
-
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
+        deserialized = self._deserialize("OperationResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationResults/{operationId}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/operationStatus/{operationId}"
     }
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_jobs_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_jobs_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,42 +25,38 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupJobs",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,27 +69,27 @@
 
 def build_get_request(
     resource_group_name: str, vault_name: str, job_id: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupJobs/{jobId}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "jobId": _SERIALIZER.url("job_id", job_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -108,15 +103,15 @@
 
 class JobsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`jobs` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -127,31 +122,29 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> Iterable["_models.AzureBackupJobResource"]:
         """Returns list of jobs belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either AzureBackupJobResource or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.AzureBackupJobResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupJobResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -197,16 +190,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -220,15 +214,15 @@
 
     @distributed_trace
     def get(
         self, resource_group_name: str, vault_name: str, job_id: str, **kwargs: Any
     ) -> _models.AzureBackupJobResource:
         """Gets a job with id in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param job_id: The Job ID. This is a GUID-formatted string (e.g.
          00000000-0000-0000-0000-000000000000). Required.
         :type job_id: str
@@ -244,17 +238,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupJobResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             job_id=job_id,
             subscription_id=self._config.subscription_id,
@@ -262,16 +254,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +23,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(location: str, operation_id: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.DataProtection/locations/{location}/operationStatus/{operationId}",
     )  # pylint: disable=line-too-long
@@ -72,15 +65,15 @@
 
 class OperationStatusOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`operation_status` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -111,33 +104,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             location=location,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_recovery_points_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_recovery_points_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,18 +25,14 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -50,27 +45,27 @@
     filter: Optional[str] = None,
     skip_token: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/recoveryPoints",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -93,27 +88,27 @@
     recovery_point_id: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/recoveryPoints/{recoveryPointId}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
         "recoveryPointId": _SERIALIZER.url("recovery_point_id", recovery_point_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -128,15 +123,15 @@
 
 class RecoveryPointsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`recovery_points` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -153,15 +148,15 @@
         backup_instance_name: str,
         filter: Optional[str] = None,
         skip_token: Optional[str] = None,
         **kwargs: Any
     ) -> Iterable["_models.AzureBackupRecoveryPointResource"]:
         """Returns a list of Recovery Points for a DataSource in a vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param filter: OData filter options. Default value is None.
@@ -174,17 +169,15 @@
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.AzureBackupRecoveryPointResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupRecoveryPointResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -233,16 +226,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -261,15 +255,15 @@
         vault_name: str,
         backup_instance_name: str,
         recovery_point_id: str,
         **kwargs: Any
     ) -> _models.AzureBackupRecoveryPointResource:
         """Gets a Recovery Point using recoveryPointId for a Datasource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param recovery_point_id: Required.
@@ -286,17 +280,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AzureBackupRecoveryPointResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             recovery_point_id=recovery_point_id,
@@ -305,16 +297,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_restorable_time_ranges_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_restorable_time_ranges_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,45 +24,41 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_find_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/backupInstances/{backupInstanceName}/findRestorableTimeRanges",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -78,15 +74,15 @@
 
 class RestorableTimeRangesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`restorable_time_ranges` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -104,15 +100,15 @@
         parameters: _models.AzureBackupFindRestorableTimeRangesRequest,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.AzureBackupFindRestorableTimeRangesResponseResource:
         """find.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -135,15 +131,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.AzureBackupFindRestorableTimeRangesResponseResource:
         """find.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
         :param parameters: Request body for operation. Required.
@@ -164,22 +160,23 @@
         vault_name: str,
         backup_instance_name: str,
         parameters: Union[_models.AzureBackupFindRestorableTimeRangesRequest, IO],
         **kwargs: Any
     ) -> _models.AzureBackupFindRestorableTimeRangesResponseResource:
         """find.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the backup instance. Required.
         :type backup_instance_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a
+         AzureBackupFindRestorableTimeRangesRequest type or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.AzureBackupFindRestorableTimeRangesRequest
          or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AzureBackupFindRestorableTimeRangesResponseResource or the result of cls(response)
@@ -193,24 +190,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AzureBackupFindRestorableTimeRangesResponseResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "AzureBackupFindRestorableTimeRangesRequest")
 
         request = build_find_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -223,16 +218,17 @@
             template_url=self.find.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_resource_group_context_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_operation_status_backup_vault_context_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,84 +23,87 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_get_request(resource_group_name: str, operation_id: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_get_request(
+    resource_group_name: str, vault_name: str, operation_id: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/operationStatus/{operationId}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationStatus/{operationId}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class OperationStatusResourceGroupContextOperations:
+class OperationStatusBackupVaultContextOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
-        :attr:`operation_status_resource_group_context` attribute.
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
+        :attr:`operation_status_backup_vault_context` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def get(self, resource_group_name: str, operation_id: str, **kwargs: Any) -> _models.OperationResource:
-        """Gets the operation status for an operation over a ResourceGroup's context.
+    def get(
+        self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
+    ) -> _models.OperationResource:
+        """Gets the operation status for an operation over a BackupVault's context.
 
-        Gets the operation status for an operation over a ResourceGroup's context.
+        Gets the operation status for an operation over a BackupVault's context.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
+        :param vault_name: The name of the backup vault. Required.
+        :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.OperationResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
@@ -112,33 +114,33 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
+            vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -147,9 +149,9 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/operationStatus/{operationId}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationStatus/{operationId}"
     }
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_operation_status_backup_vault_context_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_export_jobs_operations.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,162 +2,206 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
-from typing import Any, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_get_request(
-    resource_group_name: str, vault_name: str, operation_id: str, subscription_id: str, **kwargs: Any
+def build_trigger_request(
+    resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationStatus/{operationId}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/exportBackupJobs",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
-        "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class OperationStatusBackupVaultContextOperations:
+class ExportJobsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
-        :attr:`operation_status_backup_vault_context` attribute.
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
+        :attr:`export_jobs` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace
-    def get(
-        self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
-    ) -> _models.OperationResource:
-        """Gets the operation status for an operation over a BackupVault's context.
-
-        Gets the operation status for an operation over a BackupVault's context.
-
-        :param resource_group_name: The name of the resource group where the backup vault is present.
-         Required.
-        :type resource_group_name: str
-        :param vault_name: The name of the backup vault. Required.
-        :type vault_name: str
-        :param operation_id: Required.
-        :type operation_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: OperationResource or the result of cls(response)
-        :rtype: ~azure.mgmt.dataprotection.models.OperationResource
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    def _trigger_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, vault_name: str, **kwargs: Any
+    ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
-        cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        request = build_trigger_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
-            operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
+            template_url=self._trigger_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("OperationResource", pipeline_response)
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, None, response_headers)
+
+    _trigger_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/exportBackupJobs"
+    }
+
+    @distributed_trace
+    def begin_trigger(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> LROPoller[None]:
+        """Triggers export of jobs and returns an OperationID to track.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param vault_name: The name of the backup vault. Required.
+        :type vault_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        return deserialized
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._trigger_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                vault_name=vault_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/operationStatus/{operationId}"
+    begin_trigger.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/exportBackupJobs"
     }
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/__init__.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from ._operation_status_backup_vault_context_operations import OperationStatusBackupVaultContextOperations
 from ._operation_status_resource_group_context_operations import OperationStatusResourceGroupContextOperations
 from ._backup_vault_operation_results_operations import BackupVaultOperationResultsOperations
 from ._data_protection_operations import DataProtectionOperations
 from ._data_protection_operations_operations import DataProtectionOperationsOperations
 from ._backup_policies_operations import BackupPoliciesOperations
 from ._backup_instances_operations import BackupInstancesOperations
-from ._backup_instances_extension_routing_operations import BackupInstancesExtensionRoutingOperations
 from ._recovery_points_operations import RecoveryPointsOperations
 from ._jobs_operations import JobsOperations
 from ._restorable_time_ranges_operations import RestorableTimeRangesOperations
 from ._export_jobs_operations import ExportJobsOperations
 from ._export_jobs_operation_result_operations import ExportJobsOperationResultOperations
 from ._deleted_backup_instances_operations import DeletedBackupInstancesOperations
 from ._resource_guards_operations import ResourceGuardsOperations
@@ -37,15 +36,14 @@
     "OperationStatusBackupVaultContextOperations",
     "OperationStatusResourceGroupContextOperations",
     "BackupVaultOperationResultsOperations",
     "DataProtectionOperations",
     "DataProtectionOperationsOperations",
     "BackupPoliciesOperations",
     "BackupInstancesOperations",
-    "BackupInstancesExtensionRoutingOperations",
     "RecoveryPointsOperations",
     "JobsOperations",
     "RestorableTimeRangesOperations",
     "ExportJobsOperations",
     "ExportJobsOperationResultOperations",
     "DeletedBackupInstancesOperations",
     "ResourceGuardsOperations",
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_patch.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_resource_guards_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_resource_guards_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,32 +26,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_resources_in_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.DataProtection/resourceGuards"
     )
     path_format_arguments = {
@@ -71,27 +65,27 @@
 
 def build_get_resources_in_resource_group_request(
     resource_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -103,27 +97,27 @@
 
 def build_put_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -139,26 +133,26 @@
 
 def build_get_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -172,26 +166,26 @@
 
 def build_delete_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -205,27 +199,27 @@
 
 def build_patch_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -241,26 +235,26 @@
 
 def build_get_disable_soft_delete_requests_objects_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/disableSoftDeleteRequests",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -274,26 +268,26 @@
 
 def build_get_delete_resource_guard_proxy_requests_objects_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/deleteResourceGuardProxyRequests",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -307,26 +301,26 @@
 
 def build_get_backup_security_pin_requests_objects_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/getBackupSecurityPINRequests",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -340,26 +334,26 @@
 
 def build_get_delete_protected_item_requests_objects_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/deleteProtectedItemRequests",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -373,26 +367,26 @@
 
 def build_get_update_protection_policy_requests_objects_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/updateProtectionPolicyRequests",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -406,26 +400,26 @@
 
 def build_get_update_protected_item_requests_objects_request(
     resource_group_name: str, resource_guards_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/updateProtectedItemRequests",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -439,26 +433,26 @@
 
 def build_get_default_disable_soft_delete_requests_object_request(
     resource_group_name: str, resource_guards_name: str, request_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/disableSoftDeleteRequests/{requestName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
         "requestName": _SERIALIZER.url("request_name", request_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -473,26 +467,26 @@
 
 def build_get_default_delete_resource_guard_proxy_requests_object_request(
     resource_group_name: str, resource_guards_name: str, request_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/deleteResourceGuardProxyRequests/{requestName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
         "requestName": _SERIALIZER.url("request_name", request_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -507,26 +501,26 @@
 
 def build_get_default_backup_security_pin_requests_object_request(
     resource_group_name: str, resource_guards_name: str, request_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/getBackupSecurityPINRequests/{requestName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
         "requestName": _SERIALIZER.url("request_name", request_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -541,26 +535,26 @@
 
 def build_get_default_delete_protected_item_requests_object_request(
     resource_group_name: str, resource_guards_name: str, request_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/deleteProtectedItemRequests/{requestName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
         "requestName": _SERIALIZER.url("request_name", request_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -575,26 +569,26 @@
 
 def build_get_default_update_protection_policy_requests_object_request(
     resource_group_name: str, resource_guards_name: str, request_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/updateProtectionPolicyRequests/{requestName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
         "requestName": _SERIALIZER.url("request_name", request_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -609,26 +603,26 @@
 
 def build_get_default_update_protected_item_requests_object_request(
     resource_group_name: str, resource_guards_name: str, request_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}/updateProtectedItemRequests/{requestName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "resourceGuardsName": _SERIALIZER.url("resource_guards_name", resource_guards_name, "str"),
         "requestName": _SERIALIZER.url("request_name", request_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
@@ -643,15 +637,15 @@
 
 class ResourceGuardsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`resource_guards` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -671,17 +665,15 @@
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.ResourceGuardResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -725,16 +717,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -750,29 +743,27 @@
     def get_resources_in_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> Iterable["_models.ResourceGuardResource"]:
         """Returns ResourceGuards collection belonging to a ResourceGroup.
 
         Returns ResourceGuards collection belonging to a ResourceGroup.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ResourceGuardResource or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.ResourceGuardResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -817,16 +808,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -848,15 +840,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Creates or updates a ResourceGuard resource belonging to a resource group.
 
         Creates or updates a ResourceGuard resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -878,15 +870,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Creates or updates a ResourceGuard resource belonging to a resource group.
 
         Creates or updates a ResourceGuard resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -906,20 +898,21 @@
         parameters: Union[_models.ResourceGuardResource, IO],
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Creates or updates a ResourceGuard resource belonging to a resource group.
 
         Creates or updates a ResourceGuard resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a ResourceGuardResource type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.ResourceGuardResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
@@ -932,24 +925,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ResourceGuardResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ResourceGuardResource")
 
         request = build_put_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
@@ -961,42 +952,47 @@
             template_url=self.put.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ResourceGuardResource", pipeline_response)
+        if response.status_code == 200:
+            deserialized = self._deserialize("ResourceGuardResource", pipeline_response)
+
+        if response.status_code == 201:
+            deserialized = self._deserialize("ResourceGuardResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     put.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/resourceGuards/{resourceGuardsName}"
     }
 
     @distributed_trace
     def get(self, resource_group_name: str, resource_guards_name: str, **kwargs: Any) -> _models.ResourceGuardResource:
         """Returns a ResourceGuard belonging to a resource group.
 
         Returns a ResourceGuard belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
@@ -1009,33 +1005,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceGuardResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1055,15 +1050,15 @@
     def delete(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_guards_name: str, **kwargs: Any
     ) -> None:
         """Deletes a ResourceGuard resource from the resource group.
 
         Deletes a ResourceGuard resource from the resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
@@ -1076,33 +1071,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1115,32 +1109,32 @@
     }
 
     @overload
     def patch(
         self,
         resource_group_name: str,
         resource_guards_name: str,
-        parameters: _models.PatchResourceRequestInput,
+        parameters: _models.PatchResourceGuardInput,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
         Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
-        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput
+        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceGuardInput
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1158,15 +1152,15 @@
     ) -> _models.ResourceGuardResource:
         """Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
         Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -1179,30 +1173,31 @@
         """
 
     @distributed_trace
     def patch(
         self,
         resource_group_name: str,
         resource_guards_name: str,
-        parameters: Union[_models.PatchResourceRequestInput, IO],
+        parameters: Union[_models.PatchResourceGuardInput, IO],
         **kwargs: Any
     ) -> _models.ResourceGuardResource:
         """Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
         Updates a ResourceGuard resource belonging to a resource group. For example, updating tags for
         a resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: The name of ResourceGuard. Required.
         :type resource_guards_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
-        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput or IO
+        :param parameters: Request body for operation. Is either a PatchResourceGuardInput type or a IO
+         type. Required.
+        :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceGuardInput or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ResourceGuardResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.ResourceGuardResource
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -1214,27 +1209,25 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ResourceGuardResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "PatchResourceRequestInput")
+            _json = self._serialize.body(parameters, "PatchResourceGuardInput")
 
         request = build_patch_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -1243,16 +1236,17 @@
             template_url=self.patch.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1274,30 +1268,28 @@
     ) -> Iterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1343,16 +1335,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1370,30 +1363,28 @@
     ) -> Iterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1439,16 +1430,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1466,30 +1458,28 @@
     ) -> Iterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1535,16 +1525,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1562,30 +1553,28 @@
     ) -> Iterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1631,16 +1620,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1658,30 +1648,28 @@
     ) -> Iterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1727,16 +1715,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1754,30 +1743,28 @@
     ) -> Iterable["_models.DppBaseResource"]:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DppBaseResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.DppBaseResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1823,16 +1810,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1850,15 +1838,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1873,17 +1861,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_disable_soft_delete_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1891,16 +1877,17 @@
             template_url=self.get_default_disable_soft_delete_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1922,15 +1909,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -1945,17 +1932,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_delete_resource_guard_proxy_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -1963,16 +1948,17 @@
             template_url=self.get_default_delete_resource_guard_proxy_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1994,15 +1980,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2017,17 +2003,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_backup_security_pin_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -2035,16 +2019,17 @@
             template_url=self.get_default_backup_security_pin_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2066,15 +2051,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2089,17 +2074,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_delete_protected_item_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -2107,16 +2090,17 @@
             template_url=self.get_default_delete_protected_item_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2138,15 +2122,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2161,17 +2145,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_update_protection_policy_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -2179,16 +2161,17 @@
             template_url=self.get_default_update_protection_policy_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2210,15 +2193,15 @@
     ) -> _models.DppBaseResource:
         """Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
         Returns collection of operation request objects for a critical operation protected by the given
         ResourceGuard resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param resource_guards_name: Required.
         :type resource_guards_name: str
         :param request_name: Required.
         :type request_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -2233,17 +2216,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DppBaseResource] = kwargs.pop("cls", None)
 
         request = build_get_default_update_protected_item_requests_object_request(
             resource_group_name=resource_group_name,
             resource_guards_name=resource_guards_name,
             request_name=request_name,
             subscription_id=self._config.subscription_id,
@@ -2251,16 +2232,17 @@
             template_url=self.get_default_update_protected_item_requests_object.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_backup_vaults_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_backup_vaults_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,32 +28,26 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_in_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.DataProtection/backupVaults")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
@@ -69,26 +63,26 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_in_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -99,27 +93,27 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -132,28 +126,28 @@
 
 def build_create_or_update_request(
     resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -166,27 +160,27 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -197,28 +191,28 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -233,27 +227,27 @@
 
 def build_check_name_availability_request(
     resource_group_name: str, location: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/locations/{location}/checkNameAvailability",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "location": _SERIALIZER.url("location", location, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -269,15 +263,15 @@
 
 class BackupVaultsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`backup_vaults` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -294,17 +288,15 @@
         :return: An iterator like instance of either BackupVaultResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupVaultResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -348,16 +340,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -369,28 +362,26 @@
         "url": "/subscriptions/{subscriptionId}/providers/Microsoft.DataProtection/backupVaults"
     }
 
     @distributed_trace
     def get_in_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.BackupVaultResource"]:
         """Returns resource collection belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either BackupVaultResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupVaultResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -435,16 +426,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -456,15 +448,15 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults"
     }
 
     @distributed_trace
     def get(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> _models.BackupVaultResource:
         """Returns a resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: BackupVaultResource or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.BackupVaultResource
@@ -477,33 +469,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -533,24 +524,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "BackupVaultResource")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -562,16 +551,17 @@
             template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -599,15 +589,15 @@
         parameters: _models.BackupVaultResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.BackupVaultResource]:
         """Creates or updates a BackupVault resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BackupVaultResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -635,15 +625,15 @@
         parameters: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.BackupVaultResource]:
         """Creates or updates a BackupVault resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -669,20 +659,21 @@
         resource_group_name: str,
         vault_name: str,
         parameters: Union[_models.BackupVaultResource, IO],
         **kwargs: Any
     ) -> LROPoller[_models.BackupVaultResource]:
         """Creates or updates a BackupVault resource belonging to a resource group.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a BackupVaultResource type or a IO
+         type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.BackupVaultResource or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -695,17 +686,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -742,72 +731,122 @@
             )
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}"
     }
 
-    @distributed_trace
-    def delete(  # pylint: disable=inconsistent-return-statements
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> None:
-        """Deletes a BackupVault resource from the resource group.
-
-        :param resource_group_name: The name of the resource group where the backup vault is present.
-         Required.
-        :type resource_group_name: str
-        :param vault_name: The name of the backup vault. Required.
-        :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
+            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {
+    _delete_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}"
+    }
+
+    @distributed_trace
+    def begin_delete(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> LROPoller[None]:
+        """Deletes a BackupVault resource from the resource group.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param vault_name: The name of the backup vault. Required.
+        :type vault_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._delete_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                vault_name=vault_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})
+
+        if polling is True:
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    begin_delete.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}"
     }
 
     def _update_initial(
         self,
         resource_group_name: str,
         vault_name: str,
@@ -821,24 +860,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.BackupVaultResource]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PatchResourceRequestInput")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
@@ -850,16 +887,17 @@
             template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -886,15 +924,15 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.BackupVaultResource]:
         """Updates a BackupVault resource belonging to a resource group. For example, updating tags for a
         resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -923,15 +961,15 @@
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.BackupVaultResource]:
         """Updates a BackupVault resource belonging to a resource group. For example, updating tags for a
         resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param parameters: Request body for operation. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -958,20 +996,21 @@
         vault_name: str,
         parameters: Union[_models.PatchResourceRequestInput, IO],
         **kwargs: Any
     ) -> LROPoller[_models.BackupVaultResource]:
         """Updates a BackupVault resource belonging to a resource group. For example, updating tags for a
         resource.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
-        :param parameters: Request body for operation. Is either a model type or a IO type. Required.
+        :param parameters: Request body for operation. Is either a PatchResourceRequestInput type or a
+         IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.PatchResourceRequestInput or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -984,17 +1023,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.dataprotection.models.BackupVaultResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.BackupVaultResource] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(
@@ -1045,15 +1082,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
 
         API to check for resource name availability.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: The location in which uniqueness will be verified. Required.
         :type location: str
         :param parameters: Check name availability request. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.CheckNameAvailabilityRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -1075,15 +1112,15 @@
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
 
         API to check for resource name availability.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: The location in which uniqueness will be verified. Required.
         :type location: str
         :param parameters: Check name availability request. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -1103,21 +1140,21 @@
         parameters: Union[_models.CheckNameAvailabilityRequest, IO],
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
 
         API to check for resource name availability.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: The location in which uniqueness will be verified. Required.
         :type location: str
-        :param parameters: Check name availability request. Is either a model type or a IO type.
-         Required.
+        :param parameters: Check name availability request. Is either a CheckNameAvailabilityRequest
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.CheckNameAvailabilityRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.CheckNameAvailabilityResult
@@ -1130,24 +1167,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CheckNameAvailabilityResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "CheckNameAvailabilityRequest")
 
         request = build_check_name_availability_request(
             resource_group_name=resource_group_name,
             location=location,
@@ -1159,16 +1194,17 @@
             template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_deleted_backup_instances_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_deleted_backup_instances_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar, Union, cast
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,42 +27,38 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/deletedBackupInstances",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -76,27 +71,27 @@
 
 def build_get_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/deletedBackupInstances/{backupInstanceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -110,27 +105,27 @@
 
 def build_undelete_request(
     resource_group_name: str, vault_name: str, backup_instance_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataProtection/backupVaults/{vaultName}/deletedBackupInstances/{backupInstanceName}/undelete",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
         "backupInstanceName": _SERIALIZER.url("backup_instance_name", backup_instance_name, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
@@ -144,15 +139,15 @@
 
 class DeletedBackupInstancesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`deleted_backup_instances` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -163,32 +158,30 @@
 
     @distributed_trace
     def list(
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> Iterable["_models.DeletedBackupInstanceResource"]:
         """Gets deleted backup instances belonging to a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DeletedBackupInstanceResource or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.dataprotection.models.DeletedBackupInstanceResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DeletedBackupInstanceResourceList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -234,16 +227,17 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
+            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=False, **kwargs
+                request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -257,15 +251,15 @@
 
     @distributed_trace
     def get(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> _models.DeletedBackupInstanceResource:
         """Gets a deleted backup instance with name in a backup vault.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the deleted backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -280,17 +274,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DeletedBackupInstanceResource] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -298,16 +290,17 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -333,17 +326,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_undelete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             backup_instance_name=backup_instance_name,
             subscription_id=self._config.subscription_id,
@@ -351,16 +342,17 @@
             template_url=self._undelete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -374,15 +366,15 @@
 
     @distributed_trace
     def begin_undelete(
         self, resource_group_name: str, vault_name: str, backup_instance_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """undelete.
 
-        :param resource_group_name: The name of the resource group where the backup vault is present.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the backup vault. Required.
         :type vault_name: str
         :param backup_instance_name: The name of the deleted backup instance. Required.
         :type backup_instance_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
@@ -396,17 +388,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._undelete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure/mgmt/dataprotection/operations/_data_protection_operations.py` & `azure-mgmt-dataprotection-1.1.0/azure/mgmt/dataprotection/operations/_data_protection_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import sys
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,32 +24,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_feature_support_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2022-11-01-preview")
-    )
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-01-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.DataProtection/locations/{location}/checkFeatureSupport",
@@ -74,15 +68,15 @@
 
 class DataProtectionOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dataprotection.DataProtectionClient`'s
+        :class:`~azure.mgmt.dataprotection.DataProtectionMgmtClient`'s
         :attr:`data_protection` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
@@ -144,16 +138,16 @@
     ) -> _models.FeatureValidationResponseBase:
         """Validates if a feature is supported.
 
         Validates if a feature is supported.
 
         :param location: Required.
         :type location: str
-        :param parameters: Feature support request object. Is either a model type or a IO type.
-         Required.
+        :param parameters: Feature support request object. Is either a FeatureValidationRequestBase
+         type or a IO type. Required.
         :type parameters: ~azure.mgmt.dataprotection.models.FeatureValidationRequestBase or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FeatureValidationResponseBase or the result of cls(response)
         :rtype: ~azure.mgmt.dataprotection.models.FeatureValidationResponseBase
@@ -166,24 +160,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-11-01-preview"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.FeatureValidationResponseBase] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IO, bytes)):
+        if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "FeatureValidationRequestBase")
 
         request = build_check_feature_support_request(
             location=location,
             subscription_id=self._config.subscription_id,
@@ -194,16 +186,17 @@
             template_url=self.check_feature_support.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/PKG-INFO` & `azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-dataprotection
-Version: 1.0.0b4
+Version: 1.1.0
 Summary: Microsoft Azure Data Protection Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -65,16 +65,17 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = DataProtectionClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-
-Code samples for this package can be found at [Data Protection Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Code samples for this package can be found at:
+- [Search Data Protection Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -85,14 +86,37 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-dataprotection%2FREADME.png)
 
 
 # Release History
 
+## 1.1.0 (2023-06-16)
+
+### Features Added
+
+  - Added operation group DppResourceGuardProxyOperations
+
+## 1.0.0 (2023-02-15)
+
+### Features Added
+
+  - Model AzureBackupDiscreteRecoveryPoint has a new parameter expiry_time
+  - Model BackupVault has a new parameter feature_settings
+  - Model PatchBackupVaultInput has a new parameter feature_settings
+  - Model TargetDetails has a new parameter target_resource_arm_id
+
+### Breaking Changes
+
+  - Client name is changed from `DataProtectionClient` to `DataProtectionMgmtClient`
+  - Model ResourceGuardResource no longer has parameter identity
+  - Removed operation group BackupInstancesExtensionRoutingOperations
+  - Removed operation group DppResourceGuardProxyOperations
+  - Renamed operation BackupVaultsOperations.delete to BackupVaultsOperations.begin_delete
+
 ## 1.0.0b4 (2023-01-17)
 
 ### Features Added
 
   - Added operation group BackupInstancesExtensionRoutingOperations
   - Added operation group DppResourceGuardProxyOperations
   - Model PolicyParameters has a new parameter backup_datasource_parameters_list
```

## Comparing `azure-mgmt-dataprotection-1.0.0b4/azure_mgmt_dataprotection.egg-info/SOURCES.txt` & `azure-mgmt-dataprotection-1.1.0/azure_mgmt_dataprotection.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 README.md
 _meta.json
 setup.py
 azure/__init__.py
 azure/mgmt/__init__.py
 azure/mgmt/dataprotection/__init__.py
 azure/mgmt/dataprotection/_configuration.py
-azure/mgmt/dataprotection/_data_protection_client.py
+azure/mgmt/dataprotection/_data_protection_mgmt_client.py
 azure/mgmt/dataprotection/_patch.py
 azure/mgmt/dataprotection/_serialization.py
 azure/mgmt/dataprotection/_vendor.py
 azure/mgmt/dataprotection/_version.py
 azure/mgmt/dataprotection/py.typed
 azure/mgmt/dataprotection/aio/__init__.py
 azure/mgmt/dataprotection/aio/_configuration.py
-azure/mgmt/dataprotection/aio/_data_protection_client.py
+azure/mgmt/dataprotection/aio/_data_protection_mgmt_client.py
 azure/mgmt/dataprotection/aio/_patch.py
 azure/mgmt/dataprotection/aio/operations/__init__.py
-azure/mgmt/dataprotection/aio/operations/_backup_instances_extension_routing_operations.py
 azure/mgmt/dataprotection/aio/operations/_backup_instances_operations.py
 azure/mgmt/dataprotection/aio/operations/_backup_policies_operations.py
 azure/mgmt/dataprotection/aio/operations/_backup_vault_operation_results_operations.py
 azure/mgmt/dataprotection/aio/operations/_backup_vaults_operations.py
 azure/mgmt/dataprotection/aio/operations/_data_protection_operations.py
 azure/mgmt/dataprotection/aio/operations/_data_protection_operations_operations.py
 azure/mgmt/dataprotection/aio/operations/_deleted_backup_instances_operations.py
@@ -37,19 +36,18 @@
 azure/mgmt/dataprotection/aio/operations/_operation_status_operations.py
 azure/mgmt/dataprotection/aio/operations/_operation_status_resource_group_context_operations.py
 azure/mgmt/dataprotection/aio/operations/_patch.py
 azure/mgmt/dataprotection/aio/operations/_recovery_points_operations.py
 azure/mgmt/dataprotection/aio/operations/_resource_guards_operations.py
 azure/mgmt/dataprotection/aio/operations/_restorable_time_ranges_operations.py
 azure/mgmt/dataprotection/models/__init__.py
-azure/mgmt/dataprotection/models/_data_protection_client_enums.py
+azure/mgmt/dataprotection/models/_data_protection_mgmt_client_enums.py
 azure/mgmt/dataprotection/models/_models_py3.py
 azure/mgmt/dataprotection/models/_patch.py
 azure/mgmt/dataprotection/operations/__init__.py
-azure/mgmt/dataprotection/operations/_backup_instances_extension_routing_operations.py
 azure/mgmt/dataprotection/operations/_backup_instances_operations.py
 azure/mgmt/dataprotection/operations/_backup_policies_operations.py
 azure/mgmt/dataprotection/operations/_backup_vault_operation_results_operations.py
 azure/mgmt/dataprotection/operations/_backup_vaults_operations.py
 azure/mgmt/dataprotection/operations/_data_protection_operations.py
 azure/mgmt/dataprotection/operations/_data_protection_operations_operations.py
 azure/mgmt/dataprotection/operations/_deleted_backup_instances_operations.py
```

