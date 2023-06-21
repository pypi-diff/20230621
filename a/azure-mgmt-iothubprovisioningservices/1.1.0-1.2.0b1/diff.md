# Comparing `tmp/azure-mgmt-iothubprovisioningservices-1.1.0.zip` & `tmp/azure-mgmt-iothubprovisioningservices-1.2.0b1.zip`

## zipinfo {}

```diff
@@ -1,50 +1,55 @@
-Zip file size: 67149 bytes, number of entries: 48
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure/
--rw-rw-r--  2.0 unx     4846 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/CHANGELOG.md
--rw-rw-r--  2.0 unx     1410 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/README.md
--rw-rw-r--  2.0 unx      141 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/MANIFEST.in
--rw-rw-r--  2.0 unx       38 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/setup.cfg
--rw-rw-r--  2.0 unx      629 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/_meta.json
--rw-rw-r--  2.0 unx     8219 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/PKG-INFO
--rw-rw-r--  2.0 unx     1074 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/LICENSE
--rw-rw-r--  2.0 unx     2598 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/setup.py
--rw-rw-r--  2.0 unx     6343 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/tests/test_cli_mgmt_iothubprovisioningservices.py
--rw-rw-r--  2.0 unx        1 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx       63 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/requires.txt
--rw-rw-r--  2.0 unx     1829 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     8219 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/not-zip-safe
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/
--rw-rw-r--  2.0 unx       65 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/
--rw-rw-r--  2.0 unx     3211 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_configuration.py
--rw-rw-r--  2.0 unx      486 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_version.py
--rw-rw-r--  2.0 unx     4448 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_iot_dps_client.py
--rw-rw-r--  2.0 unx     1197 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_vendor.py
--rw-rw-r--  2.0 unx     1529 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_patch.py
--rw-rw-r--  2.0 unx      820 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-07 02:13 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/
--rw-rw-r--  2.0 unx     3229 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_configuration.py
--rw-rw-r--  2.0 unx     4520 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_iot_dps_client.py
--rw-rw-r--  2.0 unx     1529 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_patch.py
--rw-rw-r--  2.0 unx      767 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/__init__.py
--rw-rw-r--  2.0 unx    25983 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_dps_certificate_operations.py
--rw-rw-r--  2.0 unx    68001 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_iot_dps_resource_operations.py
--rw-rw-r--  2.0 unx     4849 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      734 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    60351 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/_models_py3.py
--rw-rw-r--  2.0 unx     3876 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/__init__.py
--rw-rw-r--  2.0 unx     3301 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/_iot_dps_client_enums.py
--rw-rw-r--  2.0 unx    41329 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/_dps_certificate_operations.py
--rw-rw-r--  2.0 unx    90934 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/_iot_dps_resource_operations.py
--rw-rw-r--  2.0 unx     5480 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/_operations.py
--rw-rw-r--  2.0 unx      734 b- defN 22-Feb-07 02:12 azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/__init__.py
-48 files, 362855 bytes uncompressed, 55039 bytes compressed:  84.8%
+Zip file size: 92904 bytes, number of entries: 53
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/
+-rw-rw-r--  2.0 unx     1471 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/README.md
+-rw-rw-r--  2.0 unx      660 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/_meta.json
+-rw-rw-r--  2.0 unx       38 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/setup.cfg
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/LICENSE
+-rw-rw-r--  2.0 unx      232 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     4921 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx     2850 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/setup.py
+-rw-rw-r--  2.0 unx     7311 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/
+-rw-rw-r--  2.0 unx     3770 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_configuration.py
+-rw-rw-r--  2.0 unx     1530 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_patch.py
+-rw-rw-r--  2.0 unx     4669 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_iot_dps_client.py
+-rw-rw-r--  2.0 unx    77450 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_serialization.py
+-rw-rw-r--  2.0 unx      488 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_version.py
+-rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_vendor.py
+-rw-rw-r--  2.0 unx       26 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/py.typed
+-rw-rw-r--  2.0 unx      891 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/
+-rw-rw-r--  2.0 unx     3774 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_configuration.py
+-rw-rw-r--  2.0 unx     1530 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_patch.py
+-rw-rw-r--  2.0 unx     4750 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_iot_dps_client.py
+-rw-rw-r--  2.0 unx      838 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx   100040 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_iot_dps_resource_operations.py
+-rw-rw-r--  2.0 unx     6102 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    42079 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_dps_certificate_operations.py
+-rw-rw-r--  2.0 unx      973 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_patch.py
+-rw-rw-r--  2.0 unx   123518 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_iot_dps_resource_operations.py
+-rw-rw-r--  2.0 unx     6818 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_operations.py
+-rw-rw-r--  2.0 unx    57595 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_dps_certificate_operations.py
+-rw-rw-r--  2.0 unx      973 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/__init__.py
+-rw-rw-r--  2.0 unx     3197 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_iot_dps_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_patch.py
+-rw-rw-r--  2.0 unx     4402 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/__init__.py
+-rw-rw-r--  2.0 unx    58736 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_models_py3.py
+-rw-rw-r--  2.0 unx     6343 b- defN 22-Nov-17 02:44 azure-mgmt-iothubprovisioningservices-1.2.0b1/tests/disable_test_cli_mgmt_iothubprovisioningservices.py
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx      116 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     2117 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx     7311 b- defN 22-Nov-17 02:45 azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/PKG-INFO
+53 files, 541922 bytes uncompressed, 79196 bytes compressed:  85.4%
```

## zipnote {}

```diff
@@ -1,145 +1,160 @@
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/tests/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/tests/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/CHANGELOG.md
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/README.md
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/README.md
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/_meta.json
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/MANIFEST.in
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/setup.cfg
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/LICENSE
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/_meta.json
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/PKG-INFO
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/LICENSE
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/setup.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/setup.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/tests/test_cli_mgmt_iothubprovisioningservices.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/dependency_links.txt
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/requires.txt
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/SOURCES.txt
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/top_level.txt
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/PKG-INFO
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/not-zip-safe
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/__init__.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_patch.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_iot_dps_client.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_version.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/py.typed
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_configuration.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/__init__.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_version.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_iot_dps_client.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_vendor.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_patch.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_iot_dps_client.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/__init__.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_configuration.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_iot_dps_resource_operations.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_iot_dps_client.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_patch.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_dps_certificate_operations.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/__init__.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_dps_certificate_operations.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_iot_dps_resource_operations.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_iot_dps_resource_operations.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_operations.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/__init__.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_dps_certificate_operations.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/_models_py3.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/__init__.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_iot_dps_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/_iot_dps_client_enums.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/_dps_certificate_operations.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/_iot_dps_resource_operations.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/_operations.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/tests/disable_test_cli_mgmt_iothubprovisioningservices.py
 Comment: 
 
-Filename: azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/__init__.py
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/requires.txt
+Comment: 
+
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/CHANGELOG.md` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 1.2.0b1 (2022-11-15)
+
+### Features Added
+
+  - Added model ErrorMessage
+
 ## 1.1.0 (2022-02-07)
 
 **Features**
 
   - Model CertificateResponse has a new parameter system_data
   - Model IotDpsPropertiesDescription has a new parameter enable_data_residency
   - Model PrivateEndpointConnection has a new parameter system_data
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/README.md` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure IoT Hub Provisioning Services Client Library.
-This package has been tested with Python 2.7, 3.6+.
+This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
-
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 # Usage
 
 
 To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
-
-
  
 For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/iot)
 Code samples for this package can be found at [IoT Hub Provisioning Services](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
-Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+Additional code samples for different Azure services are available at [Samples Repo](https://github.com/Azure-Samples/azure-samples-python-management/tree/main/samples/iothubprovisioningservices)
 
 
 # Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project.
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/LICENSE` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/setup.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 PACKAGE_PPRINT_NAME = "IoT Hub Provisioning Services"
 
 # a-b-c => a/b/c
 package_folder_path = PACKAGE_NAME.replace('-', '/')
 # a-b-c => a.b.c
 namespace_name = PACKAGE_NAME.replace('-', '.')
 
-
 # Version extraction inspired from 'requests'
 with open(os.path.join(package_folder_path, 'version.py')
           if os.path.exists(os.path.join(package_folder_path, 'version.py'))
           else os.path.join(package_folder_path, '_version.py'), 'r') as fd:
     version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
                         fd.read(), re.MULTILINE).group(1)
 
@@ -42,33 +41,39 @@
     description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python',
+    keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.mgmt',
     ]),
+    include_package_data=True,
+    package_data={
+        'pytyped': ['py.typed'],
+    },
     install_requires=[
-        'msrest>=0.6.21',
-        'azure-common~=1.1',
-        'azure-mgmt-core>=1.3.0,<2.0.0',
+        "msrest>=0.7.1",
+        "azure-common~=1.1",
+        "azure-mgmt-core>=1.3.2,<2.0.0",
+        "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7"
 )
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/tests/test_cli_mgmt_iothubprovisioningservices.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/tests/disable_test_cli_mgmt_iothubprovisioningservices.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure_mgmt_iothubprovisioningservices.egg-info/SOURCES.txt` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure_mgmt_iothubprovisioningservices.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,36 @@
 setup.py
 azure/__init__.py
 azure/mgmt/__init__.py
 azure/mgmt/iothubprovisioningservices/__init__.py
 azure/mgmt/iothubprovisioningservices/_configuration.py
 azure/mgmt/iothubprovisioningservices/_iot_dps_client.py
 azure/mgmt/iothubprovisioningservices/_patch.py
+azure/mgmt/iothubprovisioningservices/_serialization.py
 azure/mgmt/iothubprovisioningservices/_vendor.py
 azure/mgmt/iothubprovisioningservices/_version.py
+azure/mgmt/iothubprovisioningservices/py.typed
 azure/mgmt/iothubprovisioningservices/aio/__init__.py
 azure/mgmt/iothubprovisioningservices/aio/_configuration.py
 azure/mgmt/iothubprovisioningservices/aio/_iot_dps_client.py
 azure/mgmt/iothubprovisioningservices/aio/_patch.py
 azure/mgmt/iothubprovisioningservices/aio/operations/__init__.py
 azure/mgmt/iothubprovisioningservices/aio/operations/_dps_certificate_operations.py
 azure/mgmt/iothubprovisioningservices/aio/operations/_iot_dps_resource_operations.py
 azure/mgmt/iothubprovisioningservices/aio/operations/_operations.py
+azure/mgmt/iothubprovisioningservices/aio/operations/_patch.py
 azure/mgmt/iothubprovisioningservices/models/__init__.py
 azure/mgmt/iothubprovisioningservices/models/_iot_dps_client_enums.py
 azure/mgmt/iothubprovisioningservices/models/_models_py3.py
+azure/mgmt/iothubprovisioningservices/models/_patch.py
 azure/mgmt/iothubprovisioningservices/operations/__init__.py
 azure/mgmt/iothubprovisioningservices/operations/_dps_certificate_operations.py
 azure/mgmt/iothubprovisioningservices/operations/_iot_dps_resource_operations.py
 azure/mgmt/iothubprovisioningservices/operations/_operations.py
+azure/mgmt/iothubprovisioningservices/operations/_patch.py
 azure_mgmt_iothubprovisioningservices.egg-info/PKG-INFO
 azure_mgmt_iothubprovisioningservices.egg-info/SOURCES.txt
 azure_mgmt_iothubprovisioningservices.egg-info/dependency_links.txt
 azure_mgmt_iothubprovisioningservices.egg-info/not-zip-safe
 azure_mgmt_iothubprovisioningservices.egg-info/requires.txt
 azure_mgmt_iothubprovisioningservices.egg-info/top_level.txt
-tests/test_cli_mgmt_iothubprovisioningservices.py
+tests/disable_test_cli_mgmt_iothubprovisioningservices.py
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_iot_dps_client.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_iot_dps_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,45 +3,49 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, Optional, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
-from msrest import Deserializer, Serializer
 
 from . import models
 from ._configuration import IotDpsClientConfiguration
+from ._serialization import Deserializer, Serializer
 from .operations import DpsCertificateOperations, IotDpsResourceOperations, Operations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
-class IotDpsClient:
+
+class IotDpsClient:  # pylint: disable=client-accepts-api-version-keyword
     """API for using the Azure IoT Hub Device Provisioning Service features.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.iothubprovisioningservices.operations.Operations
     :ivar dps_certificate: DpsCertificateOperations operations
     :vartype dps_certificate:
      azure.mgmt.iothubprovisioningservices.operations.DpsCertificateOperations
     :ivar iot_dps_resource: IotDpsResourceOperations operations
     :vartype iot_dps_resource:
      azure.mgmt.iothubprovisioningservices.operations.IotDpsResourceOperations
-    :param credential: Credential needed for the client to connect to Azure.
+    :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The subscription identifier.
+    :param subscription_id: The subscription identifier. Required.
     :type subscription_id: str
-    :param base_url: Service URL. Default value is 'https://management.azure.com'.
+    :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
+    :keyword api_version: Api Version. Default value is "2022-02-05". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "TokenCredential",
@@ -56,29 +60,24 @@
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.dps_certificate = DpsCertificateOperations(self._client, self._config, self._serialize, self._deserialize)
         self.iot_dps_resource = IotDpsResourceOperations(self._client, self._config, self._serialize, self._deserialize)
 
-
-    def _send_request(
-        self,
-        request,  # type: HttpRequest
-        **kwargs: Any
-    ) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = client._send_request(request)
         <HttpResponse: 200 OK>
 
-        For more information on this code flow, see https://aka.ms/azsdk/python/protocol/quickstart
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.HttpResponse
         """
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_vendor.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_vendor.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from azure.core.pipeline.transport import HttpRequest
 
+
 def _convert_request(request, files=None):
     data = request.content if not files else None
     request = HttpRequest(method=request.method, url=request.url, headers=request.headers, data=data)
     if files:
         request.set_formdata_body(files)
     return request
 
+
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
             formatted_components = template.split("/")
-            components = [
-                c for c in formatted_components if "{}".format(key.args[0]) not in c
-            ]
+            components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/_patch.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/_patch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # This file is used for handwritten extensions to the generated code. Example:
 # https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/customize_code/how-to-patch-sdk-code.md
 def patch_sdk():
-    pass
+    pass
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/__init__.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,13 +6,21 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._iot_dps_client import IotDpsClient
 from ._version import VERSION
 
 __version__ = VERSION
-__all__ = ['IotDpsClient']
 
-# `._patch.py` is used for handwritten extensions to the generated code
-# Example: https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/customize_code/how-to-patch-sdk-code.md
-from ._patch import patch_sdk
-patch_sdk()
+try:
+    from ._patch import __all__ as _patch_all
+    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+except ImportError:
+    _patch_all = []
+from ._patch import patch_sdk as _patch_sdk
+
+__all__ = [
+    "IotDpsClient",
+]
+__all__.extend([p for p in _patch_all if p not in __all__])
+
+_patch_sdk()
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_configuration.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,66 +2,71 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class IotDpsClientConfiguration(Configuration):
+class IotDpsClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for IotDpsClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
-    :param credential: Credential needed for the client to connect to Azure.
+    :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The subscription identifier.
+    :param subscription_id: The subscription identifier. Required.
     :type subscription_id: str
+    :keyword api_version: Api Version. Default value is "2022-02-05". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
 
-    def __init__(
-        self,
-        credential: "AsyncTokenCredential",
-        subscription_id: str,
-        **kwargs: Any
-    ) -> None:
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(IotDpsClientConfiguration, self).__init__(**kwargs)
+        api_version = kwargs.pop("api_version", "2022-02-05")  # type: Literal["2022-02-05"]
+
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2021-10-15"
-        self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
-        kwargs.setdefault('sdk_moniker', 'mgmt-iothubprovisioningservices/{}'.format(VERSION))
+        self.api_version = api_version
+        self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
+        kwargs.setdefault("sdk_moniker", "mgmt-iothubprovisioningservices/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self,
-        **kwargs: Any
-    ) -> None:
-        self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
-        self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
-        self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
-        self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
-        self.http_logging_policy = kwargs.get('http_logging_policy') or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.AsyncRetryPolicy(**kwargs)
-        self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.AsyncRedirectPolicy(**kwargs)
-        self.authentication_policy = kwargs.get('authentication_policy')
+    def _configure(self, **kwargs: Any) -> None:
+        self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
+        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
+        self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
+        self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
+        self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(self.credential, *self.credential_scopes, **kwargs)
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+                self.credential, *self.credential_scopes, **kwargs
+            )
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_iot_dps_client.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_iot_dps_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,45 +3,49 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, Awaitable, Optional, TYPE_CHECKING
+from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
-from msrest import Deserializer, Serializer
 
 from .. import models
+from .._serialization import Deserializer, Serializer
 from ._configuration import IotDpsClientConfiguration
 from .operations import DpsCertificateOperations, IotDpsResourceOperations, Operations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
-class IotDpsClient:
+
+class IotDpsClient:  # pylint: disable=client-accepts-api-version-keyword
     """API for using the Azure IoT Hub Device Provisioning Service features.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.iothubprovisioningservices.aio.operations.Operations
     :ivar dps_certificate: DpsCertificateOperations operations
     :vartype dps_certificate:
      azure.mgmt.iothubprovisioningservices.aio.operations.DpsCertificateOperations
     :ivar iot_dps_resource: IotDpsResourceOperations operations
     :vartype iot_dps_resource:
      azure.mgmt.iothubprovisioningservices.aio.operations.IotDpsResourceOperations
-    :param credential: Credential needed for the client to connect to Azure.
+    :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The subscription identifier.
+    :param subscription_id: The subscription identifier. Required.
     :type subscription_id: str
-    :param base_url: Service URL. Default value is 'https://management.azure.com'.
+    :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
+    :keyword api_version: Api Version. Default value is "2022-02-05". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
         credential: "AsyncTokenCredential",
@@ -56,29 +60,24 @@
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.dps_certificate = DpsCertificateOperations(self._client, self._config, self._serialize, self._deserialize)
         self.iot_dps_resource = IotDpsResourceOperations(self._client, self._config, self._serialize, self._deserialize)
 
-
-    def _send_request(
-        self,
-        request: HttpRequest,
-        **kwargs: Any
-    ) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = await client._send_request(request)
         <AsyncHttpResponse: 200 OK>
 
-        For more information on this code flow, see https://aka.ms/azsdk/python/protocol/quickstart
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.AsyncHttpResponse
         """
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/_patch.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/_patch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # This file is used for handwritten extensions to the generated code. Example:
 # https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/customize_code/how-to-patch-sdk-code.md
 def patch_sdk():
-    pass
+    pass
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_dps_certificate_operations.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_dps_certificate_operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,526 +1,862 @@
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import datetime
-import functools
-from typing import Any, Callable, Dict, Generic, Optional, TypeVar, Union
-import warnings
+import sys
+from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
-from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+from azure.core.exceptions import (
+    ClientAuthenticationError,
+    HttpResponseError,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    ResourceNotModifiedError,
+    map_error,
+)
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._dps_certificate_operations import build_create_or_update_request, build_delete_request, build_generate_verification_code_request, build_get_request, build_list_request, build_verify_certificate_request
-T = TypeVar('T')
+from ...operations._dps_certificate_operations import (
+    build_create_or_update_request,
+    build_delete_request,
+    build_generate_verification_code_request,
+    build_get_request,
+    build_list_request,
+    build_verify_certificate_request,
+)
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-class DpsCertificateOperations:
-    """DpsCertificateOperations async operations.
 
-    You should not instantiate this class directly. Instead, you should create a Client instance that
-    instantiates it for you and attaches it as an attribute.
+class DpsCertificateOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
 
-    :ivar models: Alias to model classes used in this operation group.
-    :type models: ~azure.mgmt.iothubprovisioningservices.models
-    :param client: Client for service requests.
-    :param config: Configuration of service client.
-    :param serializer: An object model serializer.
-    :param deserializer: An object model deserializer.
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.iothubprovisioningservices.aio.IotDpsClient`'s
+        :attr:`dps_certificate` attribute.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer) -> None:
-        self._client = client
-        self._serialize = serializer
-        self._deserialize = deserializer
-        self._config = config
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def get(
         self,
         certificate_name: str,
         resource_group_name: str,
         provisioning_service_name: str,
         if_match: Optional[str] = None,
         **kwargs: Any
-    ) -> "_models.CertificateResponse":
+    ) -> _models.CertificateResponse:
         """Get the certificate from the provisioning service.
 
-        :param certificate_name: Name of the certificate to retrieve.
+        :param certificate_name: Name of the certificate to retrieve. Required.
         :type certificate_name: str
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
         :param provisioning_service_name: Name of the provisioning service the certificate is
-         associated with.
+         associated with. Required.
         :type provisioning_service_name: str
-        :param if_match: ETag of the certificate.
+        :param if_match: ETag of the certificate. Default value is None.
         :type if_match: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CertificateResponse, or the result of cls(response)
+        :return: CertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.CertificateResponse"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CertificateResponse]
 
-        
         request = build_get_request(
             certificate_name=certificate_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
             if_match=if_match,
-            template_url=self.get.metadata['url'],
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('CertificateResponse', pipeline_response)
+        deserialized = self._deserialize("CertificateResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}'}  # type: ignore
+    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}"}  # type: ignore
 
+    @overload
+    async def create_or_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        certificate_name: str,
+        certificate_description: _models.CertificateResponse,
+        if_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.CertificateResponse:
+        """Upload the certificate to the provisioning service.
+
+        Add new certificate or update an existing certificate.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: The name of the provisioning service. Required.
+        :type provisioning_service_name: str
+        :param certificate_name: The name of the certificate create or update. Required.
+        :type certificate_name: str
+        :param certificate_description: The certificate body. Required.
+        :type certificate_description:
+         ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
+        :param if_match: ETag of the certificate. This is required to update an existing certificate,
+         and ignored while creating a brand new certificate. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: CertificateResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_or_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        certificate_name: str,
+        certificate_description: IO,
+        if_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.CertificateResponse:
+        """Upload the certificate to the provisioning service.
+
+        Add new certificate or update an existing certificate.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: The name of the provisioning service. Required.
+        :type provisioning_service_name: str
+        :param certificate_name: The name of the certificate create or update. Required.
+        :type certificate_name: str
+        :param certificate_description: The certificate body. Required.
+        :type certificate_description: IO
+        :param if_match: ETag of the certificate. This is required to update an existing certificate,
+         and ignored while creating a brand new certificate. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: CertificateResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
         certificate_name: str,
-        certificate_description: "_models.CertificateBodyDescription",
+        certificate_description: Union[_models.CertificateResponse, IO],
         if_match: Optional[str] = None,
         **kwargs: Any
-    ) -> "_models.CertificateResponse":
+    ) -> _models.CertificateResponse:
         """Upload the certificate to the provisioning service.
 
         Add new certificate or update an existing certificate.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
-        :param provisioning_service_name: The name of the provisioning service.
+        :param provisioning_service_name: The name of the provisioning service. Required.
         :type provisioning_service_name: str
-        :param certificate_name: The name of the certificate create or update.
+        :param certificate_name: The name of the certificate create or update. Required.
         :type certificate_name: str
-        :param certificate_description: The certificate body.
+        :param certificate_description: The certificate body. Is either a model type or a IO type.
+         Required.
         :type certificate_description:
-         ~azure.mgmt.iothubprovisioningservices.models.CertificateBodyDescription
+         ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse or IO
         :param if_match: ETag of the certificate. This is required to update an existing certificate,
-         and ignored while creating a brand new certificate.
+         and ignored while creating a brand new certificate. Default value is None.
         :type if_match: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CertificateResponse, or the result of cls(response)
+        :return: CertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.CertificateResponse"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(certificate_description, 'CertificateBodyDescription')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CertificateResponse]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(certificate_description, (IO, bytes)):
+            _content = certificate_description
+        else:
+            _json = self._serialize.body(certificate_description, "CertificateResponse")
 
         request = build_create_or_update_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
             certificate_name=certificate_name,
+            subscription_id=self._config.subscription_id,
+            if_match=if_match,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            if_match=if_match,
-            template_url=self.create_or_update.metadata['url'],
+            content=_content,
+            template_url=self.create_or_update.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('CertificateResponse', pipeline_response)
+        deserialized = self._deserialize("CertificateResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}'}  # type: ignore
-
+    create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}"}  # type: ignore
 
     @distributed_trace_async
-    async def delete(
+    async def delete(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         if_match: str,
         provisioning_service_name: str,
         certificate_name: str,
         certificate_name1: Optional[str] = None,
-        certificate_raw_bytes: Optional[bytearray] = None,
+        certificate_raw_bytes: Optional[bytes] = None,
         certificate_is_verified: Optional[bool] = None,
-        certificate_purpose: Optional[Union[str, "_models.CertificatePurpose"]] = None,
+        certificate_purpose: Optional[Union[str, _models.CertificatePurpose]] = None,
         certificate_created: Optional[datetime.datetime] = None,
         certificate_last_updated: Optional[datetime.datetime] = None,
         certificate_has_private_key: Optional[bool] = None,
         certificate_nonce: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """Delete the Provisioning Service Certificate.
 
         Deletes the specified certificate associated with the Provisioning Service.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
-        :param if_match: ETag of the certificate.
+        :param if_match: ETag of the certificate. Required.
         :type if_match: str
-        :param provisioning_service_name: The name of the provisioning service.
+        :param provisioning_service_name: The name of the provisioning service. Required.
         :type provisioning_service_name: str
         :param certificate_name: This is a mandatory field, and is the logical name of the certificate
-         that the provisioning service will access by.
+         that the provisioning service will access by. Required.
         :type certificate_name: str
         :param certificate_name1: This is optional, and it is the Common Name of the certificate.
+         Default value is None.
         :type certificate_name1: str
-        :param certificate_raw_bytes: Raw data within the certificate.
-        :type certificate_raw_bytes: bytearray
+        :param certificate_raw_bytes: Raw data within the certificate. Default value is None.
+        :type certificate_raw_bytes: bytes
         :param certificate_is_verified: Indicates if certificate has been verified by owner of the
-         private key.
+         private key. Default value is None.
         :type certificate_is_verified: bool
-        :param certificate_purpose: A description that mentions the purpose of the certificate.
+        :param certificate_purpose: A description that mentions the purpose of the certificate. Known
+         values are: "clientAuthentication" and "serverAuthentication". Default value is None.
         :type certificate_purpose: str or
          ~azure.mgmt.iothubprovisioningservices.models.CertificatePurpose
-        :param certificate_created: Time the certificate is created.
+        :param certificate_created: Time the certificate is created. Default value is None.
         :type certificate_created: ~datetime.datetime
-        :param certificate_last_updated: Time the certificate is last updated.
+        :param certificate_last_updated: Time the certificate is last updated. Default value is None.
         :type certificate_last_updated: ~datetime.datetime
         :param certificate_has_private_key: Indicates if the certificate contains a private key.
+         Default value is None.
         :type certificate_has_private_key: bool
-        :param certificate_nonce: Random number generated to indicate Proof of Possession.
+        :param certificate_nonce: Random number generated to indicate Proof of Possession. Default
+         value is None.
         :type certificate_nonce: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None, or the result of cls(response)
+        :return: None or the result of cls(response)
         :rtype: None
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[None]
 
-        
         request = build_delete_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
             certificate_name=certificate_name,
+            subscription_id=self._config.subscription_id,
             if_match=if_match,
             certificate_name1=certificate_name1,
             certificate_raw_bytes=certificate_raw_bytes,
             certificate_is_verified=certificate_is_verified,
             certificate_purpose=certificate_purpose,
             certificate_created=certificate_created,
             certificate_last_updated=certificate_last_updated,
             certificate_has_private_key=certificate_has_private_key,
             certificate_nonce=certificate_nonce,
-            template_url=self.delete.metadata['url'],
+            api_version=api_version,
+            template_url=self.delete.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}'}  # type: ignore
-
+    delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}"}  # type: ignore
 
     @distributed_trace_async
     async def list(
-        self,
-        resource_group_name: str,
-        provisioning_service_name: str,
-        **kwargs: Any
-    ) -> "_models.CertificateListDescription":
+        self, resource_group_name: str, provisioning_service_name: str, **kwargs: Any
+    ) -> _models.CertificateListDescription:
         """Get all the certificates tied to the provisioning service.
 
-        :param resource_group_name: Name of resource group.
+        :param resource_group_name: Name of resource group. Required.
         :type resource_group_name: str
         :param provisioning_service_name: Name of provisioning service to retrieve certificates for.
+         Required.
         :type provisioning_service_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CertificateListDescription, or the result of cls(response)
+        :return: CertificateListDescription or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateListDescription
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.CertificateListDescription"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CertificateListDescription]
 
-        
         request = build_list_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
-            template_url=self.list.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('CertificateListDescription', pipeline_response)
+        deserialized = self._deserialize("CertificateListDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates'}  # type: ignore
-
+    list.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates"}  # type: ignore
 
     @distributed_trace_async
     async def generate_verification_code(
         self,
         certificate_name: str,
         if_match: str,
         resource_group_name: str,
         provisioning_service_name: str,
         certificate_name1: Optional[str] = None,
-        certificate_raw_bytes: Optional[bytearray] = None,
+        certificate_raw_bytes: Optional[bytes] = None,
         certificate_is_verified: Optional[bool] = None,
-        certificate_purpose: Optional[Union[str, "_models.CertificatePurpose"]] = None,
+        certificate_purpose: Optional[Union[str, _models.CertificatePurpose]] = None,
         certificate_created: Optional[datetime.datetime] = None,
         certificate_last_updated: Optional[datetime.datetime] = None,
         certificate_has_private_key: Optional[bool] = None,
         certificate_nonce: Optional[str] = None,
         **kwargs: Any
-    ) -> "_models.VerificationCodeResponse":
+    ) -> _models.VerificationCodeResponse:
         """Generate verification code for Proof of Possession.
 
         :param certificate_name: The mandatory logical name of the certificate, that the provisioning
-         service uses to access.
+         service uses to access. Required.
         :type certificate_name: str
         :param if_match: ETag of the certificate. This is required to update an existing certificate,
-         and ignored while creating a brand new certificate.
+         and ignored while creating a brand new certificate. Required.
         :type if_match: str
-        :param resource_group_name: name of resource group.
+        :param resource_group_name: name of resource group. Required.
         :type resource_group_name: str
-        :param provisioning_service_name: Name of provisioning service.
+        :param provisioning_service_name: Name of provisioning service. Required.
         :type provisioning_service_name: str
-        :param certificate_name1: Common Name for the certificate.
+        :param certificate_name1: Common Name for the certificate. Default value is None.
         :type certificate_name1: str
-        :param certificate_raw_bytes: Raw data of certificate.
-        :type certificate_raw_bytes: bytearray
+        :param certificate_raw_bytes: Raw data of certificate. Default value is None.
+        :type certificate_raw_bytes: bytes
         :param certificate_is_verified: Indicates if the certificate has been verified by owner of the
-         private key.
+         private key. Default value is None.
         :type certificate_is_verified: bool
-        :param certificate_purpose: Description mentioning the purpose of the certificate.
+        :param certificate_purpose: Description mentioning the purpose of the certificate. Known values
+         are: "clientAuthentication" and "serverAuthentication". Default value is None.
         :type certificate_purpose: str or
          ~azure.mgmt.iothubprovisioningservices.models.CertificatePurpose
-        :param certificate_created: Certificate creation time.
+        :param certificate_created: Certificate creation time. Default value is None.
         :type certificate_created: ~datetime.datetime
-        :param certificate_last_updated: Certificate last updated time.
+        :param certificate_last_updated: Certificate last updated time. Default value is None.
         :type certificate_last_updated: ~datetime.datetime
-        :param certificate_has_private_key: Indicates if the certificate contains private key.
+        :param certificate_has_private_key: Indicates if the certificate contains private key. Default
+         value is None.
         :type certificate_has_private_key: bool
-        :param certificate_nonce: Random number generated to indicate Proof of Possession.
+        :param certificate_nonce: Random number generated to indicate Proof of Possession. Default
+         value is None.
         :type certificate_nonce: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: VerificationCodeResponse, or the result of cls(response)
+        :return: VerificationCodeResponse or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.VerificationCodeResponse
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.VerificationCodeResponse"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.VerificationCodeResponse]
 
-        
         request = build_generate_verification_code_request(
             certificate_name=certificate_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
             if_match=if_match,
             certificate_name1=certificate_name1,
             certificate_raw_bytes=certificate_raw_bytes,
             certificate_is_verified=certificate_is_verified,
             certificate_purpose=certificate_purpose,
             certificate_created=certificate_created,
             certificate_last_updated=certificate_last_updated,
             certificate_has_private_key=certificate_has_private_key,
             certificate_nonce=certificate_nonce,
-            template_url=self.generate_verification_code.metadata['url'],
+            api_version=api_version,
+            template_url=self.generate_verification_code.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('VerificationCodeResponse', pipeline_response)
+        deserialized = self._deserialize("VerificationCodeResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    generate_verification_code.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}/generateVerificationCode'}  # type: ignore
+    generate_verification_code.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}/generateVerificationCode"}  # type: ignore
+
+    @overload
+    async def verify_certificate(
+        self,
+        certificate_name: str,
+        if_match: str,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        request: _models.VerificationCodeRequest,
+        certificate_name1: Optional[str] = None,
+        certificate_raw_bytes: Optional[bytes] = None,
+        certificate_is_verified: Optional[bool] = None,
+        certificate_purpose: Optional[Union[str, _models.CertificatePurpose]] = None,
+        certificate_created: Optional[datetime.datetime] = None,
+        certificate_last_updated: Optional[datetime.datetime] = None,
+        certificate_has_private_key: Optional[bool] = None,
+        certificate_nonce: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.CertificateResponse:
+        """Verify certificate's private key possession.
 
+        Verifies the certificate's private key possession by providing the leaf cert issued by the
+        verifying pre uploaded certificate.
+
+        :param certificate_name: The mandatory logical name of the certificate, that the provisioning
+         service uses to access. Required.
+        :type certificate_name: str
+        :param if_match: ETag of the certificate. Required.
+        :type if_match: str
+        :param resource_group_name: Resource group name. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Provisioning service name. Required.
+        :type provisioning_service_name: str
+        :param request: The name of the certificate. Required.
+        :type request: ~azure.mgmt.iothubprovisioningservices.models.VerificationCodeRequest
+        :param certificate_name1: Common Name for the certificate. Default value is None.
+        :type certificate_name1: str
+        :param certificate_raw_bytes: Raw data of certificate. Default value is None.
+        :type certificate_raw_bytes: bytes
+        :param certificate_is_verified: Indicates if the certificate has been verified by owner of the
+         private key. Default value is None.
+        :type certificate_is_verified: bool
+        :param certificate_purpose: Describe the purpose of the certificate. Known values are:
+         "clientAuthentication" and "serverAuthentication". Default value is None.
+        :type certificate_purpose: str or
+         ~azure.mgmt.iothubprovisioningservices.models.CertificatePurpose
+        :param certificate_created: Certificate creation time. Default value is None.
+        :type certificate_created: ~datetime.datetime
+        :param certificate_last_updated: Certificate last updated time. Default value is None.
+        :type certificate_last_updated: ~datetime.datetime
+        :param certificate_has_private_key: Indicates if the certificate contains private key. Default
+         value is None.
+        :type certificate_has_private_key: bool
+        :param certificate_nonce: Random number generated to indicate Proof of Possession. Default
+         value is None.
+        :type certificate_nonce: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: CertificateResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def verify_certificate(
+        self,
+        certificate_name: str,
+        if_match: str,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        request: IO,
+        certificate_name1: Optional[str] = None,
+        certificate_raw_bytes: Optional[bytes] = None,
+        certificate_is_verified: Optional[bool] = None,
+        certificate_purpose: Optional[Union[str, _models.CertificatePurpose]] = None,
+        certificate_created: Optional[datetime.datetime] = None,
+        certificate_last_updated: Optional[datetime.datetime] = None,
+        certificate_has_private_key: Optional[bool] = None,
+        certificate_nonce: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.CertificateResponse:
+        """Verify certificate's private key possession.
+
+        Verifies the certificate's private key possession by providing the leaf cert issued by the
+        verifying pre uploaded certificate.
+
+        :param certificate_name: The mandatory logical name of the certificate, that the provisioning
+         service uses to access. Required.
+        :type certificate_name: str
+        :param if_match: ETag of the certificate. Required.
+        :type if_match: str
+        :param resource_group_name: Resource group name. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Provisioning service name. Required.
+        :type provisioning_service_name: str
+        :param request: The name of the certificate. Required.
+        :type request: IO
+        :param certificate_name1: Common Name for the certificate. Default value is None.
+        :type certificate_name1: str
+        :param certificate_raw_bytes: Raw data of certificate. Default value is None.
+        :type certificate_raw_bytes: bytes
+        :param certificate_is_verified: Indicates if the certificate has been verified by owner of the
+         private key. Default value is None.
+        :type certificate_is_verified: bool
+        :param certificate_purpose: Describe the purpose of the certificate. Known values are:
+         "clientAuthentication" and "serverAuthentication". Default value is None.
+        :type certificate_purpose: str or
+         ~azure.mgmt.iothubprovisioningservices.models.CertificatePurpose
+        :param certificate_created: Certificate creation time. Default value is None.
+        :type certificate_created: ~datetime.datetime
+        :param certificate_last_updated: Certificate last updated time. Default value is None.
+        :type certificate_last_updated: ~datetime.datetime
+        :param certificate_has_private_key: Indicates if the certificate contains private key. Default
+         value is None.
+        :type certificate_has_private_key: bool
+        :param certificate_nonce: Random number generated to indicate Proof of Possession. Default
+         value is None.
+        :type certificate_nonce: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: CertificateResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
 
     @distributed_trace_async
     async def verify_certificate(
         self,
         certificate_name: str,
         if_match: str,
         resource_group_name: str,
         provisioning_service_name: str,
-        request: "_models.VerificationCodeRequest",
+        request: Union[_models.VerificationCodeRequest, IO],
         certificate_name1: Optional[str] = None,
-        certificate_raw_bytes: Optional[bytearray] = None,
+        certificate_raw_bytes: Optional[bytes] = None,
         certificate_is_verified: Optional[bool] = None,
-        certificate_purpose: Optional[Union[str, "_models.CertificatePurpose"]] = None,
+        certificate_purpose: Optional[Union[str, _models.CertificatePurpose]] = None,
         certificate_created: Optional[datetime.datetime] = None,
         certificate_last_updated: Optional[datetime.datetime] = None,
         certificate_has_private_key: Optional[bool] = None,
         certificate_nonce: Optional[str] = None,
         **kwargs: Any
-    ) -> "_models.CertificateResponse":
+    ) -> _models.CertificateResponse:
         """Verify certificate's private key possession.
 
         Verifies the certificate's private key possession by providing the leaf cert issued by the
         verifying pre uploaded certificate.
 
         :param certificate_name: The mandatory logical name of the certificate, that the provisioning
-         service uses to access.
+         service uses to access. Required.
         :type certificate_name: str
-        :param if_match: ETag of the certificate.
+        :param if_match: ETag of the certificate. Required.
         :type if_match: str
-        :param resource_group_name: Resource group name.
+        :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
-        :param provisioning_service_name: Provisioning service name.
+        :param provisioning_service_name: Provisioning service name. Required.
         :type provisioning_service_name: str
-        :param request: The name of the certificate.
-        :type request: ~azure.mgmt.iothubprovisioningservices.models.VerificationCodeRequest
-        :param certificate_name1: Common Name for the certificate.
+        :param request: The name of the certificate. Is either a model type or a IO type. Required.
+        :type request: ~azure.mgmt.iothubprovisioningservices.models.VerificationCodeRequest or IO
+        :param certificate_name1: Common Name for the certificate. Default value is None.
         :type certificate_name1: str
-        :param certificate_raw_bytes: Raw data of certificate.
-        :type certificate_raw_bytes: bytearray
+        :param certificate_raw_bytes: Raw data of certificate. Default value is None.
+        :type certificate_raw_bytes: bytes
         :param certificate_is_verified: Indicates if the certificate has been verified by owner of the
-         private key.
+         private key. Default value is None.
         :type certificate_is_verified: bool
-        :param certificate_purpose: Describe the purpose of the certificate.
+        :param certificate_purpose: Describe the purpose of the certificate. Known values are:
+         "clientAuthentication" and "serverAuthentication". Default value is None.
         :type certificate_purpose: str or
          ~azure.mgmt.iothubprovisioningservices.models.CertificatePurpose
-        :param certificate_created: Certificate creation time.
+        :param certificate_created: Certificate creation time. Default value is None.
         :type certificate_created: ~datetime.datetime
-        :param certificate_last_updated: Certificate last updated time.
+        :param certificate_last_updated: Certificate last updated time. Default value is None.
         :type certificate_last_updated: ~datetime.datetime
-        :param certificate_has_private_key: Indicates if the certificate contains private key.
+        :param certificate_has_private_key: Indicates if the certificate contains private key. Default
+         value is None.
         :type certificate_has_private_key: bool
-        :param certificate_nonce: Random number generated to indicate Proof of Possession.
+        :param certificate_nonce: Random number generated to indicate Proof of Possession. Default
+         value is None.
         :type certificate_nonce: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CertificateResponse, or the result of cls(response)
+        :return: CertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.CertificateResponse
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.CertificateResponse"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(request, 'VerificationCodeRequest')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CertificateResponse]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(request, (IO, bytes)):
+            _content = request
+        else:
+            _json = self._serialize.body(request, "VerificationCodeRequest")
 
         request = build_verify_certificate_request(
             certificate_name=certificate_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
-            content_type=content_type,
+            subscription_id=self._config.subscription_id,
             if_match=if_match,
-            json=_json,
             certificate_name1=certificate_name1,
             certificate_raw_bytes=certificate_raw_bytes,
             certificate_is_verified=certificate_is_verified,
             certificate_purpose=certificate_purpose,
             certificate_created=certificate_created,
             certificate_last_updated=certificate_last_updated,
             certificate_has_private_key=certificate_has_private_key,
             certificate_nonce=certificate_nonce,
-            template_url=self.verify_certificate.metadata['url'],
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self.verify_certificate.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('CertificateResponse', pipeline_response)
+        deserialized = self._deserialize("CertificateResponse", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    verify_certificate.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}/verify'}  # type: ignore
-
+    verify_certificate.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/certificates/{certificateName}/verify"}  # type: ignore
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_iot_dps_resource_operations.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_iot_dps_resource_operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1403 +1,2026 @@
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import functools
-from typing import Any, AsyncIterable, Callable, Dict, Generic, List, Optional, TypeVar, Union
-import warnings
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, List, Optional, TypeVar, Union, cast, overload
+import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
-from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+from azure.core.exceptions import (
+    ClientAuthenticationError,
+    HttpResponseError,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    ResourceNotModifiedError,
+    map_error,
+)
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._iot_dps_resource_operations import build_check_provisioning_service_name_availability_request, build_create_or_update_private_endpoint_connection_request_initial, build_create_or_update_request_initial, build_delete_private_endpoint_connection_request_initial, build_delete_request_initial, build_get_operation_result_request, build_get_private_endpoint_connection_request, build_get_private_link_resources_request, build_get_request, build_list_by_resource_group_request, build_list_by_subscription_request, build_list_keys_for_key_name_request, build_list_keys_request, build_list_private_endpoint_connections_request, build_list_private_link_resources_request, build_list_valid_skus_request, build_update_request_initial
-T = TypeVar('T')
+from ...operations._iot_dps_resource_operations import (
+    build_check_provisioning_service_name_availability_request,
+    build_create_or_update_private_endpoint_connection_request,
+    build_create_or_update_request,
+    build_delete_private_endpoint_connection_request,
+    build_delete_request,
+    build_get_operation_result_request,
+    build_get_private_endpoint_connection_request,
+    build_get_private_link_resources_request,
+    build_get_request,
+    build_list_by_resource_group_request,
+    build_list_by_subscription_request,
+    build_list_keys_for_key_name_request,
+    build_list_keys_request,
+    build_list_private_endpoint_connections_request,
+    build_list_private_link_resources_request,
+    build_list_valid_skus_request,
+    build_update_request,
+)
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-class IotDpsResourceOperations:
-    """IotDpsResourceOperations async operations.
 
-    You should not instantiate this class directly. Instead, you should create a Client instance that
-    instantiates it for you and attaches it as an attribute.
+class IotDpsResourceOperations:  # pylint: disable=too-many-public-methods
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
 
-    :ivar models: Alias to model classes used in this operation group.
-    :type models: ~azure.mgmt.iothubprovisioningservices.models
-    :param client: Client for service requests.
-    :param config: Configuration of service client.
-    :param serializer: An object model serializer.
-    :param deserializer: An object model deserializer.
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.iothubprovisioningservices.aio.IotDpsClient`'s
+        :attr:`iot_dps_resource` attribute.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer) -> None:
-        self._client = client
-        self._serialize = serializer
-        self._deserialize = deserializer
-        self._config = config
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace_async
     async def get(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> "_models.ProvisioningServiceDescription":
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
+    ) -> _models.ProvisioningServiceDescription:
         """Get the non-security related metadata of the provisioning service.
 
         Get the metadata of the provisioning service without SAS keys.
 
-        :param provisioning_service_name: Name of the provisioning service to retrieve.
+        :param provisioning_service_name: Name of the provisioning service to retrieve. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: Resource group name.
+        :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ProvisioningServiceDescription, or the result of cls(response)
+        :return: ProvisioningServiceDescription or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
 
-        
         request = build_get_request(
             provisioning_service_name=provisioning_service_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
-            template_url=self.get.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+        deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
-
+    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        iot_dps_description: "_models.ProvisioningServiceDescription",
+        iot_dps_description: Union[_models.ProvisioningServiceDescription, IO],
         **kwargs: Any
-    ) -> "_models.ProvisioningServiceDescription":
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
+    ) -> _models.ProvisioningServiceDescription:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(iot_dps_description, 'ProvisioningServiceDescription')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(iot_dps_description, (IO, bytes)):
+            _content = iot_dps_description
+        else:
+            _json = self._serialize.body(iot_dps_description, "ProvisioningServiceDescription")
 
-        request = build_create_or_update_request_initial(
-            subscription_id=self._config.subscription_id,
+        request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self._create_or_update_initial.metadata['url'],
+            content=_content,
+            template_url=self._create_or_update_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
-
+    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
-    @distributed_trace_async
+    @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        iot_dps_description: "_models.ProvisioningServiceDescription",
+        iot_dps_description: _models.ProvisioningServiceDescription,
+        *,
+        content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller["_models.ProvisioningServiceDescription"]:
+    ) -> AsyncLROPoller[_models.ProvisioningServiceDescription]:
         """Create or update the metadata of the provisioning service.
 
         Create or update the metadata of the provisioning service. The usual pattern to modify a
         property is to retrieve the provisioning service metadata and security metadata, and then
         combine them with the modified values in a new body to update the provisioning service.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
-        :param provisioning_service_name: Name of provisioning service to create or update.
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
         :type provisioning_service_name: str
         :param iot_dps_description: Description of the provisioning service to create or update.
+         Required.
         :type iot_dps_description:
          ~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either ProvisioningServiceDescription or
          the result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+
+    @overload
+    async def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        iot_dps_description: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ProvisioningServiceDescription]:
+        """Create or update the metadata of the provisioning service.
+
+        Create or update the metadata of the provisioning service. The usual pattern to modify a
+        property is to retrieve the provisioning service metadata and security metadata, and then
+        combine them with the modified values in a new body to update the provisioning service.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param iot_dps_description: Description of the provisioning service to create or update.
+         Required.
+        :type iot_dps_description: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either ProvisioningServiceDescription or
+         the result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        iot_dps_description: Union[_models.ProvisioningServiceDescription, IO],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ProvisioningServiceDescription]:
+        """Create or update the metadata of the provisioning service.
+
+        Create or update the metadata of the provisioning service. The usual pattern to modify a
+        property is to retrieve the provisioning service metadata and security metadata, and then
+        combine them with the modified values in a new body to update the provisioning service.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param iot_dps_description: Description of the provisioning service to create or update. Is
+         either a model type or a IO type. Required.
+        :type iot_dps_description:
+         ~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either ProvisioningServiceDescription or
+         the result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = await self._create_or_update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 provisioning_service_name=provisioning_service_name,
                 iot_dps_description=iot_dps_description,
+                api_version=api_version,
                 content_type=content_type,
-                cls=lambda x,y,z: x,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = AsyncNoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     async def _update_initial(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        provisioning_service_tags: "_models.TagsResource",
+        provisioning_service_tags: Union[_models.TagsResource, IO],
         **kwargs: Any
-    ) -> "_models.ProvisioningServiceDescription":
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
+    ) -> _models.ProvisioningServiceDescription:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(provisioning_service_tags, 'TagsResource')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(provisioning_service_tags, (IO, bytes)):
+            _content = provisioning_service_tags
+        else:
+            _json = self._serialize.body(provisioning_service_tags, "TagsResource")
 
-        request = build_update_request_initial(
-            subscription_id=self._config.subscription_id,
+        request = build_update_request(
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self._update_initial.metadata['url'],
+            content=_content,
+            template_url=self._update_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+        deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
+    @overload
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        provisioning_service_tags: _models.TagsResource,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ProvisioningServiceDescription]:
+        """Update an existing provisioning service's tags.
+
+        Update an existing provisioning service's tags. to update other fields use the CreateOrUpdate
+        method.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param provisioning_service_tags: Updated tag information to set into the provisioning service
+         instance. Required.
+        :type provisioning_service_tags: ~azure.mgmt.iothubprovisioningservices.models.TagsResource
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either ProvisioningServiceDescription or
+         the result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        provisioning_service_tags: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ProvisioningServiceDescription]:
+        """Update an existing provisioning service's tags.
+
+        Update an existing provisioning service's tags. to update other fields use the CreateOrUpdate
+        method.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param provisioning_service_tags: Updated tag information to set into the provisioning service
+         instance. Required.
+        :type provisioning_service_tags: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either ProvisioningServiceDescription or
+         the result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
 
     @distributed_trace_async
     async def begin_update(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        provisioning_service_tags: "_models.TagsResource",
+        provisioning_service_tags: Union[_models.TagsResource, IO],
         **kwargs: Any
-    ) -> AsyncLROPoller["_models.ProvisioningServiceDescription"]:
+    ) -> AsyncLROPoller[_models.ProvisioningServiceDescription]:
         """Update an existing provisioning service's tags.
 
         Update an existing provisioning service's tags. to update other fields use the CreateOrUpdate
         method.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
-        :param provisioning_service_name: Name of provisioning service to create or update.
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
         :type provisioning_service_name: str
         :param provisioning_service_tags: Updated tag information to set into the provisioning service
-         instance.
-        :type provisioning_service_tags: ~azure.mgmt.iothubprovisioningservices.models.TagsResource
+         instance. Is either a model type or a IO type. Required.
+        :type provisioning_service_tags: ~azure.mgmt.iothubprovisioningservices.models.TagsResource or
+         IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either ProvisioningServiceDescription or
          the result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = await self._update_initial(
+            raw_result = await self._update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 provisioning_service_name=provisioning_service_name,
                 provisioning_service_tags=provisioning_service_tags,
+                api_version=api_version,
                 content_type=content_type,
-                cls=lambda x,y,z: x,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = AsyncNoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
-    async def _delete_initial(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
+    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
     ) -> None:
-        cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        
-        request = build_delete_request_initial(
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+
+        request = build_delete_request(
             provisioning_service_name=provisioning_service_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
-            template_url=self._delete_initial.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._delete_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204, 404]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
-
+    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete the Provisioning Service.
 
         Deletes the Provisioning Service.
 
-        :param provisioning_service_name: Name of provisioning service to delete.
+        :param provisioning_service_name: Name of provisioning service to delete. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType[None]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = await self._delete_initial(
+            raw_result = await self._delete_initial(  # type: ignore
                 provisioning_service_name=provisioning_service_name,
                 resource_group_name=resource_group_name,
-                cls=lambda x,y,z: x,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
-        def get_long_running_output(pipeline_response):
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
-
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = AsyncNoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     @distributed_trace
-    def list_by_subscription(
-        self,
-        **kwargs: Any
-    ) -> AsyncIterable["_models.ProvisioningServiceDescriptionListResult"]:
+    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.ProvisioningServiceDescription"]:
         """Get all the provisioning services in a subscription.
 
         List all the provisioning services for a given subscription id.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ProvisioningServiceDescriptionListResult or the
-         result of cls(response)
+        :return: An iterator like instance of either ProvisioningServiceDescription or the result of
+         cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescriptionListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescriptionListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescriptionListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_by_subscription_request(
                     subscription_id=self._config.subscription_id,
-                    template_url=self.list_by_subscription.metadata['url'],
+                    api_version=api_version,
+                    template_url=self.list_by_subscription.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_by_subscription_request(
-                    subscription_id=self._config.subscription_id,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ProvisioningServiceDescriptionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return AsyncItemPaged(get_next, extract_data)
 
-        return AsyncItemPaged(
-            get_next, extract_data
-        )
-    list_by_subscription.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.Devices/provisioningServices'}  # type: ignore
+    list_by_subscription.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Devices/provisioningServices"}  # type: ignore
 
     @distributed_trace
     def list_by_resource_group(
-        self,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> AsyncIterable["_models.ProvisioningServiceDescriptionListResult"]:
+        self, resource_group_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.ProvisioningServiceDescription"]:
         """Get a list of all provisioning services in the given resource group.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ProvisioningServiceDescriptionListResult or the
-         result of cls(response)
+        :return: An iterator like instance of either ProvisioningServiceDescription or the result of
+         cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescriptionListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescriptionListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescriptionListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_by_resource_group_request(
-                    subscription_id=self._config.subscription_id,
                     resource_group_name=resource_group_name,
-                    template_url=self.list_by_resource_group.metadata['url'],
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_by_resource_group.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_by_resource_group_request(
-                    subscription_id=self._config.subscription_id,
-                    resource_group_name=resource_group_name,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ProvisioningServiceDescriptionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return AsyncItemPaged(get_next, extract_data)
 
-        return AsyncItemPaged(
-            get_next, extract_data
-        )
-    list_by_resource_group.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices'}  # type: ignore
+    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices"}  # type: ignore
 
     @distributed_trace_async
     async def get_operation_result(
         self,
         operation_id: str,
         resource_group_name: str,
         provisioning_service_name: str,
         asyncinfo: str = "true",
         **kwargs: Any
-    ) -> "_models.AsyncOperationResult":
+    ) -> _models.AsyncOperationResult:
         """Gets the status of a long running operation, such as create, update or delete a provisioning
         service.
 
         :param operation_id: Operation id corresponding to long running operation. Use this to poll for
-         the status.
+         the status. Required.
         :type operation_id: str
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
         :param provisioning_service_name: Name of provisioning service that the operation is running
-         on.
+         on. Required.
         :type provisioning_service_name: str
         :param asyncinfo: Async header used to poll on the status of the operation, obtained while
-         creating the long running operation.
+         creating the long running operation. Default value is "true".
         :type asyncinfo: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: AsyncOperationResult, or the result of cls(response)
+        :return: AsyncOperationResult or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.AsyncOperationResult
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.AsyncOperationResult"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.AsyncOperationResult]
 
-        
         request = build_get_operation_result_request(
             operation_id=operation_id,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
             asyncinfo=asyncinfo,
-            template_url=self.get_operation_result.metadata['url'],
+            api_version=api_version,
+            template_url=self.get_operation_result.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('AsyncOperationResult', pipeline_response)
+        deserialized = self._deserialize("AsyncOperationResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_operation_result.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/operationresults/{operationId}'}  # type: ignore
-
+    get_operation_result.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/operationresults/{operationId}"}  # type: ignore
 
     @distributed_trace
     def list_valid_skus(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> AsyncIterable["_models.IotDpsSkuDefinitionListResult"]:
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.IotDpsSkuDefinition"]:
         """Get the list of valid SKUs for a provisioning service.
 
         Gets the list of valid SKUs and tiers for a provisioning service.
 
-        :param provisioning_service_name: Name of provisioning service.
+        :param provisioning_service_name: Name of provisioning service. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: Name of resource group.
+        :param resource_group_name: Name of resource group. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either IotDpsSkuDefinitionListResult or the result of
-         cls(response)
+        :return: An iterator like instance of either IotDpsSkuDefinition or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuDefinitionListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuDefinition]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.IotDpsSkuDefinitionListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.IotDpsSkuDefinitionListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_valid_skus_request(
                     provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
                     resource_group_name=resource_group_name,
-                    template_url=self.list_valid_skus.metadata['url'],
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_valid_skus.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_valid_skus_request(
-                    provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
-                    resource_group_name=resource_group_name,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("IotDpsSkuDefinitionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return AsyncItemPaged(get_next, extract_data)
 
-        return AsyncItemPaged(
-            get_next, extract_data
-        )
-    list_valid_skus.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/skus'}  # type: ignore
+    list_valid_skus.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/skus"}  # type: ignore
 
-    @distributed_trace_async
+    @overload
     async def check_provisioning_service_name_availability(
-        self,
-        arguments: "_models.OperationInputs",
-        **kwargs: Any
-    ) -> "_models.NameAvailabilityInfo":
+        self, arguments: _models.OperationInputs, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.NameAvailabilityInfo:
         """Check if a provisioning service name is available.
 
         Check if a provisioning service name is available. This will validate if the name is
         syntactically valid and if the name is usable.
 
         :param arguments: Set the name parameter in the OperationInputs structure to the name of the
-         provisioning service to check.
+         provisioning service to check. Required.
         :type arguments: ~azure.mgmt.iothubprovisioningservices.models.OperationInputs
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: NameAvailabilityInfo, or the result of cls(response)
+        :return: NameAvailabilityInfo or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.NameAvailabilityInfo
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def check_provisioning_service_name_availability(
+        self, arguments: IO, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.NameAvailabilityInfo:
+        """Check if a provisioning service name is available.
+
+        Check if a provisioning service name is available. This will validate if the name is
+        syntactically valid and if the name is usable.
+
+        :param arguments: Set the name parameter in the OperationInputs structure to the name of the
+         provisioning service to check. Required.
+        :type arguments: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: NameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.NameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def check_provisioning_service_name_availability(
+        self, arguments: Union[_models.OperationInputs, IO], **kwargs: Any
+    ) -> _models.NameAvailabilityInfo:
+        """Check if a provisioning service name is available.
+
+        Check if a provisioning service name is available. This will validate if the name is
+        syntactically valid and if the name is usable.
+
+        :param arguments: Set the name parameter in the OperationInputs structure to the name of the
+         provisioning service to check. Is either a model type or a IO type. Required.
+        :type arguments: ~azure.mgmt.iothubprovisioningservices.models.OperationInputs or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: NameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.NameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.NameAvailabilityInfo"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(arguments, 'OperationInputs')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.NameAvailabilityInfo]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(arguments, (IO, bytes)):
+            _content = arguments
+        else:
+            _json = self._serialize.body(arguments, "OperationInputs")
 
         request = build_check_provisioning_service_name_availability_request(
             subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self.check_provisioning_service_name_availability.metadata['url'],
+            content=_content,
+            template_url=self.check_provisioning_service_name_availability.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('NameAvailabilityInfo', pipeline_response)
+        deserialized = self._deserialize("NameAvailabilityInfo", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    check_provisioning_service_name_availability.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.Devices/checkProvisioningServiceNameAvailability'}  # type: ignore
-
+    check_provisioning_service_name_availability.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Devices/checkProvisioningServiceNameAvailability"}  # type: ignore
 
     @distributed_trace
     def list_keys(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> AsyncIterable["_models.SharedAccessSignatureAuthorizationRuleListResult"]:
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]:
         """Get the security metadata for a provisioning service.
 
         List the primary and secondary keys for a provisioning service.
 
         :param provisioning_service_name: The provisioning service name to get the shared access keys
-         for.
+         for. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: resource group name.
+        :param resource_group_name: resource group name. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either SharedAccessSignatureAuthorizationRuleListResult
-         or the result of cls(response)
+        :return: An iterator like instance of either
+         SharedAccessSignatureAuthorizationRuleAccessRightsDescription or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.SharedAccessSignatureAuthorizationRuleListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedAccessSignatureAuthorizationRuleListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_keys_request(
                     provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
                     resource_group_name=resource_group_name,
-                    template_url=self.list_keys.metadata['url'],
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_keys.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_keys_request(
-                    provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
-                    resource_group_name=resource_group_name,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("SharedAccessSignatureAuthorizationRuleListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return AsyncItemPaged(get_next, extract_data)
 
-        return AsyncItemPaged(
-            get_next, extract_data
-        )
-    list_keys.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/listkeys'}  # type: ignore
+    list_keys.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/listkeys"}  # type: ignore
 
     @distributed_trace_async
     async def list_keys_for_key_name(
-        self,
-        provisioning_service_name: str,
-        key_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> "_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription":
+        self, provisioning_service_name: str, key_name: str, resource_group_name: str, **kwargs: Any
+    ) -> _models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription:
         """Get a shared access policy by name from a provisioning service.
 
         List primary and secondary keys for a specific key name.
 
-        :param provisioning_service_name: Name of the provisioning service.
+        :param provisioning_service_name: Name of the provisioning service. Required.
         :type provisioning_service_name: str
-        :param key_name: Logical key name to get key-values for.
+        :param key_name: Logical key name to get key-values for. Required.
         :type key_name: str
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: SharedAccessSignatureAuthorizationRuleAccessRightsDescription, or the result of
+        :return: SharedAccessSignatureAuthorizationRuleAccessRightsDescription or the result of
          cls(response)
         :rtype:
          ~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop(
+            "cls", None
+        )  # type: ClsType[_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription]
 
-        
         request = build_list_keys_for_key_name_request(
             provisioning_service_name=provisioning_service_name,
             key_name=key_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
-            template_url=self.list_keys_for_key_name.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_keys_for_key_name.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('SharedAccessSignatureAuthorizationRuleAccessRightsDescription', pipeline_response)
+        deserialized = self._deserialize(
+            "SharedAccessSignatureAuthorizationRuleAccessRightsDescription", pipeline_response
+        )
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_keys_for_key_name.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/keys/{keyName}/listkeys'}  # type: ignore
-
+    list_keys_for_key_name.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/keys/{keyName}/listkeys"}  # type: ignore
 
     @distributed_trace_async
     async def list_private_link_resources(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        **kwargs: Any
-    ) -> "_models.PrivateLinkResources":
+        self, resource_group_name: str, resource_name: str, **kwargs: Any
+    ) -> _models.PrivateLinkResources:
         """List private link resources.
 
         List private link resources for the given provisioning service.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PrivateLinkResources, or the result of cls(response)
+        :return: PrivateLinkResources or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.PrivateLinkResources
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateLinkResources"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateLinkResources]
 
-        
         request = build_list_private_link_resources_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
-            template_url=self.list_private_link_resources.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_private_link_resources.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('PrivateLinkResources', pipeline_response)
+        deserialized = self._deserialize("PrivateLinkResources", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_private_link_resources.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources'}  # type: ignore
-
+    list_private_link_resources.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources"}  # type: ignore
 
     @distributed_trace_async
     async def get_private_link_resources(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        group_id: str,
-        **kwargs: Any
-    ) -> "_models.GroupIdInformation":
+        self, resource_group_name: str, resource_name: str, group_id: str, **kwargs: Any
+    ) -> _models.GroupIdInformation:
         """Get the specified private link resource.
 
         Get the specified private link resource for the given provisioning service.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param group_id: The name of the private link resource.
+        :param group_id: The name of the private link resource. Required.
         :type group_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: GroupIdInformation, or the result of cls(response)
+        :return: GroupIdInformation or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.GroupIdInformation
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.GroupIdInformation"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.GroupIdInformation]
 
-        
         request = build_get_private_link_resources_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             group_id=group_id,
-            template_url=self.get_private_link_resources.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get_private_link_resources.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('GroupIdInformation', pipeline_response)
+        deserialized = self._deserialize("GroupIdInformation", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_private_link_resources.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources/{groupId}'}  # type: ignore
-
+    get_private_link_resources.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources/{groupId}"}  # type: ignore
 
     @distributed_trace_async
     async def list_private_endpoint_connections(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        **kwargs: Any
-    ) -> List["_models.PrivateEndpointConnection"]:
+        self, resource_group_name: str, resource_name: str, **kwargs: Any
+    ) -> List[_models.PrivateEndpointConnection]:
         """List private endpoint connections.
 
         List private endpoint connection properties.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: list of PrivateEndpointConnection, or the result of cls(response)
+        :return: list of PrivateEndpointConnection or the result of cls(response)
         :rtype: list[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType[List["_models.PrivateEndpointConnection"]]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[List[_models.PrivateEndpointConnection]]
 
-        
         request = build_list_private_endpoint_connections_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
-            template_url=self.list_private_endpoint_connections.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_private_endpoint_connections.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('[PrivateEndpointConnection]', pipeline_response)
+        deserialized = self._deserialize("[PrivateEndpointConnection]", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_private_endpoint_connections.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections'}  # type: ignore
-
+    list_private_endpoint_connections.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections"}  # type: ignore
 
     @distributed_trace_async
     async def get_private_endpoint_connection(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        private_endpoint_connection_name: str,
-        **kwargs: Any
-    ) -> "_models.PrivateEndpointConnection":
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> _models.PrivateEndpointConnection:
         """Get private endpoint connection.
 
         Get private endpoint connection properties.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param private_endpoint_connection_name: The name of the private endpoint connection.
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PrivateEndpointConnection, or the result of cls(response)
+        :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
 
-        
         request = build_get_private_endpoint_connection_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
-            template_url=self.get_private_endpoint_connection.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get_private_endpoint_connection.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+        deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_private_endpoint_connection.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
-
+    get_private_endpoint_connection.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
     async def _create_or_update_private_endpoint_connection_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
-        private_endpoint_connection: "_models.PrivateEndpointConnection",
+        private_endpoint_connection: Union[_models.PrivateEndpointConnection, IO],
         **kwargs: Any
-    ) -> "_models.PrivateEndpointConnection":
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
+    ) -> _models.PrivateEndpointConnection:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(private_endpoint_connection, 'PrivateEndpointConnection')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(private_endpoint_connection, (IO, bytes)):
+            _content = private_endpoint_connection
+        else:
+            _json = self._serialize.body(private_endpoint_connection, "PrivateEndpointConnection")
 
-        request = build_create_or_update_private_endpoint_connection_request_initial(
-            subscription_id=self._config.subscription_id,
+        request = build_create_or_update_private_endpoint_connection_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self._create_or_update_private_endpoint_connection_initial.metadata['url'],
+            content=_content,
+            template_url=self._create_or_update_private_endpoint_connection_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_private_endpoint_connection_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
-
+    _create_or_update_private_endpoint_connection_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
-    @distributed_trace_async
+    @overload
     async def begin_create_or_update_private_endpoint_connection(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
-        private_endpoint_connection: "_models.PrivateEndpointConnection",
+        private_endpoint_connection: _models.PrivateEndpointConnection,
+        *,
+        content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller["_models.PrivateEndpointConnection"]:
+    ) -> AsyncLROPoller[_models.PrivateEndpointConnection]:
         """Create or update private endpoint connection.
 
         Create or update the status of a private endpoint connection with the specified name.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param private_endpoint_connection_name: The name of the private endpoint connection.
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :param private_endpoint_connection: The private endpoint connection with updated properties.
+         Required.
         :type private_endpoint_connection:
          ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the
          result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+
+    @overload
+    async def begin_create_or_update_private_endpoint_connection(
+        self,
+        resource_group_name: str,
+        resource_name: str,
+        private_endpoint_connection_name: str,
+        private_endpoint_connection: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.PrivateEndpointConnection]:
+        """Create or update private endpoint connection.
+
+        Create or update the status of a private endpoint connection with the specified name.
+
+        :param resource_group_name: The name of the resource group that contains the provisioning
+         service. Required.
+        :type resource_group_name: str
+        :param resource_name: The name of the provisioning service. Required.
+        :type resource_name: str
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :type private_endpoint_connection_name: str
+        :param private_endpoint_connection: The private endpoint connection with updated properties.
+         Required.
+        :type private_endpoint_connection: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_create_or_update_private_endpoint_connection(
+        self,
+        resource_group_name: str,
+        resource_name: str,
+        private_endpoint_connection_name: str,
+        private_endpoint_connection: Union[_models.PrivateEndpointConnection, IO],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.PrivateEndpointConnection]:
+        """Create or update private endpoint connection.
+
+        Create or update the status of a private endpoint connection with the specified name.
+
+        :param resource_group_name: The name of the resource group that contains the provisioning
+         service. Required.
+        :type resource_group_name: str
+        :param resource_name: The name of the provisioning service. Required.
+        :type resource_name: str
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :type private_endpoint_connection_name: str
+        :param private_endpoint_connection: The private endpoint connection with updated properties. Is
+         either a model type or a IO type. Required.
+        :type private_endpoint_connection:
+         ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = await self._create_or_update_private_endpoint_connection_initial(
+            raw_result = await self._create_or_update_private_endpoint_connection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 private_endpoint_connection=private_endpoint_connection,
+                api_version=api_version,
                 content_type=content_type,
-                cls=lambda x,y,z: x,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = AsyncNoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_create_or_update_private_endpoint_connection.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
+    begin_create_or_update_private_endpoint_connection.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
     async def _delete_private_endpoint_connection_initial(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        private_endpoint_connection_name: str,
-        **kwargs: Any
-    ) -> Optional["_models.PrivateEndpointConnection"]:
-        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.PrivateEndpointConnection"]]
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> Optional[_models.PrivateEndpointConnection]:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        
-        request = build_delete_private_endpoint_connection_request_initial(
-            subscription_id=self._config.subscription_id,
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.PrivateEndpointConnection]]
+
+        request = build_delete_private_endpoint_connection_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
-            template_url=self._delete_private_endpoint_connection_initial.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._delete_private_endpoint_connection_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if response.status_code == 202:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("str", response.headers.get("Retry-After"))
+
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _delete_private_endpoint_connection_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
-
+    _delete_private_endpoint_connection_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
     @distributed_trace_async
     async def begin_delete_private_endpoint_connection(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        private_endpoint_connection_name: str,
-        **kwargs: Any
-    ) -> AsyncLROPoller["_models.PrivateEndpointConnection"]:
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[_models.PrivateEndpointConnection]:
         """Delete private endpoint connection.
 
         Delete private endpoint connection with the specified name.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param private_endpoint_connection_name: The name of the private endpoint connection.
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
          this operation to not poll, or pass in your own initialized polling object for a personal
          polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the
          result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, AsyncPollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = await self._delete_private_endpoint_connection_initial(
+            raw_result = await self._delete_private_endpoint_connection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
-                cls=lambda x,y,z: x,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = AsyncNoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))  # type: AsyncPollingMethod
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_delete_private_endpoint_connection.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
+    begin_delete_private_endpoint_connection.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/aio/operations/_operations.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/aio/operations/_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,140 @@
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import functools
-from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
-import warnings
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
-from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+from azure.core.exceptions import (
+    ClientAuthenticationError,
+    HttpResponseError,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    ResourceNotModifiedError,
+    map_error,
+)
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operations import build_list_request
-T = TypeVar('T')
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-class Operations:
-    """Operations async operations.
 
-    You should not instantiate this class directly. Instead, you should create a Client instance that
-    instantiates it for you and attaches it as an attribute.
+class Operations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
 
-    :ivar models: Alias to model classes used in this operation group.
-    :type models: ~azure.mgmt.iothubprovisioningservices.models
-    :param client: Client for service requests.
-    :param config: Configuration of service client.
-    :param serializer: An object model serializer.
-    :param deserializer: An object model deserializer.
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.iothubprovisioningservices.aio.IotDpsClient`'s
+        :attr:`operations` attribute.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer) -> None:
-        self._client = client
-        self._serialize = serializer
-        self._deserialize = deserializer
-        self._config = config
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(
-        self,
-        **kwargs: Any
-    ) -> AsyncIterable["_models.OperationListResult"]:
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
         """Lists all of the available Microsoft.Devices REST API operations.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either OperationListResult or the result of cls(response)
+        :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.OperationListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.iothubprovisioningservices.models.Operation]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.OperationListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.OperationListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_request(
-                    template_url=self.list.metadata['url'],
+                    api_version=api_version,
+                    template_url=self.list.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_request(
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return AsyncItemPaged(get_next, extract_data)
 
-        return AsyncItemPaged(
-            get_next, extract_data
-        )
-    list.metadata = {'url': '/providers/Microsoft.Devices/operations'}  # type: ignore
+    list.metadata = {"url": "/providers/Microsoft.Devices/operations"}  # type: ignore
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/_models_py3.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_models_py3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,176 +1,161 @@
 # coding=utf-8
+# pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, TYPE_CHECKING, Union
 
-from azure.core.exceptions import HttpResponseError
-import msrest.serialization
+from .. import _serialization
 
-from ._iot_dps_client_enums import *
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from .. import models as _models
 
 
-class AsyncOperationResult(msrest.serialization.Model):
+class AsyncOperationResult(_serialization.Model):
     """Result of a long running operation.
 
     :ivar status: current status of a long running operation.
     :vartype status: str
     :ivar error: Error message containing code, description and details.
-    :vartype error: ~azure.mgmt.iothubprovisioningservices.models.ErrorMesssage
+    :vartype error: ~azure.mgmt.iothubprovisioningservices.models.ErrorMessage
     """
 
     _attribute_map = {
-        'status': {'key': 'status', 'type': 'str'},
-        'error': {'key': 'error', 'type': 'ErrorMesssage'},
+        "status": {"key": "status", "type": "str"},
+        "error": {"key": "error", "type": "ErrorMessage"},
     }
 
-    def __init__(
-        self,
-        *,
-        status: Optional[str] = None,
-        error: Optional["ErrorMesssage"] = None,
-        **kwargs
-    ):
+    def __init__(self, *, status: Optional[str] = None, error: Optional["_models.ErrorMessage"] = None, **kwargs):
         """
         :keyword status: current status of a long running operation.
         :paramtype status: str
         :keyword error: Error message containing code, description and details.
-        :paramtype error: ~azure.mgmt.iothubprovisioningservices.models.ErrorMesssage
+        :paramtype error: ~azure.mgmt.iothubprovisioningservices.models.ErrorMessage
         """
-        super(AsyncOperationResult, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.status = status
         self.error = error
 
 
-class CertificateBodyDescription(msrest.serialization.Model):
+class CertificateBodyDescription(_serialization.Model):
     """The JSON-serialized X509 Certificate.
 
     :ivar certificate: Base-64 representation of the X509 leaf certificate .cer file or just .pem
      file content.
     :vartype certificate: str
     :ivar is_verified: True indicates that the certificate will be created in verified state and
      proof of possession will not be required.
     :vartype is_verified: bool
     """
 
     _attribute_map = {
-        'certificate': {'key': 'certificate', 'type': 'str'},
-        'is_verified': {'key': 'isVerified', 'type': 'bool'},
+        "certificate": {"key": "certificate", "type": "str"},
+        "is_verified": {"key": "isVerified", "type": "bool"},
     }
 
-    def __init__(
-        self,
-        *,
-        certificate: Optional[str] = None,
-        is_verified: Optional[bool] = None,
-        **kwargs
-    ):
+    def __init__(self, *, certificate: Optional[str] = None, is_verified: Optional[bool] = None, **kwargs):
         """
         :keyword certificate: Base-64 representation of the X509 leaf certificate .cer file or just
          .pem file content.
         :paramtype certificate: str
         :keyword is_verified: True indicates that the certificate will be created in verified state and
          proof of possession will not be required.
         :paramtype is_verified: bool
         """
-        super(CertificateBodyDescription, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.certificate = certificate
         self.is_verified = is_verified
 
 
-class CertificateListDescription(msrest.serialization.Model):
+class CertificateListDescription(_serialization.Model):
     """The JSON-serialized array of Certificate objects.
 
     :ivar value: The array of Certificate objects.
     :vartype value: list[~azure.mgmt.iothubprovisioningservices.models.CertificateResponse]
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[CertificateResponse]'},
+        "value": {"key": "value", "type": "[CertificateResponse]"},
     }
 
-    def __init__(
-        self,
-        *,
-        value: Optional[List["CertificateResponse"]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, value: Optional[List["_models.CertificateResponse"]] = None, **kwargs):
         """
         :keyword value: The array of Certificate objects.
         :paramtype value: list[~azure.mgmt.iothubprovisioningservices.models.CertificateResponse]
         """
-        super(CertificateListDescription, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.value = value
 
 
-class CertificateProperties(msrest.serialization.Model):
+class CertificateProperties(_serialization.Model):
     """The description of an X509 CA Certificate.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar subject: The certificate's subject name.
     :vartype subject: str
     :ivar expiry: The certificate's expiration date and time.
     :vartype expiry: ~datetime.datetime
     :ivar thumbprint: The certificate's thumbprint.
     :vartype thumbprint: str
     :ivar is_verified: Determines whether certificate has been verified.
     :vartype is_verified: bool
     :ivar certificate: base-64 representation of X509 certificate .cer file or just .pem file
      content.
-    :vartype certificate: bytearray
+    :vartype certificate: bytes
     :ivar created: The certificate's creation date and time.
     :vartype created: ~datetime.datetime
     :ivar updated: The certificate's last update date and time.
     :vartype updated: ~datetime.datetime
     """
 
     _validation = {
-        'subject': {'readonly': True},
-        'expiry': {'readonly': True},
-        'thumbprint': {'readonly': True},
-        'is_verified': {'readonly': True},
-        'certificate': {'readonly': True},
-        'created': {'readonly': True},
-        'updated': {'readonly': True},
+        "subject": {"readonly": True},
+        "expiry": {"readonly": True},
+        "thumbprint": {"readonly": True},
+        "created": {"readonly": True},
+        "updated": {"readonly": True},
     }
 
     _attribute_map = {
-        'subject': {'key': 'subject', 'type': 'str'},
-        'expiry': {'key': 'expiry', 'type': 'rfc-1123'},
-        'thumbprint': {'key': 'thumbprint', 'type': 'str'},
-        'is_verified': {'key': 'isVerified', 'type': 'bool'},
-        'certificate': {'key': 'certificate', 'type': 'bytearray'},
-        'created': {'key': 'created', 'type': 'rfc-1123'},
-        'updated': {'key': 'updated', 'type': 'rfc-1123'},
+        "subject": {"key": "subject", "type": "str"},
+        "expiry": {"key": "expiry", "type": "rfc-1123"},
+        "thumbprint": {"key": "thumbprint", "type": "str"},
+        "is_verified": {"key": "isVerified", "type": "bool"},
+        "certificate": {"key": "certificate", "type": "bytearray"},
+        "created": {"key": "created", "type": "rfc-1123"},
+        "updated": {"key": "updated", "type": "rfc-1123"},
     }
 
-    def __init__(
-        self,
-        **kwargs
-    ):
+    def __init__(self, *, is_verified: Optional[bool] = None, certificate: Optional[bytes] = None, **kwargs):
         """
+        :keyword is_verified: Determines whether certificate has been verified.
+        :paramtype is_verified: bool
+        :keyword certificate: base-64 representation of X509 certificate .cer file or just .pem file
+         content.
+        :paramtype certificate: bytes
         """
-        super(CertificateProperties, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.subject = None
         self.expiry = None
         self.thumbprint = None
-        self.is_verified = None
-        self.certificate = None
+        self.is_verified = is_verified
+        self.certificate = certificate
         self.created = None
         self.updated = None
 
 
-class CertificateResponse(msrest.serialization.Model):
+class CertificateResponse(_serialization.Model):
     """The X509 Certificate.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar properties: properties of a certificate.
     :vartype properties: ~azure.mgmt.iothubprovisioningservices.models.CertificateProperties
     :ivar id: The resource identifier.
@@ -182,50 +167,45 @@
     :ivar type: The resource type.
     :vartype type: str
     :ivar system_data: Metadata pertaining to creation and last modification of the resource.
     :vartype system_data: ~azure.mgmt.iothubprovisioningservices.models.SystemData
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True},
-        'etag': {'readonly': True},
-        'type': {'readonly': True},
-        'system_data': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "etag": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
     }
 
     _attribute_map = {
-        'properties': {'key': 'properties', 'type': 'CertificateProperties'},
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'etag': {'key': 'etag', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'system_data': {'key': 'systemData', 'type': 'SystemData'},
+        "properties": {"key": "properties", "type": "CertificateProperties"},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "etag": {"key": "etag", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(
-        self,
-        *,
-        properties: Optional["CertificateProperties"] = None,
-        **kwargs
-    ):
+    def __init__(self, *, properties: Optional["_models.CertificateProperties"] = None, **kwargs):
         """
         :keyword properties: properties of a certificate.
         :paramtype properties: ~azure.mgmt.iothubprovisioningservices.models.CertificateProperties
         """
-        super(CertificateResponse, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.properties = properties
         self.id = None
         self.name = None
         self.etag = None
         self.type = None
         self.system_data = None
 
 
-class ErrorDetails(msrest.serialization.Model):
+class ErrorDetails(_serialization.Model):
     """Error details.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar code: The error code.
     :vartype code: str
     :ivar http_status_code: The HTTP status code.
@@ -233,143 +213,129 @@
     :ivar message: The error message.
     :vartype message: str
     :ivar details: The error details.
     :vartype details: str
     """
 
     _validation = {
-        'code': {'readonly': True},
-        'http_status_code': {'readonly': True},
-        'message': {'readonly': True},
-        'details': {'readonly': True},
+        "code": {"readonly": True},
+        "http_status_code": {"readonly": True},
+        "message": {"readonly": True},
+        "details": {"readonly": True},
     }
 
     _attribute_map = {
-        'code': {'key': 'code', 'type': 'str'},
-        'http_status_code': {'key': 'httpStatusCode', 'type': 'str'},
-        'message': {'key': 'message', 'type': 'str'},
-        'details': {'key': 'details', 'type': 'str'},
+        "code": {"key": "code", "type": "str"},
+        "http_status_code": {"key": "httpStatusCode", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "details": {"key": "details", "type": "str"},
     }
 
-    def __init__(
-        self,
-        **kwargs
-    ):
-        """
-        """
-        super(ErrorDetails, self).__init__(**kwargs)
+    def __init__(self, **kwargs):
+        """ """
+        super().__init__(**kwargs)
         self.code = None
         self.http_status_code = None
         self.message = None
         self.details = None
 
 
-class ErrorMesssage(msrest.serialization.Model):
+class ErrorMessage(_serialization.Model):
     """Error response containing message and code.
 
     :ivar code: standard error code.
     :vartype code: str
     :ivar message: standard error description.
     :vartype message: str
     :ivar details: detailed summary of error.
     :vartype details: str
     """
 
     _attribute_map = {
-        'code': {'key': 'code', 'type': 'str'},
-        'message': {'key': 'message', 'type': 'str'},
-        'details': {'key': 'details', 'type': 'str'},
+        "code": {"key": "code", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "details": {"key": "details", "type": "str"},
     }
 
     def __init__(
-        self,
-        *,
-        code: Optional[str] = None,
-        message: Optional[str] = None,
-        details: Optional[str] = None,
-        **kwargs
+        self, *, code: Optional[str] = None, message: Optional[str] = None, details: Optional[str] = None, **kwargs
     ):
         """
         :keyword code: standard error code.
         :paramtype code: str
         :keyword message: standard error description.
         :paramtype message: str
         :keyword details: detailed summary of error.
         :paramtype details: str
         """
-        super(ErrorMesssage, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.code = code
         self.message = message
         self.details = details
 
 
-class GroupIdInformation(msrest.serialization.Model):
+class GroupIdInformation(_serialization.Model):
     """The group information for creating a private endpoint on a provisioning service.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: The resource identifier.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
-    :ivar properties: Required. The properties for a group information object.
+    :ivar properties: The properties for a group information object. Required.
     :vartype properties: ~azure.mgmt.iothubprovisioningservices.models.GroupIdInformationProperties
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True, 'pattern': r'^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$'},
-        'type': {'readonly': True},
-        'properties': {'required': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True, "pattern": r"^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$"},
+        "type": {"readonly": True},
+        "properties": {"required": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'properties': {'key': 'properties', 'type': 'GroupIdInformationProperties'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "properties": {"key": "properties", "type": "GroupIdInformationProperties"},
     }
 
-    def __init__(
-        self,
-        *,
-        properties: "GroupIdInformationProperties",
-        **kwargs
-    ):
+    def __init__(self, *, properties: "_models.GroupIdInformationProperties", **kwargs):
         """
-        :keyword properties: Required. The properties for a group information object.
+        :keyword properties: The properties for a group information object. Required.
         :paramtype properties:
          ~azure.mgmt.iothubprovisioningservices.models.GroupIdInformationProperties
         """
-        super(GroupIdInformation, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.properties = properties
 
 
-class GroupIdInformationProperties(msrest.serialization.Model):
+class GroupIdInformationProperties(_serialization.Model):
     """The properties for a group information object.
 
     :ivar group_id: The group id.
     :vartype group_id: str
     :ivar required_members: The required members for a specific group id.
     :vartype required_members: list[str]
     :ivar required_zone_names: The required DNS zones for a specific group id.
     :vartype required_zone_names: list[str]
     """
 
     _attribute_map = {
-        'group_id': {'key': 'groupId', 'type': 'str'},
-        'required_members': {'key': 'requiredMembers', 'type': '[str]'},
-        'required_zone_names': {'key': 'requiredZoneNames', 'type': '[str]'},
+        "group_id": {"key": "groupId", "type": "str"},
+        "required_members": {"key": "requiredMembers", "type": "[str]"},
+        "required_zone_names": {"key": "requiredZoneNames", "type": "[str]"},
     }
 
     def __init__(
         self,
         *,
         group_id: Optional[str] = None,
         required_members: Optional[List[str]] = None,
@@ -380,45 +346,45 @@
         :keyword group_id: The group id.
         :paramtype group_id: str
         :keyword required_members: The required members for a specific group id.
         :paramtype required_members: list[str]
         :keyword required_zone_names: The required DNS zones for a specific group id.
         :paramtype required_zone_names: list[str]
         """
-        super(GroupIdInformationProperties, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.group_id = group_id
         self.required_members = required_members
         self.required_zone_names = required_zone_names
 
 
-class IotDpsPropertiesDescription(msrest.serialization.Model):
+class IotDpsPropertiesDescription(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """the service specific properties of a provisioning service, including keys, linked iot hubs, current state, and system generated properties such as hostname and idScope.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar state: Current state of the provisioning service. Possible values include: "Activating",
+    :ivar state: Current state of the provisioning service. Known values are: "Activating",
      "Active", "Deleting", "Deleted", "ActivationFailed", "DeletionFailed", "Transitioning",
-     "Suspending", "Suspended", "Resuming", "FailingOver", "FailoverFailed".
+     "Suspending", "Suspended", "Resuming", "FailingOver", and "FailoverFailed".
     :vartype state: str or ~azure.mgmt.iothubprovisioningservices.models.State
-    :ivar public_network_access: Whether requests from Public Network are allowed. Possible values
-     include: "Enabled", "Disabled".
+    :ivar public_network_access: Whether requests from Public Network are allowed. Known values
+     are: "Enabled" and "Disabled".
     :vartype public_network_access: str or
      ~azure.mgmt.iothubprovisioningservices.models.PublicNetworkAccess
     :ivar ip_filter_rules: The IP filter rules.
     :vartype ip_filter_rules: list[~azure.mgmt.iothubprovisioningservices.models.IpFilterRule]
     :ivar private_endpoint_connections: Private endpoint connections created on this IotHub.
     :vartype private_endpoint_connections:
      list[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
     :ivar provisioning_state: The ARM provisioning state of the provisioning service.
     :vartype provisioning_state: str
     :ivar iot_hubs: List of IoT hubs associated with this provisioning service.
     :vartype iot_hubs:
      list[~azure.mgmt.iothubprovisioningservices.models.IotHubDefinitionDescription]
-    :ivar allocation_policy: Allocation policy to be used by this provisioning service. Possible
-     values include: "Hashed", "GeoLatency", "Static".
+    :ivar allocation_policy: Allocation policy to be used by this provisioning service. Known
+     values are: "Hashed", "GeoLatency", and "Static".
     :vartype allocation_policy: str or
      ~azure.mgmt.iothubprovisioningservices.models.AllocationPolicy
     :ivar service_operations_host_name: Service endpoint for provisioning service.
     :vartype service_operations_host_name: str
     :ivar device_provisioning_host_name: Device endpoint for this provisioning service.
     :vartype device_provisioning_host_name: str
     :ivar id_scope: Unique identifier of this provisioning service.
@@ -429,227 +395,218 @@
     :ivar enable_data_residency: Optional.
      Indicates if the DPS instance has Data Residency enabled, removing the cross geo-pair disaster
      recovery.
     :vartype enable_data_residency: bool
     """
 
     _validation = {
-        'service_operations_host_name': {'readonly': True},
-        'device_provisioning_host_name': {'readonly': True},
-        'id_scope': {'readonly': True},
+        "service_operations_host_name": {"readonly": True},
+        "device_provisioning_host_name": {"readonly": True},
+        "id_scope": {"readonly": True},
     }
 
     _attribute_map = {
-        'state': {'key': 'state', 'type': 'str'},
-        'public_network_access': {'key': 'publicNetworkAccess', 'type': 'str'},
-        'ip_filter_rules': {'key': 'ipFilterRules', 'type': '[IpFilterRule]'},
-        'private_endpoint_connections': {'key': 'privateEndpointConnections', 'type': '[PrivateEndpointConnection]'},
-        'provisioning_state': {'key': 'provisioningState', 'type': 'str'},
-        'iot_hubs': {'key': 'iotHubs', 'type': '[IotHubDefinitionDescription]'},
-        'allocation_policy': {'key': 'allocationPolicy', 'type': 'str'},
-        'service_operations_host_name': {'key': 'serviceOperationsHostName', 'type': 'str'},
-        'device_provisioning_host_name': {'key': 'deviceProvisioningHostName', 'type': 'str'},
-        'id_scope': {'key': 'idScope', 'type': 'str'},
-        'authorization_policies': {'key': 'authorizationPolicies', 'type': '[SharedAccessSignatureAuthorizationRuleAccessRightsDescription]'},
-        'enable_data_residency': {'key': 'enableDataResidency', 'type': 'bool'},
+        "state": {"key": "state", "type": "str"},
+        "public_network_access": {"key": "publicNetworkAccess", "type": "str"},
+        "ip_filter_rules": {"key": "ipFilterRules", "type": "[IpFilterRule]"},
+        "private_endpoint_connections": {"key": "privateEndpointConnections", "type": "[PrivateEndpointConnection]"},
+        "provisioning_state": {"key": "provisioningState", "type": "str"},
+        "iot_hubs": {"key": "iotHubs", "type": "[IotHubDefinitionDescription]"},
+        "allocation_policy": {"key": "allocationPolicy", "type": "str"},
+        "service_operations_host_name": {"key": "serviceOperationsHostName", "type": "str"},
+        "device_provisioning_host_name": {"key": "deviceProvisioningHostName", "type": "str"},
+        "id_scope": {"key": "idScope", "type": "str"},
+        "authorization_policies": {
+            "key": "authorizationPolicies",
+            "type": "[SharedAccessSignatureAuthorizationRuleAccessRightsDescription]",
+        },
+        "enable_data_residency": {"key": "enableDataResidency", "type": "bool"},
     }
 
     def __init__(
         self,
         *,
-        state: Optional[Union[str, "State"]] = None,
-        public_network_access: Optional[Union[str, "PublicNetworkAccess"]] = None,
-        ip_filter_rules: Optional[List["IpFilterRule"]] = None,
-        private_endpoint_connections: Optional[List["PrivateEndpointConnection"]] = None,
+        state: Optional[Union[str, "_models.State"]] = None,
+        public_network_access: Optional[Union[str, "_models.PublicNetworkAccess"]] = None,
+        ip_filter_rules: Optional[List["_models.IpFilterRule"]] = None,
+        private_endpoint_connections: Optional[List["_models.PrivateEndpointConnection"]] = None,
         provisioning_state: Optional[str] = None,
-        iot_hubs: Optional[List["IotHubDefinitionDescription"]] = None,
-        allocation_policy: Optional[Union[str, "AllocationPolicy"]] = None,
-        authorization_policies: Optional[List["SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]] = None,
+        iot_hubs: Optional[List["_models.IotHubDefinitionDescription"]] = None,
+        allocation_policy: Optional[Union[str, "_models.AllocationPolicy"]] = None,
+        authorization_policies: Optional[
+            List["_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]
+        ] = None,
         enable_data_residency: Optional[bool] = None,
         **kwargs
     ):
         """
-        :keyword state: Current state of the provisioning service. Possible values include:
-         "Activating", "Active", "Deleting", "Deleted", "ActivationFailed", "DeletionFailed",
-         "Transitioning", "Suspending", "Suspended", "Resuming", "FailingOver", "FailoverFailed".
+        :keyword state: Current state of the provisioning service. Known values are: "Activating",
+         "Active", "Deleting", "Deleted", "ActivationFailed", "DeletionFailed", "Transitioning",
+         "Suspending", "Suspended", "Resuming", "FailingOver", and "FailoverFailed".
         :paramtype state: str or ~azure.mgmt.iothubprovisioningservices.models.State
-        :keyword public_network_access: Whether requests from Public Network are allowed. Possible
-         values include: "Enabled", "Disabled".
+        :keyword public_network_access: Whether requests from Public Network are allowed. Known values
+         are: "Enabled" and "Disabled".
         :paramtype public_network_access: str or
          ~azure.mgmt.iothubprovisioningservices.models.PublicNetworkAccess
         :keyword ip_filter_rules: The IP filter rules.
         :paramtype ip_filter_rules: list[~azure.mgmt.iothubprovisioningservices.models.IpFilterRule]
         :keyword private_endpoint_connections: Private endpoint connections created on this IotHub.
         :paramtype private_endpoint_connections:
          list[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
         :keyword provisioning_state: The ARM provisioning state of the provisioning service.
         :paramtype provisioning_state: str
         :keyword iot_hubs: List of IoT hubs associated with this provisioning service.
         :paramtype iot_hubs:
          list[~azure.mgmt.iothubprovisioningservices.models.IotHubDefinitionDescription]
-        :keyword allocation_policy: Allocation policy to be used by this provisioning service. Possible
-         values include: "Hashed", "GeoLatency", "Static".
+        :keyword allocation_policy: Allocation policy to be used by this provisioning service. Known
+         values are: "Hashed", "GeoLatency", and "Static".
         :paramtype allocation_policy: str or
          ~azure.mgmt.iothubprovisioningservices.models.AllocationPolicy
         :keyword authorization_policies: List of authorization keys for a provisioning service.
         :paramtype authorization_policies:
          list[~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription]
         :keyword enable_data_residency: Optional.
          Indicates if the DPS instance has Data Residency enabled, removing the cross geo-pair disaster
          recovery.
         :paramtype enable_data_residency: bool
         """
-        super(IotDpsPropertiesDescription, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.state = state
         self.public_network_access = public_network_access
         self.ip_filter_rules = ip_filter_rules
         self.private_endpoint_connections = private_endpoint_connections
         self.provisioning_state = provisioning_state
         self.iot_hubs = iot_hubs
         self.allocation_policy = allocation_policy
         self.service_operations_host_name = None
         self.device_provisioning_host_name = None
         self.id_scope = None
         self.authorization_policies = authorization_policies
         self.enable_data_residency = enable_data_residency
 
 
-class IotDpsSkuDefinition(msrest.serialization.Model):
+class IotDpsSkuDefinition(_serialization.Model):
     """Available SKUs of tier and units.
 
-    :ivar name: Sku name. Possible values include: "S1".
+    :ivar name: Sku name. "S1"
     :vartype name: str or ~azure.mgmt.iothubprovisioningservices.models.IotDpsSku
     """
 
     _attribute_map = {
-        'name': {'key': 'name', 'type': 'str'},
+        "name": {"key": "name", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        name: Optional[Union[str, "IotDpsSku"]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, name: Optional[Union[str, "_models.IotDpsSku"]] = None, **kwargs):
         """
-        :keyword name: Sku name. Possible values include: "S1".
+        :keyword name: Sku name. "S1"
         :paramtype name: str or ~azure.mgmt.iothubprovisioningservices.models.IotDpsSku
         """
-        super(IotDpsSkuDefinition, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.name = name
 
 
-class IotDpsSkuDefinitionListResult(msrest.serialization.Model):
+class IotDpsSkuDefinitionListResult(_serialization.Model):
     """List of available SKUs.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: The list of SKUs.
     :vartype value: list[~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuDefinition]
     :ivar next_link: The next link.
     :vartype next_link: str
     """
 
     _validation = {
-        'next_link': {'readonly': True},
+        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[IotDpsSkuDefinition]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[IotDpsSkuDefinition]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        value: Optional[List["IotDpsSkuDefinition"]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, value: Optional[List["_models.IotDpsSkuDefinition"]] = None, **kwargs):
         """
         :keyword value: The list of SKUs.
         :paramtype value: list[~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuDefinition]
         """
-        super(IotDpsSkuDefinitionListResult, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
-class IotDpsSkuInfo(msrest.serialization.Model):
+class IotDpsSkuInfo(_serialization.Model):
     """List of possible provisioning service SKUs.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar name: Sku name. Possible values include: "S1".
+    :ivar name: Sku name. "S1"
     :vartype name: str or ~azure.mgmt.iothubprovisioningservices.models.IotDpsSku
     :ivar tier: Pricing tier name of the provisioning service.
     :vartype tier: str
     :ivar capacity: The number of units to provision.
-    :vartype capacity: long
+    :vartype capacity: int
     """
 
     _validation = {
-        'tier': {'readonly': True},
+        "tier": {"readonly": True},
     }
 
     _attribute_map = {
-        'name': {'key': 'name', 'type': 'str'},
-        'tier': {'key': 'tier', 'type': 'str'},
-        'capacity': {'key': 'capacity', 'type': 'long'},
+        "name": {"key": "name", "type": "str"},
+        "tier": {"key": "tier", "type": "str"},
+        "capacity": {"key": "capacity", "type": "int"},
     }
 
     def __init__(
-        self,
-        *,
-        name: Optional[Union[str, "IotDpsSku"]] = None,
-        capacity: Optional[int] = None,
-        **kwargs
+        self, *, name: Optional[Union[str, "_models.IotDpsSku"]] = None, capacity: Optional[int] = None, **kwargs
     ):
         """
-        :keyword name: Sku name. Possible values include: "S1".
+        :keyword name: Sku name. "S1"
         :paramtype name: str or ~azure.mgmt.iothubprovisioningservices.models.IotDpsSku
         :keyword capacity: The number of units to provision.
-        :paramtype capacity: long
+        :paramtype capacity: int
         """
-        super(IotDpsSkuInfo, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.name = name
         self.tier = None
         self.capacity = capacity
 
 
-class IotHubDefinitionDescription(msrest.serialization.Model):
+class IotHubDefinitionDescription(_serialization.Model):
     """Description of the IoT hub.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar apply_allocation_policy: flag for applying allocationPolicy or not for a given iot hub.
     :vartype apply_allocation_policy: bool
     :ivar allocation_weight: weight to apply for a given iot h.
     :vartype allocation_weight: int
     :ivar name: Host name of the IoT hub.
     :vartype name: str
-    :ivar connection_string: Required. Connection string of the IoT hub.
+    :ivar connection_string: Connection string of the IoT hub. Required.
     :vartype connection_string: str
-    :ivar location: Required. ARM region of the IoT hub.
+    :ivar location: ARM region of the IoT hub. Required.
     :vartype location: str
     """
 
     _validation = {
-        'name': {'readonly': True},
-        'connection_string': {'required': True},
-        'location': {'required': True},
+        "name": {"readonly": True},
+        "connection_string": {"required": True},
+        "location": {"required": True},
     }
 
     _attribute_map = {
-        'apply_allocation_policy': {'key': 'applyAllocationPolicy', 'type': 'bool'},
-        'allocation_weight': {'key': 'allocationWeight', 'type': 'int'},
-        'name': {'key': 'name', 'type': 'str'},
-        'connection_string': {'key': 'connectionString', 'type': 'str'},
-        'location': {'key': 'location', 'type': 'str'},
+        "apply_allocation_policy": {"key": "applyAllocationPolicy", "type": "bool"},
+        "allocation_weight": {"key": "allocationWeight", "type": "int"},
+        "name": {"key": "name", "type": "str"},
+        "connection_string": {"key": "connectionString", "type": "str"},
+        "location": {"key": "location", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         connection_string: str,
         location: str,
@@ -659,514 +616,479 @@
     ):
         """
         :keyword apply_allocation_policy: flag for applying allocationPolicy or not for a given iot
          hub.
         :paramtype apply_allocation_policy: bool
         :keyword allocation_weight: weight to apply for a given iot h.
         :paramtype allocation_weight: int
-        :keyword connection_string: Required. Connection string of the IoT hub.
+        :keyword connection_string: Connection string of the IoT hub. Required.
         :paramtype connection_string: str
-        :keyword location: Required. ARM region of the IoT hub.
+        :keyword location: ARM region of the IoT hub. Required.
         :paramtype location: str
         """
-        super(IotHubDefinitionDescription, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.apply_allocation_policy = apply_allocation_policy
         self.allocation_weight = allocation_weight
         self.name = None
         self.connection_string = connection_string
         self.location = location
 
 
-class IpFilterRule(msrest.serialization.Model):
+class IpFilterRule(_serialization.Model):
     """The IP filter rules for a provisioning Service.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar filter_name: Required. The name of the IP filter rule.
+    :ivar filter_name: The name of the IP filter rule. Required.
     :vartype filter_name: str
-    :ivar action: Required. The desired action for requests captured by this rule. Possible values
-     include: "Accept", "Reject".
+    :ivar action: The desired action for requests captured by this rule. Required. Known values
+     are: "Accept" and "Reject".
     :vartype action: str or ~azure.mgmt.iothubprovisioningservices.models.IpFilterActionType
-    :ivar ip_mask: Required. A string that contains the IP address range in CIDR notation for the
-     rule.
+    :ivar ip_mask: A string that contains the IP address range in CIDR notation for the rule.
+     Required.
     :vartype ip_mask: str
-    :ivar target: Target for requests captured by this rule. Possible values include: "all",
-     "serviceApi", "deviceApi".
+    :ivar target: Target for requests captured by this rule. Known values are: "all", "serviceApi",
+     and "deviceApi".
     :vartype target: str or ~azure.mgmt.iothubprovisioningservices.models.IpFilterTargetType
     """
 
     _validation = {
-        'filter_name': {'required': True},
-        'action': {'required': True},
-        'ip_mask': {'required': True},
+        "filter_name": {"required": True},
+        "action": {"required": True},
+        "ip_mask": {"required": True},
     }
 
     _attribute_map = {
-        'filter_name': {'key': 'filterName', 'type': 'str'},
-        'action': {'key': 'action', 'type': 'str'},
-        'ip_mask': {'key': 'ipMask', 'type': 'str'},
-        'target': {'key': 'target', 'type': 'str'},
+        "filter_name": {"key": "filterName", "type": "str"},
+        "action": {"key": "action", "type": "str"},
+        "ip_mask": {"key": "ipMask", "type": "str"},
+        "target": {"key": "target", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         filter_name: str,
-        action: Union[str, "IpFilterActionType"],
+        action: Union[str, "_models.IpFilterActionType"],
         ip_mask: str,
-        target: Optional[Union[str, "IpFilterTargetType"]] = None,
+        target: Optional[Union[str, "_models.IpFilterTargetType"]] = None,
         **kwargs
     ):
         """
-        :keyword filter_name: Required. The name of the IP filter rule.
+        :keyword filter_name: The name of the IP filter rule. Required.
         :paramtype filter_name: str
-        :keyword action: Required. The desired action for requests captured by this rule. Possible
-         values include: "Accept", "Reject".
+        :keyword action: The desired action for requests captured by this rule. Required. Known values
+         are: "Accept" and "Reject".
         :paramtype action: str or ~azure.mgmt.iothubprovisioningservices.models.IpFilterActionType
-        :keyword ip_mask: Required. A string that contains the IP address range in CIDR notation for
-         the rule.
+        :keyword ip_mask: A string that contains the IP address range in CIDR notation for the rule.
+         Required.
         :paramtype ip_mask: str
-        :keyword target: Target for requests captured by this rule. Possible values include: "all",
-         "serviceApi", "deviceApi".
+        :keyword target: Target for requests captured by this rule. Known values are: "all",
+         "serviceApi", and "deviceApi".
         :paramtype target: str or ~azure.mgmt.iothubprovisioningservices.models.IpFilterTargetType
         """
-        super(IpFilterRule, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.filter_name = filter_name
         self.action = action
         self.ip_mask = ip_mask
         self.target = target
 
 
-class NameAvailabilityInfo(msrest.serialization.Model):
+class NameAvailabilityInfo(_serialization.Model):
     """Description of name availability.
 
     :ivar name_available: specifies if a name is available or not.
     :vartype name_available: bool
-    :ivar reason: specifies the reason a name is unavailable. Possible values include: "Invalid",
+    :ivar reason: specifies the reason a name is unavailable. Known values are: "Invalid" and
      "AlreadyExists".
     :vartype reason: str or ~azure.mgmt.iothubprovisioningservices.models.NameUnavailabilityReason
     :ivar message: message containing a detailed reason name is unavailable.
     :vartype message: str
     """
 
     _attribute_map = {
-        'name_available': {'key': 'nameAvailable', 'type': 'bool'},
-        'reason': {'key': 'reason', 'type': 'str'},
-        'message': {'key': 'message', 'type': 'str'},
+        "name_available": {"key": "nameAvailable", "type": "bool"},
+        "reason": {"key": "reason", "type": "str"},
+        "message": {"key": "message", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         name_available: Optional[bool] = None,
-        reason: Optional[Union[str, "NameUnavailabilityReason"]] = None,
+        reason: Optional[Union[str, "_models.NameUnavailabilityReason"]] = None,
         message: Optional[str] = None,
         **kwargs
     ):
         """
         :keyword name_available: specifies if a name is available or not.
         :paramtype name_available: bool
-        :keyword reason: specifies the reason a name is unavailable. Possible values include:
-         "Invalid", "AlreadyExists".
+        :keyword reason: specifies the reason a name is unavailable. Known values are: "Invalid" and
+         "AlreadyExists".
         :paramtype reason: str or
          ~azure.mgmt.iothubprovisioningservices.models.NameUnavailabilityReason
         :keyword message: message containing a detailed reason name is unavailable.
         :paramtype message: str
         """
-        super(NameAvailabilityInfo, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.name_available = name_available
         self.reason = reason
         self.message = message
 
 
-class Operation(msrest.serialization.Model):
+class Operation(_serialization.Model):
     """Provisioning Service REST API operation.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar name: Operation name: {provider}/{resource}/{read | write | action | delete}.
     :vartype name: str
     :ivar display: The object that represents the operation.
     :vartype display: ~azure.mgmt.iothubprovisioningservices.models.OperationDisplay
     """
 
     _validation = {
-        'name': {'readonly': True},
+        "name": {"readonly": True},
     }
 
     _attribute_map = {
-        'name': {'key': 'name', 'type': 'str'},
-        'display': {'key': 'display', 'type': 'OperationDisplay'},
+        "name": {"key": "name", "type": "str"},
+        "display": {"key": "display", "type": "OperationDisplay"},
     }
 
-    def __init__(
-        self,
-        *,
-        display: Optional["OperationDisplay"] = None,
-        **kwargs
-    ):
+    def __init__(self, *, display: Optional["_models.OperationDisplay"] = None, **kwargs):
         """
         :keyword display: The object that represents the operation.
         :paramtype display: ~azure.mgmt.iothubprovisioningservices.models.OperationDisplay
         """
-        super(Operation, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.name = None
         self.display = display
 
 
-class OperationDisplay(msrest.serialization.Model):
+class OperationDisplay(_serialization.Model):
     """The object that represents the operation.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar provider: Service provider: Microsoft Devices.
     :vartype provider: str
     :ivar resource: Resource Type: ProvisioningServices.
     :vartype resource: str
     :ivar operation: Name of the operation.
     :vartype operation: str
     """
 
     _validation = {
-        'provider': {'readonly': True},
-        'resource': {'readonly': True},
-        'operation': {'readonly': True},
+        "provider": {"readonly": True},
+        "resource": {"readonly": True},
+        "operation": {"readonly": True},
     }
 
     _attribute_map = {
-        'provider': {'key': 'provider', 'type': 'str'},
-        'resource': {'key': 'resource', 'type': 'str'},
-        'operation': {'key': 'operation', 'type': 'str'},
+        "provider": {"key": "provider", "type": "str"},
+        "resource": {"key": "resource", "type": "str"},
+        "operation": {"key": "operation", "type": "str"},
     }
 
-    def __init__(
-        self,
-        **kwargs
-    ):
-        """
-        """
-        super(OperationDisplay, self).__init__(**kwargs)
+    def __init__(self, **kwargs):
+        """ """
+        super().__init__(**kwargs)
         self.provider = None
         self.resource = None
         self.operation = None
 
 
-class OperationInputs(msrest.serialization.Model):
+class OperationInputs(_serialization.Model):
     """Input values for operation results call.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar name: Required. The name of the Provisioning Service to check.
+    :ivar name: The name of the Provisioning Service to check. Required.
     :vartype name: str
     """
 
     _validation = {
-        'name': {'required': True},
+        "name": {"required": True},
     }
 
     _attribute_map = {
-        'name': {'key': 'name', 'type': 'str'},
+        "name": {"key": "name", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        name: str,
-        **kwargs
-    ):
+    def __init__(self, *, name: str, **kwargs):
         """
-        :keyword name: Required. The name of the Provisioning Service to check.
+        :keyword name: The name of the Provisioning Service to check. Required.
         :paramtype name: str
         """
-        super(OperationInputs, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.name = name
 
 
-class OperationListResult(msrest.serialization.Model):
+class OperationListResult(_serialization.Model):
     """Result of the request to list provisioning service operations. It contains a list of operations and a URL link to get the next set of results.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: Provisioning service operations supported by the Microsoft.Devices resource
      provider.
     :vartype value: list[~azure.mgmt.iothubprovisioningservices.models.Operation]
     :ivar next_link: URL to get the next set of operation list results if there are any.
     :vartype next_link: str
     """
 
     _validation = {
-        'value': {'readonly': True},
-        'next_link': {'readonly': True},
+        "value": {"readonly": True},
+        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[Operation]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[Operation]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(
-        self,
-        **kwargs
-    ):
-        """
-        """
-        super(OperationListResult, self).__init__(**kwargs)
+    def __init__(self, **kwargs):
+        """ """
+        super().__init__(**kwargs)
         self.value = None
         self.next_link = None
 
 
-class PrivateEndpoint(msrest.serialization.Model):
+class PrivateEndpoint(_serialization.Model):
     """The private endpoint property of a private endpoint connection.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: The resource identifier.
     :vartype id: str
     """
 
     _validation = {
-        'id': {'readonly': True},
+        "id": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
+        "id": {"key": "id", "type": "str"},
     }
 
-    def __init__(
-        self,
-        **kwargs
-    ):
-        """
-        """
-        super(PrivateEndpoint, self).__init__(**kwargs)
+    def __init__(self, **kwargs):
+        """ """
+        super().__init__(**kwargs)
         self.id = None
 
 
-class PrivateEndpointConnection(msrest.serialization.Model):
+class PrivateEndpointConnection(_serialization.Model):
     """The private endpoint connection of a provisioning service.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: The resource identifier.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
-    :ivar properties: Required. The properties of a private endpoint connection.
+    :ivar properties: The properties of a private endpoint connection. Required.
     :vartype properties:
      ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnectionProperties
     :ivar system_data: Metadata pertaining to creation and last modification of the resource.
     :vartype system_data: ~azure.mgmt.iothubprovisioningservices.models.SystemData
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True, 'pattern': r'^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$'},
-        'type': {'readonly': True},
-        'properties': {'required': True},
-        'system_data': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True, "pattern": r"^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$"},
+        "type": {"readonly": True},
+        "properties": {"required": True},
+        "system_data": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'properties': {'key': 'properties', 'type': 'PrivateEndpointConnectionProperties'},
-        'system_data': {'key': 'systemData', 'type': 'SystemData'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "properties": {"key": "properties", "type": "PrivateEndpointConnectionProperties"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
-    def __init__(
-        self,
-        *,
-        properties: "PrivateEndpointConnectionProperties",
-        **kwargs
-    ):
+    def __init__(self, *, properties: "_models.PrivateEndpointConnectionProperties", **kwargs):
         """
-        :keyword properties: Required. The properties of a private endpoint connection.
+        :keyword properties: The properties of a private endpoint connection. Required.
         :paramtype properties:
          ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnectionProperties
         """
-        super(PrivateEndpointConnection, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.properties = properties
         self.system_data = None
 
 
-class PrivateEndpointConnectionProperties(msrest.serialization.Model):
+class PrivateEndpointConnectionProperties(_serialization.Model):
     """The properties of a private endpoint connection.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar private_endpoint: The private endpoint property of a private endpoint connection.
     :vartype private_endpoint: ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpoint
-    :ivar private_link_service_connection_state: Required. The current state of a private endpoint
-     connection.
+    :ivar private_link_service_connection_state: The current state of a private endpoint
+     connection. Required.
     :vartype private_link_service_connection_state:
      ~azure.mgmt.iothubprovisioningservices.models.PrivateLinkServiceConnectionState
     """
 
     _validation = {
-        'private_link_service_connection_state': {'required': True},
+        "private_link_service_connection_state": {"required": True},
     }
 
     _attribute_map = {
-        'private_endpoint': {'key': 'privateEndpoint', 'type': 'PrivateEndpoint'},
-        'private_link_service_connection_state': {'key': 'privateLinkServiceConnectionState', 'type': 'PrivateLinkServiceConnectionState'},
+        "private_endpoint": {"key": "privateEndpoint", "type": "PrivateEndpoint"},
+        "private_link_service_connection_state": {
+            "key": "privateLinkServiceConnectionState",
+            "type": "PrivateLinkServiceConnectionState",
+        },
     }
 
     def __init__(
         self,
         *,
-        private_link_service_connection_state: "PrivateLinkServiceConnectionState",
-        private_endpoint: Optional["PrivateEndpoint"] = None,
+        private_link_service_connection_state: "_models.PrivateLinkServiceConnectionState",
+        private_endpoint: Optional["_models.PrivateEndpoint"] = None,
         **kwargs
     ):
         """
         :keyword private_endpoint: The private endpoint property of a private endpoint connection.
         :paramtype private_endpoint: ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpoint
-        :keyword private_link_service_connection_state: Required. The current state of a private
-         endpoint connection.
+        :keyword private_link_service_connection_state: The current state of a private endpoint
+         connection. Required.
         :paramtype private_link_service_connection_state:
          ~azure.mgmt.iothubprovisioningservices.models.PrivateLinkServiceConnectionState
         """
-        super(PrivateEndpointConnectionProperties, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.private_endpoint = private_endpoint
         self.private_link_service_connection_state = private_link_service_connection_state
 
 
-class PrivateLinkResources(msrest.serialization.Model):
+class PrivateLinkResources(_serialization.Model):
     """The available private link resources for a provisioning service.
 
     :ivar value: The list of available private link resources for a provisioning service.
     :vartype value: list[~azure.mgmt.iothubprovisioningservices.models.GroupIdInformation]
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[GroupIdInformation]'},
+        "value": {"key": "value", "type": "[GroupIdInformation]"},
     }
 
-    def __init__(
-        self,
-        *,
-        value: Optional[List["GroupIdInformation"]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, value: Optional[List["_models.GroupIdInformation"]] = None, **kwargs):
         """
         :keyword value: The list of available private link resources for a provisioning service.
         :paramtype value: list[~azure.mgmt.iothubprovisioningservices.models.GroupIdInformation]
         """
-        super(PrivateLinkResources, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.value = value
 
 
-class PrivateLinkServiceConnectionState(msrest.serialization.Model):
+class PrivateLinkServiceConnectionState(_serialization.Model):
     """The current state of a private endpoint connection.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar status: Required. The status of a private endpoint connection. Possible values include:
-     "Pending", "Approved", "Rejected", "Disconnected".
+    :ivar status: The status of a private endpoint connection. Required. Known values are:
+     "Pending", "Approved", "Rejected", and "Disconnected".
     :vartype status: str or
      ~azure.mgmt.iothubprovisioningservices.models.PrivateLinkServiceConnectionStatus
-    :ivar description: Required. The description for the current state of a private endpoint
-     connection.
+    :ivar description: The description for the current state of a private endpoint connection.
+     Required.
     :vartype description: str
     :ivar actions_required: Actions required for a private endpoint connection.
     :vartype actions_required: str
     """
 
     _validation = {
-        'status': {'required': True},
-        'description': {'required': True},
+        "status": {"required": True},
+        "description": {"required": True},
     }
 
     _attribute_map = {
-        'status': {'key': 'status', 'type': 'str'},
-        'description': {'key': 'description', 'type': 'str'},
-        'actions_required': {'key': 'actionsRequired', 'type': 'str'},
+        "status": {"key": "status", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "actions_required": {"key": "actionsRequired", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        status: Union[str, "PrivateLinkServiceConnectionStatus"],
+        status: Union[str, "_models.PrivateLinkServiceConnectionStatus"],
         description: str,
         actions_required: Optional[str] = None,
         **kwargs
     ):
         """
-        :keyword status: Required. The status of a private endpoint connection. Possible values
-         include: "Pending", "Approved", "Rejected", "Disconnected".
+        :keyword status: The status of a private endpoint connection. Required. Known values are:
+         "Pending", "Approved", "Rejected", and "Disconnected".
         :paramtype status: str or
          ~azure.mgmt.iothubprovisioningservices.models.PrivateLinkServiceConnectionStatus
-        :keyword description: Required. The description for the current state of a private endpoint
-         connection.
+        :keyword description: The description for the current state of a private endpoint connection.
+         Required.
         :paramtype description: str
         :keyword actions_required: Actions required for a private endpoint connection.
         :paramtype actions_required: str
         """
-        super(PrivateLinkServiceConnectionState, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.status = status
         self.description = description
         self.actions_required = actions_required
 
 
-class Resource(msrest.serialization.Model):
+class Resource(_serialization.Model):
     """The common properties of an Azure resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: The resource identifier.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
-    :ivar location: Required. The resource location.
+    :ivar location: The resource location. Required.
     :vartype location: str
-    :ivar tags: A set of tags. The resource tags.
+    :ivar tags: The resource tags.
     :vartype tags: dict[str, str]
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True, 'pattern': r'^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$'},
-        'type': {'readonly': True},
-        'location': {'required': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True, "pattern": r"^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$"},
+        "type": {"readonly": True},
+        "location": {"required": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'location': {'key': 'location', 'type': 'str'},
-        'tags': {'key': 'tags', 'type': '{str}'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "location": {"key": "location", "type": "str"},
+        "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(
-        self,
-        *,
-        location: str,
-        tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs):
         """
-        :keyword location: Required. The resource location.
+        :keyword location: The resource location. Required.
         :paramtype location: str
-        :keyword tags: A set of tags. The resource tags.
+        :keyword tags: The resource tags.
         :paramtype tags: dict[str, str]
         """
-        super(Resource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.location = location
         self.tags = tags
 
 
@@ -1179,332 +1101,317 @@
 
     :ivar id: The resource identifier.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
-    :ivar location: Required. The resource location.
+    :ivar location: The resource location. Required.
     :vartype location: str
-    :ivar tags: A set of tags. The resource tags.
+    :ivar tags: The resource tags.
     :vartype tags: dict[str, str]
     :ivar etag: The Etag field is *not* required. If it is provided in the response body, it must
      also be provided as a header per the normal ETag convention.
     :vartype etag: str
-    :ivar properties: Required. Service specific properties for a provisioning service.
+    :ivar properties: Service specific properties for a provisioning service. Required.
     :vartype properties: ~azure.mgmt.iothubprovisioningservices.models.IotDpsPropertiesDescription
-    :ivar sku: Required. Sku info for a provisioning Service.
+    :ivar sku: Sku info for a provisioning Service. Required.
     :vartype sku: ~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuInfo
     :ivar system_data: Metadata pertaining to creation and last modification of the resource.
     :vartype system_data: ~azure.mgmt.iothubprovisioningservices.models.SystemData
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True, 'pattern': r'^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$'},
-        'type': {'readonly': True},
-        'location': {'required': True},
-        'properties': {'required': True},
-        'sku': {'required': True},
-        'system_data': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True, "pattern": r"^(?![0-9]+$)(?!-)[a-zA-Z0-9-]{2,49}[a-zA-Z0-9]$"},
+        "type": {"readonly": True},
+        "location": {"required": True},
+        "properties": {"required": True},
+        "sku": {"required": True},
+        "system_data": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'location': {'key': 'location', 'type': 'str'},
-        'tags': {'key': 'tags', 'type': '{str}'},
-        'etag': {'key': 'etag', 'type': 'str'},
-        'properties': {'key': 'properties', 'type': 'IotDpsPropertiesDescription'},
-        'sku': {'key': 'sku', 'type': 'IotDpsSkuInfo'},
-        'system_data': {'key': 'systemData', 'type': 'SystemData'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "location": {"key": "location", "type": "str"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "etag": {"key": "etag", "type": "str"},
+        "properties": {"key": "properties", "type": "IotDpsPropertiesDescription"},
+        "sku": {"key": "sku", "type": "IotDpsSkuInfo"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
     }
 
     def __init__(
         self,
         *,
         location: str,
-        properties: "IotDpsPropertiesDescription",
-        sku: "IotDpsSkuInfo",
+        properties: "_models.IotDpsPropertiesDescription",
+        sku: "_models.IotDpsSkuInfo",
         tags: Optional[Dict[str, str]] = None,
         etag: Optional[str] = None,
         **kwargs
     ):
         """
-        :keyword location: Required. The resource location.
+        :keyword location: The resource location. Required.
         :paramtype location: str
-        :keyword tags: A set of tags. The resource tags.
+        :keyword tags: The resource tags.
         :paramtype tags: dict[str, str]
         :keyword etag: The Etag field is *not* required. If it is provided in the response body, it
          must also be provided as a header per the normal ETag convention.
         :paramtype etag: str
-        :keyword properties: Required. Service specific properties for a provisioning service.
+        :keyword properties: Service specific properties for a provisioning service. Required.
         :paramtype properties:
          ~azure.mgmt.iothubprovisioningservices.models.IotDpsPropertiesDescription
-        :keyword sku: Required. Sku info for a provisioning Service.
+        :keyword sku: Sku info for a provisioning Service. Required.
         :paramtype sku: ~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuInfo
         """
-        super(ProvisioningServiceDescription, self).__init__(location=location, tags=tags, **kwargs)
+        super().__init__(location=location, tags=tags, **kwargs)
         self.etag = etag
         self.properties = properties
         self.sku = sku
         self.system_data = None
 
 
-class ProvisioningServiceDescriptionListResult(msrest.serialization.Model):
+class ProvisioningServiceDescriptionListResult(_serialization.Model):
     """List of provisioning service descriptions.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: List of provisioning service descriptions.
     :vartype value:
      list[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
     :ivar next_link: the next link.
     :vartype next_link: str
     """
 
     _validation = {
-        'next_link': {'readonly': True},
+        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[ProvisioningServiceDescription]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[ProvisioningServiceDescription]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        value: Optional[List["ProvisioningServiceDescription"]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, value: Optional[List["_models.ProvisioningServiceDescription"]] = None, **kwargs):
         """
         :keyword value: List of provisioning service descriptions.
         :paramtype value:
          list[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
         """
-        super(ProvisioningServiceDescriptionListResult, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
-class SharedAccessSignatureAuthorizationRuleAccessRightsDescription(msrest.serialization.Model):
+class SharedAccessSignatureAuthorizationRuleAccessRightsDescription(_serialization.Model):
     """Description of the shared access key.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar key_name: Required. Name of the key.
+    :ivar key_name: Name of the key. Required.
     :vartype key_name: str
     :ivar primary_key: Primary SAS key value.
     :vartype primary_key: str
     :ivar secondary_key: Secondary SAS key value.
     :vartype secondary_key: str
-    :ivar rights: Required. Rights that this key has. Possible values include: "ServiceConfig",
-     "EnrollmentRead", "EnrollmentWrite", "DeviceConnect", "RegistrationStatusRead",
+    :ivar rights: Rights that this key has. Required. Known values are: "ServiceConfig",
+     "EnrollmentRead", "EnrollmentWrite", "DeviceConnect", "RegistrationStatusRead", and
      "RegistrationStatusWrite".
     :vartype rights: str or ~azure.mgmt.iothubprovisioningservices.models.AccessRightsDescription
     """
 
     _validation = {
-        'key_name': {'required': True},
-        'rights': {'required': True},
+        "key_name": {"required": True},
+        "rights": {"required": True},
     }
 
     _attribute_map = {
-        'key_name': {'key': 'keyName', 'type': 'str'},
-        'primary_key': {'key': 'primaryKey', 'type': 'str'},
-        'secondary_key': {'key': 'secondaryKey', 'type': 'str'},
-        'rights': {'key': 'rights', 'type': 'str'},
+        "key_name": {"key": "keyName", "type": "str"},
+        "primary_key": {"key": "primaryKey", "type": "str"},
+        "secondary_key": {"key": "secondaryKey", "type": "str"},
+        "rights": {"key": "rights", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         key_name: str,
-        rights: Union[str, "AccessRightsDescription"],
+        rights: Union[str, "_models.AccessRightsDescription"],
         primary_key: Optional[str] = None,
         secondary_key: Optional[str] = None,
         **kwargs
     ):
         """
-        :keyword key_name: Required. Name of the key.
+        :keyword key_name: Name of the key. Required.
         :paramtype key_name: str
         :keyword primary_key: Primary SAS key value.
         :paramtype primary_key: str
         :keyword secondary_key: Secondary SAS key value.
         :paramtype secondary_key: str
-        :keyword rights: Required. Rights that this key has. Possible values include: "ServiceConfig",
-         "EnrollmentRead", "EnrollmentWrite", "DeviceConnect", "RegistrationStatusRead",
+        :keyword rights: Rights that this key has. Required. Known values are: "ServiceConfig",
+         "EnrollmentRead", "EnrollmentWrite", "DeviceConnect", "RegistrationStatusRead", and
          "RegistrationStatusWrite".
         :paramtype rights: str or ~azure.mgmt.iothubprovisioningservices.models.AccessRightsDescription
         """
-        super(SharedAccessSignatureAuthorizationRuleAccessRightsDescription, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.key_name = key_name
         self.primary_key = primary_key
         self.secondary_key = secondary_key
         self.rights = rights
 
 
-class SharedAccessSignatureAuthorizationRuleListResult(msrest.serialization.Model):
+class SharedAccessSignatureAuthorizationRuleListResult(_serialization.Model):
     """List of shared access keys.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: The list of shared access policies.
     :vartype value:
      list[~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription]
     :ivar next_link: The next link.
     :vartype next_link: str
     """
 
     _validation = {
-        'next_link': {'readonly': True},
+        "next_link": {"readonly": True},
     }
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[SharedAccessSignatureAuthorizationRuleAccessRightsDescription]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[SharedAccessSignatureAuthorizationRuleAccessRightsDescription]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        value: Optional[List["SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]] = None,
+        value: Optional[List["_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]] = None,
         **kwargs
     ):
         """
         :keyword value: The list of shared access policies.
         :paramtype value:
          list[~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription]
         """
-        super(SharedAccessSignatureAuthorizationRuleListResult, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
-class SystemData(msrest.serialization.Model):
+class SystemData(_serialization.Model):
     """Metadata pertaining to creation and last modification of the resource.
 
     :ivar created_by: The identity that created the resource.
     :vartype created_by: str
-    :ivar created_by_type: The type of identity that created the resource. Possible values include:
-     "User", "Application", "ManagedIdentity", "Key".
+    :ivar created_by_type: The type of identity that created the resource. Known values are:
+     "User", "Application", "ManagedIdentity", and "Key".
     :vartype created_by_type: str or ~azure.mgmt.iothubprovisioningservices.models.CreatedByType
     :ivar created_at: The timestamp of resource creation (UTC).
     :vartype created_at: ~datetime.datetime
     :ivar last_modified_by: The identity that last modified the resource.
     :vartype last_modified_by: str
-    :ivar last_modified_by_type: The type of identity that last modified the resource. Possible
-     values include: "User", "Application", "ManagedIdentity", "Key".
+    :ivar last_modified_by_type: The type of identity that last modified the resource. Known values
+     are: "User", "Application", "ManagedIdentity", and "Key".
     :vartype last_modified_by_type: str or
      ~azure.mgmt.iothubprovisioningservices.models.CreatedByType
     :ivar last_modified_at: The timestamp of resource last modification (UTC).
     :vartype last_modified_at: ~datetime.datetime
     """
 
     _attribute_map = {
-        'created_by': {'key': 'createdBy', 'type': 'str'},
-        'created_by_type': {'key': 'createdByType', 'type': 'str'},
-        'created_at': {'key': 'createdAt', 'type': 'iso-8601'},
-        'last_modified_by': {'key': 'lastModifiedBy', 'type': 'str'},
-        'last_modified_by_type': {'key': 'lastModifiedByType', 'type': 'str'},
-        'last_modified_at': {'key': 'lastModifiedAt', 'type': 'iso-8601'},
+        "created_by": {"key": "createdBy", "type": "str"},
+        "created_by_type": {"key": "createdByType", "type": "str"},
+        "created_at": {"key": "createdAt", "type": "iso-8601"},
+        "last_modified_by": {"key": "lastModifiedBy", "type": "str"},
+        "last_modified_by_type": {"key": "lastModifiedByType", "type": "str"},
+        "last_modified_at": {"key": "lastModifiedAt", "type": "iso-8601"},
     }
 
     def __init__(
         self,
         *,
         created_by: Optional[str] = None,
-        created_by_type: Optional[Union[str, "CreatedByType"]] = None,
+        created_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         created_at: Optional[datetime.datetime] = None,
         last_modified_by: Optional[str] = None,
-        last_modified_by_type: Optional[Union[str, "CreatedByType"]] = None,
+        last_modified_by_type: Optional[Union[str, "_models.CreatedByType"]] = None,
         last_modified_at: Optional[datetime.datetime] = None,
         **kwargs
     ):
         """
         :keyword created_by: The identity that created the resource.
         :paramtype created_by: str
-        :keyword created_by_type: The type of identity that created the resource. Possible values
-         include: "User", "Application", "ManagedIdentity", "Key".
+        :keyword created_by_type: The type of identity that created the resource. Known values are:
+         "User", "Application", "ManagedIdentity", and "Key".
         :paramtype created_by_type: str or ~azure.mgmt.iothubprovisioningservices.models.CreatedByType
         :keyword created_at: The timestamp of resource creation (UTC).
         :paramtype created_at: ~datetime.datetime
         :keyword last_modified_by: The identity that last modified the resource.
         :paramtype last_modified_by: str
-        :keyword last_modified_by_type: The type of identity that last modified the resource. Possible
-         values include: "User", "Application", "ManagedIdentity", "Key".
+        :keyword last_modified_by_type: The type of identity that last modified the resource. Known
+         values are: "User", "Application", "ManagedIdentity", and "Key".
         :paramtype last_modified_by_type: str or
          ~azure.mgmt.iothubprovisioningservices.models.CreatedByType
         :keyword last_modified_at: The timestamp of resource last modification (UTC).
         :paramtype last_modified_at: ~datetime.datetime
         """
-        super(SystemData, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.created_by = created_by
         self.created_by_type = created_by_type
         self.created_at = created_at
         self.last_modified_by = last_modified_by
         self.last_modified_by_type = last_modified_by_type
         self.last_modified_at = last_modified_at
 
 
-class TagsResource(msrest.serialization.Model):
+class TagsResource(_serialization.Model):
     """A container holding only the Tags for a resource, allowing the user to update the tags on a Provisioning Service instance.
 
-    :ivar tags: A set of tags. Resource tags.
+    :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     """
 
     _attribute_map = {
-        'tags': {'key': 'tags', 'type': '{str}'},
+        "tags": {"key": "tags", "type": "{str}"},
     }
 
-    def __init__(
-        self,
-        *,
-        tags: Optional[Dict[str, str]] = None,
-        **kwargs
-    ):
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs):
         """
-        :keyword tags: A set of tags. Resource tags.
+        :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         """
-        super(TagsResource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.tags = tags
 
 
-class VerificationCodeRequest(msrest.serialization.Model):
+class VerificationCodeRequest(_serialization.Model):
     """The JSON-serialized leaf certificate.
 
     :ivar certificate: base-64 representation of X509 certificate .cer file or just .pem file
      content.
     :vartype certificate: str
     """
 
     _attribute_map = {
-        'certificate': {'key': 'certificate', 'type': 'str'},
+        "certificate": {"key": "certificate", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        certificate: Optional[str] = None,
-        **kwargs
-    ):
+    def __init__(self, *, certificate: Optional[str] = None, **kwargs):
         """
         :keyword certificate: base-64 representation of X509 certificate .cer file or just .pem file
          content.
         :paramtype certificate: str
         """
-        super(VerificationCodeRequest, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.certificate = certificate
 
 
-class VerificationCodeResponse(msrest.serialization.Model):
+class VerificationCodeResponse(_serialization.Model):
     """Description of the response of the verification code.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar name: Name of certificate.
     :vartype name: str
     :ivar etag: Request etag.
@@ -1515,89 +1422,84 @@
     :vartype type: str
     :ivar properties:
     :vartype properties:
      ~azure.mgmt.iothubprovisioningservices.models.VerificationCodeResponseProperties
     """
 
     _validation = {
-        'name': {'readonly': True},
-        'etag': {'readonly': True},
-        'id': {'readonly': True},
-        'type': {'readonly': True},
+        "name": {"readonly": True},
+        "etag": {"readonly": True},
+        "id": {"readonly": True},
+        "type": {"readonly": True},
     }
 
     _attribute_map = {
-        'name': {'key': 'name', 'type': 'str'},
-        'etag': {'key': 'etag', 'type': 'str'},
-        'id': {'key': 'id', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'properties': {'key': 'properties', 'type': 'VerificationCodeResponseProperties'},
+        "name": {"key": "name", "type": "str"},
+        "etag": {"key": "etag", "type": "str"},
+        "id": {"key": "id", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "properties": {"key": "properties", "type": "VerificationCodeResponseProperties"},
     }
 
-    def __init__(
-        self,
-        *,
-        properties: Optional["VerificationCodeResponseProperties"] = None,
-        **kwargs
-    ):
+    def __init__(self, *, properties: Optional["_models.VerificationCodeResponseProperties"] = None, **kwargs):
         """
         :keyword properties:
         :paramtype properties:
          ~azure.mgmt.iothubprovisioningservices.models.VerificationCodeResponseProperties
         """
-        super(VerificationCodeResponse, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.name = None
         self.etag = None
         self.id = None
         self.type = None
         self.properties = properties
 
 
-class VerificationCodeResponseProperties(msrest.serialization.Model):
+class VerificationCodeResponseProperties(_serialization.Model):
     """VerificationCodeResponseProperties.
 
     :ivar verification_code: Verification code.
     :vartype verification_code: str
     :ivar subject: Certificate subject.
     :vartype subject: str
     :ivar expiry: Code expiry.
     :vartype expiry: str
     :ivar thumbprint: Certificate thumbprint.
     :vartype thumbprint: str
     :ivar is_verified: Indicate if the certificate is verified by owner of private key.
     :vartype is_verified: bool
     :ivar certificate: base-64 representation of X509 certificate .cer file or just .pem file
      content.
-    :vartype certificate: bytearray
+    :vartype certificate: bytes
     :ivar created: Certificate created time.
     :vartype created: str
     :ivar updated: Certificate updated time.
     :vartype updated: str
     """
 
     _attribute_map = {
-        'verification_code': {'key': 'verificationCode', 'type': 'str'},
-        'subject': {'key': 'subject', 'type': 'str'},
-        'expiry': {'key': 'expiry', 'type': 'str'},
-        'thumbprint': {'key': 'thumbprint', 'type': 'str'},
-        'is_verified': {'key': 'isVerified', 'type': 'bool'},
-        'certificate': {'key': 'certificate', 'type': 'bytearray'},
-        'created': {'key': 'created', 'type': 'str'},
-        'updated': {'key': 'updated', 'type': 'str'},
+        "verification_code": {"key": "verificationCode", "type": "str"},
+        "subject": {"key": "subject", "type": "str"},
+        "expiry": {"key": "expiry", "type": "str"},
+        "thumbprint": {"key": "thumbprint", "type": "str"},
+        "is_verified": {"key": "isVerified", "type": "bool"},
+        "certificate": {"key": "certificate", "type": "bytearray"},
+        "created": {"key": "created", "type": "str"},
+        "updated": {"key": "updated", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         verification_code: Optional[str] = None,
         subject: Optional[str] = None,
         expiry: Optional[str] = None,
         thumbprint: Optional[str] = None,
         is_verified: Optional[bool] = None,
-        certificate: Optional[bytearray] = None,
+        certificate: Optional[bytes] = None,
         created: Optional[str] = None,
         updated: Optional[str] = None,
         **kwargs
     ):
         """
         :keyword verification_code: Verification code.
         :paramtype verification_code: str
@@ -1607,21 +1509,21 @@
         :paramtype expiry: str
         :keyword thumbprint: Certificate thumbprint.
         :paramtype thumbprint: str
         :keyword is_verified: Indicate if the certificate is verified by owner of private key.
         :paramtype is_verified: bool
         :keyword certificate: base-64 representation of X509 certificate .cer file or just .pem file
          content.
-        :paramtype certificate: bytearray
+        :paramtype certificate: bytes
         :keyword created: Certificate created time.
         :paramtype created: str
         :keyword updated: Certificate updated time.
         :paramtype updated: str
         """
-        super(VerificationCodeResponseProperties, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.verification_code = verification_code
         self.subject = subject
         self.expiry = expiry
         self.thumbprint = thumbprint
         self.is_verified = is_verified
         self.certificate = certificate
         self.created = created
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/__init__.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ._models_py3 import AsyncOperationResult
 from ._models_py3 import CertificateBodyDescription
 from ._models_py3 import CertificateListDescription
 from ._models_py3 import CertificateProperties
 from ._models_py3 import CertificateResponse
 from ._models_py3 import ErrorDetails
-from ._models_py3 import ErrorMesssage
+from ._models_py3 import ErrorMessage
 from ._models_py3 import GroupIdInformation
 from ._models_py3 import GroupIdInformationProperties
 from ._models_py3 import IotDpsPropertiesDescription
 from ._models_py3 import IotDpsSkuDefinition
 from ._models_py3 import IotDpsSkuDefinitionListResult
 from ._models_py3 import IotDpsSkuInfo
 from ._models_py3 import IotHubDefinitionDescription
@@ -38,70 +38,72 @@
 from ._models_py3 import SharedAccessSignatureAuthorizationRuleListResult
 from ._models_py3 import SystemData
 from ._models_py3 import TagsResource
 from ._models_py3 import VerificationCodeRequest
 from ._models_py3 import VerificationCodeResponse
 from ._models_py3 import VerificationCodeResponseProperties
 
-
-from ._iot_dps_client_enums import (
-    AccessRightsDescription,
-    AllocationPolicy,
-    CertificatePurpose,
-    CreatedByType,
-    IotDpsSku,
-    IpFilterActionType,
-    IpFilterTargetType,
-    NameUnavailabilityReason,
-    PrivateLinkServiceConnectionStatus,
-    PublicNetworkAccess,
-    State,
-)
+from ._iot_dps_client_enums import AccessRightsDescription
+from ._iot_dps_client_enums import AllocationPolicy
+from ._iot_dps_client_enums import CertificatePurpose
+from ._iot_dps_client_enums import CreatedByType
+from ._iot_dps_client_enums import IotDpsSku
+from ._iot_dps_client_enums import IpFilterActionType
+from ._iot_dps_client_enums import IpFilterTargetType
+from ._iot_dps_client_enums import NameUnavailabilityReason
+from ._iot_dps_client_enums import PrivateLinkServiceConnectionStatus
+from ._iot_dps_client_enums import PublicNetworkAccess
+from ._iot_dps_client_enums import State
+from ._patch import __all__ as _patch_all
+from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    'AsyncOperationResult',
-    'CertificateBodyDescription',
-    'CertificateListDescription',
-    'CertificateProperties',
-    'CertificateResponse',
-    'ErrorDetails',
-    'ErrorMesssage',
-    'GroupIdInformation',
-    'GroupIdInformationProperties',
-    'IotDpsPropertiesDescription',
-    'IotDpsSkuDefinition',
-    'IotDpsSkuDefinitionListResult',
-    'IotDpsSkuInfo',
-    'IotHubDefinitionDescription',
-    'IpFilterRule',
-    'NameAvailabilityInfo',
-    'Operation',
-    'OperationDisplay',
-    'OperationInputs',
-    'OperationListResult',
-    'PrivateEndpoint',
-    'PrivateEndpointConnection',
-    'PrivateEndpointConnectionProperties',
-    'PrivateLinkResources',
-    'PrivateLinkServiceConnectionState',
-    'ProvisioningServiceDescription',
-    'ProvisioningServiceDescriptionListResult',
-    'Resource',
-    'SharedAccessSignatureAuthorizationRuleAccessRightsDescription',
-    'SharedAccessSignatureAuthorizationRuleListResult',
-    'SystemData',
-    'TagsResource',
-    'VerificationCodeRequest',
-    'VerificationCodeResponse',
-    'VerificationCodeResponseProperties',
-    'AccessRightsDescription',
-    'AllocationPolicy',
-    'CertificatePurpose',
-    'CreatedByType',
-    'IotDpsSku',
-    'IpFilterActionType',
-    'IpFilterTargetType',
-    'NameUnavailabilityReason',
-    'PrivateLinkServiceConnectionStatus',
-    'PublicNetworkAccess',
-    'State',
+    "AsyncOperationResult",
+    "CertificateBodyDescription",
+    "CertificateListDescription",
+    "CertificateProperties",
+    "CertificateResponse",
+    "ErrorDetails",
+    "ErrorMessage",
+    "GroupIdInformation",
+    "GroupIdInformationProperties",
+    "IotDpsPropertiesDescription",
+    "IotDpsSkuDefinition",
+    "IotDpsSkuDefinitionListResult",
+    "IotDpsSkuInfo",
+    "IotHubDefinitionDescription",
+    "IpFilterRule",
+    "NameAvailabilityInfo",
+    "Operation",
+    "OperationDisplay",
+    "OperationInputs",
+    "OperationListResult",
+    "PrivateEndpoint",
+    "PrivateEndpointConnection",
+    "PrivateEndpointConnectionProperties",
+    "PrivateLinkResources",
+    "PrivateLinkServiceConnectionState",
+    "ProvisioningServiceDescription",
+    "ProvisioningServiceDescriptionListResult",
+    "Resource",
+    "SharedAccessSignatureAuthorizationRuleAccessRightsDescription",
+    "SharedAccessSignatureAuthorizationRuleListResult",
+    "SystemData",
+    "TagsResource",
+    "VerificationCodeRequest",
+    "VerificationCodeResponse",
+    "VerificationCodeResponseProperties",
+    "AccessRightsDescription",
+    "AllocationPolicy",
+    "CertificatePurpose",
+    "CreatedByType",
+    "IotDpsSku",
+    "IpFilterActionType",
+    "IpFilterTargetType",
+    "NameUnavailabilityReason",
+    "PrivateLinkServiceConnectionStatus",
+    "PublicNetworkAccess",
+    "State",
 ]
+__all__.extend([p for p in _patch_all if p not in __all__])
+_patch_sdk()
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/models/_iot_dps_client_enums.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/models/_iot_dps_client_enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,98 +3,98 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
-from six import with_metaclass
 from azure.core import CaseInsensitiveEnumMeta
 
 
-class AccessRightsDescription(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """Rights that this key has.
-    """
+class AccessRightsDescription(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Rights that this key has."""
 
     SERVICE_CONFIG = "ServiceConfig"
     ENROLLMENT_READ = "EnrollmentRead"
     ENROLLMENT_WRITE = "EnrollmentWrite"
     DEVICE_CONNECT = "DeviceConnect"
     REGISTRATION_STATUS_READ = "RegistrationStatusRead"
     REGISTRATION_STATUS_WRITE = "RegistrationStatusWrite"
 
-class AllocationPolicy(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """Allocation policy to be used by this provisioning service.
-    """
+
+class AllocationPolicy(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Allocation policy to be used by this provisioning service."""
 
     HASHED = "Hashed"
     GEO_LATENCY = "GeoLatency"
     STATIC = "Static"
 
-class CertificatePurpose(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
+
+class CertificatePurpose(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """CertificatePurpose."""
 
     CLIENT_AUTHENTICATION = "clientAuthentication"
     SERVER_AUTHENTICATION = "serverAuthentication"
 
-class CreatedByType(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """The type of identity that created the resource.
-    """
+
+class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
 
-class IotDpsSku(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """Sku name.
-    """
+
+class IotDpsSku(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Sku name."""
 
     S1 = "S1"
 
-class IpFilterActionType(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """The desired action for requests captured by this rule.
-    """
+
+class IpFilterActionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The desired action for requests captured by this rule."""
 
     ACCEPT = "Accept"
     REJECT = "Reject"
 
-class IpFilterTargetType(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """Target for requests captured by this rule.
-    """
+
+class IpFilterTargetType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Target for requests captured by this rule."""
 
     ALL = "all"
     SERVICE_API = "serviceApi"
     DEVICE_API = "deviceApi"
 
-class NameUnavailabilityReason(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """specifies the reason a name is unavailable
-    """
+
+class NameUnavailabilityReason(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """specifies the reason a name is unavailable."""
 
     INVALID = "Invalid"
     ALREADY_EXISTS = "AlreadyExists"
 
-class PrivateLinkServiceConnectionStatus(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """The status of a private endpoint connection
-    """
+
+class PrivateLinkServiceConnectionStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The status of a private endpoint connection."""
 
     PENDING = "Pending"
     APPROVED = "Approved"
     REJECTED = "Rejected"
     DISCONNECTED = "Disconnected"
 
-class PublicNetworkAccess(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """Whether requests from Public Network are allowed
-    """
+
+class PublicNetworkAccess(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Whether requests from Public Network are allowed."""
 
     ENABLED = "Enabled"
     DISABLED = "Disabled"
 
-class State(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
-    """Current state of the provisioning service.
-    """
+
+class State(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Current state of the provisioning service."""
 
     ACTIVATING = "Activating"
     ACTIVE = "Active"
     DELETING = "Deleting"
     DELETED = "Deleted"
     ACTIVATION_FAILED = "ActivationFailed"
     DELETION_FAILED = "DeletionFailed"
```

## Comparing `azure-mgmt-iothubprovisioningservices-1.1.0/azure/mgmt/iothubprovisioningservices/operations/_iot_dps_resource_operations.py` & `azure-mgmt-iothubprovisioningservices-1.2.0b1/azure/mgmt/iothubprovisioningservices/operations/_iot_dps_resource_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,2041 +1,2566 @@
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-import functools
-from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, TypeVar, Union
-import warnings
-
-from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, List, Optional, TypeVar, Union, cast, overload
+import urllib.parse
+
+from azure.core.exceptions import (
+    ClientAuthenticationError,
+    HttpResponseError,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    ResourceNotModifiedError,
+    map_error,
+)
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
-from msrest import Serializer
 
 from .. import models as _models
+from .._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
-T = TypeVar('T')
-JSONType = Any
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
+
 def build_get_request(
-    provisioning_service_name: str,
-    subscription_id: str,
-    resource_group_name: str,
-    **kwargs: Any
+    provisioning_service_name: str, resource_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_create_or_update_request_initial(
-    subscription_id: str,
-    resource_group_name: str,
-    provisioning_service_name: str,
-    *,
-    json: JSONType = None,
-    content: Any = None,
-    **kwargs: Any
+def build_create_or_update_request(
+    resource_group_name: str, provisioning_service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    content_type = kwargs.pop('content_type', None)  # type: Optional[str]
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    accept = _headers.pop("Accept", "application/json")
 
-    api_version = "2021-10-15"
-    accept = "application/json"
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
     if content_type is not None:
-        header_parameters['Content-Type'] = _SERIALIZER.header("content_type", content_type, 'str')
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="PUT",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        json=json,
-        content=content,
-        **kwargs
-    )
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_update_request_initial(
-    subscription_id: str,
-    resource_group_name: str,
-    provisioning_service_name: str,
-    *,
-    json: JSONType = None,
-    content: Any = None,
-    **kwargs: Any
+def build_update_request(
+    resource_group_name: str, provisioning_service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    content_type = kwargs.pop('content_type', None)  # type: Optional[str]
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    accept = _headers.pop("Accept", "application/json")
 
-    api_version = "2021-10-15"
-    accept = "application/json"
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
     if content_type is not None:
-        header_parameters['Content-Type'] = _SERIALIZER.header("content_type", content_type, 'str')
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="PATCH",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        json=json,
-        content=content,
-        **kwargs
-    )
+    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_delete_request_initial(
-    provisioning_service_name: str,
-    subscription_id: str,
-    resource_group_name: str,
-    **kwargs: Any
+def build_delete_request(
+    provisioning_service_name: str, resource_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="DELETE",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_by_subscription_request(
-    subscription_id: str,
-    **kwargs: Any
-) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/providers/Microsoft.Devices/provisioningServices')
+    _url = kwargs.pop(
+        "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Devices/provisioningServices"
+    )
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_by_resource_group_request(
-    subscription_id: str,
-    resource_group_name: str,
-    **kwargs: Any
-) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_operation_result_request(
     operation_id: str,
-    subscription_id: str,
     resource_group_name: str,
     provisioning_service_name: str,
+    subscription_id: str,
     *,
     asyncinfo: str = "true",
     **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/operationresults/{operationId}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/operationresults/{operationId}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "operationId": _SERIALIZER.url("operation_id", operation_id, 'str'),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
+        "operationId": _SERIALIZER.url("operation_id", operation_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['asyncinfo'] = _SERIALIZER.query("asyncinfo", asyncinfo, 'str')
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["asyncinfo"] = _SERIALIZER.query("asyncinfo", asyncinfo, "str")
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_valid_skus_request(
-    provisioning_service_name: str,
-    subscription_id: str,
-    resource_group_name: str,
-    **kwargs: Any
+    provisioning_service_name: str, resource_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/skus')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/skus",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_check_provisioning_service_name_availability_request(
-    subscription_id: str,
-    *,
-    json: JSONType = None,
-    content: Any = None,
-    **kwargs: Any
-) -> HttpRequest:
-    content_type = kwargs.pop('content_type', None)  # type: Optional[str]
+def build_check_provisioning_service_name_availability_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    accept = _headers.pop("Accept", "application/json")
 
-    api_version = "2021-10-15"
-    accept = "application/json"
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/providers/Microsoft.Devices/checkProvisioningServiceNameAvailability')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/providers/Microsoft.Devices/checkProvisioningServiceNameAvailability",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
     if content_type is not None:
-        header_parameters['Content-Type'] = _SERIALIZER.header("content_type", content_type, 'str')
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="POST",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        json=json,
-        content=content,
-        **kwargs
-    )
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_keys_request(
-    provisioning_service_name: str,
-    subscription_id: str,
-    resource_group_name: str,
-    **kwargs: Any
+    provisioning_service_name: str, resource_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/listkeys')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/listkeys",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="POST",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_keys_for_key_name_request(
-    provisioning_service_name: str,
-    key_name: str,
-    subscription_id: str,
-    resource_group_name: str,
-    **kwargs: Any
+    provisioning_service_name: str, key_name: str, resource_group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/keys/{keyName}/listkeys')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/keys/{keyName}/listkeys",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, 'str'),
-        "keyName": _SERIALIZER.url("key_name", key_name, 'str'),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "provisioningServiceName": _SERIALIZER.url("provisioning_service_name", provisioning_service_name, "str"),
+        "keyName": _SERIALIZER.url("key_name", key_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="POST",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_private_link_resources_request(
-    subscription_id: str,
-    resource_group_name: str,
-    resource_name: str,
-    **kwargs: Any
+    resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_private_link_resources_request(
-    subscription_id: str,
-    resource_group_name: str,
-    resource_name: str,
-    group_id: str,
-    **kwargs: Any
+    resource_group_name: str, resource_name: str, group_id: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources/{groupId}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources/{groupId}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, 'str'),
-        "groupId": _SERIALIZER.url("group_id", group_id, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "groupId": _SERIALIZER.url("group_id", group_id, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_private_endpoint_connections_request(
-    subscription_id: str,
-    resource_group_name: str,
-    resource_name: str,
-    **kwargs: Any
+    resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_private_endpoint_connection_request(
-    subscription_id: str,
     resource_group_name: str,
     resource_name: str,
     private_endpoint_connection_name: str,
+    subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, 'str'),
-        "privateEndpointConnectionName": _SERIALIZER.url("private_endpoint_connection_name", private_endpoint_connection_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
+        ),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="GET",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_create_or_update_private_endpoint_connection_request_initial(
-    subscription_id: str,
+def build_create_or_update_private_endpoint_connection_request(
     resource_group_name: str,
     resource_name: str,
     private_endpoint_connection_name: str,
-    *,
-    json: JSONType = None,
-    content: Any = None,
+    subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
-    content_type = kwargs.pop('content_type', None)  # type: Optional[str]
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+    accept = _headers.pop("Accept", "application/json")
 
-    api_version = "2021-10-15"
-    accept = "application/json"
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, 'str'),
-        "privateEndpointConnectionName": _SERIALIZER.url("private_endpoint_connection_name", private_endpoint_connection_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
+        ),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
     if content_type is not None:
-        header_parameters['Content-Type'] = _SERIALIZER.header("content_type", content_type, 'str')
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="PUT",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        json=json,
-        content=content,
-        **kwargs
-    )
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_delete_private_endpoint_connection_request_initial(
-    subscription_id: str,
+def build_delete_private_endpoint_connection_request(
     resource_group_name: str,
     resource_name: str,
     private_endpoint_connection_name: str,
+    subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
-    api_version = "2021-10-15"
-    accept = "application/json"
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-05"))  # type: Literal["2022-02-05"]
+    accept = _headers.pop("Accept", "application/json")
+
     # Construct URL
-    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}')
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, 'str'),
-        "privateEndpointConnectionName": _SERIALIZER.url("private_endpoint_connection_name", private_endpoint_connection_name, 'str'),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
+        ),
     }
 
-    url = _format_url_section(url, **path_format_arguments)
+    _url = _format_url_section(_url, **path_format_arguments)
 
     # Construct parameters
-    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
-    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
-    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(
-        method="DELETE",
-        url=url,
-        params=query_parameters,
-        headers=header_parameters,
-        **kwargs
-    )
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
-class IotDpsResourceOperations(object):
-    """IotDpsResourceOperations operations.
 
-    You should not instantiate this class directly. Instead, you should create a Client instance that
-    instantiates it for you and attaches it as an attribute.
+class IotDpsResourceOperations:  # pylint: disable=too-many-public-methods
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
 
-    :ivar models: Alias to model classes used in this operation group.
-    :type models: ~azure.mgmt.iothubprovisioningservices.models
-    :param client: Client for service requests.
-    :param config: Configuration of service client.
-    :param serializer: An object model serializer.
-    :param deserializer: An object model deserializer.
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.iothubprovisioningservices.IotDpsClient`'s
+        :attr:`iot_dps_resource` attribute.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer):
-        self._client = client
-        self._serialize = serializer
-        self._deserialize = deserializer
-        self._config = config
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def get(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> "_models.ProvisioningServiceDescription":
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
+    ) -> _models.ProvisioningServiceDescription:
         """Get the non-security related metadata of the provisioning service.
 
         Get the metadata of the provisioning service without SAS keys.
 
-        :param provisioning_service_name: Name of the provisioning service to retrieve.
+        :param provisioning_service_name: Name of the provisioning service to retrieve. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: Resource group name.
+        :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ProvisioningServiceDescription, or the result of cls(response)
+        :return: ProvisioningServiceDescription or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
 
-        
         request = build_get_request(
             provisioning_service_name=provisioning_service_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
-            template_url=self.get.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+        deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
-
+    get.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        iot_dps_description: "_models.ProvisioningServiceDescription",
+        iot_dps_description: Union[_models.ProvisioningServiceDescription, IO],
         **kwargs: Any
-    ) -> "_models.ProvisioningServiceDescription":
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
+    ) -> _models.ProvisioningServiceDescription:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(iot_dps_description, 'ProvisioningServiceDescription')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(iot_dps_description, (IO, bytes)):
+            _content = iot_dps_description
+        else:
+            _json = self._serialize.body(iot_dps_description, "ProvisioningServiceDescription")
 
-        request = build_create_or_update_request_initial(
-            subscription_id=self._config.subscription_id,
+        request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self._create_or_update_initial.metadata['url'],
+            content=_content,
+            template_url=self._create_or_update_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
-
+    _create_or_update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
-    @distributed_trace
+    @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        iot_dps_description: "_models.ProvisioningServiceDescription",
+        iot_dps_description: _models.ProvisioningServiceDescription,
+        *,
+        content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller["_models.ProvisioningServiceDescription"]:
+    ) -> LROPoller[_models.ProvisioningServiceDescription]:
         """Create or update the metadata of the provisioning service.
 
         Create or update the metadata of the provisioning service. The usual pattern to modify a
         property is to retrieve the provisioning service metadata and security metadata, and then
         combine them with the modified values in a new body to update the provisioning service.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
-        :param provisioning_service_name: Name of provisioning service to create or update.
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
         :type provisioning_service_name: str
         :param iot_dps_description: Description of the provisioning service to create or update.
+         Required.
         :type iot_dps_description:
          ~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either ProvisioningServiceDescription or the
          result of cls(response)
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+
+    @overload
+    def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        iot_dps_description: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.ProvisioningServiceDescription]:
+        """Create or update the metadata of the provisioning service.
+
+        Create or update the metadata of the provisioning service. The usual pattern to modify a
+        property is to retrieve the provisioning service metadata and security metadata, and then
+        combine them with the modified values in a new body to update the provisioning service.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param iot_dps_description: Description of the provisioning service to create or update.
+         Required.
+        :type iot_dps_description: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either ProvisioningServiceDescription or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        iot_dps_description: Union[_models.ProvisioningServiceDescription, IO],
+        **kwargs: Any
+    ) -> LROPoller[_models.ProvisioningServiceDescription]:
+        """Create or update the metadata of the provisioning service.
+
+        Create or update the metadata of the provisioning service. The usual pattern to modify a
+        property is to retrieve the provisioning service metadata and security metadata, and then
+        combine them with the modified values in a new body to update the provisioning service.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param iot_dps_description: Description of the provisioning service to create or update. Is
+         either a model type or a IO type. Required.
+        :type iot_dps_description:
+         ~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either ProvisioningServiceDescription or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = self._create_or_update_initial(
+            raw_result = self._create_or_update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 provisioning_service_name=provisioning_service_name,
                 iot_dps_description=iot_dps_description,
+                api_version=api_version,
                 content_type=content_type,
-                cls=lambda x,y,z: x,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = NoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    begin_create_or_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     def _update_initial(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        provisioning_service_tags: "_models.TagsResource",
+        provisioning_service_tags: Union[_models.TagsResource, IO],
         **kwargs: Any
-    ) -> "_models.ProvisioningServiceDescription":
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
+    ) -> _models.ProvisioningServiceDescription:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(provisioning_service_tags, 'TagsResource')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(provisioning_service_tags, (IO, bytes)):
+            _content = provisioning_service_tags
+        else:
+            _json = self._serialize.body(provisioning_service_tags, "TagsResource")
 
-        request = build_update_request_initial(
-            subscription_id=self._config.subscription_id,
+        request = build_update_request(
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self._update_initial.metadata['url'],
+            content=_content,
+            template_url=self._update_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+        deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    _update_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
+
+    @overload
+    def begin_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        provisioning_service_tags: _models.TagsResource,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.ProvisioningServiceDescription]:
+        """Update an existing provisioning service's tags.
+
+        Update an existing provisioning service's tags. to update other fields use the CreateOrUpdate
+        method.
 
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param provisioning_service_tags: Updated tag information to set into the provisioning service
+         instance. Required.
+        :type provisioning_service_tags: ~azure.mgmt.iothubprovisioningservices.models.TagsResource
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either ProvisioningServiceDescription or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_update(
+        self,
+        resource_group_name: str,
+        provisioning_service_name: str,
+        provisioning_service_tags: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.ProvisioningServiceDescription]:
+        """Update an existing provisioning service's tags.
+
+        Update an existing provisioning service's tags. to update other fields use the CreateOrUpdate
+        method.
+
+        :param resource_group_name: Resource group identifier. Required.
+        :type resource_group_name: str
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
+        :type provisioning_service_name: str
+        :param provisioning_service_tags: Updated tag information to set into the provisioning service
+         instance. Required.
+        :type provisioning_service_tags: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either ProvisioningServiceDescription or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
 
     @distributed_trace
     def begin_update(
         self,
         resource_group_name: str,
         provisioning_service_name: str,
-        provisioning_service_tags: "_models.TagsResource",
+        provisioning_service_tags: Union[_models.TagsResource, IO],
         **kwargs: Any
-    ) -> LROPoller["_models.ProvisioningServiceDescription"]:
+    ) -> LROPoller[_models.ProvisioningServiceDescription]:
         """Update an existing provisioning service's tags.
 
         Update an existing provisioning service's tags. to update other fields use the CreateOrUpdate
         method.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
-        :param provisioning_service_name: Name of provisioning service to create or update.
+        :param provisioning_service_name: Name of provisioning service to create or update. Required.
         :type provisioning_service_name: str
         :param provisioning_service_tags: Updated tag information to set into the provisioning service
-         instance.
-        :type provisioning_service_tags: ~azure.mgmt.iothubprovisioningservices.models.TagsResource
+         instance. Is either a model type or a IO type. Required.
+        :type provisioning_service_tags: ~azure.mgmt.iothubprovisioningservices.models.TagsResource or
+         IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either ProvisioningServiceDescription or the
          result of cls(response)
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescription"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescription]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = self._update_initial(
+            raw_result = self._update_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 provisioning_service_name=provisioning_service_name,
                 provisioning_service_tags=provisioning_service_tags,
+                api_version=api_version,
                 content_type=content_type,
-                cls=lambda x,y,z: x,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('ProvisioningServiceDescription', pipeline_response)
+            deserialized = self._deserialize("ProvisioningServiceDescription", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = NoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    begin_update.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
-    def _delete_initial(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
     ) -> None:
-        cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        
-        request = build_delete_request_initial(
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+
+        request = build_delete_request(
             provisioning_service_name=provisioning_service_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
-            template_url=self._delete_initial.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._delete_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204, 404]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
-
+    _delete_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     @distributed_trace
-    def begin_delete(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> LROPoller[None]:
+    def begin_delete(self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any) -> LROPoller[None]:
         """Delete the Provisioning Service.
 
         Deletes the Provisioning Service.
 
-        :param provisioning_service_name: Name of provisioning service to delete.
+        :param provisioning_service_name: Name of provisioning service to delete. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType[None]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = self._delete_initial(
+            raw_result = self._delete_initial(  # type: ignore
                 provisioning_service_name=provisioning_service_name,
                 resource_group_name=resource_group_name,
-                cls=lambda x,y,z: x,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
-        def get_long_running_output(pipeline_response):
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
-
-        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = NoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}'}  # type: ignore
+    begin_delete.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}"}  # type: ignore
 
     @distributed_trace
-    def list_by_subscription(
-        self,
-        **kwargs: Any
-    ) -> Iterable["_models.ProvisioningServiceDescriptionListResult"]:
+    def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.ProvisioningServiceDescription"]:
         """Get all the provisioning services in a subscription.
 
         List all the provisioning services for a given subscription id.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ProvisioningServiceDescriptionListResult or the
-         result of cls(response)
+        :return: An iterator like instance of either ProvisioningServiceDescription or the result of
+         cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescriptionListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescriptionListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescriptionListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_by_subscription_request(
                     subscription_id=self._config.subscription_id,
-                    template_url=self.list_by_subscription.metadata['url'],
+                    api_version=api_version,
+                    template_url=self.list_by_subscription.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_by_subscription_request(
-                    subscription_id=self._config.subscription_id,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ProvisioningServiceDescriptionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return ItemPaged(get_next, extract_data)
 
-        return ItemPaged(
-            get_next, extract_data
-        )
-    list_by_subscription.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.Devices/provisioningServices'}  # type: ignore
+    list_by_subscription.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Devices/provisioningServices"}  # type: ignore
 
     @distributed_trace
     def list_by_resource_group(
-        self,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> Iterable["_models.ProvisioningServiceDescriptionListResult"]:
+        self, resource_group_name: str, **kwargs: Any
+    ) -> Iterable["_models.ProvisioningServiceDescription"]:
         """Get a list of all provisioning services in the given resource group.
 
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ProvisioningServiceDescriptionListResult or the
-         result of cls(response)
+        :return: An iterator like instance of either ProvisioningServiceDescription or the result of
+         cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescriptionListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.ProvisioningServiceDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.ProvisioningServiceDescriptionListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ProvisioningServiceDescriptionListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_by_resource_group_request(
-                    subscription_id=self._config.subscription_id,
                     resource_group_name=resource_group_name,
-                    template_url=self.list_by_resource_group.metadata['url'],
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_by_resource_group.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_by_resource_group_request(
-                    subscription_id=self._config.subscription_id,
-                    resource_group_name=resource_group_name,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ProvisioningServiceDescriptionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return ItemPaged(get_next, extract_data)
 
-        return ItemPaged(
-            get_next, extract_data
-        )
-    list_by_resource_group.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices'}  # type: ignore
+    list_by_resource_group.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices"}  # type: ignore
 
     @distributed_trace
     def get_operation_result(
         self,
         operation_id: str,
         resource_group_name: str,
         provisioning_service_name: str,
         asyncinfo: str = "true",
         **kwargs: Any
-    ) -> "_models.AsyncOperationResult":
+    ) -> _models.AsyncOperationResult:
         """Gets the status of a long running operation, such as create, update or delete a provisioning
         service.
 
         :param operation_id: Operation id corresponding to long running operation. Use this to poll for
-         the status.
+         the status. Required.
         :type operation_id: str
-        :param resource_group_name: Resource group identifier.
+        :param resource_group_name: Resource group identifier. Required.
         :type resource_group_name: str
         :param provisioning_service_name: Name of provisioning service that the operation is running
-         on.
+         on. Required.
         :type provisioning_service_name: str
         :param asyncinfo: Async header used to poll on the status of the operation, obtained while
-         creating the long running operation.
+         creating the long running operation. Default value is "true".
         :type asyncinfo: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: AsyncOperationResult, or the result of cls(response)
+        :return: AsyncOperationResult or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.AsyncOperationResult
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.AsyncOperationResult"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.AsyncOperationResult]
 
-        
         request = build_get_operation_result_request(
             operation_id=operation_id,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             provisioning_service_name=provisioning_service_name,
+            subscription_id=self._config.subscription_id,
             asyncinfo=asyncinfo,
-            template_url=self.get_operation_result.metadata['url'],
+            api_version=api_version,
+            template_url=self.get_operation_result.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('AsyncOperationResult', pipeline_response)
+        deserialized = self._deserialize("AsyncOperationResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_operation_result.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/operationresults/{operationId}'}  # type: ignore
-
+    get_operation_result.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/operationresults/{operationId}"}  # type: ignore
 
     @distributed_trace
     def list_valid_skus(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> Iterable["_models.IotDpsSkuDefinitionListResult"]:
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
+    ) -> Iterable["_models.IotDpsSkuDefinition"]:
         """Get the list of valid SKUs for a provisioning service.
 
         Gets the list of valid SKUs and tiers for a provisioning service.
 
-        :param provisioning_service_name: Name of provisioning service.
+        :param provisioning_service_name: Name of provisioning service. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: Name of resource group.
+        :param resource_group_name: Name of resource group. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either IotDpsSkuDefinitionListResult or the result of
-         cls(response)
+        :return: An iterator like instance of either IotDpsSkuDefinition or the result of cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuDefinitionListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.IotDpsSkuDefinition]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.IotDpsSkuDefinitionListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.IotDpsSkuDefinitionListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_valid_skus_request(
                     provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
                     resource_group_name=resource_group_name,
-                    template_url=self.list_valid_skus.metadata['url'],
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_valid_skus.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_valid_skus_request(
-                    provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
-                    resource_group_name=resource_group_name,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("IotDpsSkuDefinitionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return ItemPaged(get_next, extract_data)
 
-        return ItemPaged(
-            get_next, extract_data
-        )
-    list_valid_skus.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/skus'}  # type: ignore
+    list_valid_skus.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/skus"}  # type: ignore
 
-    @distributed_trace
+    @overload
     def check_provisioning_service_name_availability(
-        self,
-        arguments: "_models.OperationInputs",
-        **kwargs: Any
-    ) -> "_models.NameAvailabilityInfo":
+        self, arguments: _models.OperationInputs, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.NameAvailabilityInfo:
         """Check if a provisioning service name is available.
 
         Check if a provisioning service name is available. This will validate if the name is
         syntactically valid and if the name is usable.
 
         :param arguments: Set the name parameter in the OperationInputs structure to the name of the
-         provisioning service to check.
+         provisioning service to check. Required.
         :type arguments: ~azure.mgmt.iothubprovisioningservices.models.OperationInputs
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: NameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.NameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def check_provisioning_service_name_availability(
+        self, arguments: IO, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.NameAvailabilityInfo:
+        """Check if a provisioning service name is available.
+
+        Check if a provisioning service name is available. This will validate if the name is
+        syntactically valid and if the name is usable.
+
+        :param arguments: Set the name parameter in the OperationInputs structure to the name of the
+         provisioning service to check. Required.
+        :type arguments: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: NameAvailabilityInfo, or the result of cls(response)
+        :return: NameAvailabilityInfo or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.NameAvailabilityInfo
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def check_provisioning_service_name_availability(
+        self, arguments: Union[_models.OperationInputs, IO], **kwargs: Any
+    ) -> _models.NameAvailabilityInfo:
+        """Check if a provisioning service name is available.
+
+        Check if a provisioning service name is available. This will validate if the name is
+        syntactically valid and if the name is usable.
+
+        :param arguments: Set the name parameter in the OperationInputs structure to the name of the
+         provisioning service to check. Is either a model type or a IO type. Required.
+        :type arguments: ~azure.mgmt.iothubprovisioningservices.models.OperationInputs or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: NameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.iothubprovisioningservices.models.NameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.NameAvailabilityInfo"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(arguments, 'OperationInputs')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.NameAvailabilityInfo]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(arguments, (IO, bytes)):
+            _content = arguments
+        else:
+            _json = self._serialize.body(arguments, "OperationInputs")
 
         request = build_check_provisioning_service_name_availability_request(
             subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self.check_provisioning_service_name_availability.metadata['url'],
+            content=_content,
+            template_url=self.check_provisioning_service_name_availability.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('NameAvailabilityInfo', pipeline_response)
+        deserialized = self._deserialize("NameAvailabilityInfo", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    check_provisioning_service_name_availability.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.Devices/checkProvisioningServiceNameAvailability'}  # type: ignore
-
+    check_provisioning_service_name_availability.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Devices/checkProvisioningServiceNameAvailability"}  # type: ignore
 
     @distributed_trace
     def list_keys(
-        self,
-        provisioning_service_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> Iterable["_models.SharedAccessSignatureAuthorizationRuleListResult"]:
+        self, provisioning_service_name: str, resource_group_name: str, **kwargs: Any
+    ) -> Iterable["_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]:
         """Get the security metadata for a provisioning service.
 
         List the primary and secondary keys for a provisioning service.
 
         :param provisioning_service_name: The provisioning service name to get the shared access keys
-         for.
+         for. Required.
         :type provisioning_service_name: str
-        :param resource_group_name: resource group name.
+        :param resource_group_name: resource group name. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either SharedAccessSignatureAuthorizationRuleListResult
-         or the result of cls(response)
+        :return: An iterator like instance of either
+         SharedAccessSignatureAuthorizationRuleAccessRightsDescription or the result of cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleListResult]
-        :raises: ~azure.core.exceptions.HttpResponseError
+         ~azure.core.paging.ItemPaged[~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.SharedAccessSignatureAuthorizationRuleListResult"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.SharedAccessSignatureAuthorizationRuleListResult]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
         def prepare_request(next_link=None):
             if not next_link:
-                
+
                 request = build_list_keys_request(
                     provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
                     resource_group_name=resource_group_name,
-                    template_url=self.list_keys.metadata['url'],
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    template_url=self.list_keys.metadata["url"],
+                    headers=_headers,
+                    params=_params,
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
 
             else:
-                
-                request = build_list_keys_request(
-                    provisioning_service_name=provisioning_service_name,
-                    subscription_id=self._config.subscription_id,
-                    resource_group_name=resource_group_name,
-                    template_url=next_link,
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                request.url = self._client.format_url(request.url)  # type: ignore
                 request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("SharedAccessSignatureAuthorizationRuleListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+        return ItemPaged(get_next, extract_data)
 
-        return ItemPaged(
-            get_next, extract_data
-        )
-    list_keys.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/listkeys'}  # type: ignore
+    list_keys.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/listkeys"}  # type: ignore
 
     @distributed_trace
     def list_keys_for_key_name(
-        self,
-        provisioning_service_name: str,
-        key_name: str,
-        resource_group_name: str,
-        **kwargs: Any
-    ) -> "_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription":
+        self, provisioning_service_name: str, key_name: str, resource_group_name: str, **kwargs: Any
+    ) -> _models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription:
         """Get a shared access policy by name from a provisioning service.
 
         List primary and secondary keys for a specific key name.
 
-        :param provisioning_service_name: Name of the provisioning service.
+        :param provisioning_service_name: Name of the provisioning service. Required.
         :type provisioning_service_name: str
-        :param key_name: Logical key name to get key-values for.
+        :param key_name: Logical key name to get key-values for. Required.
         :type key_name: str
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: SharedAccessSignatureAuthorizationRuleAccessRightsDescription, or the result of
+        :return: SharedAccessSignatureAuthorizationRuleAccessRightsDescription or the result of
          cls(response)
         :rtype:
          ~azure.mgmt.iothubprovisioningservices.models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop(
+            "cls", None
+        )  # type: ClsType[_models.SharedAccessSignatureAuthorizationRuleAccessRightsDescription]
 
-        
         request = build_list_keys_for_key_name_request(
             provisioning_service_name=provisioning_service_name,
             key_name=key_name,
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
-            template_url=self.list_keys_for_key_name.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_keys_for_key_name.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('SharedAccessSignatureAuthorizationRuleAccessRightsDescription', pipeline_response)
+        deserialized = self._deserialize(
+            "SharedAccessSignatureAuthorizationRuleAccessRightsDescription", pipeline_response
+        )
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_keys_for_key_name.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/keys/{keyName}/listkeys'}  # type: ignore
-
+    list_keys_for_key_name.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{provisioningServiceName}/keys/{keyName}/listkeys"}  # type: ignore
 
     @distributed_trace
     def list_private_link_resources(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        **kwargs: Any
-    ) -> "_models.PrivateLinkResources":
+        self, resource_group_name: str, resource_name: str, **kwargs: Any
+    ) -> _models.PrivateLinkResources:
         """List private link resources.
 
         List private link resources for the given provisioning service.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PrivateLinkResources, or the result of cls(response)
+        :return: PrivateLinkResources or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.PrivateLinkResources
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateLinkResources"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateLinkResources]
 
-        
         request = build_list_private_link_resources_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
-            template_url=self.list_private_link_resources.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_private_link_resources.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('PrivateLinkResources', pipeline_response)
+        deserialized = self._deserialize("PrivateLinkResources", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_private_link_resources.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources'}  # type: ignore
-
+    list_private_link_resources.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources"}  # type: ignore
 
     @distributed_trace
     def get_private_link_resources(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        group_id: str,
-        **kwargs: Any
-    ) -> "_models.GroupIdInformation":
+        self, resource_group_name: str, resource_name: str, group_id: str, **kwargs: Any
+    ) -> _models.GroupIdInformation:
         """Get the specified private link resource.
 
         Get the specified private link resource for the given provisioning service.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param group_id: The name of the private link resource.
+        :param group_id: The name of the private link resource. Required.
         :type group_id: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: GroupIdInformation, or the result of cls(response)
+        :return: GroupIdInformation or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.GroupIdInformation
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.GroupIdInformation"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.GroupIdInformation]
 
-        
         request = build_get_private_link_resources_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             group_id=group_id,
-            template_url=self.get_private_link_resources.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get_private_link_resources.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('GroupIdInformation', pipeline_response)
+        deserialized = self._deserialize("GroupIdInformation", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_private_link_resources.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources/{groupId}'}  # type: ignore
-
+    get_private_link_resources.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateLinkResources/{groupId}"}  # type: ignore
 
     @distributed_trace
     def list_private_endpoint_connections(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        **kwargs: Any
-    ) -> List["_models.PrivateEndpointConnection"]:
+        self, resource_group_name: str, resource_name: str, **kwargs: Any
+    ) -> List[_models.PrivateEndpointConnection]:
         """List private endpoint connections.
 
         List private endpoint connection properties.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: list of PrivateEndpointConnection, or the result of cls(response)
+        :return: list of PrivateEndpointConnection or the result of cls(response)
         :rtype: list[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType[List["_models.PrivateEndpointConnection"]]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[List[_models.PrivateEndpointConnection]]
 
-        
         request = build_list_private_endpoint_connections_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
-            template_url=self.list_private_endpoint_connections.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.list_private_endpoint_connections.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('[PrivateEndpointConnection]', pipeline_response)
+        deserialized = self._deserialize("[PrivateEndpointConnection]", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    list_private_endpoint_connections.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections'}  # type: ignore
-
+    list_private_endpoint_connections.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections"}  # type: ignore
 
     @distributed_trace
     def get_private_endpoint_connection(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        private_endpoint_connection_name: str,
-        **kwargs: Any
-    ) -> "_models.PrivateEndpointConnection":
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> _models.PrivateEndpointConnection:
         """Get private endpoint connection.
 
         Get private endpoint connection properties.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param private_endpoint_connection_name: The name of the private endpoint connection.
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: PrivateEndpointConnection, or the result of cls(response)
+        :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
 
-        
         request = build_get_private_endpoint_connection_request(
-            subscription_id=self._config.subscription_id,
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
-            template_url=self.get_private_endpoint_connection.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self.get_private_endpoint_connection.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+        deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    get_private_endpoint_connection.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
-
+    get_private_endpoint_connection.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
     def _create_or_update_private_endpoint_connection_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
-        private_endpoint_connection: "_models.PrivateEndpointConnection",
+        private_endpoint_connection: Union[_models.PrivateEndpointConnection, IO],
         **kwargs: Any
-    ) -> "_models.PrivateEndpointConnection":
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
+    ) -> _models.PrivateEndpointConnection:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _json = self._serialize.body(private_endpoint_connection, 'PrivateEndpointConnection')
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(private_endpoint_connection, (IO, bytes)):
+            _content = private_endpoint_connection
+        else:
+            _json = self._serialize.body(private_endpoint_connection, "PrivateEndpointConnection")
 
-        request = build_create_or_update_private_endpoint_connection_request_initial(
-            subscription_id=self._config.subscription_id,
+        request = build_create_or_update_private_endpoint_connection_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
             content_type=content_type,
             json=_json,
-            template_url=self._create_or_update_private_endpoint_connection_initial.metadata['url'],
+            content=_content,
+            template_url=self._create_or_update_private_endpoint_connection_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
-    _create_or_update_private_endpoint_connection_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
-
+    _create_or_update_private_endpoint_connection_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
-    @distributed_trace
+    @overload
     def begin_create_or_update_private_endpoint_connection(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
-        private_endpoint_connection: "_models.PrivateEndpointConnection",
+        private_endpoint_connection: _models.PrivateEndpointConnection,
+        *,
+        content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller["_models.PrivateEndpointConnection"]:
+    ) -> LROPoller[_models.PrivateEndpointConnection]:
         """Create or update private endpoint connection.
 
         Create or update the status of a private endpoint connection with the specified name.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param private_endpoint_connection_name: The name of the private endpoint connection.
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :param private_endpoint_connection: The private endpoint connection with updated properties.
+         Required.
         :type private_endpoint_connection:
          ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result
          of cls(response)
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+
+    @overload
+    def begin_create_or_update_private_endpoint_connection(
+        self,
+        resource_group_name: str,
+        resource_name: str,
+        private_endpoint_connection_name: str,
+        private_endpoint_connection: IO,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.PrivateEndpointConnection]:
+        """Create or update private endpoint connection.
+
+        Create or update the status of a private endpoint connection with the specified name.
+
+        :param resource_group_name: The name of the resource group that contains the provisioning
+         service. Required.
+        :type resource_group_name: str
+        :param resource_name: The name of the provisioning service. Required.
+        :type resource_name: str
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :type private_endpoint_connection_name: str
+        :param private_endpoint_connection: The private endpoint connection with updated properties.
+         Required.
+        :type private_endpoint_connection: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result
+         of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_create_or_update_private_endpoint_connection(
+        self,
+        resource_group_name: str,
+        resource_name: str,
+        private_endpoint_connection_name: str,
+        private_endpoint_connection: Union[_models.PrivateEndpointConnection, IO],
+        **kwargs: Any
+    ) -> LROPoller[_models.PrivateEndpointConnection]:
+        """Create or update private endpoint connection.
+
+        Create or update the status of a private endpoint connection with the specified name.
+
+        :param resource_group_name: The name of the resource group that contains the provisioning
+         service. Required.
+        :type resource_group_name: str
+        :param resource_name: The name of the provisioning service. Required.
+        :type resource_name: str
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
+        :type private_endpoint_connection_name: str
+        :param private_endpoint_connection: The private endpoint connection with updated properties. Is
+         either a model type or a IO type. Required.
+        :type private_endpoint_connection:
+         ~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result
+         of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = self._create_or_update_private_endpoint_connection_initial(
+            raw_result = self._create_or_update_private_endpoint_connection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 private_endpoint_connection=private_endpoint_connection,
+                api_version=api_version,
                 content_type=content_type,
-                cls=lambda x,y,z: x,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = NoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_create_or_update_private_endpoint_connection.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
+    begin_create_or_update_private_endpoint_connection.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
     def _delete_private_endpoint_connection_initial(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        private_endpoint_connection_name: str,
-        **kwargs: Any
-    ) -> Optional["_models.PrivateEndpointConnection"]:
-        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.PrivateEndpointConnection"]]
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> Optional[_models.PrivateEndpointConnection]:
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        
-        request = build_delete_private_endpoint_connection_request_initial(
-            subscription_id=self._config.subscription_id,
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[Optional[_models.PrivateEndpointConnection]]
+
+        request = build_delete_private_endpoint_connection_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
-            template_url=self._delete_private_endpoint_connection_initial.metadata['url'],
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            template_url=self._delete_private_endpoint_connection_initial.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
         request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
+        response_headers = {}
         if response.status_code == 200:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if response.status_code == 202:
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("str", response.headers.get("Retry-After"))
+
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
-    _delete_private_endpoint_connection_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
-
+    _delete_private_endpoint_connection_initial.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
 
     @distributed_trace
     def begin_delete_private_endpoint_connection(
-        self,
-        resource_group_name: str,
-        resource_name: str,
-        private_endpoint_connection_name: str,
-        **kwargs: Any
-    ) -> LROPoller["_models.PrivateEndpointConnection"]:
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> LROPoller[_models.PrivateEndpointConnection]:
         """Delete private endpoint connection.
 
         Delete private endpoint connection with the specified name.
 
         :param resource_group_name: The name of the resource group that contains the provisioning
-         service.
+         service. Required.
         :type resource_group_name: str
-        :param resource_name: The name of the provisioning service.
+        :param resource_name: The name of the provisioning service. Required.
         :type resource_name: str
-        :param private_endpoint_connection_name: The name of the private endpoint connection.
+        :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
         :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
          operation to not poll, or pass in your own initialized polling object for a personal polling
          strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
         :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result
          of cls(response)
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.iothubprovisioningservices.models.PrivateEndpointConnection]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
-        lro_delay = kwargs.pop(
-            'polling_interval',
-            self._config.polling_interval
-        )
-        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2022-02-05"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.PrivateEndpointConnection]
+        polling = kwargs.pop("polling", True)  # type: Union[bool, PollingMethod]
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token = kwargs.pop("continuation_token", None)  # type: Optional[str]
         if cont_token is None:
-            raw_result = self._delete_private_endpoint_connection_initial(
+            raw_result = self._delete_private_endpoint_connection_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 resource_name=resource_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
-                cls=lambda x,y,z: x,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
                 **kwargs
             )
-        kwargs.pop('error_map', None)
+        kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            response = pipeline_response.http_response
-            deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-
-        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
-        elif polling is False: polling_method = NoPolling()
-        else: polling_method = polling
+        if polling is True:
+            polling_method = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))  # type: PollingMethod
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
-                deserialization_callback=get_long_running_output
+                deserialization_callback=get_long_running_output,
             )
-        else:
-            return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
 
-    begin_delete_private_endpoint_connection.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
+    begin_delete_private_endpoint_connection.metadata = {"url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/provisioningServices/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"}  # type: ignore
```

