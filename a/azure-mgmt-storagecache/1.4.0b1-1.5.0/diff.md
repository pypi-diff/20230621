# Comparing `tmp/azure-mgmt-storagecache-1.4.0b1.zip` & `tmp/azure-mgmt-storagecache-1.5.0.zip`

## zipinfo {}

```diff
@@ -1,63 +1,68 @@
-Zip file size: 119746 bytes, number of entries: 61
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure/
--rw-rw-r--  2.0 unx      632 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/_meta.json
--rw-rw-r--  2.0 unx     4270 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     6545 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/PKG-INFO
--rw-rw-r--  2.0 unx     1375 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/README.md
--rw-rw-r--  2.0 unx     1074 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/LICENSE
--rw-rw-r--  2.0 unx     2831 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/setup.py
--rw-rw-r--  2.0 unx       38 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/setup.cfg
--rw-rw-r--  2.0 unx      218 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx      116 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     6545 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     2280 b- defN 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/SOURCES.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/
--rw-rw-r--  2.0 unx       65 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/
--rw-rw-r--  2.0 unx      488 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_version.py
--rw-rw-r--  2.0 unx     1530 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_patch.py
--rw-rw-r--  2.0 unx     3873 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_configuration.py
--rw-rw-r--  2.0 unx     1169 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_vendor.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/py.typed
--rw-rw-r--  2.0 unx     6275 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_storage_cache_management_client.py
--rw-rw-r--  2.0 unx      925 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/__init__.py
--rw-rw-r--  2.0 unx    77872 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_serialization.py
--rw-rw-r--  2.0 unx    42006 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_storage_targets_operations.py
--rw-rw-r--  2.0 unx     6652 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_operations.py
--rw-rw-r--  2.0 unx    31915 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_storage_target_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_patch.py
--rw-rw-r--  2.0 unx     7390 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_asc_usages_operations.py
--rw-rw-r--  2.0 unx     7038 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_usage_models_operations.py
--rw-rw-r--  2.0 unx     7019 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_skus_operations.py
--rw-rw-r--  2.0 unx   139340 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_caches_operations.py
--rw-rw-r--  2.0 unx     6205 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_asc_operations_operations.py
--rw-rw-r--  2.0 unx     1361 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Dec-12 06:55 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/
--rw-rw-r--  2.0 unx     1530 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_patch.py
--rw-rw-r--  2.0 unx     3921 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_configuration.py
--rw-rw-r--  2.0 unx     6434 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_storage_cache_management_client.py
--rw-rw-r--  2.0 unx      872 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/__init__.py
--rw-rw-r--  2.0 unx    34509 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
--rw-rw-r--  2.0 unx     5930 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    26066 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     6254 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
--rw-rw-r--  2.0 unx     6048 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
--rw-rw-r--  2.0 unx     6028 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_skus_operations.py
--rw-rw-r--  2.0 unx   118522 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_caches_operations.py
--rw-rw-r--  2.0 unx     4906 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
--rw-rw-r--  2.0 unx     1361 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     4657 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_patch.py
--rw-rw-r--  2.0 unx   102929 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_models_py3.py
--rw-rw-r--  2.0 unx     5934 b- defN 22-Dec-12 06:54 azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/__init__.py
-61 files, 705069 bytes uncompressed, 106274 bytes compressed:  84.9%
+Zip file size: 144195 bytes, number of entries: 66
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/
+-rw-rw-r--  2.0 unx      632 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/_meta.json
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/LICENSE
+-rw-rw-r--  2.0 unx     2864 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/setup.py
+-rw-rw-r--  2.0 unx     4891 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx     7983 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/PKG-INFO
+-rw-rw-r--  2.0 unx      218 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/MANIFEST.in
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/setup.cfg
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/README.md
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/
+-rw-rw-r--  2.0 unx     6571 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_storage_cache_management_client.py
+-rw-rw-r--  2.0 unx     1849 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_vendor.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_serialization.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_patch.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/__init__.py
+-rw-rw-r--  2.0 unx      486 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_version.py
+-rw-rw-r--  2.0 unx     3509 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_configuration.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/py.typed
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/
+-rw-rw-r--  2.0 unx     6739 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_storage_cache_management_client.py
+-rw-rw-r--  2.0 unx     1084 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_vendor.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_patch.py
+-rw-rw-r--  2.0 unx      872 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/__init__.py
+-rw-rw-r--  2.0 unx     3557 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_configuration.py
+-rw-rw-r--  2.0 unx   125977 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_caches_operations.py
+-rw-rw-r--  2.0 unx     5749 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    41238 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx     1611 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    51677 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_aml_filesystems_operations.py
+-rw-rw-r--  2.0 unx     4651 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
+-rw-rw-r--  2.0 unx     6073 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
+-rw-rw-r--  2.0 unx     5847 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_skus_operations.py
+-rw-rw-r--  2.0 unx    13442 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py
+-rw-rw-r--  2.0 unx     5867 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
+-rw-rw-r--  2.0 unx    27243 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
+-rw-rw-r--  2.0 unx     6672 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_patch.py
+-rw-rw-r--  2.0 unx     8682 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/__init__.py
+-rw-rw-r--  2.0 unx   147426 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_models_py3.py
+-rw-rw-r--  2.0 unx   147331 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_caches_operations.py
+-rw-rw-r--  2.0 unx     6432 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_operations.py
+-rw-rw-r--  2.0 unx    50480 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_targets_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_patch.py
+-rw-rw-r--  2.0 unx     1611 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/__init__.py
+-rw-rw-r--  2.0 unx    63404 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_aml_filesystems_operations.py
+-rw-rw-r--  2.0 unx     5953 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_asc_operations_operations.py
+-rw-rw-r--  2.0 unx     7184 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_asc_usages_operations.py
+-rw-rw-r--  2.0 unx     6813 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_skus_operations.py
+-rw-rw-r--  2.0 unx    15882 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py
+-rw-rw-r--  2.0 unx     6832 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_usage_models_operations.py
+-rw-rw-r--  2.0 unx    33259 b- defN 23-Jun-21 05:27 azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_target_operations.py
+-rw-rw-r--  2.0 unx     7983 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     2623 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx      124 b- defN 23-Jun-21 05:28 azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/requires.txt
+66 files, 937621 bytes uncompressed, 129611 bytes compressed:  86.2%
```

## zipnote {}

```diff
@@ -1,184 +1,199 @@
-Filename: azure-mgmt-storagecache-1.4.0b1/
+Filename: azure-mgmt-storagecache-1.5.0/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/
+Filename: azure-mgmt-storagecache-1.5.0/azure/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/
+Filename: azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/_meta.json
+Filename: azure-mgmt-storagecache-1.5.0/_meta.json
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/CHANGELOG.md
+Filename: azure-mgmt-storagecache-1.5.0/LICENSE
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/PKG-INFO
+Filename: azure-mgmt-storagecache-1.5.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/README.md
+Filename: azure-mgmt-storagecache-1.5.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/LICENSE
+Filename: azure-mgmt-storagecache-1.5.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/setup.py
+Filename: azure-mgmt-storagecache-1.5.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/setup.cfg
+Filename: azure-mgmt-storagecache-1.5.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/MANIFEST.in
+Filename: azure-mgmt-storagecache-1.5.0/README.md
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/requires.txt
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/dependency_links.txt
+Filename: azure-mgmt-storagecache-1.5.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/PKG-INFO
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/top_level.txt
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/not-zip-safe
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/SOURCES.txt
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/__init__.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_storage_cache_management_client.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/__init__.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_patch.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/__init__.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_version.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_version.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_patch.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/py.typed
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_configuration.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_vendor.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_storage_cache_management_client.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/py.typed
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_storage_cache_management_client.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/__init__.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_serialization.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_storage_targets_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_caches_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_storage_target_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_patch.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_asc_usages_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_usage_models_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_aml_filesystems_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_skus_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_caches_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_asc_operations_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_skus_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/__init__.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_patch.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_configuration.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_storage_cache_management_client.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/__init__.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_caches_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_patch.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_targets_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_skus_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_aml_filesystems_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_caches_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_asc_operations_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_asc_usages_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/__init__.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_skus_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_patch.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_usage_models_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_models_py3.py
+Filename: azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_target_operations.py
 Comment: 
 
-Filename: azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/__init__.py
+Filename: azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/PKG-INFO
+Comment: 
+
+Filename: azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/requires.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/_meta.json` & `azure-mgmt-storagecache-1.5.0/_meta.json`

 * *Files 7% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/storagecache/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.5.0 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'a04dcf17baa7d980c29248fa00c14a7c5b69e67f'",*

 * * "'use'": "{in […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/storagecache/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.2.7 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "23b62d4e4dab07dccda851cfe50f6c6afb705a3b",
+    "autorest_command": "autorest specification/storagecache/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.5.0 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "a04dcf17baa7d980c29248fa00c14a7c5b69e67f",
     "readme": "specification/storagecache/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.2.7",
+        "@autorest/python@6.5.0",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/CHANGELOG.md` & `azure-mgmt-storagecache-1.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Release History
 
+## 1.5.0 (2023-06-16)
+
+### Features Added
+
+  - Added operation group AmlFilesystemsOperations
+  - Added operation group StorageCacheManagementClientOperationsMixin
+
+## 1.4.0 (2023-02-15)
+
+### Features Added
+
+  - Added operation StorageTargetsOperations.begin_restore_defaults
+  - Model BlobNfsTarget has a new parameter verification_timer
+  - Model BlobNfsTarget has a new parameter write_back_timer
+  - Model Nfs3Target has a new parameter verification_timer
+  - Model Nfs3Target has a new parameter write_back_timer
+
+### Breaking Changes
+
+  - Renamed operation CachesOperations.update to CachesOperations.begin_update
+
 ## 1.4.0b1 (2022-12-12)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/PKG-INFO` & `azure-mgmt-storagecache-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-storagecache
-Version: 1.4.0b1
+Version: 1.5.0
 Summary: Microsoft Azure Storage Cache Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,36 +27,93 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-# Usage
+## Getting started
 
+### Prerequisites
 
-To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
- 
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [Storage Cache Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-storagecache
+pip install azure-identity
+```
+
+### Authentication
+
+By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
+
+- `AZURE_CLIENT_ID` for Azure client ID.
+- `AZURE_TENANT_ID` for Azure tenant ID.
+- `AZURE_CLIENT_SECRET` for Azure client secret.
+
+In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
+
+With above configuration, client can be authenticated by following code:
+
+```python
+from azure.identity import DefaultAzureCredential
+from azure.mgmt.storagecache import StorageCacheManagementClient
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = StorageCacheManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search Storage Cache Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+
+## Troubleshooting
+
+## Next steps
+
+## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-storagecache%2FREADME.png)
 
 
 # Release History
 
+## 1.5.0 (2023-06-16)
+
+### Features Added
+
+  - Added operation group AmlFilesystemsOperations
+  - Added operation group StorageCacheManagementClientOperationsMixin
+
+## 1.4.0 (2023-02-15)
+
+### Features Added
+
+  - Added operation StorageTargetsOperations.begin_restore_defaults
+  - Model BlobNfsTarget has a new parameter verification_timer
+  - Model BlobNfsTarget has a new parameter write_back_timer
+  - Model Nfs3Target has a new parameter verification_timer
+  - Model Nfs3Target has a new parameter write_back_timer
+
+### Breaking Changes
+
+  - Renamed operation CachesOperations.update to CachesOperations.begin_update
+
 ## 1.4.0b1 (2022-12-12)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/README.md` & `azure-mgmt-storagecache-1.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,25 +4,61 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-# Usage
+## Getting started
 
+### Prerequisites
 
-To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
- 
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [Storage Cache Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-storagecache
+pip install azure-identity
+```
+
+### Authentication
+
+By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
+
+- `AZURE_CLIENT_ID` for Azure client ID.
+- `AZURE_TENANT_ID` for Azure tenant ID.
+- `AZURE_CLIENT_SECRET` for Azure client secret.
+
+In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
+
+With above configuration, client can be authenticated by following code:
+
+```python
+from azure.identity import DefaultAzureCredential
+from azure.mgmt.storagecache import StorageCacheManagementClient
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = StorageCacheManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search Storage Cache Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+
+## Troubleshooting
+
+## Next steps
+
+## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-storagecache%2FREADME.png)
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/LICENSE` & `azure-mgmt-storagecache-1.5.0/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/setup.py` & `azure-mgmt-storagecache-1.5.0/setup.py`

 * *Files 11% similar despite different names*

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
 PACKAGE_NAME = "azure-mgmt-storagecache"
 PACKAGE_PPRINT_NAME = "Storage Cache Management"
 
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
+        "Development Status :: 5 - Production/Stable",
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

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/PKG-INFO` & `azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-storagecache
-Version: 1.4.0b1
+Version: 1.5.0
 Summary: Microsoft Azure Storage Cache Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,36 +27,93 @@
 This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-# Usage
+## Getting started
 
+### Prerequisites
 
-To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
- 
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [Storage Cache Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+- Python 3.7+ is required to use this package.
+- [Azure subscription](https://azure.microsoft.com/free/)
 
+### Install the package
 
-# Provide Feedback
+```bash
+pip install azure-mgmt-storagecache
+pip install azure-identity
+```
+
+### Authentication
+
+By default, [Azure Active Directory](https://aka.ms/awps/aad) token authentication depends on correct configure of following environment variables.
+
+- `AZURE_CLIENT_ID` for Azure client ID.
+- `AZURE_TENANT_ID` for Azure tenant ID.
+- `AZURE_CLIENT_SECRET` for Azure client secret.
+
+In addition, Azure subscription ID can be configured via environment variable `AZURE_SUBSCRIPTION_ID`.
+
+With above configuration, client can be authenticated by following code:
+
+```python
+from azure.identity import DefaultAzureCredential
+from azure.mgmt.storagecache import StorageCacheManagementClient
+import os
+
+sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
+client = StorageCacheManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
+```
+
+## Examples
+
+Code samples for this package can be found at:
+- [Search Storage Cache Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
+- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+
+## Troubleshooting
+
+## Next steps
+
+## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-storagecache%2FREADME.png)
 
 
 # Release History
 
+## 1.5.0 (2023-06-16)
+
+### Features Added
+
+  - Added operation group AmlFilesystemsOperations
+  - Added operation group StorageCacheManagementClientOperationsMixin
+
+## 1.4.0 (2023-02-15)
+
+### Features Added
+
+  - Added operation StorageTargetsOperations.begin_restore_defaults
+  - Model BlobNfsTarget has a new parameter verification_timer
+  - Model BlobNfsTarget has a new parameter write_back_timer
+  - Model Nfs3Target has a new parameter verification_timer
+  - Model Nfs3Target has a new parameter write_back_timer
+
+### Breaking Changes
+
+  - Renamed operation CachesOperations.update to CachesOperations.begin_update
+
 ## 1.4.0b1 (2022-12-12)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure_mgmt_storagecache.egg-info/SOURCES.txt` & `azure-mgmt-storagecache-1.5.0/azure_mgmt_storagecache.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,40 @@
 azure/mgmt/storagecache/_vendor.py
 azure/mgmt/storagecache/_version.py
 azure/mgmt/storagecache/py.typed
 azure/mgmt/storagecache/aio/__init__.py
 azure/mgmt/storagecache/aio/_configuration.py
 azure/mgmt/storagecache/aio/_patch.py
 azure/mgmt/storagecache/aio/_storage_cache_management_client.py
+azure/mgmt/storagecache/aio/_vendor.py
 azure/mgmt/storagecache/aio/operations/__init__.py
+azure/mgmt/storagecache/aio/operations/_aml_filesystems_operations.py
 azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py
 azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py
 azure/mgmt/storagecache/aio/operations/_caches_operations.py
 azure/mgmt/storagecache/aio/operations/_operations.py
 azure/mgmt/storagecache/aio/operations/_patch.py
 azure/mgmt/storagecache/aio/operations/_skus_operations.py
+azure/mgmt/storagecache/aio/operations/_storage_cache_management_client_operations.py
 azure/mgmt/storagecache/aio/operations/_storage_target_operations.py
 azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py
 azure/mgmt/storagecache/aio/operations/_usage_models_operations.py
 azure/mgmt/storagecache/models/__init__.py
 azure/mgmt/storagecache/models/_models_py3.py
 azure/mgmt/storagecache/models/_patch.py
 azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py
 azure/mgmt/storagecache/operations/__init__.py
+azure/mgmt/storagecache/operations/_aml_filesystems_operations.py
 azure/mgmt/storagecache/operations/_asc_operations_operations.py
 azure/mgmt/storagecache/operations/_asc_usages_operations.py
 azure/mgmt/storagecache/operations/_caches_operations.py
 azure/mgmt/storagecache/operations/_operations.py
 azure/mgmt/storagecache/operations/_patch.py
 azure/mgmt/storagecache/operations/_skus_operations.py
+azure/mgmt/storagecache/operations/_storage_cache_management_client_operations.py
 azure/mgmt/storagecache/operations/_storage_target_operations.py
 azure/mgmt/storagecache/operations/_storage_targets_operations.py
 azure/mgmt/storagecache/operations/_usage_models_operations.py
 azure_mgmt_storagecache.egg-info/PKG-INFO
 azure_mgmt_storagecache.egg-info/SOURCES.txt
 azure_mgmt_storagecache.egg-info/dependency_links.txt
 azure_mgmt_storagecache.egg-info/not-zip-safe
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_patch.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_configuration.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,52 +2,45 @@
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
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
-
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class StorageCacheManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for StorageCacheManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-05-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-05-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(StorageCacheManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-05-01"] = kwargs.pop("api_version", "2022-05-01")
+        api_version: str = kwargs.pop("api_version", "2023-05-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -59,15 +52,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_storage_cache_management_client.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_storage_cache_management_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,34 +12,40 @@
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
 from . import models as _models
 from ._configuration import StorageCacheManagementClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
+    AmlFilesystemsOperations,
     AscOperationsOperations,
     AscUsagesOperations,
     CachesOperations,
     Operations,
     SkusOperations,
+    StorageCacheManagementClientOperationsMixin,
     StorageTargetOperations,
     StorageTargetsOperations,
     UsageModelsOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class StorageCacheManagementClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
-    """A Storage Cache provides scalable caching service for NAS clients, serving data from either
-    NFSv3 or Blob at-rest storage (referred to as "Storage Targets"). These operations allow you to
-    manage Caches.
+class StorageCacheManagementClient(
+    StorageCacheManagementClientOperationsMixin
+):  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+    """Azure Managed Lustre provides a fully managed Lustre® file system, integrated with Blob
+    storage, for use on demand. These operations create and manage Azure Managed Lustre file
+    systems.
 
+    :ivar aml_filesystems: AmlFilesystemsOperations operations
+    :vartype aml_filesystems: azure.mgmt.storagecache.operations.AmlFilesystemsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.storagecache.operations.Operations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.storagecache.operations.SkusOperations
     :ivar usage_models: UsageModelsOperations operations
     :vartype usage_models: azure.mgmt.storagecache.operations.UsageModelsOperations
     :ivar asc_operations: AscOperationsOperations operations
@@ -50,20 +56,19 @@
     :vartype caches: azure.mgmt.storagecache.operations.CachesOperations
     :ivar storage_targets: StorageTargetsOperations operations
     :vartype storage_targets: azure.mgmt.storagecache.operations.StorageTargetsOperations
     :ivar storage_target: StorageTargetOperations operations
     :vartype storage_target: azure.mgmt.storagecache.operations.StorageTargetOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-05-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-05-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -72,20 +77,21 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = StorageCacheManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
+        self.aml_filesystems = AmlFilesystemsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.usage_models = UsageModelsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_operations = AscOperationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_usages = AscUsagesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.caches = CachesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.storage_targets = StorageTargetsOperations(self._client, self._config, self._serialize, self._deserialize)
@@ -116,9 +122,9 @@
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "StorageCacheManagementClient":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details) -> None:
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/__init__.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/_serialization.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_serialization.py`

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

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_storage_targets_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_targets_operations.py`

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
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,44 +26,42 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_dns_refresh_request(
     resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -79,25 +77,27 @@
 
 def build_list_by_cache_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -116,25 +116,27 @@
     *,
     force: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -152,25 +154,27 @@
 
 def build_get_request(
     resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -186,26 +190,28 @@
 
 def build_create_or_update_request(
     resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -217,14 +223,50 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_restore_defaults_request(
+    resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
+        "storageTargetName": _SERIALIZER.url(
+            "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
+        ),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 class StorageTargetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.storagecache.StorageCacheManagementClient`'s
@@ -250,17 +292,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_dns_refresh_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -268,40 +308,49 @@
             template_url=self._dns_refresh_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _dns_refresh_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh"
     }
 
     @distributed_trace
     def begin_dns_refresh(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Tells a storage target to refresh its DNS information.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -313,17 +362,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._dns_refresh_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -362,32 +409,31 @@
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh"
     }
 
     @distributed_trace
     def list_by_cache(
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> Iterable["_models.StorageTarget"]:
-        """Returns a list of Storage Targets for the specified Cache.
+        """Returns a list of Storage Targets for the specified cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either StorageTarget or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.StorageTargetsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -433,16 +479,17 @@
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
 
@@ -469,17 +516,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -488,48 +533,57 @@
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
     }
 
     @distributed_trace
     def begin_delete(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
         force: Optional[str] = None,
         **kwargs: Any
     ) -> LROPoller[None]:
-        """Removes a Storage Target from a Cache. This operation is allowed at any time, but if the Cache
-        is down or unhealthy, the actual removal of the Storage Target may be delayed until the Cache
-        is healthy again. Note that if the Cache has data to flush to the Storage Target, the data will
+        """Removes a Storage Target from a cache. This operation is allowed at any time, but if the cache
+        is down or unhealthy, the actual removal of the Storage Target may be delayed until the cache
+        is healthy again. Note that if the cache has data to flush to the Storage Target, the data will
         be flushed before the Storage Target will be deleted.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :param force: Boolean value requesting the force delete operation for a storage target. Force
          delete discards unwritten-data in the cache instead of flushing it to back-end storage. Default
          value is None.
@@ -545,17 +599,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
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
@@ -593,19 +645,20 @@
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
     }
 
     @distributed_trace
     def get(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> _models.StorageTarget:
-        """Returns a Storage Target from a Cache.
+        """Returns a Storage Target from a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: StorageTarget or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.StorageTarget
@@ -618,17 +671,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -636,16 +687,17 @@
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
@@ -662,44 +714,39 @@
     }
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[Union[_models.StorageTarget, IO]] = None,
+        storagetarget: Union[_models.StorageTarget, IO],
         **kwargs: Any
     ) -> Optional[_models.StorageTarget]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.StorageTarget]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(storagetarget, (IO, bytes)):
+        if isinstance(storagetarget, (IOBase, bytes)):
             _content = storagetarget
         else:
-            if storagetarget is not None:
-                _json = self._serialize.body(storagetarget, "StorageTarget")
-            else:
-                _json = None
+            _json = self._serialize.body(storagetarget, "StorageTarget")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -709,16 +756,17 @@
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
@@ -741,32 +789,32 @@
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[_models.StorageTarget] = None,
+        storagetarget: _models.StorageTarget,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.StorageTarget]:
-        """Create or update a Storage Target. This operation is allowed at any time, but if the Cache is
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
-        the Cache is healthy again.
+        the cache is healthy again.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :param storagetarget: Object containing the definition of a Storage Target. Default value is
-         None.
+        :param storagetarget: Object containing the definition of a Storage Target. Required.
         :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -783,32 +831,32 @@
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[IO] = None,
+        storagetarget: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.StorageTarget]:
-        """Create or update a Storage Target. This operation is allowed at any time, but if the Cache is
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
-        the Cache is healthy again.
+        the cache is healthy again.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :param storagetarget: Object containing the definition of a Storage Target. Default value is
-         None.
+        :param storagetarget: Object containing the definition of a Storage Target. Required.
         :type storagetarget: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -825,30 +873,31 @@
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[Union[_models.StorageTarget, IO]] = None,
+        storagetarget: Union[_models.StorageTarget, IO],
         **kwargs: Any
     ) -> LROPoller[_models.StorageTarget]:
-        """Create or update a Storage Target. This operation is allowed at any time, but if the Cache is
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
-        the Cache is healthy again.
+        the cache is healthy again.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :param storagetarget: Object containing the definition of a Storage Target. Is either a model
-         type or a IO type. Default value is None.
+        :param storagetarget: Object containing the definition of a Storage Target. Is either a
+         StorageTarget type or a IO type. Required.
         :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -861,17 +910,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -908,7 +955,134 @@
                 deserialization_callback=get_long_running_output,
             )
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
     }
+
+    def _restore_defaults_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> None:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_restore_defaults_request(
+            resource_group_name=resource_group_name,
+            cache_name=cache_name,
+            storage_target_name=storage_target_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._restore_defaults_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
+        if cls:
+            return cls(pipeline_response, None, response_headers)
+
+    _restore_defaults_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults"
+    }
+
+    @distributed_trace
+    def begin_restore_defaults(
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> LROPoller[None]:
+        """Tells a storage target to restore its settings to their default values.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
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
+            raw_result = self._restore_defaults_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                cache_name=cache_name,
+                storage_target_name=storage_target_name,
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
+
+    begin_restore_defaults.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults"
+    }
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_operations.py`

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
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -24,32 +23,28 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.StorageCache/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -87,17 +82,15 @@
         :return: An iterator like instance of either ApiOperation or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.ApiOperation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApiOperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -140,16 +133,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_storage_target_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_storage_target_operations.py`

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
@@ -24,44 +23,42 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_flush_request(
     resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -77,25 +74,27 @@
 
 def build_suspend_request(
     resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -111,25 +110,27 @@
 
 def build_resume_request(
     resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -145,25 +146,27 @@
 
 def build_invalidate_request(
     resource_group_name: str, cache_name: str, storage_target_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
         "storageTargetName": _SERIALIZER.url(
             "storage_target_name", storage_target_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
@@ -206,17 +209,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_flush_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -224,42 +225,51 @@
             template_url=self._flush_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _flush_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush"
     }
 
     @distributed_trace
     def begin_flush(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Tells the cache to write all dirty data to the Storage Target's backend storage. Client
         requests to this storage target's namespace will return errors until the flush operation
         completes.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -271,17 +281,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._flush_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -330,17 +338,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_suspend_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -348,40 +354,49 @@
             template_url=self._suspend_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _suspend_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend"
     }
 
     @distributed_trace
     def begin_suspend(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Suspends client access to a storage target.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -393,17 +408,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._suspend_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -452,17 +465,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_resume_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -470,40 +481,49 @@
             template_url=self._resume_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _resume_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume"
     }
 
     @distributed_trace
     def begin_resume(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Resumes client access to a previously suspended storage target.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -515,17 +535,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._resume_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -574,17 +592,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_invalidate_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -592,41 +608,50 @@
             template_url=self._invalidate_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _invalidate_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate"
     }
 
     @distributed_trace
     def begin_invalidate(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Invalidate all cached data for a storage target. Cached files are discarded and fetched from
         the back end on the next request.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -638,17 +663,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._invalidate_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_patch.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_asc_usages_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_asc_usages_operations.py`

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
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -24,40 +23,36 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/usages"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "location": _SERIALIZER.url("location", location, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -97,17 +92,15 @@
         :return: An iterator like instance of either ResourceUsage or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.ResourceUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceUsagesListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -152,16 +145,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_usage_models_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_usage_models_operations.py`

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
@@ -24,38 +23,34 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/usageModels")
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -82,27 +77,25 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.UsageModel"]:
-        """Get the list of Cache Usage Models available to this subscription.
+        """Get the list of cache usage models available to this subscription.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either UsageModel or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.UsageModel]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.UsageModelsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -146,16 +139,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_skus_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_skus_operations.py`

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
 from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -24,38 +23,34 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/skus")
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -92,17 +87,15 @@
         :return: An iterator like instance of either ResourceSku or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.ResourceSku]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceSkusResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -146,16 +139,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_caches_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_caches_operations.py`

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
 from typing import Any, Callable, Dict, IO, Iterable, List, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,38 +26,34 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request, _format_url_section
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/caches")
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -67,25 +63,27 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -95,26 +93,28 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_request(resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -124,26 +124,28 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -155,26 +157,28 @@
 
 def build_create_or_update_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -187,26 +191,28 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_request(resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -221,25 +227,27 @@
 
 def build_debug_info_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/debugInfo",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -250,25 +258,27 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_flush_request(resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/flush",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -279,25 +289,27 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_start_request(resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/start",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -308,25 +320,27 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_stop_request(resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stop",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -339,26 +353,28 @@
 
 def build_start_priming_job_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/startPrimingJob",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -373,27 +389,29 @@
 
 def build_stop_priming_job_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stopPrimingJob",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -407,27 +425,29 @@
 
 def build_pause_priming_job_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/pausePrimingJob",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -441,27 +461,29 @@
 
 def build_resume_priming_job_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/resumePrimingJob",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -475,25 +497,27 @@
 
 def build_upgrade_firmware_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/upgrade",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -506,26 +530,28 @@
 
 def build_space_allocation_request(
     resource_group_name: str, cache_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/spaceAllocation",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "cacheName": _SERIALIZER.url("cache_name", cache_name, "str", pattern=r"^[-0-9a-zA-Z_]{1,80}$"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -555,27 +581,25 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.Cache"]:
-        """Returns all Caches the user has access to under a subscription.
+        """Returns all caches the user has access to under a subscription.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cache or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CachesListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -619,16 +643,17 @@
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
 
@@ -636,29 +661,28 @@
 
         return ItemPaged(get_next, extract_data)
 
     list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/caches"}
 
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.Cache"]:
-        """Returns all Caches the user has access to under a resource group.
+        """Returns all caches the user has access to under a resource group.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cache or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CachesListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -703,16 +727,17 @@
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
 
@@ -734,55 +759,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> LROPoller[None]:
-        """Schedules a Cache for deletion.
+        """Schedules a cache for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
@@ -792,17 +824,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
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
@@ -836,19 +866,20 @@
 
     begin_delete.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     @distributed_trace
     def get(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> _models.Cache:
-        """Returns a Cache.
+        """Returns a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Cache or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.Cache
         :raises ~azure.core.exceptions.HttpResponseError:
         """
@@ -859,33 +890,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Cache] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
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
@@ -898,43 +928,38 @@
         return deserialized
 
     get.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     def _create_or_update_initial(
-        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO], **kwargs: Any
     ) -> Optional[_models.Cache]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.Cache]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(cache, (IO, bytes)):
+        if isinstance(cache, (IOBase, bytes)):
             _content = cache
         else:
-            if cache is not None:
-                _json = self._serialize.body(cache, "Cache")
-            else:
-                _json = None
+            _json = self._serialize.body(cache, "Cache")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -943,16 +968,17 @@
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
@@ -974,29 +1000,29 @@
     }
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
-        cache: Optional[_models.Cache] = None,
+        cache: _models.Cache,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Cache]:
-        """Create or update a Cache.
+        """Create or update a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the new Cache. If read-only
-         properties are included, they must match the existing values of those properties. Default value
-         is None.
+        :param cache: Object containing the user-selectable properties of the new cache. If read-only
+         properties are included, they must match the existing values of those properties. Required.
         :type cache: ~azure.mgmt.storagecache.models.Cache
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1011,29 +1037,29 @@
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
-        cache: Optional[IO] = None,
+        cache: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Cache]:
-        """Create or update a Cache.
+        """Create or update a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the new Cache. If read-only
-         properties are included, they must match the existing values of those properties. Default value
-         is None.
+        :param cache: Object containing the user-selectable properties of the new cache. If read-only
+         properties are included, they must match the existing values of those properties. Required.
         :type cache: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1045,26 +1071,27 @@
         :return: An instance of LROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
-        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO], **kwargs: Any
     ) -> LROPoller[_models.Cache]:
-        """Create or update a Cache.
+        """Create or update a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the new Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the new cache. If read-only
          properties are included, they must match the existing values of those properties. Is either a
-         model type or a IO type. Default value is None.
+         Cache type or a IO type. Required.
         :type cache: ~azure.mgmt.storagecache.models.Cache or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1076,17 +1103,15 @@
         :return: An instance of LROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Cache] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -1123,158 +1148,243 @@
             )
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
+    def _update_initial(
+        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+    ) -> Optional[_models.Cache]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.Cache]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(cache, (IOBase, bytes)):
+            _content = cache
+        else:
+            if cache is not None:
+                _json = self._serialize.body(cache, "Cache")
+            else:
+                _json = None
+
+        request = build_update_request(
+            resource_group_name=resource_group_name,
+            cache_name=cache_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._update_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("Cache", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)
+
+        return deserialized
+
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
+    }
+
     @overload
-    def update(
+    def begin_update(
         self,
         resource_group_name: str,
         cache_name: str,
         cache: Optional[_models.Cache] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Cache:
-        """Update a Cache instance.
+    ) -> LROPoller[_models.Cache]:
+        """Update a cache instance.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Default value
          is None.
         :type cache: ~azure.mgmt.storagecache.models.Cache
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Cache or the result of cls(response)
-        :rtype: ~azure.mgmt.storagecache.models.Cache
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either Cache or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def update(
+    def begin_update(
         self,
         resource_group_name: str,
         cache_name: str,
         cache: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Cache:
-        """Update a Cache instance.
+    ) -> LROPoller[_models.Cache]:
+        """Update a cache instance.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Default value
          is None.
         :type cache: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Cache or the result of cls(response)
-        :rtype: ~azure.mgmt.storagecache.models.Cache
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either Cache or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
-    def update(
+    def begin_update(
         self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
-    ) -> _models.Cache:
-        """Update a Cache instance.
+    ) -> LROPoller[_models.Cache]:
+        """Update a cache instance.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Is either a
-         model type or a IO type. Default value is None.
+         Cache type or a IO type. Default value is None.
         :type cache: ~azure.mgmt.storagecache.models.Cache or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Cache or the result of cls(response)
-        :rtype: ~azure.mgmt.storagecache.models.Cache
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either Cache or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Cache] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._update_initial(
+                resource_group_name=resource_group_name,
+                cache_name=cache_name,
+                cache=cache,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
 
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(cache, (IO, bytes)):
-            _content = cache
-        else:
-            if cache is not None:
-                _json = self._serialize.body(cache, "Cache")
-            else:
-                _json = None
-
-        request = build_update_request(
-            resource_group_name=resource_group_name,
-            cache_name=cache_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self.update.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("Cache", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("Cache", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
 
-        return deserialized
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
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
 
-    update.metadata = {
+    begin_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     def _debug_info_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
@@ -1284,55 +1394,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_debug_info_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._debug_info_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _debug_info_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/debugInfo"
     }
 
     @distributed_trace
     def begin_debug_info(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> LROPoller[None]:
-        """Tells a Cache to write generate debug info for support to process.
+        """Tells a cache to write generate debug info for support to process.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
@@ -1342,17 +1459,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._debug_info_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1400,56 +1515,63 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_flush_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._flush_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _flush_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/flush"
     }
 
     @distributed_trace
     def begin_flush(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> LROPoller[None]:
-        """Tells a Cache to write all dirty data to the Storage Target(s). During the flush, clients will
+        """Tells a cache to write all dirty data to the Storage Target(s). During the flush, clients will
         see errors returned until the flush is complete.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
@@ -1459,17 +1581,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._flush_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1517,55 +1637,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_start_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._start_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _start_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/start"
     }
 
     @distributed_trace
     def begin_start(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> LROPoller[None]:
-        """Tells a Stopped state Cache to transition to Active state.
+        """Tells a Stopped state cache to transition to Active state.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
@@ -1575,17 +1702,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._start_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1633,55 +1758,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_stop_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._stop_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _stop_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stop"
     }
 
     @distributed_trace
     def begin_stop(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> LROPoller[None]:
-        """Tells an Active Cache to transition to Stopped state.
+        """Tells an Active cache to transition to Stopped state.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
@@ -1691,17 +1823,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._stop_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1753,24 +1883,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(primingjob, (IO, bytes)):
+        if isinstance(primingjob, (IOBase, bytes)):
             _content = primingjob
         else:
             if primingjob is not None:
                 _json = self._serialize.body(primingjob, "PrimingJob")
             else:
                 _json = None
 
@@ -1785,16 +1913,17 @@
             template_url=self._start_priming_job_initial.metadata["url"],
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
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1820,17 +1949,18 @@
         primingjob: Optional[_models.PrimingJob] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param primingjob: Object containing the definition of a priming job. Default value is None.
         :type primingjob: ~azure.mgmt.storagecache.models.PrimingJob
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1855,17 +1985,18 @@
         primingjob: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param primingjob: Object containing the definition of a priming job. Default value is None.
         :type primingjob: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1888,21 +2019,22 @@
         resource_group_name: str,
         cache_name: str,
         primingjob: Optional[Union[_models.PrimingJob, IO]] = None,
         **kwargs: Any
     ) -> LROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param primingjob: Object containing the definition of a priming job. Is either a model type or
-         a IO type. Default value is None.
+        :param primingjob: Object containing the definition of a priming job. Is either a PrimingJob
+         type or a IO type. Default value is None.
         :type primingjob: ~azure.mgmt.storagecache.models.PrimingJob or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -1914,17 +2046,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._start_priming_job_initial(  # type: ignore
@@ -1979,24 +2109,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(priming_job_id, (IO, bytes)):
+        if isinstance(priming_job_id, (IOBase, bytes)):
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
@@ -2011,16 +2139,17 @@
             template_url=self._stop_priming_job_initial.metadata["url"],
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
@@ -2047,17 +2176,18 @@
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Schedule a priming job for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2082,17 +2212,18 @@
         priming_job_id: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Schedule a priming job for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2115,21 +2246,22 @@
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
         **kwargs: Any
     ) -> LROPoller[None]:
         """Schedule a priming job for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param priming_job_id: Object containing the priming job ID. Is either a model type or a IO
-         type. Default value is None.
+        :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
+         type or a IO type. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -2141,17 +2273,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._stop_priming_job_initial(  # type: ignore
@@ -2206,24 +2336,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(priming_job_id, (IO, bytes)):
+        if isinstance(priming_job_id, (IOBase, bytes)):
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
@@ -2238,16 +2366,17 @@
             template_url=self._pause_priming_job_initial.metadata["url"],
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
@@ -2274,17 +2403,18 @@
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Schedule a priming job to be paused.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2309,17 +2439,18 @@
         priming_job_id: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Schedule a priming job to be paused.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2342,21 +2473,22 @@
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
         **kwargs: Any
     ) -> LROPoller[None]:
         """Schedule a priming job to be paused.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param priming_job_id: Object containing the priming job ID. Is either a model type or a IO
-         type. Default value is None.
+        :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
+         type or a IO type. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -2368,17 +2500,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._pause_priming_job_initial(  # type: ignore
@@ -2433,24 +2563,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(priming_job_id, (IO, bytes)):
+        if isinstance(priming_job_id, (IOBase, bytes)):
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
@@ -2465,16 +2593,17 @@
             template_url=self._resume_priming_job_initial.metadata["url"],
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
@@ -2501,17 +2630,18 @@
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Resumes a paused priming job.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2536,17 +2666,18 @@
         priming_job_id: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Resumes a paused priming job.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2569,21 +2700,22 @@
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
         **kwargs: Any
     ) -> LROPoller[None]:
         """Resumes a paused priming job.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param priming_job_id: Object containing the priming job ID. Is either a model type or a IO
-         type. Default value is None.
+        :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
+         type or a IO type. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
@@ -2595,17 +2727,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._resume_priming_job_initial(  # type: ignore
@@ -2656,56 +2786,63 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_upgrade_firmware_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._upgrade_firmware_initial.metadata["url"],
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
 
         if response.status_code not in [201, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _upgrade_firmware_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/upgrade"
     }
 
     @distributed_trace
     def begin_upgrade_firmware(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> LROPoller[None]:
-        """Upgrade a Cache's firmware if a new version is available. Otherwise, this operation has no
+        """Upgrade a cache's firmware if a new version is available. Otherwise, this operation has no
         effect.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
@@ -2715,17 +2852,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._upgrade_firmware_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2777,24 +2912,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(space_allocation, (IO, bytes)):
+        if isinstance(space_allocation, (IOBase, bytes)):
             _content = space_allocation
         else:
             if space_allocation is not None:
                 _json = self._serialize.body(space_allocation, "[StorageTargetSpaceAllocation]")
             else:
                 _json = None
 
@@ -2809,16 +2942,17 @@
             template_url=self._space_allocation_initial.metadata["url"],
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
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2844,17 +2978,18 @@
         space_allocation: Optional[List[_models.StorageTargetSpaceAllocation]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Update cache space allocation.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations.
          Default value is None.
         :type space_allocation: list[~azure.mgmt.storagecache.models.StorageTargetSpaceAllocation]
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -2880,17 +3015,18 @@
         space_allocation: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[None]:
         """Update cache space allocation.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations.
          Default value is None.
         :type space_allocation: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -2914,21 +3050,22 @@
         resource_group_name: str,
         cache_name: str,
         space_allocation: Optional[Union[List[_models.StorageTargetSpaceAllocation], IO]] = None,
         **kwargs: Any
     ) -> LROPoller[None]:
         """Update cache space allocation.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations. Is
-         either a list type or a IO type. Default value is None.
+         either a [StorageTargetSpaceAllocation] type or a IO type. Default value is None.
         :type space_allocation: list[~azure.mgmt.storagecache.models.StorageTargetSpaceAllocation] or
          IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
@@ -2941,17 +3078,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._space_allocation_initial(  # type: ignore
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/_asc_operations_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_asc_operations_operations.py`

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
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -22,43 +21,39 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import StorageCacheManagementClientMixinABC, _convert_request, _format_url_section
 
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
 
-    api_version: Literal["2022-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2022-05-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/locations/{location}/ascOperations/{operationId}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "location": _SERIALIZER.url("location", location, "str"),
-        "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "location": _SERIALIZER.url("location", location, "str", min_length=1),
+        "operationId": _SERIALIZER.url("operation_id", operation_id, "str", min_length=1),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -87,18 +82,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def get(self, location: str, operation_id: str, **kwargs: Any) -> _models.AscOperation:
         """Gets the status of an asynchronous operation for the Azure HPC Cache.
 
-        :param location: The name of the region used to look up the operation. Required.
+        :param location: The name of Azure region. Required.
         :type location: str
-        :param operation_id: The operation id which uniquely identifies the asynchronous operation.
-         Required.
+        :param operation_id: The ID of an ongoing async operation. Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AscOperation or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.AscOperation
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
@@ -108,33 +102,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AscOperation] = kwargs.pop("cls", None)
 
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

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/operations/__init__.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._aml_filesystems_operations import AmlFilesystemsOperations
+from ._storage_cache_management_client_operations import StorageCacheManagementClientOperationsMixin
 from ._operations import Operations
 from ._skus_operations import SkusOperations
 from ._usage_models_operations import UsageModelsOperations
 from ._asc_operations_operations import AscOperationsOperations
 from ._asc_usages_operations import AscUsagesOperations
 from ._caches_operations import CachesOperations
 from ._storage_targets_operations import StorageTargetsOperations
 from ._storage_target_operations import StorageTargetOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "AmlFilesystemsOperations",
+    "StorageCacheManagementClientOperationsMixin",
     "Operations",
     "SkusOperations",
     "UsageModelsOperations",
     "AscOperationsOperations",
     "AscUsagesOperations",
     "CachesOperations",
     "StorageTargetsOperations",
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_patch.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_configuration.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/_configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,52 +2,45 @@
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
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
-
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class StorageCacheManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for StorageCacheManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :type credential: ~azure.core.credentials.TokenCredential
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2022-05-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-05-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(StorageCacheManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2022-05-01"] = kwargs.pop("api_version", "2022-05-01")
+        api_version: str = kwargs.pop("api_version", "2023-05-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -59,15 +52,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/_storage_cache_management_client.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/_storage_cache_management_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,34 +12,40 @@
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import StorageCacheManagementClientConfiguration
 from .operations import (
+    AmlFilesystemsOperations,
     AscOperationsOperations,
     AscUsagesOperations,
     CachesOperations,
     Operations,
     SkusOperations,
+    StorageCacheManagementClientOperationsMixin,
     StorageTargetOperations,
     StorageTargetsOperations,
     UsageModelsOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class StorageCacheManagementClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
-    """A Storage Cache provides scalable caching service for NAS clients, serving data from either
-    NFSv3 or Blob at-rest storage (referred to as "Storage Targets"). These operations allow you to
-    manage Caches.
+class StorageCacheManagementClient(
+    StorageCacheManagementClientOperationsMixin
+):  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+    """Azure Managed Lustre provides a fully managed Lustre® file system, integrated with Blob
+    storage, for use on demand. These operations create and manage Azure Managed Lustre file
+    systems.
 
+    :ivar aml_filesystems: AmlFilesystemsOperations operations
+    :vartype aml_filesystems: azure.mgmt.storagecache.aio.operations.AmlFilesystemsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.storagecache.aio.operations.Operations
     :ivar skus: SkusOperations operations
     :vartype skus: azure.mgmt.storagecache.aio.operations.SkusOperations
     :ivar usage_models: UsageModelsOperations operations
     :vartype usage_models: azure.mgmt.storagecache.aio.operations.UsageModelsOperations
     :ivar asc_operations: AscOperationsOperations operations
@@ -50,20 +56,19 @@
     :vartype caches: azure.mgmt.storagecache.aio.operations.CachesOperations
     :ivar storage_targets: StorageTargetsOperations operations
     :vartype storage_targets: azure.mgmt.storagecache.aio.operations.StorageTargetsOperations
     :ivar storage_target: StorageTargetOperations operations
     :vartype storage_target: azure.mgmt.storagecache.aio.operations.StorageTargetOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2022-05-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2023-05-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -72,20 +77,21 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = StorageCacheManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
+        self.aml_filesystems = AmlFilesystemsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.skus = SkusOperations(self._client, self._config, self._serialize, self._deserialize)
         self.usage_models = UsageModelsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_operations = AscOperationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.asc_usages = AscUsagesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.caches = CachesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.storage_targets = StorageTargetsOperations(self._client, self._config, self._serialize, self._deserialize)
@@ -116,9 +122,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "StorageCacheManagementClient":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/__init__.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_targets_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -33,20 +33,18 @@
 from ..._vendor import _convert_request
 from ...operations._storage_targets_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_dns_refresh_request,
     build_get_request,
     build_list_by_cache_request,
+    build_restore_defaults_request,
 )
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class StorageTargetsOperations:
     """
     .. warning::
@@ -76,17 +74,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_dns_refresh_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -94,40 +90,49 @@
             template_url=self._dns_refresh_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _dns_refresh_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh"
     }
 
     @distributed_trace_async
     async def begin_dns_refresh(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Tells a storage target to refresh its DNS information.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -139,17 +144,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._dns_refresh_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -189,32 +192,31 @@
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/dnsRefresh"
     }
 
     @distributed_trace
     def list_by_cache(
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.StorageTarget"]:
-        """Returns a list of Storage Targets for the specified Cache.
+        """Returns a list of Storage Targets for the specified cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either StorageTarget or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.StorageTargetsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -260,16 +262,17 @@
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
 
@@ -296,17 +299,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -315,48 +316,57 @@
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
     }
 
     @distributed_trace_async
     async def begin_delete(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
         force: Optional[str] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
-        """Removes a Storage Target from a Cache. This operation is allowed at any time, but if the Cache
-        is down or unhealthy, the actual removal of the Storage Target may be delayed until the Cache
-        is healthy again. Note that if the Cache has data to flush to the Storage Target, the data will
+        """Removes a Storage Target from a cache. This operation is allowed at any time, but if the cache
+        is down or unhealthy, the actual removal of the Storage Target may be delayed until the cache
+        is healthy again. Note that if the cache has data to flush to the Storage Target, the data will
         be flushed before the Storage Target will be deleted.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :param force: Boolean value requesting the force delete operation for a storage target. Force
          delete discards unwritten-data in the cache instead of flushing it to back-end storage. Default
          value is None.
@@ -372,17 +382,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
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
@@ -420,19 +428,20 @@
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
     }
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> _models.StorageTarget:
-        """Returns a Storage Target from a Cache.
+        """Returns a Storage Target from a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: StorageTarget or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.StorageTarget
@@ -445,17 +454,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -463,16 +470,17 @@
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
@@ -489,44 +497,39 @@
     }
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[Union[_models.StorageTarget, IO]] = None,
+        storagetarget: Union[_models.StorageTarget, IO],
         **kwargs: Any
     ) -> Optional[_models.StorageTarget]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.StorageTarget]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(storagetarget, (IO, bytes)):
+        if isinstance(storagetarget, (IOBase, bytes)):
             _content = storagetarget
         else:
-            if storagetarget is not None:
-                _json = self._serialize.body(storagetarget, "StorageTarget")
-            else:
-                _json = None
+            _json = self._serialize.body(storagetarget, "StorageTarget")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -536,16 +539,17 @@
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
@@ -568,32 +572,32 @@
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[_models.StorageTarget] = None,
+        storagetarget: _models.StorageTarget,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.StorageTarget]:
-        """Create or update a Storage Target. This operation is allowed at any time, but if the Cache is
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
-        the Cache is healthy again.
+        the cache is healthy again.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :param storagetarget: Object containing the definition of a Storage Target. Default value is
-         None.
+        :param storagetarget: Object containing the definition of a Storage Target. Required.
         :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -610,32 +614,32 @@
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[IO] = None,
+        storagetarget: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.StorageTarget]:
-        """Create or update a Storage Target. This operation is allowed at any time, but if the Cache is
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
-        the Cache is healthy again.
+        the cache is healthy again.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :param storagetarget: Object containing the definition of a Storage Target. Default value is
-         None.
+        :param storagetarget: Object containing the definition of a Storage Target. Required.
         :type storagetarget: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -652,30 +656,31 @@
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
         storage_target_name: str,
-        storagetarget: Optional[Union[_models.StorageTarget, IO]] = None,
+        storagetarget: Union[_models.StorageTarget, IO],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.StorageTarget]:
-        """Create or update a Storage Target. This operation is allowed at any time, but if the Cache is
+        """Create or update a Storage Target. This operation is allowed at any time, but if the cache is
         down or unhealthy, the actual creation/modification of the Storage Target may be delayed until
-        the Cache is healthy again.
+        the cache is healthy again.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
-        :param storagetarget: Object containing the definition of a Storage Target. Is either a model
-         type or a IO type. Default value is None.
+        :param storagetarget: Object containing the definition of a Storage Target. Is either a
+         StorageTarget type or a IO type. Required.
         :type storagetarget: ~azure.mgmt.storagecache.models.StorageTarget or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -688,17 +693,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.StorageTarget]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.StorageTarget] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -735,7 +738,134 @@
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}"
     }
+
+    async def _restore_defaults_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> None:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_restore_defaults_request(
+            resource_group_name=resource_group_name,
+            cache_name=cache_name,
+            storage_target_name=storage_target_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._restore_defaults_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
+        if cls:
+            return cls(pipeline_response, None, response_headers)
+
+    _restore_defaults_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults"
+    }
+
+    @distributed_trace_async
+    async def begin_restore_defaults(
+        self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[None]:
+        """Tells a storage target to restore its settings to their default values.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
+         from the [-0-9a-zA-Z_] char class. Required.
+        :type cache_name: str
+        :param storage_target_name: Name of Storage Target. Required.
+        :type storage_target_name: str
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
+            raw_result = await self._restore_defaults_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                cache_name=cache_name,
+                storage_target_name=storage_target_name,
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
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
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
+    begin_restore_defaults.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/restoreDefaults"
+    }
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_operations.py`

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
@@ -25,19 +24,16 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operations import build_list_request
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class Operations:
     """
     .. warning::
@@ -65,17 +61,15 @@
         :return: An iterator like instance of either ApiOperation or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ApiOperation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApiOperationListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -118,16 +112,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_storage_target_operations.py`

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
@@ -30,19 +29,16 @@
 from ..._vendor import _convert_request
 from ...operations._storage_target_operations import (
     build_flush_request,
     build_invalidate_request,
     build_resume_request,
     build_suspend_request,
 )
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class StorageTargetOperations:
     """
     .. warning::
@@ -72,17 +68,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_flush_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -90,42 +84,51 @@
             template_url=self._flush_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _flush_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/flush"
     }
 
     @distributed_trace_async
     async def begin_flush(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Tells the cache to write all dirty data to the Storage Target's backend storage. Client
         requests to this storage target's namespace will return errors until the flush operation
         completes.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -137,17 +140,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._flush_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -197,17 +198,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_suspend_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -215,40 +214,49 @@
             template_url=self._suspend_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _suspend_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/suspend"
     }
 
     @distributed_trace_async
     async def begin_suspend(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Suspends client access to a storage target.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -260,17 +268,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._suspend_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -320,17 +326,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_resume_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -338,40 +342,49 @@
             template_url=self._resume_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _resume_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/resume"
     }
 
     @distributed_trace_async
     async def begin_resume(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Resumes client access to a previously suspended storage target.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -383,17 +396,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._resume_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -443,17 +454,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_invalidate_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             storage_target_name=storage_target_name,
             subscription_id=self._config.subscription_id,
@@ -461,41 +470,50 @@
             template_url=self._invalidate_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _invalidate_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/storageTargets/{storageTargetName}/invalidate"
     }
 
     @distributed_trace_async
     async def begin_invalidate(
         self, resource_group_name: str, cache_name: str, storage_target_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Invalidate all cached data for a storage target. Cached files are discarded and fetched from
         the back end on the next request.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param storage_target_name: Name of Storage Target. Required.
         :type storage_target_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -507,17 +525,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._invalidate_initial(  # type: ignore
                 resource_group_name=resource_group_name,
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_patch.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_asc_usages_operations.py`

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
@@ -25,19 +24,16 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._asc_usages_operations import build_list_request
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AscUsagesOperations:
     """
     .. warning::
@@ -67,17 +63,15 @@
         :return: An iterator like instance of either ResourceUsage or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ResourceUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceUsagesListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -122,16 +116,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_usage_models_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -25,19 +24,16 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._usage_models_operations import build_list_request
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class UsageModelsOperations:
     """
     .. warning::
@@ -55,27 +51,25 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.UsageModel"]:
-        """Get the list of Cache Usage Models available to this subscription.
+        """Get the list of cache usage models available to this subscription.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either UsageModel or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.UsageModel]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.UsageModelsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -119,16 +113,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_skus_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_skus_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -25,19 +24,16 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._skus_operations import build_list_request
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SkusOperations:
     """
     .. warning::
@@ -65,17 +61,15 @@
         :return: An iterator like instance of either ResourceSku or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.ResourceSku]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ResourceSkusResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -119,16 +113,17 @@
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
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_caches_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_caches_operations.py`

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
 from typing import Any, AsyncIterable, Callable, Dict, IO, List, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -45,19 +45,16 @@
     build_start_priming_job_request,
     build_start_request,
     build_stop_priming_job_request,
     build_stop_request,
     build_update_request,
     build_upgrade_firmware_request,
 )
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class CachesOperations:  # pylint: disable=too-many-public-methods
     """
     .. warning::
@@ -75,27 +72,25 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.Cache"]:
-        """Returns all Caches the user has access to under a subscription.
+        """Returns all caches the user has access to under a subscription.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cache or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CachesListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -139,16 +134,17 @@
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
 
@@ -156,29 +152,28 @@
 
         return AsyncItemPaged(get_next, extract_data)
 
     list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.StorageCache/caches"}
 
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.Cache"]:
-        """Returns all Caches the user has access to under a resource group.
+        """Returns all caches the user has access to under a resource group.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cache or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.CachesListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -223,16 +218,17 @@
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
 
@@ -254,55 +250,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     @distributed_trace_async
     async def begin_delete(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """Schedules a Cache for deletion.
+        """Schedules a cache for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
@@ -312,17 +315,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
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
@@ -356,19 +357,20 @@
 
     begin_delete.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     @distributed_trace_async
     async def get(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> _models.Cache:
-        """Returns a Cache.
+        """Returns a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Cache or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.Cache
         :raises ~azure.core.exceptions.HttpResponseError:
         """
@@ -379,33 +381,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Cache] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
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
@@ -418,43 +419,38 @@
         return deserialized
 
     get.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     async def _create_or_update_initial(
-        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO], **kwargs: Any
     ) -> Optional[_models.Cache]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[Optional[_models.Cache]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(cache, (IO, bytes)):
+        if isinstance(cache, (IOBase, bytes)):
             _content = cache
         else:
-            if cache is not None:
-                _json = self._serialize.body(cache, "Cache")
-            else:
-                _json = None
+            _json = self._serialize.body(cache, "Cache")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
@@ -463,16 +459,17 @@
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
@@ -494,29 +491,29 @@
     }
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
-        cache: Optional[_models.Cache] = None,
+        cache: _models.Cache,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cache]:
-        """Create or update a Cache.
+        """Create or update a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the new Cache. If read-only
-         properties are included, they must match the existing values of those properties. Default value
-         is None.
+        :param cache: Object containing the user-selectable properties of the new cache. If read-only
+         properties are included, they must match the existing values of those properties. Required.
         :type cache: ~azure.mgmt.storagecache.models.Cache
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -531,29 +528,29 @@
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cache_name: str,
-        cache: Optional[IO] = None,
+        cache: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cache]:
-        """Create or update a Cache.
+        """Create or update a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the new Cache. If read-only
-         properties are included, they must match the existing values of those properties. Default value
-         is None.
+        :param cache: Object containing the user-selectable properties of the new cache. If read-only
+         properties are included, they must match the existing values of those properties. Required.
         :type cache: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -565,26 +562,27 @@
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
-        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+        self, resource_group_name: str, cache_name: str, cache: Union[_models.Cache, IO], **kwargs: Any
     ) -> AsyncLROPoller[_models.Cache]:
-        """Create or update a Cache.
+        """Create or update a cache.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the new Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the new cache. If read-only
          properties are included, they must match the existing values of those properties. Is either a
-         model type or a IO type. Default value is None.
+         Cache type or a IO type. Required.
         :type cache: ~azure.mgmt.storagecache.models.Cache or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -596,17 +594,15 @@
         :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Cache] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -643,158 +639,244 @@
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_create_or_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
+    async def _update_initial(
+        self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
+    ) -> Optional[_models.Cache]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.Cache]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(cache, (IOBase, bytes)):
+            _content = cache
+        else:
+            if cache is not None:
+                _json = self._serialize.body(cache, "Cache")
+            else:
+                _json = None
+
+        request = build_update_request(
+            resource_group_name=resource_group_name,
+            cache_name=cache_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self._update_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("Cache", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)
+
+        return deserialized
+
+    _update_initial.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
+    }
+
     @overload
-    async def update(
+    async def begin_update(
         self,
         resource_group_name: str,
         cache_name: str,
         cache: Optional[_models.Cache] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Cache:
-        """Update a Cache instance.
+    ) -> AsyncLROPoller[_models.Cache]:
+        """Update a cache instance.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Default value
          is None.
         :type cache: ~azure.mgmt.storagecache.models.Cache
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Cache or the result of cls(response)
-        :rtype: ~azure.mgmt.storagecache.models.Cache
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def update(
+    async def begin_update(
         self,
         resource_group_name: str,
         cache_name: str,
         cache: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Cache:
-        """Update a Cache instance.
+    ) -> AsyncLROPoller[_models.Cache]:
+        """Update a cache instance.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Default value
          is None.
         :type cache: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Cache or the result of cls(response)
-        :rtype: ~azure.mgmt.storagecache.models.Cache
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
-    async def update(
+    async def begin_update(
         self, resource_group_name: str, cache_name: str, cache: Optional[Union[_models.Cache, IO]] = None, **kwargs: Any
-    ) -> _models.Cache:
-        """Update a Cache instance.
+    ) -> AsyncLROPoller[_models.Cache]:
+        """Update a cache instance.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param cache: Object containing the user-selectable properties of the Cache. If read-only
+        :param cache: Object containing the user-selectable properties of the cache. If read-only
          properties are included, they must match the existing values of those properties. Is either a
-         model type or a IO type. Default value is None.
+         Cache type or a IO type. Default value is None.
         :type cache: ~azure.mgmt.storagecache.models.Cache or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Cache or the result of cls(response)
-        :rtype: ~azure.mgmt.storagecache.models.Cache
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either Cache or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.storagecache.models.Cache]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Cache] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._update_initial(
+                resource_group_name=resource_group_name,
+                cache_name=cache_name,
+                cache=cache,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
 
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(cache, (IO, bytes)):
-            _content = cache
-        else:
-            if cache is not None:
-                _json = self._serialize.body(cache, "Cache")
-            else:
-                _json = None
-
-        request = build_update_request(
-            resource_group_name=resource_group_name,
-            cache_name=cache_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self.update.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("Cache", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("Cache", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
 
-        return deserialized
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
+            )
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
 
-    update.metadata = {
+    begin_update.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}"
     }
 
     async def _debug_info_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> None:
         error_map = {
@@ -804,55 +886,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_debug_info_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._debug_info_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _debug_info_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/debugInfo"
     }
 
     @distributed_trace_async
     async def begin_debug_info(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """Tells a Cache to write generate debug info for support to process.
+        """Tells a cache to write generate debug info for support to process.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
@@ -862,17 +951,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._debug_info_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -921,56 +1008,63 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_flush_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._flush_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _flush_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/flush"
     }
 
     @distributed_trace_async
     async def begin_flush(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """Tells a Cache to write all dirty data to the Storage Target(s). During the flush, clients will
+        """Tells a cache to write all dirty data to the Storage Target(s). During the flush, clients will
         see errors returned until the flush is complete.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
@@ -980,17 +1074,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._flush_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1039,55 +1131,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_start_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._start_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _start_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/start"
     }
 
     @distributed_trace_async
     async def begin_start(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """Tells a Stopped state Cache to transition to Active state.
+        """Tells a Stopped state cache to transition to Active state.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
@@ -1097,17 +1196,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._start_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1156,55 +1253,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_stop_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._stop_initial.metadata["url"],
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
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _stop_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/stop"
     }
 
     @distributed_trace_async
     async def begin_stop(self, resource_group_name: str, cache_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """Tells an Active Cache to transition to Stopped state.
+        """Tells an Active cache to transition to Stopped state.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
@@ -1214,17 +1318,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._stop_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -1277,24 +1379,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(primingjob, (IO, bytes)):
+        if isinstance(primingjob, (IOBase, bytes)):
             _content = primingjob
         else:
             if primingjob is not None:
                 _json = self._serialize.body(primingjob, "PrimingJob")
             else:
                 _json = None
 
@@ -1309,16 +1409,17 @@
             template_url=self._start_priming_job_initial.metadata["url"],
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
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -1344,17 +1445,18 @@
         primingjob: Optional[_models.PrimingJob] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param primingjob: Object containing the definition of a priming job. Default value is None.
         :type primingjob: ~azure.mgmt.storagecache.models.PrimingJob
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1379,17 +1481,18 @@
         primingjob: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param primingjob: Object containing the definition of a priming job. Default value is None.
         :type primingjob: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1412,21 +1515,22 @@
         resource_group_name: str,
         cache_name: str,
         primingjob: Optional[Union[_models.PrimingJob, IO]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Create a priming job. This operation is only allowed when the cache is healthy.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param primingjob: Object containing the definition of a priming job. Is either a model type or
-         a IO type. Default value is None.
+        :param primingjob: Object containing the definition of a priming job. Is either a PrimingJob
+         type or a IO type. Default value is None.
         :type primingjob: ~azure.mgmt.storagecache.models.PrimingJob or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1438,17 +1542,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._start_priming_job_initial(  # type: ignore
@@ -1504,24 +1606,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(priming_job_id, (IO, bytes)):
+        if isinstance(priming_job_id, (IOBase, bytes)):
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
@@ -1536,16 +1636,17 @@
             template_url=self._stop_priming_job_initial.metadata["url"],
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
@@ -1572,17 +1673,18 @@
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1607,17 +1709,18 @@
         priming_job_id: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1640,21 +1743,22 @@
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job for deletion.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param priming_job_id: Object containing the priming job ID. Is either a model type or a IO
-         type. Default value is None.
+        :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
+         type or a IO type. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1666,17 +1770,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._stop_priming_job_initial(  # type: ignore
@@ -1732,24 +1834,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(priming_job_id, (IO, bytes)):
+        if isinstance(priming_job_id, (IOBase, bytes)):
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
@@ -1764,16 +1864,17 @@
             template_url=self._pause_priming_job_initial.metadata["url"],
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
@@ -1800,17 +1901,18 @@
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job to be paused.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1835,17 +1937,18 @@
         priming_job_id: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job to be paused.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -1868,21 +1971,22 @@
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Schedule a priming job to be paused.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param priming_job_id: Object containing the priming job ID. Is either a model type or a IO
-         type. Default value is None.
+        :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
+         type or a IO type. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -1894,17 +1998,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._pause_priming_job_initial(  # type: ignore
@@ -1960,24 +2062,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(priming_job_id, (IO, bytes)):
+        if isinstance(priming_job_id, (IOBase, bytes)):
             _content = priming_job_id
         else:
             if priming_job_id is not None:
                 _json = self._serialize.body(priming_job_id, "PrimingJobIdParameter")
             else:
                 _json = None
 
@@ -1992,16 +2092,17 @@
             template_url=self._resume_priming_job_initial.metadata["url"],
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
@@ -2028,17 +2129,18 @@
         priming_job_id: Optional[_models.PrimingJobIdParameter] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Resumes a paused priming job.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2063,17 +2165,18 @@
         priming_job_id: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Resumes a paused priming job.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param priming_job_id: Object containing the priming job ID. Default value is None.
         :type priming_job_id: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
@@ -2096,21 +2199,22 @@
         resource_group_name: str,
         cache_name: str,
         priming_job_id: Optional[Union[_models.PrimingJobIdParameter, IO]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Resumes a paused priming job.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
-        :param priming_job_id: Object containing the priming job ID. Is either a model type or a IO
-         type. Default value is None.
+        :param priming_job_id: Object containing the priming job ID. Is either a PrimingJobIdParameter
+         type or a IO type. Default value is None.
         :type priming_job_id: ~azure.mgmt.storagecache.models.PrimingJobIdParameter or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
@@ -2122,17 +2226,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._resume_priming_job_initial(  # type: ignore
@@ -2184,58 +2286,65 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_upgrade_firmware_request(
             resource_group_name=resource_group_name,
             cache_name=cache_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self._upgrade_firmware_initial.metadata["url"],
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
 
         if response.status_code not in [201, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)
 
     _upgrade_firmware_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.StorageCache/caches/{cacheName}/upgrade"
     }
 
     @distributed_trace_async
     async def begin_upgrade_firmware(
         self, resource_group_name: str, cache_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
-        """Upgrade a Cache's firmware if a new version is available. Otherwise, this operation has no
+        """Upgrade a cache's firmware if a new version is available. Otherwise, this operation has no
         effect.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
@@ -2245,17 +2354,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._upgrade_firmware_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -2308,24 +2415,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(space_allocation, (IO, bytes)):
+        if isinstance(space_allocation, (IOBase, bytes)):
             _content = space_allocation
         else:
             if space_allocation is not None:
                 _json = self._serialize.body(space_allocation, "[StorageTargetSpaceAllocation]")
             else:
                 _json = None
 
@@ -2340,16 +2445,17 @@
             template_url=self._space_allocation_initial.metadata["url"],
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
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -2375,17 +2481,18 @@
         space_allocation: Optional[List[_models.StorageTargetSpaceAllocation]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Update cache space allocation.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations.
          Default value is None.
         :type space_allocation: list[~azure.mgmt.storagecache.models.StorageTargetSpaceAllocation]
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
@@ -2411,17 +2518,18 @@
         space_allocation: Optional[IO] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Update cache space allocation.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations.
          Default value is None.
         :type space_allocation: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
@@ -2445,21 +2553,22 @@
         resource_group_name: str,
         cache_name: str,
         space_allocation: Optional[Union[List[_models.StorageTargetSpaceAllocation], IO]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Update cache space allocation.
 
-        :param resource_group_name: Target resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param cache_name: Name of Cache. Length of name must not be greater than 80 and chars must be
+        :param cache_name: Name of cache. Length of name must not be greater than 80 and chars must be
          from the [-0-9a-zA-Z_] char class. Required.
         :type cache_name: str
         :param space_allocation: List containing storage target cache space percentage allocations. Is
-         either a list type or a IO type. Default value is None.
+         either a [StorageTargetSpaceAllocation] type or a IO type. Default value is None.
         :type space_allocation: list[~azure.mgmt.storagecache.models.StorageTargetSpaceAllocation] or
          IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
@@ -2472,17 +2581,15 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._space_allocation_initial(  # type: ignore
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/aio/operations/_asc_operations_operations.py`

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
@@ -23,19 +22,16 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._asc_operations_operations import build_get_request
+from .._vendor import StorageCacheManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class AscOperationsOperations:
     """
     .. warning::
@@ -55,18 +51,17 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def get(self, location: str, operation_id: str, **kwargs: Any) -> _models.AscOperation:
         """Gets the status of an asynchronous operation for the Azure HPC Cache.
 
-        :param location: The name of the region used to look up the operation. Required.
+        :param location: The name of Azure region. Required.
         :type location: str
-        :param operation_id: The operation id which uniquely identifies the asynchronous operation.
-         Required.
+        :param operation_id: The ID of an ongoing async operation. Required.
         :type operation_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AscOperation or the result of cls(response)
         :rtype: ~azure.mgmt.storagecache.models.AscOperation
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
@@ -76,33 +71,32 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: Literal["2022-05-01"] = kwargs.pop(
-            "api_version", _params.pop("api-version", self._config.api_version)
-        )
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.AscOperation] = kwargs.pop("cls", None)
 
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

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/aio/operations/__init__.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._aml_filesystems_operations import AmlFilesystemsOperations
+from ._storage_cache_management_client_operations import StorageCacheManagementClientOperationsMixin
 from ._operations import Operations
 from ._skus_operations import SkusOperations
 from ._usage_models_operations import UsageModelsOperations
 from ._asc_operations_operations import AscOperationsOperations
 from ._asc_usages_operations import AscUsagesOperations
 from ._caches_operations import CachesOperations
 from ._storage_targets_operations import StorageTargetsOperations
 from ._storage_target_operations import StorageTargetOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "AmlFilesystemsOperations",
+    "StorageCacheManagementClientOperationsMixin",
     "Operations",
     "SkusOperations",
     "UsageModelsOperations",
     "AscOperationsOperations",
     "AscUsagesOperations",
     "CachesOperations",
     "StorageTargetsOperations",
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_storage_cache_management_client_enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,55 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
+class AmlFilesystemHealthStateType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """List of AML file system health states."""
+
+    UNAVAILABLE = "Unavailable"
+    AVAILABLE = "Available"
+    DEGRADED = "Degraded"
+    TRANSITIONING = "Transitioning"
+    MAINTENANCE = "Maintenance"
+
+
+class AmlFilesystemIdentityType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The type of identity used for the resource."""
+
+    USER_ASSIGNED = "UserAssigned"
+    NONE = "None"
+
+
+class AmlFilesystemProvisioningStateType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """ARM provisioning state."""
+
+    SUCCEEDED = "Succeeded"
+    FAILED = "Failed"
+    CREATING = "Creating"
+    DELETING = "Deleting"
+    UPDATING = "Updating"
+    CANCELED = "Canceled"
+
+
+class ArchiveStatusType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The state of the archive operation."""
+
+    NOT_CONFIGURED = "NotConfigured"
+    IDLE = "Idle"
+    IN_PROGRESS = "InProgress"
+    CANCELED = "Canceled"
+    COMPLETED = "Completed"
+    FAILED = "Failed"
+    CANCELLING = "Cancelling"
+    FS_SCAN_IN_PROGRESS = "FSScanInProgress"
+
+
 class CacheIdentityType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity used for the cache."""
 
     SYSTEM_ASSIGNED = "SystemAssigned"
     USER_ASSIGNED = "UserAssigned"
     SYSTEM_ASSIGNED_USER_ASSIGNED = "SystemAssigned, UserAssigned"
     NONE = "None"
@@ -32,26 +73,38 @@
     """True if the HPC Cache is joined to the Active Directory domain."""
 
     YES = "Yes"
     NO = "No"
     ERROR = "Error"
 
 
+class FilesystemSubnetStatusType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The status of the AML file system subnet check."""
+
+    OK = "Ok"
+    INVALID = "Invalid"
+
+
 class FirmwareStatusType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """True if there is a firmware update ready to install on this Cache. The firmware will
+    """True if there is a firmware update ready to install on this cache. The firmware will
     automatically be installed after firmwareUpdateDeadline if not triggered earlier via the
     upgrade operation.
     """
 
     AVAILABLE = "available"
     UNAVAILABLE = "unavailable"
 
 
 class HealthStateType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """List of Cache health states."""
+    """List of cache health states. Down is when the cluster is not responding.  Degraded is when its
+    functioning but has some alerts. Transitioning when it is creating or deleting. Unknown will be
+    returned in old api versions when a new value is added in future versions. WaitingForKey is
+    when the create is waiting for the system assigned identity to be given access to the
+    encryption key in the encryption settings.
+    """
 
     UNKNOWN = "Unknown"
     HEALTHY = "Healthy"
     DEGRADED = "Degraded"
     DOWN = "Down"
     TRANSITIONING = "Transitioning"
     STOPPING = "Stopping"
@@ -59,14 +112,26 @@
     UPGRADING = "Upgrading"
     FLUSHING = "Flushing"
     WAITING_FOR_KEY = "WaitingForKey"
     START_FAILED = "StartFailed"
     UPGRADE_FAILED = "UpgradeFailed"
 
 
+class MaintenanceDayOfWeekType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Day of the week on which the maintenance window will occur."""
+
+    MONDAY = "Monday"
+    TUESDAY = "Tuesday"
+    WEDNESDAY = "Wednesday"
+    THURSDAY = "Thursday"
+    FRIDAY = "Friday"
+    SATURDAY = "Saturday"
+    SUNDAY = "Sunday"
+
+
 class MetricAggregationType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """MetricAggregationType."""
 
     NOT_SPECIFIED = "NotSpecified"
     NONE = "None"
     AVERAGE = "Average"
     MINIMUM = "Minimum"
@@ -112,15 +177,15 @@
 class ProvisioningStateType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """ARM provisioning state, see
     https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/Addendum.md#provisioningstate-property.
     """
 
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
-    CANCELLED = "Cancelled"
+    CANCELED = "Canceled"
     CREATING = "Creating"
     DELETING = "Deleting"
     UPDATING = "Updating"
 
 
 class ReasonCode(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The reason for the restriction. As of now this can be "QuotaId" or
```

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_patch.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-storagecache-1.4.0b1/azure/mgmt/storagecache/models/_models_py3.py` & `azure-mgmt-storagecache-1.5.0/azure/mgmt/storagecache/models/_models_py3.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,16 +20,892 @@
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 
 
+class Resource(_serialization.Model):
+    """Common fields that are returned in the response for all Azure Resource Manager resources.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.storagecache.models.SystemData
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
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.id = None
+        self.name = None
+        self.type = None
+        self.system_data = None
+
+
+class TrackedResource(Resource):
+    """The resource model definition for an Azure Resource Manager tracked top level resource which
+    has 'tags' and a 'location'.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.storagecache.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+    }
+
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
+        self.location = location
+
+
+class AmlFilesystem(TrackedResource):  # pylint: disable=too-many-instance-attributes
+    """An AML file system instance. Follows Azure Resource Manager standards:
+    https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/resource-api-reference.md.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.storagecache.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    :ivar identity: The managed identity used by the AML file system, if configured.
+    :vartype identity: ~azure.mgmt.storagecache.models.AmlFilesystemIdentity
+    :ivar sku: SKU for the resource.
+    :vartype sku: ~azure.mgmt.storagecache.models.SkuName
+    :ivar zones: Availability zones for resources. This field should only contain a single element
+     in the array.
+    :vartype zones: list[str]
+    :ivar storage_capacity_ti_b: The size of the AML file system, in TiB. This might be rounded up.
+    :vartype storage_capacity_ti_b: float
+    :ivar health: Health of the AML file system.
+    :vartype health: ~azure.mgmt.storagecache.models.AmlFilesystemHealth
+    :ivar provisioning_state: ARM provisioning state. Known values are: "Succeeded", "Failed",
+     "Creating", "Deleting", "Updating", and "Canceled".
+    :vartype provisioning_state: str or
+     ~azure.mgmt.storagecache.models.AmlFilesystemProvisioningStateType
+    :ivar filesystem_subnet: Subnet used for managing the AML file system and for client-facing
+     operations. This subnet should have at least a /24 subnet mask within the VNET's address space.
+    :vartype filesystem_subnet: str
+    :ivar client_info: Client information for the AML file system.
+    :vartype client_info: ~azure.mgmt.storagecache.models.AmlFilesystemClientInfo
+    :ivar throughput_provisioned_m_bps: Throughput provisioned in MB per sec, calculated as
+     storageCapacityTiB * per-unit storage throughput.
+    :vartype throughput_provisioned_m_bps: int
+    :ivar encryption_settings: Specifies encryption settings of the AML file system.
+    :vartype encryption_settings: ~azure.mgmt.storagecache.models.AmlFilesystemEncryptionSettings
+    :ivar maintenance_window: Start time of a 30-minute weekly maintenance window.
+    :vartype maintenance_window:
+     ~azure.mgmt.storagecache.models.AmlFilesystemPropertiesMaintenanceWindow
+    :ivar hsm: Hydration and archive settings and status.
+    :vartype hsm: ~azure.mgmt.storagecache.models.AmlFilesystemPropertiesHsm
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+        "health": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "client_info": {"readonly": True},
+        "throughput_provisioned_m_bps": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+        "identity": {"key": "identity", "type": "AmlFilesystemIdentity"},
+        "sku": {"key": "sku", "type": "SkuName"},
+        "zones": {"key": "zones", "type": "[str]"},
+        "storage_capacity_ti_b": {"key": "properties.storageCapacityTiB", "type": "float"},
+        "health": {"key": "properties.health", "type": "AmlFilesystemHealth"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "filesystem_subnet": {"key": "properties.filesystemSubnet", "type": "str"},
+        "client_info": {"key": "properties.clientInfo", "type": "AmlFilesystemClientInfo"},
+        "throughput_provisioned_m_bps": {"key": "properties.throughputProvisionedMBps", "type": "int"},
+        "encryption_settings": {"key": "properties.encryptionSettings", "type": "AmlFilesystemEncryptionSettings"},
+        "maintenance_window": {
+            "key": "properties.maintenanceWindow",
+            "type": "AmlFilesystemPropertiesMaintenanceWindow",
+        },
+        "hsm": {"key": "properties.hsm", "type": "AmlFilesystemPropertiesHsm"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        tags: Optional[Dict[str, str]] = None,
+        identity: Optional["_models.AmlFilesystemIdentity"] = None,
+        sku: Optional["_models.SkuName"] = None,
+        zones: Optional[List[str]] = None,
+        storage_capacity_ti_b: Optional[float] = None,
+        filesystem_subnet: Optional[str] = None,
+        encryption_settings: Optional["_models.AmlFilesystemEncryptionSettings"] = None,
+        maintenance_window: Optional["_models.AmlFilesystemPropertiesMaintenanceWindow"] = None,
+        hsm: Optional["_models.AmlFilesystemPropertiesHsm"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        :keyword identity: The managed identity used by the AML file system, if configured.
+        :paramtype identity: ~azure.mgmt.storagecache.models.AmlFilesystemIdentity
+        :keyword sku: SKU for the resource.
+        :paramtype sku: ~azure.mgmt.storagecache.models.SkuName
+        :keyword zones: Availability zones for resources. This field should only contain a single
+         element in the array.
+        :paramtype zones: list[str]
+        :keyword storage_capacity_ti_b: The size of the AML file system, in TiB. This might be rounded
+         up.
+        :paramtype storage_capacity_ti_b: float
+        :keyword filesystem_subnet: Subnet used for managing the AML file system and for client-facing
+         operations. This subnet should have at least a /24 subnet mask within the VNET's address space.
+        :paramtype filesystem_subnet: str
+        :keyword encryption_settings: Specifies encryption settings of the AML file system.
+        :paramtype encryption_settings: ~azure.mgmt.storagecache.models.AmlFilesystemEncryptionSettings
+        :keyword maintenance_window: Start time of a 30-minute weekly maintenance window.
+        :paramtype maintenance_window:
+         ~azure.mgmt.storagecache.models.AmlFilesystemPropertiesMaintenanceWindow
+        :keyword hsm: Hydration and archive settings and status.
+        :paramtype hsm: ~azure.mgmt.storagecache.models.AmlFilesystemPropertiesHsm
+        """
+        super().__init__(tags=tags, location=location, **kwargs)
+        self.identity = identity
+        self.sku = sku
+        self.zones = zones
+        self.storage_capacity_ti_b = storage_capacity_ti_b
+        self.health = None
+        self.provisioning_state = None
+        self.filesystem_subnet = filesystem_subnet
+        self.client_info = None
+        self.throughput_provisioned_m_bps = None
+        self.encryption_settings = encryption_settings
+        self.maintenance_window = maintenance_window
+        self.hsm = hsm
+
+
+class AmlFilesystemArchive(_serialization.Model):
+    """Information about the AML file system archive.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar filesystem_path: Lustre file system path to archive relative to the file system root.
+     Specify '/' to archive all modified data.
+    :vartype filesystem_path: str
+    :ivar status: The status of the archive.
+    :vartype status: ~azure.mgmt.storagecache.models.AmlFilesystemArchiveStatus
+    """
+
+    _validation = {
+        "filesystem_path": {"readonly": True},
+        "status": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "filesystem_path": {"key": "filesystemPath", "type": "str"},
+        "status": {"key": "status", "type": "AmlFilesystemArchiveStatus"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.filesystem_path = None
+        self.status = None
+
+
+class AmlFilesystemArchiveInfo(_serialization.Model):
+    """Information required to execute the archive operation.
+
+    :ivar filesystem_path: Lustre file system path to archive relative to the file system root.
+     Specify '/' to archive all modified data.
+    :vartype filesystem_path: str
+    """
+
+    _attribute_map = {
+        "filesystem_path": {"key": "filesystemPath", "type": "str"},
+    }
+
+    def __init__(self, *, filesystem_path: str = "/", **kwargs: Any) -> None:
+        """
+        :keyword filesystem_path: Lustre file system path to archive relative to the file system root.
+         Specify '/' to archive all modified data.
+        :paramtype filesystem_path: str
+        """
+        super().__init__(**kwargs)
+        self.filesystem_path = filesystem_path
+
+
+class AmlFilesystemArchiveStatus(_serialization.Model):
+    """The status of the archive.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar state: The state of the archive operation. Known values are: "NotConfigured", "Idle",
+     "InProgress", "Canceled", "Completed", "Failed", "Cancelling", and "FSScanInProgress".
+    :vartype state: str or ~azure.mgmt.storagecache.models.ArchiveStatusType
+    :ivar last_completion_time: The time of the last completed archive operation.
+    :vartype last_completion_time: ~datetime.datetime
+    :ivar last_started_time: The time the latest archive operation started.
+    :vartype last_started_time: ~datetime.datetime
+    :ivar percent_complete: The completion percentage of the archive operation.
+    :vartype percent_complete: int
+    :ivar error_code: Server-defined error code for the archive operation.
+    :vartype error_code: str
+    :ivar error_message: Server-defined error message for the archive operation.
+    :vartype error_message: str
+    """
+
+    _validation = {
+        "state": {"readonly": True},
+        "last_completion_time": {"readonly": True},
+        "last_started_time": {"readonly": True},
+        "percent_complete": {"readonly": True},
+        "error_code": {"readonly": True},
+        "error_message": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "state": {"key": "state", "type": "str"},
+        "last_completion_time": {"key": "lastCompletionTime", "type": "iso-8601"},
+        "last_started_time": {"key": "lastStartedTime", "type": "iso-8601"},
+        "percent_complete": {"key": "percentComplete", "type": "int"},
+        "error_code": {"key": "errorCode", "type": "str"},
+        "error_message": {"key": "errorMessage", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.state = None
+        self.last_completion_time = None
+        self.last_started_time = None
+        self.percent_complete = None
+        self.error_code = None
+        self.error_message = None
+
+
+class AmlFilesystemCheckSubnetError(_serialization.Model):
+    """The error details provided when the checkAmlFSSubnets call fails.
+
+    :ivar filesystem_subnet: The error details for the AML file system's subnet.
+    :vartype filesystem_subnet:
+     ~azure.mgmt.storagecache.models.AmlFilesystemCheckSubnetErrorFilesystemSubnet
+    """
+
+    _attribute_map = {
+        "filesystem_subnet": {"key": "filesystemSubnet", "type": "AmlFilesystemCheckSubnetErrorFilesystemSubnet"},
+    }
+
+    def __init__(
+        self,
+        *,
+        filesystem_subnet: Optional["_models.AmlFilesystemCheckSubnetErrorFilesystemSubnet"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword filesystem_subnet: The error details for the AML file system's subnet.
+        :paramtype filesystem_subnet:
+         ~azure.mgmt.storagecache.models.AmlFilesystemCheckSubnetErrorFilesystemSubnet
+        """
+        super().__init__(**kwargs)
+        self.filesystem_subnet = filesystem_subnet
+
+
+class AmlFilesystemCheckSubnetErrorFilesystemSubnet(_serialization.Model):
+    """The error details for the AML file system's subnet.
+
+    :ivar status: The status of the AML file system subnet check. Known values are: "Ok" and
+     "Invalid".
+    :vartype status: str or ~azure.mgmt.storagecache.models.FilesystemSubnetStatusType
+    :ivar message: The details of the AML file system subnet check.
+    :vartype message: str
+    """
+
+    _attribute_map = {
+        "status": {"key": "status", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        status: Optional[Union[str, "_models.FilesystemSubnetStatusType"]] = None,
+        message: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword status: The status of the AML file system subnet check. Known values are: "Ok" and
+         "Invalid".
+        :paramtype status: str or ~azure.mgmt.storagecache.models.FilesystemSubnetStatusType
+        :keyword message: The details of the AML file system subnet check.
+        :paramtype message: str
+        """
+        super().__init__(**kwargs)
+        self.status = status
+        self.message = message
+
+
+class AmlFilesystemClientInfo(_serialization.Model):
+    """AML file system client information.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar mgs_address: The IPv4 address used by clients to mount the AML file system's Lustre
+     Management Service (MGS).
+    :vartype mgs_address: str
+    :ivar mount_command: Recommended command to mount the AML file system.
+    :vartype mount_command: str
+    :ivar lustre_version: The version of Lustre running in the AML file system.
+    :vartype lustre_version: str
+    :ivar container_storage_interface: Container Storage Interface information for the AML file
+     system.
+    :vartype container_storage_interface:
+     ~azure.mgmt.storagecache.models.AmlFilesystemContainerStorageInterface
+    """
+
+    _validation = {
+        "mgs_address": {"readonly": True},
+        "mount_command": {"readonly": True},
+        "lustre_version": {"readonly": True},
+        "container_storage_interface": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "mgs_address": {"key": "mgsAddress", "type": "str"},
+        "mount_command": {"key": "mountCommand", "type": "str"},
+        "lustre_version": {"key": "lustreVersion", "type": "str"},
+        "container_storage_interface": {
+            "key": "containerStorageInterface",
+            "type": "AmlFilesystemContainerStorageInterface",
+        },
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.mgs_address = None
+        self.mount_command = None
+        self.lustre_version = None
+        self.container_storage_interface = None
+
+
+class AmlFilesystemContainerStorageInterface(_serialization.Model):
+    """AML file system container storage interface information.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar persistent_volume_claim: Recommended AKS Persistent Volume Claim for the CSI driver, in
+     Base64 encoded YAML.
+    :vartype persistent_volume_claim: str
+    :ivar persistent_volume: Recommended AKS Persistent Volume for the CSI driver, in Base64
+     encoded YAML.
+    :vartype persistent_volume: str
+    :ivar storage_class: Recommended AKS Storage Class for the CSI driver, in Base64 encoded YAML.
+    :vartype storage_class: str
+    """
+
+    _validation = {
+        "persistent_volume_claim": {"readonly": True},
+        "persistent_volume": {"readonly": True},
+        "storage_class": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "persistent_volume_claim": {"key": "persistentVolumeClaim", "type": "str"},
+        "persistent_volume": {"key": "persistentVolume", "type": "str"},
+        "storage_class": {"key": "storageClass", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.persistent_volume_claim = None
+        self.persistent_volume = None
+        self.storage_class = None
+
+
+class AmlFilesystemEncryptionSettings(_serialization.Model):
+    """AML file system encryption settings.
+
+    :ivar key_encryption_key: Specifies the location of the encryption key in Key Vault.
+    :vartype key_encryption_key: ~azure.mgmt.storagecache.models.KeyVaultKeyReference
+    """
+
+    _attribute_map = {
+        "key_encryption_key": {"key": "keyEncryptionKey", "type": "KeyVaultKeyReference"},
+    }
+
+    def __init__(self, *, key_encryption_key: Optional["_models.KeyVaultKeyReference"] = None, **kwargs: Any) -> None:
+        """
+        :keyword key_encryption_key: Specifies the location of the encryption key in Key Vault.
+        :paramtype key_encryption_key: ~azure.mgmt.storagecache.models.KeyVaultKeyReference
+        """
+        super().__init__(**kwargs)
+        self.key_encryption_key = key_encryption_key
+
+
+class AmlFilesystemHealth(_serialization.Model):
+    """An indication of AML file system health. Gives more information about health than just that
+    related to provisioning.
+
+    :ivar state: List of AML file system health states. Known values are: "Unavailable",
+     "Available", "Degraded", "Transitioning", and "Maintenance".
+    :vartype state: str or ~azure.mgmt.storagecache.models.AmlFilesystemHealthStateType
+    :ivar status_code: Server-defined error code for the AML file system health.
+    :vartype status_code: str
+    :ivar status_description: Describes the health state.
+    :vartype status_description: str
+    """
+
+    _attribute_map = {
+        "state": {"key": "state", "type": "str"},
+        "status_code": {"key": "statusCode", "type": "str"},
+        "status_description": {"key": "statusDescription", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        state: Optional[Union[str, "_models.AmlFilesystemHealthStateType"]] = None,
+        status_code: Optional[str] = None,
+        status_description: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword state: List of AML file system health states. Known values are: "Unavailable",
+         "Available", "Degraded", "Transitioning", and "Maintenance".
+        :paramtype state: str or ~azure.mgmt.storagecache.models.AmlFilesystemHealthStateType
+        :keyword status_code: Server-defined error code for the AML file system health.
+        :paramtype status_code: str
+        :keyword status_description: Describes the health state.
+        :paramtype status_description: str
+        """
+        super().__init__(**kwargs)
+        self.state = state
+        self.status_code = status_code
+        self.status_description = status_description
+
+
+class AmlFilesystemHsmSettings(_serialization.Model):
+    """AML file system HSM settings.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar container: Resource ID of storage container used for hydrating the namespace and
+     archiving from the namespace. The resource provider must have permission to create SAS tokens
+     on the storage account. Required.
+    :vartype container: str
+    :ivar logging_container: Resource ID of storage container used for logging events and errors.
+     Must be a separate container in the same storage account as the hydration and archive
+     container. The resource provider must have permission to create SAS tokens on the storage
+     account. Required.
+    :vartype logging_container: str
+    :ivar import_prefix: Only blobs in the non-logging container that start with this path/prefix
+     get hydrated into the cluster namespace.
+    :vartype import_prefix: str
+    """
+
+    _validation = {
+        "container": {"required": True},
+        "logging_container": {"required": True},
+    }
+
+    _attribute_map = {
+        "container": {"key": "container", "type": "str"},
+        "logging_container": {"key": "loggingContainer", "type": "str"},
+        "import_prefix": {"key": "importPrefix", "type": "str"},
+    }
+
+    def __init__(self, *, container: str, logging_container: str, import_prefix: str = "/", **kwargs: Any) -> None:
+        """
+        :keyword container: Resource ID of storage container used for hydrating the namespace and
+         archiving from the namespace. The resource provider must have permission to create SAS tokens
+         on the storage account. Required.
+        :paramtype container: str
+        :keyword logging_container: Resource ID of storage container used for logging events and
+         errors.  Must be a separate container in the same storage account as the hydration and archive
+         container. The resource provider must have permission to create SAS tokens on the storage
+         account. Required.
+        :paramtype logging_container: str
+        :keyword import_prefix: Only blobs in the non-logging container that start with this
+         path/prefix get hydrated into the cluster namespace.
+        :paramtype import_prefix: str
+        """
+        super().__init__(**kwargs)
+        self.container = container
+        self.logging_container = logging_container
+        self.import_prefix = import_prefix
+
+
+class AmlFilesystemIdentity(_serialization.Model):
+    """Managed Identity properties.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar principal_id: The principal ID for the user-assigned identity of the resource.
+    :vartype principal_id: str
+    :ivar tenant_id: The tenant ID associated with the resource.
+    :vartype tenant_id: str
+    :ivar type: The type of identity used for the resource. Known values are: "UserAssigned" and
+     "None".
+    :vartype type: str or ~azure.mgmt.storagecache.models.AmlFilesystemIdentityType
+    :ivar user_assigned_identities: A dictionary where each key is a user assigned identity
+     resource ID, and each key's value is an empty dictionary.
+    :vartype user_assigned_identities: dict[str,
+     ~azure.mgmt.storagecache.models.UserAssignedIdentitiesValue]
+    """
+
+    _validation = {
+        "principal_id": {"readonly": True},
+        "tenant_id": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "principal_id": {"key": "principalId", "type": "str"},
+        "tenant_id": {"key": "tenantId", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentitiesValue}"},
+    }
+
+    def __init__(
+        self,
+        *,
+        type: Optional[Union[str, "_models.AmlFilesystemIdentityType"]] = None,
+        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentitiesValue"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword type: The type of identity used for the resource. Known values are: "UserAssigned" and
+         "None".
+        :paramtype type: str or ~azure.mgmt.storagecache.models.AmlFilesystemIdentityType
+        :keyword user_assigned_identities: A dictionary where each key is a user assigned identity
+         resource ID, and each key's value is an empty dictionary.
+        :paramtype user_assigned_identities: dict[str,
+         ~azure.mgmt.storagecache.models.UserAssignedIdentitiesValue]
+        """
+        super().__init__(**kwargs)
+        self.principal_id = None
+        self.tenant_id = None
+        self.type = type
+        self.user_assigned_identities = user_assigned_identities
+
+
+class AmlFilesystemPropertiesHsm(_serialization.Model):
+    """Hydration and archive settings and status.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar settings: Specifies HSM settings of the AML file system.
+    :vartype settings: ~azure.mgmt.storagecache.models.AmlFilesystemHsmSettings
+    :ivar archive_status: Archive status.
+    :vartype archive_status: list[~azure.mgmt.storagecache.models.AmlFilesystemArchive]
+    """
+
+    _validation = {
+        "archive_status": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "settings": {"key": "settings", "type": "AmlFilesystemHsmSettings"},
+        "archive_status": {"key": "archiveStatus", "type": "[AmlFilesystemArchive]"},
+    }
+
+    def __init__(self, *, settings: Optional["_models.AmlFilesystemHsmSettings"] = None, **kwargs: Any) -> None:
+        """
+        :keyword settings: Specifies HSM settings of the AML file system.
+        :paramtype settings: ~azure.mgmt.storagecache.models.AmlFilesystemHsmSettings
+        """
+        super().__init__(**kwargs)
+        self.settings = settings
+        self.archive_status = None
+
+
+class AmlFilesystemPropertiesMaintenanceWindow(_serialization.Model):
+    """Start time of a 30-minute weekly maintenance window.
+
+    :ivar day_of_week: Day of the week on which the maintenance window will occur. Known values
+     are: "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", and "Sunday".
+    :vartype day_of_week: str or ~azure.mgmt.storagecache.models.MaintenanceDayOfWeekType
+    :ivar time_of_day_utc: The time of day (in UTC) to start the maintenance window.
+    :vartype time_of_day_utc: str
+    """
+
+    _validation = {
+        "time_of_day_utc": {"pattern": r"^([0-9]|0[0-9]|1[0-9]|2[0-3]):[0-5][0-9]$"},
+    }
+
+    _attribute_map = {
+        "day_of_week": {"key": "dayOfWeek", "type": "str"},
+        "time_of_day_utc": {"key": "timeOfDayUTC", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        day_of_week: Optional[Union[str, "_models.MaintenanceDayOfWeekType"]] = None,
+        time_of_day_utc: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword day_of_week: Day of the week on which the maintenance window will occur. Known values
+         are: "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", and "Sunday".
+        :paramtype day_of_week: str or ~azure.mgmt.storagecache.models.MaintenanceDayOfWeekType
+        :keyword time_of_day_utc: The time of day (in UTC) to start the maintenance window.
+        :paramtype time_of_day_utc: str
+        """
+        super().__init__(**kwargs)
+        self.day_of_week = day_of_week
+        self.time_of_day_utc = time_of_day_utc
+
+
+class AmlFilesystemsListResult(_serialization.Model):
+    """Result of the request to list AML file systems. It contains a list of AML file systems and a
+    URL link to get the next set of results.
+
+    :ivar next_link: URL to get the next set of AML file system list results, if there are any.
+    :vartype next_link: str
+    :ivar value: List of AML file systems.
+    :vartype value: list[~azure.mgmt.storagecache.models.AmlFilesystem]
+    """
+
+    _attribute_map = {
+        "next_link": {"key": "nextLink", "type": "str"},
+        "value": {"key": "value", "type": "[AmlFilesystem]"},
+    }
+
+    def __init__(
+        self, *, next_link: Optional[str] = None, value: Optional[List["_models.AmlFilesystem"]] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword next_link: URL to get the next set of AML file system list results, if there are any.
+        :paramtype next_link: str
+        :keyword value: List of AML file systems.
+        :paramtype value: list[~azure.mgmt.storagecache.models.AmlFilesystem]
+        """
+        super().__init__(**kwargs)
+        self.next_link = next_link
+        self.value = value
+
+
+class AmlFilesystemSubnetInfo(_serialization.Model):
+    """Information required to validate the subnet that will be used in AML file system create.
+
+    :ivar filesystem_subnet: Subnet used for managing the AML file system and for client-facing
+     operations. This subnet should have at least a /24 subnet mask within the VNET's address space.
+    :vartype filesystem_subnet: str
+    :ivar storage_capacity_ti_b: The size of the AML file system, in TiB.
+    :vartype storage_capacity_ti_b: float
+    :ivar sku: SKU for the resource.
+    :vartype sku: ~azure.mgmt.storagecache.models.SkuName
+    :ivar location: Region that the AML file system will be created in.
+    :vartype location: str
+    """
+
+    _attribute_map = {
+        "filesystem_subnet": {"key": "filesystemSubnet", "type": "str"},
+        "storage_capacity_ti_b": {"key": "storageCapacityTiB", "type": "float"},
+        "sku": {"key": "sku", "type": "SkuName"},
+        "location": {"key": "location", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        filesystem_subnet: Optional[str] = None,
+        storage_capacity_ti_b: Optional[float] = None,
+        sku: Optional["_models.SkuName"] = None,
+        location: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword filesystem_subnet: Subnet used for managing the AML file system and for client-facing
+         operations. This subnet should have at least a /24 subnet mask within the VNET's address space.
+        :paramtype filesystem_subnet: str
+        :keyword storage_capacity_ti_b: The size of the AML file system, in TiB.
+        :paramtype storage_capacity_ti_b: float
+        :keyword sku: SKU for the resource.
+        :paramtype sku: ~azure.mgmt.storagecache.models.SkuName
+        :keyword location: Region that the AML file system will be created in.
+        :paramtype location: str
+        """
+        super().__init__(**kwargs)
+        self.filesystem_subnet = filesystem_subnet
+        self.storage_capacity_ti_b = storage_capacity_ti_b
+        self.sku = sku
+        self.location = location
+
+
+class AmlFilesystemUpdate(_serialization.Model):
+    """An AML file system update instance.
+
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar encryption_settings: Specifies encryption settings of the AML file system.
+    :vartype encryption_settings: ~azure.mgmt.storagecache.models.AmlFilesystemEncryptionSettings
+    :ivar maintenance_window: Start time of a 30-minute weekly maintenance window.
+    :vartype maintenance_window:
+     ~azure.mgmt.storagecache.models.AmlFilesystemUpdatePropertiesMaintenanceWindow
+    """
+
+    _attribute_map = {
+        "tags": {"key": "tags", "type": "{str}"},
+        "encryption_settings": {"key": "properties.encryptionSettings", "type": "AmlFilesystemEncryptionSettings"},
+        "maintenance_window": {
+            "key": "properties.maintenanceWindow",
+            "type": "AmlFilesystemUpdatePropertiesMaintenanceWindow",
+        },
+    }
+
+    def __init__(
+        self,
+        *,
+        tags: Optional[Dict[str, str]] = None,
+        encryption_settings: Optional["_models.AmlFilesystemEncryptionSettings"] = None,
+        maintenance_window: Optional["_models.AmlFilesystemUpdatePropertiesMaintenanceWindow"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword encryption_settings: Specifies encryption settings of the AML file system.
+        :paramtype encryption_settings: ~azure.mgmt.storagecache.models.AmlFilesystemEncryptionSettings
+        :keyword maintenance_window: Start time of a 30-minute weekly maintenance window.
+        :paramtype maintenance_window:
+         ~azure.mgmt.storagecache.models.AmlFilesystemUpdatePropertiesMaintenanceWindow
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
+        self.encryption_settings = encryption_settings
+        self.maintenance_window = maintenance_window
+
+
+class AmlFilesystemUpdatePropertiesMaintenanceWindow(_serialization.Model):
+    """Start time of a 30-minute weekly maintenance window.
+
+    :ivar day_of_week: Day of the week on which the maintenance window will occur. Known values
+     are: "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", and "Sunday".
+    :vartype day_of_week: str or ~azure.mgmt.storagecache.models.MaintenanceDayOfWeekType
+    :ivar time_of_day_utc: The time of day (in UTC) to start the maintenance window.
+    :vartype time_of_day_utc: str
+    """
+
+    _validation = {
+        "time_of_day_utc": {"pattern": r"^([0-9]|0[0-9]|1[0-9]|2[0-3]):[0-5][0-9]$"},
+    }
+
+    _attribute_map = {
+        "day_of_week": {"key": "dayOfWeek", "type": "str"},
+        "time_of_day_utc": {"key": "timeOfDayUTC", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        day_of_week: Optional[Union[str, "_models.MaintenanceDayOfWeekType"]] = None,
+        time_of_day_utc: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword day_of_week: Day of the week on which the maintenance window will occur. Known values
+         are: "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", and "Sunday".
+        :paramtype day_of_week: str or ~azure.mgmt.storagecache.models.MaintenanceDayOfWeekType
+        :keyword time_of_day_utc: The time of day (in UTC) to start the maintenance window.
+        :paramtype time_of_day_utc: str
+        """
+        super().__init__(**kwargs)
+        self.day_of_week = day_of_week
+        self.time_of_day_utc = time_of_day_utc
+
+
 class ApiOperation(_serialization.Model):
-    """REST API operation description: see https://github.com/Azure/azure-rest-api-specs/blob/master/documentation/openapi-authoring-automated-guidelines.md#r3023-operationsapiimplementation.
+    """REST API operation description: see
+    https://github.com/Azure/azure-rest-api-specs/blob/master/documentation/openapi-authoring-automated-guidelines.md#r3023-operationsapiimplementation.
 
     :ivar display: The object that represents the operation.
     :vartype display: ~azure.mgmt.storagecache.models.ApiOperationDisplay
     :ivar origin: Origin of the operation.
     :vartype origin: str
     :ivar is_data_action: The flag that indicates whether the operation applies to data plane.
     :vartype is_data_action: bool
@@ -55,16 +931,16 @@
         self,
         *,
         display: Optional["_models.ApiOperationDisplay"] = None,
         origin: Optional[str] = None,
         is_data_action: Optional[bool] = None,
         name: Optional[str] = None,
         service_specification: Optional["_models.ApiOperationPropertiesServiceSpecification"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword display: The object that represents the operation.
         :paramtype display: ~azure.mgmt.storagecache.models.ApiOperationDisplay
         :keyword origin: Origin of the operation.
         :paramtype origin: str
         :keyword is_data_action: The flag that indicates whether the operation applies to data plane.
         :paramtype is_data_action: bool
@@ -106,16 +982,16 @@
     def __init__(
         self,
         *,
         operation: Optional[str] = None,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
         description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword operation: Operation type: Read, write, delete, etc.
         :paramtype operation: str
         :keyword provider: Service provider: Microsoft.StorageCache.
         :paramtype provider: str
         :keyword resource: Resource on which the operation is performed: Cache, etc.
         :paramtype resource: str
@@ -126,31 +1002,32 @@
         self.operation = operation
         self.provider = provider
         self.resource = resource
         self.description = description
 
 
 class ApiOperationListResult(_serialization.Model):
-    """Result of the request to list Resource Provider operations. It contains a list of operations and a URL link to get the next set of results.
+    """Result of the request to list Resource Provider operations. It contains a list of operations
+    and a URL link to get the next set of results.
 
     :ivar next_link: URL to get the next set of operation list results if there are any.
     :vartype next_link: str
     :ivar value: List of Resource Provider operations supported by the Microsoft.StorageCache
      resource provider.
     :vartype value: list[~azure.mgmt.storagecache.models.ApiOperation]
     """
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
         "value": {"key": "value", "type": "[ApiOperation]"},
     }
 
     def __init__(
-        self, *, next_link: Optional[str] = None, value: Optional[List["_models.ApiOperation"]] = None, **kwargs
-    ):
+        self, *, next_link: Optional[str] = None, value: Optional[List["_models.ApiOperation"]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: URL to get the next set of operation list results if there are any.
         :paramtype next_link: str
         :keyword value: List of Resource Provider operations supported by the Microsoft.StorageCache
          resource provider.
         :paramtype value: list[~azure.mgmt.storagecache.models.ApiOperation]
         """
@@ -174,16 +1051,16 @@
     }
 
     def __init__(
         self,
         *,
         metric_specifications: Optional[List["_models.MetricSpecification"]] = None,
         log_specifications: Optional[List["_models.LogSpecification"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword metric_specifications: Details about operations related to metrics.
         :paramtype metric_specifications: list[~azure.mgmt.storagecache.models.MetricSpecification]
         :keyword log_specifications: Details about operations related to logs.
         :paramtype log_specifications: list[~azure.mgmt.storagecache.models.LogSpecification]
         """
         super().__init__(**kwargs)
@@ -226,16 +1103,16 @@
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
         start_time: Optional[str] = None,
         end_time: Optional[str] = None,
         status: Optional[str] = None,
         error: Optional["_models.ErrorResponse"] = None,
         output: Optional[Dict[str, JSON]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword id: The operation Id.
         :paramtype id: str
         :keyword name: The operation name.
         :paramtype name: str
         :keyword start_time: The start time of the operation.
         :paramtype start_time: str
@@ -261,70 +1138,95 @@
 class BlobNfsTarget(_serialization.Model):
     """Properties pertaining to the BlobNfsTarget.
 
     :ivar target: Resource ID of the storage container.
     :vartype target: str
     :ivar usage_model: Identifies the StorageCache usage model to be used for this storage target.
     :vartype usage_model: str
+    :ivar verification_timer: Amount of time (in seconds) the cache waits before it checks the
+     back-end storage for file updates.
+    :vartype verification_timer: int
+    :ivar write_back_timer: Amount of time (in seconds) the cache waits after the last file change
+     before it copies the changed file to back-end storage.
+    :vartype write_back_timer: int
     """
 
     _attribute_map = {
         "target": {"key": "target", "type": "str"},
         "usage_model": {"key": "usageModel", "type": "str"},
+        "verification_timer": {"key": "verificationTimer", "type": "int"},
+        "write_back_timer": {"key": "writeBackTimer", "type": "int"},
     }
 
-    def __init__(self, *, target: Optional[str] = None, usage_model: Optional[str] = None, **kwargs):
+    def __init__(
+        self,
+        *,
+        target: Optional[str] = None,
+        usage_model: Optional[str] = None,
+        verification_timer: Optional[int] = None,
+        write_back_timer: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword target: Resource ID of the storage container.
         :paramtype target: str
         :keyword usage_model: Identifies the StorageCache usage model to be used for this storage
          target.
         :paramtype usage_model: str
+        :keyword verification_timer: Amount of time (in seconds) the cache waits before it checks the
+         back-end storage for file updates.
+        :paramtype verification_timer: int
+        :keyword write_back_timer: Amount of time (in seconds) the cache waits after the last file
+         change before it copies the changed file to back-end storage.
+        :paramtype write_back_timer: int
         """
         super().__init__(**kwargs)
         self.target = target
         self.usage_model = usage_model
+        self.verification_timer = verification_timer
+        self.write_back_timer = write_back_timer
 
 
 class Cache(_serialization.Model):  # pylint: disable=too-many-instance-attributes
-    """A Cache instance. Follows Azure Resource Manager standards: https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/resource-api-reference.md.
+    """A cache instance. Follows Azure Resource Manager standards:
+    https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/resource-api-reference.md.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
-    :ivar id: Resource ID of the Cache.
+    :ivar id: Resource ID of the cache.
     :vartype id: str
     :ivar location: Region name string.
     :vartype location: str
-    :ivar name: Name of Cache.
+    :ivar name: Name of cache.
     :vartype name: str
-    :ivar type: Type of the Cache; Microsoft.StorageCache/Cache.
+    :ivar type: Type of the cache; Microsoft.StorageCache/Cache.
     :vartype type: str
     :ivar identity: The identity of the cache, if configured.
     :vartype identity: ~azure.mgmt.storagecache.models.CacheIdentity
     :ivar system_data: The system meta data relating to this resource.
     :vartype system_data: ~azure.mgmt.storagecache.models.SystemData
-    :ivar sku: SKU for the Cache.
+    :ivar sku: SKU for the cache.
     :vartype sku: ~azure.mgmt.storagecache.models.CacheSku
     :ivar cache_size_gb: The size of this Cache, in GB.
     :vartype cache_size_gb: int
-    :ivar health: Health of the Cache.
+    :ivar health: Health of the cache.
     :vartype health: ~azure.mgmt.storagecache.models.CacheHealth
-    :ivar mount_addresses: Array of IP addresses that can be used by clients mounting this Cache.
+    :ivar mount_addresses: Array of IPv4 addresses that can be used by clients mounting this cache.
     :vartype mount_addresses: list[str]
     :ivar provisioning_state: ARM provisioning state, see
      https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/Addendum.md#provisioningstate-property.
-     Known values are: "Succeeded", "Failed", "Cancelled", "Creating", "Deleting", and "Updating".
+     Known values are: "Succeeded", "Failed", "Canceled", "Creating", "Deleting", and "Updating".
     :vartype provisioning_state: str or ~azure.mgmt.storagecache.models.ProvisioningStateType
-    :ivar subnet: Subnet used for the Cache.
+    :ivar subnet: Subnet used for the cache.
     :vartype subnet: str
-    :ivar upgrade_status: Upgrade status of the Cache.
+    :ivar upgrade_status: Upgrade status of the cache.
     :vartype upgrade_status: ~azure.mgmt.storagecache.models.CacheUpgradeStatus
-    :ivar upgrade_settings: Upgrade settings of the Cache.
+    :ivar upgrade_settings: Upgrade settings of the cache.
     :vartype upgrade_settings: ~azure.mgmt.storagecache.models.CacheUpgradeSettings
     :ivar network_settings: Specifies network settings of the cache.
     :vartype network_settings: ~azure.mgmt.storagecache.models.CacheNetworkSettings
     :ivar encryption_settings: Specifies encryption settings of the cache.
     :vartype encryption_settings: ~azure.mgmt.storagecache.models.CacheEncryptionSettings
     :ivar security_settings: Specifies security settings of the cache.
     :vartype security_settings: ~azure.mgmt.storagecache.models.CacheSecuritySettings
@@ -392,30 +1294,30 @@
         subnet: Optional[str] = None,
         upgrade_settings: Optional["_models.CacheUpgradeSettings"] = None,
         network_settings: Optional["_models.CacheNetworkSettings"] = None,
         encryption_settings: Optional["_models.CacheEncryptionSettings"] = None,
         security_settings: Optional["_models.CacheSecuritySettings"] = None,
         directory_services_settings: Optional["_models.CacheDirectorySettings"] = None,
         zones: Optional[List[str]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: Region name string.
         :paramtype location: str
         :keyword identity: The identity of the cache, if configured.
         :paramtype identity: ~azure.mgmt.storagecache.models.CacheIdentity
-        :keyword sku: SKU for the Cache.
+        :keyword sku: SKU for the cache.
         :paramtype sku: ~azure.mgmt.storagecache.models.CacheSku
         :keyword cache_size_gb: The size of this Cache, in GB.
         :paramtype cache_size_gb: int
-        :keyword subnet: Subnet used for the Cache.
+        :keyword subnet: Subnet used for the cache.
         :paramtype subnet: str
-        :keyword upgrade_settings: Upgrade settings of the Cache.
+        :keyword upgrade_settings: Upgrade settings of the cache.
         :paramtype upgrade_settings: ~azure.mgmt.storagecache.models.CacheUpgradeSettings
         :keyword network_settings: Specifies network settings of the cache.
         :paramtype network_settings: ~azure.mgmt.storagecache.models.CacheNetworkSettings
         :keyword encryption_settings: Specifies encryption settings of the cache.
         :paramtype encryption_settings: ~azure.mgmt.storagecache.models.CacheEncryptionSettings
         :keyword security_settings: Specifies security settings of the cache.
         :paramtype security_settings: ~azure.mgmt.storagecache.models.CacheSecuritySettings
@@ -502,16 +1404,16 @@
         *,
         primary_dns_ip_address: str,
         domain_name: str,
         domain_net_bios_name: str,
         cache_net_bios_name: str,
         secondary_dns_ip_address: Optional[str] = None,
         credentials: Optional["_models.CacheActiveDirectorySettingsCredentials"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword primary_dns_ip_address: Primary DNS IP address used to resolve the Active Directory
          domain controller's fully qualified domain name. Required.
         :paramtype primary_dns_ip_address: str
         :keyword secondary_dns_ip_address: Secondary DNS IP address used to resolve the Active
          Directory domain controller's fully qualified domain name.
         :paramtype secondary_dns_ip_address: str
@@ -543,35 +1445,34 @@
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar username: Username of the Active Directory domain administrator. This value is stored
      encrypted and not returned on response. Required.
     :vartype username: str
     :ivar password: Plain text password of the Active Directory domain administrator. This value is
-     stored encrypted and not returned on response. Required.
+     stored encrypted and not returned on response.
     :vartype password: str
     """
 
     _validation = {
         "username": {"required": True},
-        "password": {"required": True},
     }
 
     _attribute_map = {
         "username": {"key": "username", "type": "str"},
         "password": {"key": "password", "type": "str"},
     }
 
-    def __init__(self, *, username: str, password: str, **kwargs):
+    def __init__(self, *, username: str, password: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword username: Username of the Active Directory domain administrator. This value is stored
          encrypted and not returned on response. Required.
         :paramtype username: str
         :keyword password: Plain text password of the Active Directory domain administrator. This value
-         is stored encrypted and not returned on response. Required.
+         is stored encrypted and not returned on response.
         :paramtype password: str
         """
         super().__init__(**kwargs)
         self.username = username
         self.password = password
 
 
@@ -592,16 +1493,16 @@
     }
 
     def __init__(
         self,
         *,
         active_directory: Optional["_models.CacheActiveDirectorySettings"] = None,
         username_download: Optional["_models.CacheUsernameDownloadSettings"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword active_directory: Specifies settings for joining the HPC Cache to an Active Directory
          domain.
         :paramtype active_directory: ~azure.mgmt.storagecache.models.CacheActiveDirectorySettings
         :keyword username_download: Specifies settings for Extended Groups. Extended Groups allows
          users to be members of more than 16 groups.
         :paramtype username_download: ~azure.mgmt.storagecache.models.CacheUsernameDownloadSettings
@@ -610,53 +1511,58 @@
         self.active_directory = active_directory
         self.username_download = username_download
 
 
 class CacheEncryptionSettings(_serialization.Model):
     """Cache encryption settings.
 
-    :ivar key_encryption_key: Specifies the location of the key encryption key in Key Vault.
+    :ivar key_encryption_key: Specifies the location of the key encryption key in key vault.
     :vartype key_encryption_key: ~azure.mgmt.storagecache.models.KeyVaultKeyReference
     :ivar rotation_to_latest_key_version_enabled: Specifies whether the service will automatically
-     rotate to the newest version of the key in the Key Vault.
+     rotate to the newest version of the key in the key vault.
     :vartype rotation_to_latest_key_version_enabled: bool
     """
 
     _attribute_map = {
         "key_encryption_key": {"key": "keyEncryptionKey", "type": "KeyVaultKeyReference"},
         "rotation_to_latest_key_version_enabled": {"key": "rotationToLatestKeyVersionEnabled", "type": "bool"},
     }
 
     def __init__(
         self,
         *,
         key_encryption_key: Optional["_models.KeyVaultKeyReference"] = None,
         rotation_to_latest_key_version_enabled: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword key_encryption_key: Specifies the location of the key encryption key in Key Vault.
+        :keyword key_encryption_key: Specifies the location of the key encryption key in key vault.
         :paramtype key_encryption_key: ~azure.mgmt.storagecache.models.KeyVaultKeyReference
         :keyword rotation_to_latest_key_version_enabled: Specifies whether the service will
-         automatically rotate to the newest version of the key in the Key Vault.
+         automatically rotate to the newest version of the key in the key vault.
         :paramtype rotation_to_latest_key_version_enabled: bool
         """
         super().__init__(**kwargs)
         self.key_encryption_key = key_encryption_key
         self.rotation_to_latest_key_version_enabled = rotation_to_latest_key_version_enabled
 
 
 class CacheHealth(_serialization.Model):
-    """An indication of Cache health. Gives more information about health than just that related to provisioning.
+    """An indication of cache health. Gives more information about health than just that related to
+    provisioning.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar state: List of Cache health states. Known values are: "Unknown", "Healthy", "Degraded",
-     "Down", "Transitioning", "Stopping", "Stopped", "Upgrading", "Flushing", "WaitingForKey",
-     "StartFailed", and "UpgradeFailed".
+    :ivar state: List of cache health states. Down is when the cluster is not responding.  Degraded
+     is when its functioning but has some alerts. Transitioning when it is creating or deleting.
+     Unknown will be returned in old api versions when a new value is added in future versions.
+     WaitingForKey is when the create is waiting for the system assigned identity to be given access
+     to the encryption key in the encryption settings. Known values are: "Unknown", "Healthy",
+     "Degraded", "Down", "Transitioning", "Stopping", "Stopped", "Upgrading", "Flushing",
+     "WaitingForKey", "StartFailed", and "UpgradeFailed".
     :vartype state: str or ~azure.mgmt.storagecache.models.HealthStateType
     :ivar status_description: Describes explanation of state.
     :vartype status_description: str
     :ivar conditions: Outstanding conditions that need to be investigated and resolved.
     :vartype conditions: list[~azure.mgmt.storagecache.models.Condition]
     """
 
@@ -671,19 +1577,23 @@
     }
 
     def __init__(
         self,
         *,
         state: Optional[Union[str, "_models.HealthStateType"]] = None,
         status_description: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword state: List of Cache health states. Known values are: "Unknown", "Healthy",
-         "Degraded", "Down", "Transitioning", "Stopping", "Stopped", "Upgrading", "Flushing",
+        :keyword state: List of cache health states. Down is when the cluster is not responding.
+         Degraded is when its functioning but has some alerts. Transitioning when it is creating or
+         deleting. Unknown will be returned in old api versions when a new value is added in future
+         versions. WaitingForKey is when the create is waiting for the system assigned identity to be
+         given access to the encryption key in the encryption settings. Known values are: "Unknown",
+         "Healthy", "Degraded", "Down", "Transitioning", "Stopping", "Stopped", "Upgrading", "Flushing",
          "WaitingForKey", "StartFailed", and "UpgradeFailed".
         :paramtype state: str or ~azure.mgmt.storagecache.models.HealthStateType
         :keyword status_description: Describes explanation of state.
         :paramtype status_description: str
         """
         super().__init__(**kwargs)
         self.state = state
@@ -702,44 +1612,47 @@
     :vartype tenant_id: str
     :ivar type: The type of identity used for the cache. Known values are: "SystemAssigned",
      "UserAssigned", "SystemAssigned, UserAssigned", and "None".
     :vartype type: str or ~azure.mgmt.storagecache.models.CacheIdentityType
     :ivar user_assigned_identities: A dictionary where each key is a user assigned identity
      resource ID, and each key's value is an empty dictionary.
     :vartype user_assigned_identities: dict[str,
-     ~azure.mgmt.storagecache.models.UserAssignedIdentitiesValue]
+     ~azure.mgmt.storagecache.models.UserAssignedIdentitiesValueAutoGenerated]
     """
 
     _validation = {
         "principal_id": {"readonly": True},
         "tenant_id": {"readonly": True},
     }
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "tenant_id": {"key": "tenantId", "type": "str"},
         "type": {"key": "type", "type": "str"},
-        "user_assigned_identities": {"key": "userAssignedIdentities", "type": "{UserAssignedIdentitiesValue}"},
+        "user_assigned_identities": {
+            "key": "userAssignedIdentities",
+            "type": "{UserAssignedIdentitiesValueAutoGenerated}",
+        },
     }
 
     def __init__(
         self,
         *,
         type: Optional[Union[str, "_models.CacheIdentityType"]] = None,
-        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentitiesValue"]] = None,
-        **kwargs
-    ):
+        user_assigned_identities: Optional[Dict[str, "_models.UserAssignedIdentitiesValueAutoGenerated"]] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword type: The type of identity used for the cache. Known values are: "SystemAssigned",
          "UserAssigned", "SystemAssigned, UserAssigned", and "None".
         :paramtype type: str or ~azure.mgmt.storagecache.models.CacheIdentityType
         :keyword user_assigned_identities: A dictionary where each key is a user assigned identity
          resource ID, and each key's value is an empty dictionary.
         :paramtype user_assigned_identities: dict[str,
-         ~azure.mgmt.storagecache.models.UserAssignedIdentitiesValue]
+         ~azure.mgmt.storagecache.models.UserAssignedIdentitiesValueAutoGenerated]
         """
         super().__init__(**kwargs)
         self.principal_id = None
         self.tenant_id = None
         self.type = type
         self.user_assigned_identities = user_assigned_identities
 
@@ -747,15 +1660,15 @@
 class CacheNetworkSettings(_serialization.Model):
     """Cache network settings.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar mtu: The IPv4 maximum transmission unit configured for the subnet.
     :vartype mtu: int
-    :ivar utility_addresses: Array of additional IP addresses used by this Cache.
+    :ivar utility_addresses: Array of additional IP addresses used by this cache.
     :vartype utility_addresses: list[str]
     :ivar dns_servers: DNS servers for the cache to use.  It will be set from the network
      configuration if no value is provided.
     :vartype dns_servers: list[str]
     :ivar dns_search_domain: DNS search domain.
     :vartype dns_search_domain: str
     :ivar ntp_server: NTP server IP Address or FQDN for the cache to use. The default is
@@ -779,16 +1692,16 @@
     def __init__(
         self,
         *,
         mtu: int = 1500,
         dns_servers: Optional[List[str]] = None,
         dns_search_domain: Optional[str] = None,
         ntp_server: str = "time.windows.com",
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword mtu: The IPv4 maximum transmission unit configured for the subnet.
         :paramtype mtu: int
         :keyword dns_servers: DNS servers for the cache to use.  It will be set from the network
          configuration if no value is provided.
         :paramtype dns_servers: list[str]
         :keyword dns_search_domain: DNS search domain.
@@ -812,60 +1725,63 @@
     :vartype access_policies: list[~azure.mgmt.storagecache.models.NfsAccessPolicy]
     """
 
     _attribute_map = {
         "access_policies": {"key": "accessPolicies", "type": "[NfsAccessPolicy]"},
     }
 
-    def __init__(self, *, access_policies: Optional[List["_models.NfsAccessPolicy"]] = None, **kwargs):
+    def __init__(self, *, access_policies: Optional[List["_models.NfsAccessPolicy"]] = None, **kwargs: Any) -> None:
         """
         :keyword access_policies: NFS access policies defined for this cache.
         :paramtype access_policies: list[~azure.mgmt.storagecache.models.NfsAccessPolicy]
         """
         super().__init__(**kwargs)
         self.access_policies = access_policies
 
 
 class CacheSku(_serialization.Model):
-    """SKU for the Cache.
+    """SKU for the cache.
 
-    :ivar name: SKU name for this Cache.
+    :ivar name: SKU name for this cache.
     :vartype name: str
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, **kwargs: Any) -> None:
         """
-        :keyword name: SKU name for this Cache.
+        :keyword name: SKU name for this cache.
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.name = name
 
 
 class CachesListResult(_serialization.Model):
-    """Result of the request to list Caches. It contains a list of Caches and a URL link to get the next set of results.
+    """Result of the request to list caches. It contains a list of caches and a URL link to get the
+    next set of results.
 
-    :ivar next_link: URL to get the next set of Cache list results, if there are any.
+    :ivar next_link: URL to get the next set of cache list results, if there are any.
     :vartype next_link: str
     :ivar value: List of Caches.
     :vartype value: list[~azure.mgmt.storagecache.models.Cache]
     """
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
         "value": {"key": "value", "type": "[Cache]"},
     }
 
-    def __init__(self, *, next_link: Optional[str] = None, value: Optional[List["_models.Cache"]] = None, **kwargs):
+    def __init__(
+        self, *, next_link: Optional[str] = None, value: Optional[List["_models.Cache"]] = None, **kwargs: Any
+    ) -> None:
         """
-        :keyword next_link: URL to get the next set of Cache list results, if there are any.
+        :keyword next_link: URL to get the next set of cache list results, if there are any.
         :paramtype next_link: str
         :keyword value: List of Caches.
         :paramtype value: list[~azure.mgmt.storagecache.models.Cache]
         """
         super().__init__(**kwargs)
         self.next_link = next_link
         self.value = value
@@ -890,16 +1806,16 @@
     }
 
     def __init__(
         self,
         *,
         upgrade_schedule_enabled: Optional[bool] = None,
         scheduled_time: Optional[datetime.datetime] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword upgrade_schedule_enabled: True if the user chooses to select an installation time
          between now and firmwareUpdateDeadline. Else the firmware will automatically be installed after
          firmwareUpdateDeadline if not triggered earlier via the upgrade operation.
         :paramtype upgrade_schedule_enabled: bool
         :keyword scheduled_time: When upgradeScheduleEnabled is true, this field holds the user-chosen
          upgrade time. At the user-chosen time, the firmware update will automatically be installed on
@@ -908,27 +1824,27 @@
         """
         super().__init__(**kwargs)
         self.upgrade_schedule_enabled = upgrade_schedule_enabled
         self.scheduled_time = scheduled_time
 
 
 class CacheUpgradeStatus(_serialization.Model):
-    """Properties describing the software upgrade state of the Cache.
+    """Properties describing the software upgrade state of the cache.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar current_firmware_version: Version string of the firmware currently installed on this
-     Cache.
+     cache.
     :vartype current_firmware_version: str
     :ivar firmware_update_status: True if there is a firmware update ready to install on this
-     Cache. The firmware will automatically be installed after firmwareUpdateDeadline if not
+     cache. The firmware will automatically be installed after firmwareUpdateDeadline if not
      triggered earlier via the upgrade operation. Known values are: "available" and "unavailable".
     :vartype firmware_update_status: str or ~azure.mgmt.storagecache.models.FirmwareStatusType
     :ivar firmware_update_deadline: Time at which the pending firmware update will automatically be
-     installed on the Cache.
+     installed on the cache.
     :vartype firmware_update_deadline: ~datetime.datetime
     :ivar last_firmware_update: Time of the last successful firmware update.
     :vartype last_firmware_update: ~datetime.datetime
     :ivar pending_firmware_version: When firmwareUpdateAvailable is true, this field holds the
      version string for the update.
     :vartype pending_firmware_version: str
     """
@@ -945,15 +1861,15 @@
         "current_firmware_version": {"key": "currentFirmwareVersion", "type": "str"},
         "firmware_update_status": {"key": "firmwareUpdateStatus", "type": "str"},
         "firmware_update_deadline": {"key": "firmwareUpdateDeadline", "type": "iso-8601"},
         "last_firmware_update": {"key": "lastFirmwareUpdate", "type": "iso-8601"},
         "pending_firmware_version": {"key": "pendingFirmwareVersion", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.current_firmware_version = None
         self.firmware_update_status = None
         self.firmware_update_deadline = None
         self.last_firmware_update = None
         self.pending_firmware_version = None
@@ -1021,21 +1937,21 @@
         *,
         extended_groups: Optional[bool] = None,
         username_source: Union[str, "_models.UsernameSource"] = "None",
         group_file_uri: Optional[str] = None,
         user_file_uri: Optional[str] = None,
         ldap_server: Optional[str] = None,
         ldap_base_dn: Optional[str] = None,
-        encrypt_ldap_connection: Optional[bool] = None,
-        require_valid_certificate: Optional[bool] = None,
-        auto_download_certificate: Optional[bool] = None,
+        encrypt_ldap_connection: bool = False,
+        require_valid_certificate: bool = False,
+        auto_download_certificate: bool = False,
         ca_certificate_uri: Optional[str] = None,
         credentials: Optional["_models.CacheUsernameDownloadSettingsCredentials"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword extended_groups: Whether or not Extended Groups is enabled.
         :paramtype extended_groups: bool
         :keyword username_source: This setting determines how the cache gets username and group names
          for clients. Known values are: "AD", "LDAP", "File", and "None".
         :paramtype username_source: str or ~azure.mgmt.storagecache.models.UsernameSource
         :keyword group_file_uri: The URI of the file containing group information (in /etc/group file
@@ -1090,15 +2006,15 @@
     """
 
     _attribute_map = {
         "bind_dn": {"key": "bindDn", "type": "str"},
         "bind_password": {"key": "bindPassword", "type": "str"},
     }
 
-    def __init__(self, *, bind_dn: Optional[str] = None, bind_password: Optional[str] = None, **kwargs):
+    def __init__(self, *, bind_dn: Optional[str] = None, bind_password: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword bind_dn: The Bind Distinguished Name identity to be used in the secure LDAP
          connection. This value is stored encrypted and not returned on response.
         :paramtype bind_dn: str
         :keyword bind_password: The Bind password to be used in the secure LDAP connection. This value
          is stored encrypted and not returned on response.
         :paramtype bind_password: str
@@ -1115,15 +2031,15 @@
     :vartype target: str
     """
 
     _attribute_map = {
         "target": {"key": "target", "type": "str"},
     }
 
-    def __init__(self, *, target: Optional[str] = None, **kwargs):
+    def __init__(self, *, target: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword target: Resource ID of storage container.
         :paramtype target: str
         """
         super().__init__(**kwargs)
         self.target = target
 
@@ -1154,16 +2070,16 @@
     def __init__(
         self,
         *,
         code: Optional[str] = None,
         details: Optional[List["_models.CloudErrorBody"]] = None,
         message: Optional[str] = None,
         target: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword code: An identifier for the error. Codes are invariant and are intended to be consumed
          programmatically.
         :paramtype code: str
         :keyword details: A list of additional details about the error.
         :paramtype details: list[~azure.mgmt.storagecache.models.CloudErrorBody]
         :keyword message: A message describing the error, intended to be suitable for display in a user
@@ -1197,15 +2113,15 @@
     }
 
     _attribute_map = {
         "timestamp": {"key": "timestamp", "type": "iso-8601"},
         "message": {"key": "message", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.timestamp = None
         self.message = None
 
 
 class ErrorResponse(_serialization.Model):
@@ -1218,71 +2134,71 @@
     """
 
     _attribute_map = {
         "code": {"key": "code", "type": "str"},
         "message": {"key": "message", "type": "str"},
     }
 
-    def __init__(self, *, code: Optional[str] = None, message: Optional[str] = None, **kwargs):
+    def __init__(self, *, code: Optional[str] = None, message: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword code: Error code.
         :paramtype code: str
         :keyword message: Error message indicating why the operation failed.
         :paramtype message: str
         """
         super().__init__(**kwargs)
         self.code = code
         self.message = message
 
 
 class KeyVaultKeyReference(_serialization.Model):
-    """Describes a reference to Key Vault Key.
+    """Describes a reference to key vault key.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar key_url: The URL referencing a key encryption key in Key Vault. Required.
+    :ivar key_url: The URL referencing a key encryption key in key vault. Required.
     :vartype key_url: str
-    :ivar source_vault: Describes a resource Id to source Key Vault. Required.
+    :ivar source_vault: Describes a resource Id to source key vault. Required.
     :vartype source_vault: ~azure.mgmt.storagecache.models.KeyVaultKeyReferenceSourceVault
     """
 
     _validation = {
         "key_url": {"required": True},
         "source_vault": {"required": True},
     }
 
     _attribute_map = {
         "key_url": {"key": "keyUrl", "type": "str"},
         "source_vault": {"key": "sourceVault", "type": "KeyVaultKeyReferenceSourceVault"},
     }
 
-    def __init__(self, *, key_url: str, source_vault: "_models.KeyVaultKeyReferenceSourceVault", **kwargs):
+    def __init__(self, *, key_url: str, source_vault: "_models.KeyVaultKeyReferenceSourceVault", **kwargs: Any) -> None:
         """
-        :keyword key_url: The URL referencing a key encryption key in Key Vault. Required.
+        :keyword key_url: The URL referencing a key encryption key in key vault. Required.
         :paramtype key_url: str
-        :keyword source_vault: Describes a resource Id to source Key Vault. Required.
+        :keyword source_vault: Describes a resource Id to source key vault. Required.
         :paramtype source_vault: ~azure.mgmt.storagecache.models.KeyVaultKeyReferenceSourceVault
         """
         super().__init__(**kwargs)
         self.key_url = key_url
         self.source_vault = source_vault
 
 
 class KeyVaultKeyReferenceSourceVault(_serialization.Model):
-    """Describes a resource Id to source Key Vault.
+    """Describes a resource Id to source key vault.
 
     :ivar id: Resource Id.
     :vartype id: str
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(self, *, id: Optional[str] = None, **kwargs):  # pylint: disable=redefined-builtin
+    def __init__(self, *, id: Optional[str] = None, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
         """
         :keyword id: Resource Id.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
@@ -1297,15 +2213,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "display_name": {"key": "displayName", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, display_name: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, display_name: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: The name of the log.
         :paramtype name: str
         :keyword display_name: Localized display name of the log.
         :paramtype display_name: str
         """
         super().__init__(**kwargs)
@@ -1336,16 +2252,16 @@
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         display_name: Optional[str] = None,
         internal_name: Optional[str] = None,
         to_be_exported_for_shoebox: Optional[bool] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: Name of the dimension.
         :paramtype name: str
         :keyword display_name: Localized friendly display name of the dimension.
         :paramtype display_name: str
         :keyword internal_name: Internal name of the dimension.
         :paramtype internal_name: str
@@ -1399,16 +2315,16 @@
         display_name: Optional[str] = None,
         display_description: Optional[str] = None,
         unit: Optional[str] = None,
         aggregation_type: Optional[str] = None,
         supported_aggregation_types: Optional[List[Union[str, "_models.MetricAggregationType"]]] = None,
         metric_class: Optional[str] = None,
         dimensions: Optional[List["_models.MetricDimension"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword name: The name of the metric.
         :paramtype name: str
         :keyword display_name: Localized display name of the metric.
         :paramtype display_name: str
         :keyword display_description: The description of the metric.
         :paramtype display_description: str
@@ -1434,15 +2350,15 @@
         self.metric_class = metric_class
         self.dimensions = dimensions
 
 
 class NamespaceJunction(_serialization.Model):
     """A namespace junction.
 
-    :ivar namespace_path: Namespace path on a Cache for a Storage Target.
+    :ivar namespace_path: Namespace path on a cache for a Storage Target.
     :vartype namespace_path: str
     :ivar target_path: Path in Storage Target to which namespacePath points.
     :vartype target_path: str
     :ivar nfs_export: NFS export where targetPath exists.
     :vartype nfs_export: str
     :ivar nfs_access_policy: Name of the access policy applied to this junction.
     :vartype nfs_access_policy: str
@@ -1458,18 +2374,18 @@
     def __init__(
         self,
         *,
         namespace_path: Optional[str] = None,
         target_path: Optional[str] = None,
         nfs_export: Optional[str] = None,
         nfs_access_policy: str = "default",
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword namespace_path: Namespace path on a Cache for a Storage Target.
+        :keyword namespace_path: Namespace path on a cache for a Storage Target.
         :paramtype namespace_path: str
         :keyword target_path: Path in Storage Target to which namespacePath points.
         :paramtype target_path: str
         :keyword nfs_export: NFS export where targetPath exists.
         :paramtype nfs_export: str
         :keyword nfs_access_policy: Name of the access policy applied to this junction.
         :paramtype nfs_access_policy: str
@@ -1484,36 +2400,60 @@
 class Nfs3Target(_serialization.Model):
     """Properties pertaining to the Nfs3Target.
 
     :ivar target: IP address or host name of an NFSv3 host (e.g., 10.0.44.44).
     :vartype target: str
     :ivar usage_model: Identifies the StorageCache usage model to be used for this storage target.
     :vartype usage_model: str
+    :ivar verification_timer: Amount of time (in seconds) the cache waits before it checks the
+     back-end storage for file updates.
+    :vartype verification_timer: int
+    :ivar write_back_timer: Amount of time (in seconds) the cache waits after the last file change
+     before it copies the changed file to back-end storage.
+    :vartype write_back_timer: int
     """
 
     _validation = {
         "target": {"pattern": r"^[-.,0-9a-zA-Z]+$"},
     }
 
     _attribute_map = {
         "target": {"key": "target", "type": "str"},
         "usage_model": {"key": "usageModel", "type": "str"},
+        "verification_timer": {"key": "verificationTimer", "type": "int"},
+        "write_back_timer": {"key": "writeBackTimer", "type": "int"},
     }
 
-    def __init__(self, *, target: Optional[str] = None, usage_model: Optional[str] = None, **kwargs):
+    def __init__(
+        self,
+        *,
+        target: Optional[str] = None,
+        usage_model: Optional[str] = None,
+        verification_timer: Optional[int] = None,
+        write_back_timer: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword target: IP address or host name of an NFSv3 host (e.g., 10.0.44.44).
         :paramtype target: str
         :keyword usage_model: Identifies the StorageCache usage model to be used for this storage
          target.
         :paramtype usage_model: str
+        :keyword verification_timer: Amount of time (in seconds) the cache waits before it checks the
+         back-end storage for file updates.
+        :paramtype verification_timer: int
+        :keyword write_back_timer: Amount of time (in seconds) the cache waits after the last file
+         change before it copies the changed file to back-end storage.
+        :paramtype write_back_timer: int
         """
         super().__init__(**kwargs)
         self.target = target
         self.usage_model = usage_model
+        self.verification_timer = verification_timer
+        self.write_back_timer = write_back_timer
 
 
 class NfsAccessPolicy(_serialization.Model):
     """A set of rules describing access policies applied to NFSv3 clients of the cache.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -1530,15 +2470,15 @@
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "access_rules": {"key": "accessRules", "type": "[NfsAccessRule]"},
     }
 
-    def __init__(self, *, name: str, access_rules: List["_models.NfsAccessRule"], **kwargs):
+    def __init__(self, *, name: str, access_rules: List["_models.NfsAccessRule"], **kwargs: Any) -> None:
         """
         :keyword name: Name identifying this policy. Access Policy names are not case sensitive.
          Required.
         :paramtype name: str
         :keyword access_rules: The set of rules describing client accesses allowed under this policy.
          Required.
         :paramtype access_rules: list[~azure.mgmt.storagecache.models.NfsAccessRule]
@@ -1603,16 +2543,16 @@
         access: Union[str, "_models.NfsAccessRuleAccess"],
         filter: Optional[str] = None,  # pylint: disable=redefined-builtin
         suid: Optional[bool] = None,
         submount_access: Optional[bool] = None,
         root_squash: Optional[bool] = None,
         anonymous_uid: Optional[str] = None,
         anonymous_gid: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword scope: Scope for this rule. The scope and filter determine which clients match the
          rule. Required. Known values are: "default", "network", and "host".
         :paramtype scope: str or ~azure.mgmt.storagecache.models.NfsAccessRuleScope
         :keyword filter: Filter applied to the scope for this rule. The filter's format depends on its
          scope. 'default' scope matches all clients and has no filter value. 'network' scope takes a
          filter in CIDR format (for example, 10.99.1.0/24). 'host' takes an IP address or fully
@@ -1689,15 +2629,15 @@
         "priming_job_id": {"key": "primingJobId", "type": "str"},
         "priming_job_state": {"key": "primingJobState", "type": "str"},
         "priming_job_status": {"key": "primingJobStatus", "type": "str"},
         "priming_job_details": {"key": "primingJobDetails", "type": "str"},
         "priming_job_percent_complete": {"key": "primingJobPercentComplete", "type": "float"},
     }
 
-    def __init__(self, *, priming_job_name: str, priming_manifest_url: str, **kwargs):
+    def __init__(self, *, priming_job_name: str, priming_manifest_url: str, **kwargs: Any) -> None:
         """
         :keyword priming_job_name: The priming job name. Required.
         :paramtype priming_job_name: str
         :keyword priming_manifest_url: The URL for the priming manifest file to download. This file
          must be readable from the HPC Cache. When the file is in Azure blob storage the URL should
          include a Shared Access Signature (SAS) granting read permissions on the blob. Required.
         :paramtype priming_manifest_url: str
@@ -1725,23 +2665,75 @@
         "priming_job_id": {"required": True, "pattern": r"^[-0-9a-zA-Z_]{1,80}$"},
     }
 
     _attribute_map = {
         "priming_job_id": {"key": "primingJobId", "type": "str"},
     }
 
-    def __init__(self, *, priming_job_id: str, **kwargs):
+    def __init__(self, *, priming_job_id: str, **kwargs: Any) -> None:
         """
         :keyword priming_job_id: The unique identifier of the priming job. Required.
         :paramtype priming_job_id: str
         """
         super().__init__(**kwargs)
         self.priming_job_id = priming_job_id
 
 
+class RequiredAmlFilesystemSubnetsSize(_serialization.Model):
+    """Information about the number of available IP addresses that are required for the AML file
+    system.
+
+    :ivar filesystem_subnet_size: The number of available IP addresses that are required for the
+     AML file system.
+    :vartype filesystem_subnet_size: int
+    """
+
+    _attribute_map = {
+        "filesystem_subnet_size": {"key": "filesystemSubnetSize", "type": "int"},
+    }
+
+    def __init__(self, *, filesystem_subnet_size: Optional[int] = None, **kwargs: Any) -> None:
+        """
+        :keyword filesystem_subnet_size: The number of available IP addresses that are required for the
+         AML file system.
+        :paramtype filesystem_subnet_size: int
+        """
+        super().__init__(**kwargs)
+        self.filesystem_subnet_size = filesystem_subnet_size
+
+
+class RequiredAmlFilesystemSubnetsSizeInfo(_serialization.Model):
+    """Information required to get the number of available IP addresses a subnet should have that will
+    be used in AML file system create.
+
+    :ivar storage_capacity_ti_b: The size of the AML file system, in TiB.
+    :vartype storage_capacity_ti_b: float
+    :ivar sku: SKU for the resource.
+    :vartype sku: ~azure.mgmt.storagecache.models.SkuName
+    """
+
+    _attribute_map = {
+        "storage_capacity_ti_b": {"key": "storageCapacityTiB", "type": "float"},
+        "sku": {"key": "sku", "type": "SkuName"},
+    }
+
+    def __init__(
+        self, *, storage_capacity_ti_b: Optional[float] = None, sku: Optional["_models.SkuName"] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword storage_capacity_ti_b: The size of the AML file system, in TiB.
+        :paramtype storage_capacity_ti_b: float
+        :keyword sku: SKU for the resource.
+        :paramtype sku: ~azure.mgmt.storagecache.models.SkuName
+        """
+        super().__init__(**kwargs)
+        self.storage_capacity_ti_b = storage_capacity_ti_b
+        self.sku = sku
+
+
 class ResourceSku(_serialization.Model):
     """A resource SKU.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar resource_type: The type of resource the SKU applies to.
     :vartype resource_type: str
@@ -1776,16 +2768,16 @@
     def __init__(
         self,
         *,
         capabilities: Optional[List["_models.ResourceSkuCapabilities"]] = None,
         location_info: Optional[List["_models.ResourceSkuLocationInfo"]] = None,
         name: Optional[str] = None,
         restrictions: Optional[List["_models.Restriction"]] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword capabilities: A list of capabilities of this SKU, such as throughput or ops/sec.
         :paramtype capabilities: list[~azure.mgmt.storagecache.models.ResourceSkuCapabilities]
         :keyword location_info: The set of locations where the SKU is available.
         :paramtype location_info: list[~azure.mgmt.storagecache.models.ResourceSkuLocationInfo]
         :keyword name: The name of this SKU.
         :paramtype name: str
@@ -1812,15 +2804,15 @@
     """
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "value": {"key": "value", "type": "str"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, value: Optional[str] = None, **kwargs):
+    def __init__(self, *, name: Optional[str] = None, value: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword name: Name of a capability, such as ops/sec.
         :paramtype name: str
         :keyword value: Quantity, if the capability is measured by quantity.
         :paramtype value: str
         """
         super().__init__(**kwargs)
@@ -1838,15 +2830,15 @@
     """
 
     _attribute_map = {
         "location": {"key": "location", "type": "str"},
         "zones": {"key": "zones", "type": "[str]"},
     }
 
-    def __init__(self, *, location: Optional[str] = None, zones: Optional[List[str]] = None, **kwargs):
+    def __init__(self, *, location: Optional[str] = None, zones: Optional[List[str]] = None, **kwargs: Any) -> None:
         """
         :keyword location: Location where this SKU is available.
         :paramtype location: str
         :keyword zones: Zones if any.
         :paramtype zones: list[str]
         """
         super().__init__(**kwargs)
@@ -1855,32 +2847,32 @@
 
 
 class ResourceSkusResult(_serialization.Model):
     """The response from the List Cache SKUs operation.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar next_link: The URI to fetch the next page of Cache SKUs.
+    :ivar next_link: The URI to fetch the next page of cache SKUs.
     :vartype next_link: str
     :ivar value: The list of SKUs available for the subscription.
     :vartype value: list[~azure.mgmt.storagecache.models.ResourceSku]
     """
 
     _validation = {
         "value": {"readonly": True},
     }
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
         "value": {"key": "value", "type": "[ResourceSku]"},
     }
 
-    def __init__(self, *, next_link: Optional[str] = None, **kwargs):
+    def __init__(self, *, next_link: Optional[str] = None, **kwargs: Any) -> None:
         """
-        :keyword next_link: The URI to fetch the next page of Cache SKUs.
+        :keyword next_link: The URI to fetch the next page of cache SKUs.
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.next_link = next_link
         self.value = None
 
 
@@ -1909,15 +2901,15 @@
     _attribute_map = {
         "limit": {"key": "limit", "type": "int"},
         "unit": {"key": "unit", "type": "str"},
         "current_value": {"key": "currentValue", "type": "int"},
         "name": {"key": "name", "type": "ResourceUsageName"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.limit = None
         self.unit = None
         self.current_value = None
         self.name = None
 
@@ -1932,28 +2924,29 @@
     """
 
     _attribute_map = {
         "value": {"key": "value", "type": "str"},
         "localized_value": {"key": "localizedValue", "type": "str"},
     }
 
-    def __init__(self, *, value: Optional[str] = None, localized_value: Optional[str] = None, **kwargs):
+    def __init__(self, *, value: Optional[str] = None, localized_value: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword value: Canonical name for this resource type.
         :paramtype value: str
         :keyword localized_value: Localized name for this resource type.
         :paramtype localized_value: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.localized_value = localized_value
 
 
 class ResourceUsagesListResult(_serialization.Model):
-    """Result of the request to list resource usages. It contains a list of resource usages & limits and a URL link to get the next set of results.
+    """Result of the request to list resource usages. It contains a list of resource usages & limits
+    and a URL link to get the next set of results.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar next_link: URL to get the next set of resource usage list results if there are any.
     :vartype next_link: str
     :ivar value: List of usages and limits for resources controlled by the Microsoft.StorageCache
      resource provider.
@@ -1966,15 +2959,15 @@
     }
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
         "value": {"key": "value", "type": "[ResourceUsage]"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.next_link = None
         self.value = None
 
 
 class Restriction(_serialization.Model):
@@ -2002,30 +2995,50 @@
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "values": {"key": "values", "type": "[str]"},
         "reason_code": {"key": "reasonCode", "type": "str"},
     }
 
-    def __init__(self, *, reason_code: Optional[Union[str, "_models.ReasonCode"]] = None, **kwargs):
+    def __init__(self, *, reason_code: Optional[Union[str, "_models.ReasonCode"]] = None, **kwargs: Any) -> None:
         """
         :keyword reason_code: The reason for the restriction. As of now this can be "QuotaId" or
          "NotAvailableForSubscription". "QuotaId" is set when the SKU has requiredQuotas parameter as
          the subscription does not belong to that quota. "NotAvailableForSubscription" is related to
          capacity at the datacenter. Known values are: "QuotaId" and "NotAvailableForSubscription".
         :paramtype reason_code: str or ~azure.mgmt.storagecache.models.ReasonCode
         """
         super().__init__(**kwargs)
         self.type = None
         self.values = None
         self.reason_code = reason_code
 
 
+class SkuName(_serialization.Model):
+    """SKU for the resource.
+
+    :ivar name: SKU name for this resource.
+    :vartype name: str
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+    }
+
+    def __init__(self, *, name: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword name: SKU name for this resource.
+        :paramtype name: str
+        """
+        super().__init__(**kwargs)
+        self.name = name
+
+
 class StorageTargetResource(_serialization.Model):
-    """Resource used by a Cache.
+    """Resource used by a cache.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar name: Name of the Storage Target.
     :vartype name: str
     :ivar id: Resource ID of the Storage Target.
     :vartype id: str
@@ -2049,15 +3062,15 @@
         "name": {"key": "name", "type": "str"},
         "id": {"key": "id", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "location": {"key": "location", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.name = None
         self.id = None
         self.type = None
         self.location = None
         self.system_data = None
@@ -2074,22 +3087,22 @@
     :vartype id: str
     :ivar type: Type of the Storage Target; Microsoft.StorageCache/Cache/StorageTarget.
     :vartype type: str
     :ivar location: Region name string.
     :vartype location: str
     :ivar system_data: The system meta data relating to this resource.
     :vartype system_data: ~azure.mgmt.storagecache.models.SystemData
-    :ivar junctions: List of Cache namespace junctions to target for namespace associations.
+    :ivar junctions: List of cache namespace junctions to target for namespace associations.
     :vartype junctions: list[~azure.mgmt.storagecache.models.NamespaceJunction]
     :ivar target_type: Type of the Storage Target. Known values are: "nfs3", "clfs", "unknown", and
      "blobNfs".
     :vartype target_type: str or ~azure.mgmt.storagecache.models.StorageTargetType
     :ivar provisioning_state: ARM provisioning state, see
      https://github.com/Azure/azure-resource-manager-rpc/blob/master/v1.0/Addendum.md#provisioningstate-property.
-     Known values are: "Succeeded", "Failed", "Cancelled", "Creating", "Deleting", and "Updating".
+     Known values are: "Succeeded", "Failed", "Canceled", "Creating", "Deleting", and "Updating".
     :vartype provisioning_state: str or ~azure.mgmt.storagecache.models.ProvisioningStateType
     :ivar state: Storage target operational state. Known values are: "Ready", "Busy", "Suspended",
      and "Flushing".
     :vartype state: str or ~azure.mgmt.storagecache.models.OperationalStateType
     :ivar nfs3: Properties when targetType is nfs3.
     :vartype nfs3: ~azure.mgmt.storagecache.models.Nfs3Target
     :ivar clfs: Properties when targetType is clfs.
@@ -2135,18 +3148,18 @@
         junctions: Optional[List["_models.NamespaceJunction"]] = None,
         target_type: Optional[Union[str, "_models.StorageTargetType"]] = None,
         state: Optional[Union[str, "_models.OperationalStateType"]] = None,
         nfs3: Optional["_models.Nfs3Target"] = None,
         clfs: Optional["_models.ClfsTarget"] = None,
         unknown: Optional["_models.UnknownTarget"] = None,
         blob_nfs: Optional["_models.BlobNfsTarget"] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
-        :keyword junctions: List of Cache namespace junctions to target for namespace associations.
+        :keyword junctions: List of cache namespace junctions to target for namespace associations.
         :paramtype junctions: list[~azure.mgmt.storagecache.models.NamespaceJunction]
         :keyword target_type: Type of the Storage Target. Known values are: "nfs3", "clfs", "unknown",
          and "blobNfs".
         :paramtype target_type: str or ~azure.mgmt.storagecache.models.StorageTargetType
         :keyword state: Storage target operational state. Known values are: "Ready", "Busy",
          "Suspended", and "Flushing".
         :paramtype state: str or ~azure.mgmt.storagecache.models.OperationalStateType
@@ -2186,15 +3199,17 @@
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "allocation_percentage": {"key": "allocationPercentage", "type": "int"},
     }
 
-    def __init__(self, *, name: Optional[str] = None, allocation_percentage: Optional[int] = None, **kwargs):
+    def __init__(
+        self, *, name: Optional[str] = None, allocation_percentage: Optional[int] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword name: Name of the storage target.
         :paramtype name: str
         :keyword allocation_percentage: The percentage of cache space allocated for this storage
          target.
         :paramtype allocation_percentage: int
         """
@@ -2204,30 +3219,30 @@
 
 
 class StorageTargetsResult(_serialization.Model):
     """A list of Storage Targets.
 
     :ivar next_link: The URI to fetch the next page of Storage Targets.
     :vartype next_link: str
-    :ivar value: The list of Storage Targets defined for the Cache.
+    :ivar value: The list of Storage Targets defined for the cache.
     :vartype value: list[~azure.mgmt.storagecache.models.StorageTarget]
     """
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
         "value": {"key": "value", "type": "[StorageTarget]"},
     }
 
     def __init__(
-        self, *, next_link: Optional[str] = None, value: Optional[List["_models.StorageTarget"]] = None, **kwargs
-    ):
+        self, *, next_link: Optional[str] = None, value: Optional[List["_models.StorageTarget"]] = None, **kwargs: Any
+    ) -> None:
         """
         :keyword next_link: The URI to fetch the next page of Storage Targets.
         :paramtype next_link: str
-        :keyword value: The list of Storage Targets defined for the Cache.
+        :keyword value: The list of Storage Targets defined for the cache.
         :paramtype value: list[~azure.mgmt.storagecache.models.StorageTarget]
         """
         super().__init__(**kwargs)
         self.next_link = next_link
         self.value = value
 
 
@@ -2264,16 +3279,16 @@
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
         :paramtype created_by_type: str or ~azure.mgmt.storagecache.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
@@ -2303,15 +3318,15 @@
     :vartype attributes: dict[str, str]
     """
 
     _attribute_map = {
         "attributes": {"key": "attributes", "type": "{str}"},
     }
 
-    def __init__(self, *, attributes: Optional[Dict[str, str]] = None, **kwargs):
+    def __init__(self, *, attributes: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
         """
         :keyword attributes: Dictionary of string->string pairs containing information about the
          Storage Target.
         :paramtype attributes: dict[str, str]
         """
         super().__init__(**kwargs)
         self.attributes = attributes
@@ -2337,16 +3352,16 @@
 
     def __init__(
         self,
         *,
         display: Optional["_models.UsageModelDisplay"] = None,
         model_name: Optional[str] = None,
         target_type: Optional[str] = None,
-        **kwargs
-    ):
+        **kwargs: Any
+    ) -> None:
         """
         :keyword display: Localized information describing this usage model.
         :paramtype display: ~azure.mgmt.storagecache.models.UsageModelDisplay
         :keyword model_name: Non-localized keyword name for this usage model.
         :paramtype model_name: str
         :keyword target_type: The type of Storage Target to which this model is applicable (only nfs3
          as of this version).
@@ -2365,42 +3380,42 @@
     :vartype description: str
     """
 
     _attribute_map = {
         "description": {"key": "description", "type": "str"},
     }
 
-    def __init__(self, *, description: Optional[str] = None, **kwargs):
+    def __init__(self, *, description: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword description: String to display for this usage model.
         :paramtype description: str
         """
         super().__init__(**kwargs)
         self.description = description
 
 
 class UsageModelsResult(_serialization.Model):
-    """A list of Cache usage models.
+    """A list of cache usage models.
 
-    :ivar next_link: The URI to fetch the next page of Cache usage models.
+    :ivar next_link: The URI to fetch the next page of cache usage models.
     :vartype next_link: str
     :ivar value: The list of usage models available for the subscription.
     :vartype value: list[~azure.mgmt.storagecache.models.UsageModel]
     """
 
     _attribute_map = {
         "next_link": {"key": "nextLink", "type": "str"},
         "value": {"key": "value", "type": "[UsageModel]"},
     }
 
     def __init__(
-        self, *, next_link: Optional[str] = None, value: Optional[List["_models.UsageModel"]] = None, **kwargs
-    ):
+        self, *, next_link: Optional[str] = None, value: Optional[List["_models.UsageModel"]] = None, **kwargs: Any
+    ) -> None:
         """
-        :keyword next_link: The URI to fetch the next page of Cache usage models.
+        :keyword next_link: The URI to fetch the next page of cache usage models.
         :paramtype next_link: str
         :keyword value: The list of usage models available for the subscription.
         :paramtype value: list[~azure.mgmt.storagecache.models.UsageModel]
         """
         super().__init__(**kwargs)
         self.next_link = next_link
         self.value = value
@@ -2423,12 +3438,40 @@
     }
 
     _attribute_map = {
         "principal_id": {"key": "principalId", "type": "str"},
         "client_id": {"key": "clientId", "type": "str"},
     }
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.principal_id = None
+        self.client_id = None
+
+
+class UserAssignedIdentitiesValueAutoGenerated(_serialization.Model):
+    """UserAssignedIdentitiesValueAutoGenerated.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar principal_id: The principal ID of the user-assigned identity.
+    :vartype principal_id: str
+    :ivar client_id: The client ID of the user-assigned identity.
+    :vartype client_id: str
+    """
+
+    _validation = {
+        "principal_id": {"readonly": True},
+        "client_id": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "principal_id": {"key": "principalId", "type": "str"},
+        "client_id": {"key": "clientId", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.principal_id = None
         self.client_id = None
```

