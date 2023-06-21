# Comparing `tmp/aos_prov-4.2.0b1-py3-none-any.whl.zip` & `tmp/aos_prov-4.2.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,66 @@
-Zip file size: 33153 bytes, number of entries: 36
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/__init__.py
--rw-rw-r--  2.0 unx     3064 b- defN 23-Jun-17 06:38 aos_prov/actions.py
--rw-rw-r--  2.0 unx     7660 b- defN 23-Jun-16 12:56 aos_prov/main.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/commands/__init__.py
--rw-rw-r--  2.0 unx     5861 b- defN 23-May-25 16:52 aos_prov/commands/command_provision.py
--rw-rw-r--  2.0 unx    12474 b- defN 23-Jun-17 10:47 aos_prov/commands/command_vm_multi_node_manage.py
--rw-rw-r--  2.0 unx     3799 b- defN 23-Apr-04 10:59 aos_prov/commands/download.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/__init__.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/cloud/__init__.py
--rw-rw-r--  2.0 unx     8549 b- defN 23-May-25 16:53 aos_prov/communication/cloud/cloud_api.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Apr-10 14:06 aos_prov/communication/unit/__init__.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/__init__.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/__init__.py
--rw-rw-r--  2.0 unx     9583 b- defN 23-May-25 17:01 aos_prov/communication/unit/v4/unit_communication_v4.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/__init__.py
--rw-rw-r--  2.0 unx    18433 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
--rw-rw-r--  2.0 unx    33405 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
--rw-rw-r--  2.0 unx     2705 b- defN 22-Apr-10 14:06 aos_prov/files/1rootCA.crt
--rw-rw-r--  2.0 unx      748 b- defN 22-Nov-13 13:27 aos_prov/utils/__init__.py
--rw-rw-r--  2.0 unx     1649 b- defN 23-Apr-04 10:59 aos_prov/utils/common.py
--rw-rw-r--  2.0 unx     2579 b- defN 23-May-25 16:54 aos_prov/utils/config.py
--rw-rw-r--  2.0 unx      468 b- defN 23-May-25 16:47 aos_prov/utils/errors.py
--rw-rw-r--  2.0 unx     1176 b- defN 22-Dec-01 17:44 aos_prov/utils/unit_certificate.py
--rw-rw-r--  2.0 unx     7475 b- defN 23-Apr-04 10:59 aos_prov/utils/user_credentials.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/utils/__init__.py
--rw-rw-r--  2.0 unx      642 b- defN 22-Dec-01 17:44 test/utils/test_config.py
--rw-rw-r--  2.0 unx      632 b- defN 22-Dec-01 17:44 test/utils/test_unit_certificate.py
--rw-rw-r--  2.0 unx      439 b- defN 22-Nov-13 13:27 test/utils/test_user_credentials.py
--rw-rw-r--  2.0 unx     2554 b- defN 23-Jun-19 15:46 aos_prov-4.2.0b1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 15:46 aos_prov-4.2.0b1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Jun-19 15:46 aos_prov-4.2.0b1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-19 15:46 aos_prov-4.2.0b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3217 b- defN 23-Jun-19 15:46 aos_prov-4.2.0b1.dist-info/RECORD
-36 files, 127889 bytes uncompressed, 27883 bytes compressed:  78.2%
+Zip file size: 78751 bytes, number of entries: 64
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/__init__.py
+-rw-rw-rw-  2.0 fat     3156 b- defN 23-Jun-21 10:54 aos_prov/actions.py
+-rw-rw-rw-  2.0 fat     7927 b- defN 23-Jun-21 10:54 aos_prov/main.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/commands/__init__.py
+-rw-rw-rw-  2.0 fat     6021 b- defN 23-May-30 08:28 aos_prov/commands/command_provision.py
+-rw-rw-rw-  2.0 fat     5021 b- defN 23-Jan-19 15:42 aos_prov/commands/command_vm.py
+-rw-rw-rw-  2.0 fat     2406 b- defN 22-Dec-15 18:20 aos_prov/commands/command_vm_libvirt.py
+-rw-rw-rw-  2.0 fat     5627 b- defN 23-Feb-01 10:29 aos_prov/commands/command_vm_multi_node.py
+-rw-rw-rw-  2.0 fat    13173 b- defN 23-Jun-21 10:54 aos_prov/commands/command_vm_multi_node_manage.py
+-rw-rw-rw-  2.0 fat     3915 b- defN 23-Mar-03 11:42 aos_prov/commands/download.py
+-rw-rw-rw-  2.0 fat     1721 b- defN 23-Jan-23 12:22 aos_prov/commands/vbox_sdk.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/__init__.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/cloud/__init__.py
+-rw-rw-rw-  2.0 fat     8732 b- defN 23-May-30 08:28 aos_prov/communication/cloud/cloud_api.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Feb-07 18:56 aos_prov/communication/unit/__init__.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/__init__.py
+-rw-rw-rw-  2.0 fat     5403 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/unit_communacation.py
+-rw-rw-rw-  2.0 fat     5346 b- defN 23-Mar-13 10:35 aos_prov/communication/unit/v0/unit_communication.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/__init__.py
+-rw-rw-rw-  2.0 fat    29503 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
+-rw-rw-rw-  2.0 fat    20612 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/__init__.py
+-rw-rw-rw-  2.0 fat     6942 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/unit_communacation_v1.py
+-rw-rw-rw-  2.0 fat     6528 b- defN 23-Mar-13 10:35 aos_prov/communication/unit/v1/unit_communication_v1.py
+-rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/__init__.py
+-rw-rw-rw-  2.0 fat     5568 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
+-rw-rw-rw-  2.0 fat      163 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
+-rw-rw-rw-  2.0 fat    31801 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
+-rw-rw-rw-  2.0 fat    20208 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
+-rw-rw-rw-  2.0 fat     9306 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
+-rw-rw-rw-  2.0 fat     8101 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/__init__.py
+-rw-rw-rw-  2.0 fat     7346 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/unit_communacation_v2.py
+-rw-rw-rw-  2.0 fat     6874 b- defN 23-Mar-13 10:35 aos_prov/communication/unit/v2/unit_communication_v2.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/__init__.py
+-rw-rw-rw-  2.0 fat     5568 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
+-rw-rw-rw-  2.0 fat      163 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
+-rw-rw-rw-  2.0 fat    25101 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
+-rw-rw-rw-  2.0 fat    16786 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
+-rw-rw-rw-  2.0 fat    17715 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
+-rw-rw-rw-  2.0 fat    13170 b- defN 22-Oct-13 13:59 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/__init__.py
+-rw-rw-rw-  2.0 fat     9804 b- defN 23-May-30 08:28 aos_prov/communication/unit/v4/unit_communication_v4.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/__init__.py
+-rw-rw-rw-  2.0 fat    18732 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
+-rw-rw-rw-  2.0 fat    34140 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 22-Feb-07 18:56 aos_prov/files/1rootCA.crt
+-rw-rw-rw-  2.0 fat     2767 b- defN 22-Oct-13 13:59 aos_prov/files/vm.xml
+-rw-rw-rw-  2.0 fat      771 b- defN 22-Oct-13 13:59 aos_prov/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1703 b- defN 23-Mar-13 12:54 aos_prov/utils/common.py
+-rw-rw-rw-  2.0 fat     2667 b- defN 23-May-30 08:28 aos_prov/utils/config.py
+-rw-rw-rw-  2.0 fat      504 b- defN 23-May-30 08:28 aos_prov/utils/errors.py
+-rw-rw-rw-  2.0 fat     1229 b- defN 22-Dec-02 13:22 aos_prov/utils/unit_certificate.py
+-rw-rw-rw-  2.0 fat     7659 b- defN 23-Mar-13 10:35 aos_prov/utils/user_credentials.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/utils/__init__.py
+-rw-rw-rw-  2.0 fat      665 b- defN 22-Dec-02 13:22 test/utils/test_config.py
+-rw-rw-rw-  2.0 fat      656 b- defN 22-Dec-02 13:22 test/utils/test_unit_certificate.py
+-rw-rw-rw-  2.0 fat      456 b- defN 22-Oct-13 13:59 test/utils/test_user_credentials.py
+-rw-rw-rw-  2.0 fat     2575 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     6399 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/RECORD
+64 files, 394372 bytes uncompressed, 68179 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -9,20 +9,32 @@
 
 Filename: aos_prov/commands/__init__.py
 Comment: 
 
 Filename: aos_prov/commands/command_provision.py
 Comment: 
 
+Filename: aos_prov/commands/command_vm.py
+Comment: 
+
+Filename: aos_prov/commands/command_vm_libvirt.py
+Comment: 
+
+Filename: aos_prov/commands/command_vm_multi_node.py
+Comment: 
+
 Filename: aos_prov/commands/command_vm_multi_node_manage.py
 Comment: 
 
 Filename: aos_prov/commands/download.py
 Comment: 
 
+Filename: aos_prov/commands/vbox_sdk.py
+Comment: 
+
 Filename: aos_prov/communication/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/cloud/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/cloud/cloud_api.py
@@ -30,20 +42,89 @@
 
 Filename: aos_prov/communication/unit/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v0/__init__.py
 Comment: 
 
+Filename: aos_prov/communication/unit/v0/unit_communacation.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/unit_communication.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/generated/__init__.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
+Comment: 
+
 Filename: aos_prov/communication/unit/v1/__init__.py
 Comment: 
 
+Filename: aos_prov/communication/unit/v1/unit_communacation_v1.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/unit_communication_v1.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/generated/__init__.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
+Comment: 
+
 Filename: aos_prov/communication/unit/v2/__init__.py
 Comment: 
 
+Filename: aos_prov/communication/unit/v2/unit_communacation_v2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/unit_communication_v2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/__init__.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
+Comment: 
+
+Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
+Comment: 
+
 Filename: aos_prov/communication/unit/v4/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v4/unit_communication_v4.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v4/generated/__init__.py
@@ -54,14 +135,17 @@
 
 Filename: aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
 Comment: 
 
 Filename: aos_prov/files/1rootCA.crt
 Comment: 
 
+Filename: aos_prov/files/vm.xml
+Comment: 
+
 Filename: aos_prov/utils/__init__.py
 Comment: 
 
 Filename: aos_prov/utils/common.py
 Comment: 
 
 Filename: aos_prov/utils/config.py
@@ -87,23 +171,23 @@
 
 Filename: test/utils/test_unit_certificate.py
 Comment: 
 
 Filename: test/utils/test_user_credentials.py
 Comment: 
 
-Filename: aos_prov-4.2.0b1.dist-info/METADATA
+Filename: aos_prov-4.2.0b2.dist-info/METADATA
 Comment: 
 
-Filename: aos_prov-4.2.0b1.dist-info/WHEEL
+Filename: aos_prov-4.2.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: aos_prov-4.2.0b1.dist-info/entry_points.txt
+Filename: aos_prov-4.2.0b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_prov-4.2.0b1.dist-info/top_level.txt
+Filename: aos_prov-4.2.0b2.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_prov-4.2.0b1.dist-info/RECORD
+Filename: aos_prov-4.2.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_prov/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/actions.py

 * *Ordering differences only*

```diff
@@ -1,92 +1,92 @@
-#
-#  Copyright (c) 2018-2023 Renesas Inc.
-#  Copyright (c) 2018-2023 EPAM Systems Inc.
-#
-"""aos-prov supported actions module."""
-import time
-
-from aos_prov.commands.command_provision import run_provision
-from aos_prov.commands.command_vm_multi_node_manage import new_vm, start_vms, remove_vms_in_group
-from aos_prov.commands.download import download_and_save_multinode
-from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.utils.common import DOWNLOADS_PATH, print_message
-from aos_prov.utils.user_credentials import UserCredentials
-
-
-def provision_unit(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1) -> None:
-    """
-    Rub provisioning process for the unit.
-
-    Args:
-        unit_address (str): address:port of the unit.
-        cloud_api (CloudAPI): instance of CloudAPI with user info.
-        reconnect_times (int): Number of connections retries.
-    """
-    run_provision(unit_address, cloud_api, reconnect_times)
-
-
-def create_new_unit(
-    vm_name: str,
-    uc: UserCredentials,
-    disk_location: str,
-    do_provision=False,
-    nodes_count=2,
-    headless=False
-) -> []:
-    """
-    Create a new VirtualBox multi-node Unit.
-
-    Args:
-        vm_name (str): Name of the group of units.
-        uc (UserCredentials): UserCredentials instance.
-        disk_location (str): Full path to the folder with nodes images.
-        do_provision (Boolean): Provision unit after creation or not.
-        nodes_count (int): Count of nodes to create. Supported 1 or 2 nodes.
-        headless (bool): Start VM in headless mode if True
-    Returns:
-        [provisioning_port, node0_ssh_port, node1_ssh_port]: Forwarded ports.
-    """
-    cloud_api = CloudAPI(uc)
-
-    if do_provision:
-        cloud_api.check_cloud_access()
-
-    provisioning_port, node0_ssh_port, node1_ssh_port = new_vm(vm_name, disk_location, nodes_count)
-
-    if do_provision:
-        start_vms(f'/AosUnits/{vm_name}', headless=headless)
-        time.sleep(10)
-        run_provision(f'127.0.0.1:{provisioning_port}', cloud_api, reconnect_times=40)
-
-    return [provisioning_port, node0_ssh_port, node1_ssh_port]
-
-
-def remove_vm(name: str) -> None:
-    """Remove all VMs in the group.
-
-    Args:
-        name (str): Name of the group for removing without root AosUnits group.
-    """
-    remove_vms_in_group(name)
-
-
-def start_vm(name: str, headless=False) -> None:
-    """Start all VMs in the group.
-
-    Args:
-        name (str): Name of the group to start without root AosUnits group.
-        headless (bool): Start VM in headless mode if True.
-    """
-    start_vms(f'/AosUnits/{name}', check_virtualbox=True, headless=headless)
-
-
-def download_image(download_url: str, force: bool = False) -> None:
-    """
-    Download unit image.
-
-    Args:
-        download_url (str): URL to download from.
-        force (bool): If set downloaded image will overwrite existing one.
-    """
-    download_and_save_multinode(download_url, DOWNLOADS_PATH, force)
-    print_message(f'Download finished. You may find Unit images in: [b]{str(DOWNLOADS_PATH.resolve())}[/b]')
+#
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
+#
+"""aos-prov supported actions module."""
+import time
+
+from aos_prov.commands.command_provision import run_provision
+from aos_prov.commands.command_vm_multi_node_manage import new_vm, start_vms, remove_vms_in_group
+from aos_prov.commands.download import download_and_save_multinode
+from aos_prov.communication.cloud.cloud_api import CloudAPI
+from aos_prov.utils.common import DOWNLOADS_PATH, print_message
+from aos_prov.utils.user_credentials import UserCredentials
+
+
+def provision_unit(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1) -> None:
+    """
+    Rub provisioning process for the unit.
+
+    Args:
+        unit_address (str): address:port of the unit.
+        cloud_api (CloudAPI): instance of CloudAPI with user info.
+        reconnect_times (int): Number of connections retries.
+    """
+    run_provision(unit_address, cloud_api, reconnect_times)
+
+
+def create_new_unit(
+    vm_name: str,
+    uc: UserCredentials,
+    disk_location: str,
+    do_provision=False,
+    nodes_count=2,
+    headless=False
+) -> []:
+    """
+    Create a new VirtualBox multi-node Unit.
+
+    Args:
+        vm_name (str): Name of the group of units.
+        uc (UserCredentials): UserCredentials instance.
+        disk_location (str): Full path to the folder with nodes images.
+        do_provision (Boolean): Provision unit after creation or not.
+        nodes_count (int): Count of nodes to create. Supported 1 or 2 nodes.
+        headless (bool): Start VM in headless mode if True
+    Returns:
+        [provisioning_port, node0_ssh_port, node1_ssh_port]: Forwarded ports.
+    """
+    cloud_api = CloudAPI(uc)
+
+    if do_provision:
+        cloud_api.check_cloud_access()
+
+    provisioning_port, node0_ssh_port, node1_ssh_port = new_vm(vm_name, disk_location, nodes_count)
+
+    if do_provision:
+        start_vms(f'/AosUnits/{vm_name}', headless=headless)
+        time.sleep(10)
+        run_provision(f'127.0.0.1:{provisioning_port}', cloud_api, reconnect_times=40)
+
+    return [provisioning_port, node0_ssh_port, node1_ssh_port]
+
+
+def remove_vm(name: str) -> None:
+    """Remove all VMs in the group.
+
+    Args:
+        name (str): Name of the group for removing without root AosUnits group.
+    """
+    remove_vms_in_group(name)
+
+
+def start_vm(name: str, headless=False) -> None:
+    """Start all VMs in the group.
+
+    Args:
+        name (str): Name of the group to start without root AosUnits group.
+        headless (bool): Start VM in headless mode if True.
+    """
+    start_vms(f'/AosUnits/{name}', check_virtualbox=True, headless=headless)
+
+
+def download_image(download_url: str, force: bool = False) -> None:
+    """
+    Download unit image.
+
+    Args:
+        download_url (str): URL to download from.
+        force (bool): If set downloaded image will overwrite existing one.
+    """
+    download_and_save_multinode(download_url, DOWNLOADS_PATH, force)
+    print_message(f'Download finished. You may find Unit images in: [b]{str(DOWNLOADS_PATH.resolve())}[/b]')
```

## aos_prov/main.py

 * *Ordering differences only*

```diff
@@ -1,267 +1,267 @@
-#
-#  Copyright (c) 2018-2023 Renesas Inc.
-#  Copyright (c) 2018-2023 EPAM Systems Inc.
-#
-
-import argparse
-import logging
-import sys
-from pathlib import Path
-
-from aos_prov.actions import create_new_unit, download_image, provision_unit, start_vm, remove_vm
-from aos_prov.communication.cloud.cloud_api import DEFAULT_REGISTER_PORT, CloudAPI
-from aos_prov.utils import DEFAULT_USER_CERT_PATH, DEFAULT_USER_KEY_PATH
-from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISKS_PATH, print_error
-from aos_prov.utils.errors import CloudAccessError, UnitError, DeviceRegisterError, OnUnitError
-from aos_prov.utils.user_credentials import UserCredentials
-
-try:
-    from importlib.metadata import version  # noqa: WPS433
-except ImportError:
-    import importlib_metadata as version  # noqa: WPS433
-
-_ARGUMENT_USER_CERTIFICATE = '--cert'
-_ARGUMENT_USER_KEY = '--key'
-_ARGUMENT_USER_PKCS12 = '--pkcs12'
-
-_COMMAND_NEW_VM = 'vm-new'
-_COMMAND_REMOVE_VM = 'vm-remove'
-_COMMAND_START_VM = 'vm-start'
-_COMMAND_UNIT_CREATE = 'unit-new'
-_COMMAND_DOWNLOAD = 'download'
-
-_DEFAULT_USER_CERTIFICATE = str(Path.home() / '.aos' / 'security' / 'aos-user-oem.p12')
-
-logger = logging.getLogger(__name__)
-
-
-def _parse_args():
-    parser = argparse.ArgumentParser(
-        prog='aos-prov',
-        description="The unit provisioning tool using gRPC protocol",
-        epilog="Run 'aos-prov --help' for more information about commands, "
-               "or 'aos-prov COMMAND --help' to see info about command about desired command")
-
-    parser.add_argument(
-        '-u',
-        '--unit',
-        required=False,
-        help="Unit address in format IP_ADDRESS or IP_ADDRESS:PORT"
-    )
-
-    parser.add_argument(
-        _ARGUMENT_USER_CERTIFICATE,
-        default=DEFAULT_USER_CERT_PATH,
-        help=f'User certificate file. Default: {DEFAULT_USER_CERT_PATH}')
-
-    parser.add_argument(
-        _ARGUMENT_USER_KEY,
-        default=DEFAULT_USER_KEY_PATH,
-        help=f'User key file. Default: {DEFAULT_USER_KEY_PATH}')
-
-    parser.add_argument(
-        '-p',
-        _ARGUMENT_USER_PKCS12,
-        required=False,
-        help='Path to user certificate in pkcs12 format.',
-        dest='pkcs',
-        default=_DEFAULT_USER_CERTIFICATE,
-    )
-
-    parser.add_argument(
-        '--register-port',
-        default=DEFAULT_REGISTER_PORT,
-        help=f'Cloud port. Default: {DEFAULT_REGISTER_PORT}'
-    )
-
-    parser.add_argument(
-        '-w',
-        '--wait-unit',
-        action='store',
-        metavar='N',
-        help=f'Wait for unit to respond for the first time in seconds. Default value 0 means try once',
-        dest='wait_unit',
-        default=0,
-        type=int
-    )
-
-    parser.set_defaults(which=None)
-
-    sub_parser = parser.add_subparsers(title='Commands')
-
-    new_vm_command = sub_parser.add_parser(
-        _COMMAND_NEW_VM,
-        help='Create new Oracle VM'
-    )
-    new_vm_command.set_defaults(which=_COMMAND_NEW_VM)
-
-    new_vm_command.add_argument(
-        '-N',
-        '--name',
-        required=True,
-        help='Name of the VM'
-    )
-
-    new_vm_command.add_argument(
-        '-D',
-        '--disk',
-        required=False,
-        help='Full path to the AosCore-powered disk.',
-        default=AOS_DISKS_PATH
-    )
-
-    remove_vm_command = sub_parser.add_parser(
-        _COMMAND_REMOVE_VM,
-        help='Remove Oracle VM'
-    )
-    remove_vm_command.set_defaults(which=_COMMAND_REMOVE_VM)
-
-    remove_vm_command.add_argument(
-        '-N',
-        '--name',
-        required=True,
-        help='Name of the VM'
-    )
-
-    start_vm_command = sub_parser.add_parser(
-        _COMMAND_START_VM,
-        help='Start the VM'
-    )
-    start_vm_command.add_argument(
-        '-N',
-        '--name',
-        required=True,
-        help='Name of the VirtualBox group where VMs are located.'
-    )
-
-    start_vm_command.add_argument(
-        '-H',
-        '--headless',
-        action='store_true',
-        help='Start VMs in headless mode.'
-    )
-    start_vm_command.set_defaults(which=_COMMAND_START_VM)
-
-    create_unit_command = sub_parser.add_parser(
-        _COMMAND_UNIT_CREATE,
-        help='Create and provision new VirtualBox-based unit'
-    )
-    create_unit_command.set_defaults(which=_COMMAND_UNIT_CREATE)
-
-    create_unit_command.add_argument(
-        '--name',
-        required=True,
-        help='Name of the VM'
-    )
-
-    create_unit_command.add_argument(
-        '--disk',
-        required=False,
-        help='Full path to the AosCore-powered disk.',
-        default=AOS_DISKS_PATH
-    )
-
-    create_unit_command.add_argument(
-        '-H',
-        '--headless',
-        action='store_true',
-        help='Start created VMs in headless mode.'
-    )
-
-    create_unit_command.add_argument(
-        '-p',
-        _ARGUMENT_USER_PKCS12,
-        required=False,
-        help='Path to user certificate in pkcs12 format',
-        dest='pkcs',
-        default=_DEFAULT_USER_CERTIFICATE,
-    )
-
-    parser.add_argument(
-        '-V',
-        '--version',
-        action='version',
-        version=f'%(prog)s {version("aos-prov")}',  # noqa: WPS323,WPS237
-    )
-
-    download_command = sub_parser.add_parser(_COMMAND_DOWNLOAD, help='Download image')
-    download_command.set_defaults(which=_COMMAND_DOWNLOAD)
-    download_command.add_argument(
-        '-a',
-        '--address',
-        dest='download_address',
-        help='Address to download image'
-    )
-
-    download_command.add_argument(
-        '-f',
-        '--force',
-        action='store_true',
-        help='Force overwrite existing file'
-    )
-
-    args = parser.parse_args()
-    return args
-
-def _parse_user_creds(args) -> UserCredentials:
-    if args.pkcs == _DEFAULT_USER_CERTIFICATE and \
-        (args.cert != DEFAULT_USER_CERT_PATH or args.key != DEFAULT_USER_KEY_PATH):
-        args.pkcs = None
-    return UserCredentials(cert_file_path=args.cert, key_file_path=args.key, pkcs12=args.pkcs)
-
-
-def main():
-    """The main entry point."""
-    status = 0
-    args = _parse_args()
-
-    try:
-        if args.which is None:
-            uc = _parse_user_creds(args)
-            cloud_api = CloudAPI(uc, args.register_port)
-            cloud_api.check_cloud_access()
-            wait = args.wait_unit // 5 or 1
-            provision_unit(args.unit, cloud_api, wait)
-
-        if args.which == _COMMAND_DOWNLOAD:
-            url = DISK_IMAGE_DOWNLOAD_URL
-            if args.download_address:
-                url = args.download_address
-            download_image(url, args.force)
-
-        if args.which == _COMMAND_NEW_VM:
-            uc = _parse_user_creds(args)
-            create_new_unit(args.name, uc, args.disk)
-
-        if args.which == _COMMAND_REMOVE_VM:
-            remove_vm(args.name)
-
-        if args.which == _COMMAND_START_VM:
-            start_vm(args.name, args.headless)
-
-        if args.which == _COMMAND_UNIT_CREATE:
-            uc = _parse_user_creds(args)
-            create_new_unit(args.name, uc, args.disk, do_provision=True, headless=args.headless)
-
-    except CloudAccessError as e:
-        print_error(f"Failed during communication with the AosCloud with error: {str(e)}")
-        status = 1
-    except DeviceRegisterError as e:
-        print_error(f"FAILED with error: {str(e)}")
-        status = 1
-    except UnitError as e:
-        print_error(f'Failed during communication with device with error: \n {str(e)}')
-        status = 1
-    except OnUnitError as e:
-        print_error('Failed to execute the command!')
-        print_error(f'Error: {str(e)} ')
-        status = 1
-    except (AssertionError, KeyboardInterrupt):
-        print_error('Stopped by keyboard...')
-        status = 1
-
-    sys.exit(status)
-
-
-if __name__ == '__main__':
-    main()
+#
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
+#
+
+import argparse
+import logging
+import sys
+from pathlib import Path
+
+from aos_prov.actions import create_new_unit, download_image, provision_unit, start_vm, remove_vm
+from aos_prov.communication.cloud.cloud_api import DEFAULT_REGISTER_PORT, CloudAPI
+from aos_prov.utils import DEFAULT_USER_CERT_PATH, DEFAULT_USER_KEY_PATH
+from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISKS_PATH, print_error
+from aos_prov.utils.errors import CloudAccessError, UnitError, DeviceRegisterError, OnUnitError
+from aos_prov.utils.user_credentials import UserCredentials
+
+try:
+    from importlib.metadata import version  # noqa: WPS433
+except ImportError:
+    import importlib_metadata as version  # noqa: WPS433
+
+_ARGUMENT_USER_CERTIFICATE = '--cert'
+_ARGUMENT_USER_KEY = '--key'
+_ARGUMENT_USER_PKCS12 = '--pkcs12'
+
+_COMMAND_NEW_VM = 'vm-new'
+_COMMAND_REMOVE_VM = 'vm-remove'
+_COMMAND_START_VM = 'vm-start'
+_COMMAND_UNIT_CREATE = 'unit-new'
+_COMMAND_DOWNLOAD = 'download'
+
+_DEFAULT_USER_CERTIFICATE = str(Path.home() / '.aos' / 'security' / 'aos-user-oem.p12')
+
+logger = logging.getLogger(__name__)
+
+
+def _parse_args():
+    parser = argparse.ArgumentParser(
+        prog='aos-prov',
+        description="The unit provisioning tool using gRPC protocol",
+        epilog="Run 'aos-prov --help' for more information about commands, "
+               "or 'aos-prov COMMAND --help' to see info about command about desired command")
+
+    parser.add_argument(
+        '-u',
+        '--unit',
+        required=False,
+        help="Unit address in format IP_ADDRESS or IP_ADDRESS:PORT"
+    )
+
+    parser.add_argument(
+        _ARGUMENT_USER_CERTIFICATE,
+        default=DEFAULT_USER_CERT_PATH,
+        help=f'User certificate file. Default: {DEFAULT_USER_CERT_PATH}')
+
+    parser.add_argument(
+        _ARGUMENT_USER_KEY,
+        default=DEFAULT_USER_KEY_PATH,
+        help=f'User key file. Default: {DEFAULT_USER_KEY_PATH}')
+
+    parser.add_argument(
+        '-p',
+        _ARGUMENT_USER_PKCS12,
+        required=False,
+        help='Path to user certificate in pkcs12 format.',
+        dest='pkcs',
+        default=_DEFAULT_USER_CERTIFICATE,
+    )
+
+    parser.add_argument(
+        '--register-port',
+        default=DEFAULT_REGISTER_PORT,
+        help=f'Cloud port. Default: {DEFAULT_REGISTER_PORT}'
+    )
+
+    parser.add_argument(
+        '-w',
+        '--wait-unit',
+        action='store',
+        metavar='N',
+        help=f'Wait for unit to respond for the first time in seconds. Default value 0 means try once',
+        dest='wait_unit',
+        default=0,
+        type=int
+    )
+
+    parser.set_defaults(which=None)
+
+    sub_parser = parser.add_subparsers(title='Commands')
+
+    new_vm_command = sub_parser.add_parser(
+        _COMMAND_NEW_VM,
+        help='Create new Oracle VM'
+    )
+    new_vm_command.set_defaults(which=_COMMAND_NEW_VM)
+
+    new_vm_command.add_argument(
+        '-N',
+        '--name',
+        required=True,
+        help='Name of the VM'
+    )
+
+    new_vm_command.add_argument(
+        '-D',
+        '--disk',
+        required=False,
+        help='Full path to the AosCore-powered disk.',
+        default=AOS_DISKS_PATH
+    )
+
+    remove_vm_command = sub_parser.add_parser(
+        _COMMAND_REMOVE_VM,
+        help='Remove Oracle VM'
+    )
+    remove_vm_command.set_defaults(which=_COMMAND_REMOVE_VM)
+
+    remove_vm_command.add_argument(
+        '-N',
+        '--name',
+        required=True,
+        help='Name of the VM'
+    )
+
+    start_vm_command = sub_parser.add_parser(
+        _COMMAND_START_VM,
+        help='Start the VM'
+    )
+    start_vm_command.add_argument(
+        '-N',
+        '--name',
+        required=True,
+        help='Name of the VirtualBox group where VMs are located.'
+    )
+
+    start_vm_command.add_argument(
+        '-H',
+        '--headless',
+        action='store_true',
+        help='Start VMs in headless mode.'
+    )
+    start_vm_command.set_defaults(which=_COMMAND_START_VM)
+
+    create_unit_command = sub_parser.add_parser(
+        _COMMAND_UNIT_CREATE,
+        help='Create and provision new VirtualBox-based unit'
+    )
+    create_unit_command.set_defaults(which=_COMMAND_UNIT_CREATE)
+
+    create_unit_command.add_argument(
+        '--name',
+        required=True,
+        help='Name of the VM'
+    )
+
+    create_unit_command.add_argument(
+        '--disk',
+        required=False,
+        help='Full path to the AosCore-powered disk.',
+        default=AOS_DISKS_PATH
+    )
+
+    create_unit_command.add_argument(
+        '-H',
+        '--headless',
+        action='store_true',
+        help='Start created VMs in headless mode.'
+    )
+
+    create_unit_command.add_argument(
+        '-p',
+        _ARGUMENT_USER_PKCS12,
+        required=False,
+        help='Path to user certificate in pkcs12 format',
+        dest='pkcs',
+        default=_DEFAULT_USER_CERTIFICATE,
+    )
+
+    parser.add_argument(
+        '-V',
+        '--version',
+        action='version',
+        version=f'%(prog)s {version("aos-prov")}',  # noqa: WPS323,WPS237
+    )
+
+    download_command = sub_parser.add_parser(_COMMAND_DOWNLOAD, help='Download image')
+    download_command.set_defaults(which=_COMMAND_DOWNLOAD)
+    download_command.add_argument(
+        '-a',
+        '--address',
+        dest='download_address',
+        help='Address to download image'
+    )
+
+    download_command.add_argument(
+        '-f',
+        '--force',
+        action='store_true',
+        help='Force overwrite existing file'
+    )
+
+    args = parser.parse_args()
+    return args
+
+def _parse_user_creds(args) -> UserCredentials:
+    if args.pkcs == _DEFAULT_USER_CERTIFICATE and \
+        (args.cert != DEFAULT_USER_CERT_PATH or args.key != DEFAULT_USER_KEY_PATH):
+        args.pkcs = None
+    return UserCredentials(cert_file_path=args.cert, key_file_path=args.key, pkcs12=args.pkcs)
+
+
+def main():
+    """The main entry point."""
+    status = 0
+    args = _parse_args()
+
+    try:
+        if args.which is None:
+            uc = _parse_user_creds(args)
+            cloud_api = CloudAPI(uc, args.register_port)
+            cloud_api.check_cloud_access()
+            wait = args.wait_unit // 5 or 1
+            provision_unit(args.unit, cloud_api, wait)
+
+        if args.which == _COMMAND_DOWNLOAD:
+            url = DISK_IMAGE_DOWNLOAD_URL
+            if args.download_address:
+                url = args.download_address
+            download_image(url, args.force)
+
+        if args.which == _COMMAND_NEW_VM:
+            uc = _parse_user_creds(args)
+            create_new_unit(args.name, uc, args.disk)
+
+        if args.which == _COMMAND_REMOVE_VM:
+            remove_vm(args.name)
+
+        if args.which == _COMMAND_START_VM:
+            start_vm(args.name, args.headless)
+
+        if args.which == _COMMAND_UNIT_CREATE:
+            uc = _parse_user_creds(args)
+            create_new_unit(args.name, uc, args.disk, do_provision=True, headless=args.headless)
+
+    except CloudAccessError as e:
+        print_error(f"Failed during communication with the AosCloud with error: {str(e)}")
+        status = 1
+    except DeviceRegisterError as e:
+        print_error(f"FAILED with error: {str(e)}")
+        status = 1
+    except UnitError as e:
+        print_error(f'Failed during communication with device with error: \n {str(e)}')
+        status = 1
+    except OnUnitError as e:
+        print_error('Failed to execute the command!')
+        print_error(f'Error: {str(e)} ')
+        status = 1
+    except (AssertionError, KeyboardInterrupt):
+        print_error('Stopped by keyboard...')
+        status = 1
+
+    sys.exit(status)
+
+
+if __name__ == '__main__':
+    main()
```

## aos_prov/commands/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/commands/command_provision.py

 * *Ordering differences only*

```diff
@@ -1,160 +1,160 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-"""Provision unit."""
-
-import time
-
-from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.communication.unit.v4.unit_communication_v4 import UnitCommunicationV4
-from aos_prov.utils.common import generate_random_password, print_message
-from aos_prov.utils.config import Config
-from aos_prov.utils.errors import GrpcUnimplemented, UnitError
-
-COMMAND_TO_DECRYPT = 'diskencryption'
-
-
-def run_provision(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1):
-    """
-    Provision Unit. This function will try to provision starting from the newest to the oldest.
-
-    Args:
-         unit_address (str): Address of the Unit
-         cloud_api (CloudAPI): URL to download
-         reconnect_times (int): URL to download
-
-    Raises:
-        AosProvError: If provision fails.
-    """
-    config = Config()
-    uc = UnitCommunicationV4(unit_address)
-    model_name = ''
-    for retry in range(reconnect_times):
-        try:
-            print_message('Starting provisioning...')
-            config.system_id, model_name = uc.get_system_info()
-            config.protocol_version = uc.get_protocol_version()
-            break
-        except GrpcUnimplemented as gu:
-            print_message(f'[red]Grpc protocol error: {gu}.')
-            raise gu
-        except UnitError as be:
-            print_message('[yellow]Connection failed')
-            if retry + 1 < reconnect_times:
-                time.sleep(5)
-            else:
-                raise be
-
-    if config.system_id is None:
-        raise UnitError('Cannot read system_id')
-
-    config.set_model(model_name)
-    cloud_api.check_unit_is_not_provisioned(config.system_id)
-    if config.protocol_version >= 4:  # support of multi domains
-        config.node_ids = uc.get_all_node_ids()
-        for node_id in config.node_ids:
-            config.supported_cert_types = uc.get_cert_types(node_id)
-            need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
-
-            password = generate_random_password()
-
-            for cert_type in config.supported_cert_types:
-                uc.clear(cert_type, node_id)
-
-            for cert_type in config.supported_cert_types:
-                uc.set_cert_owner(cert_type, password, node_id)
-
-            if need_disk_encryption:
-                uc.encrypt_disk(password, node_id)
-                config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
-                if config.protocol_version < 4:
-                    uc.wait_for_connection()
-
-
-            for cert_type in config.supported_cert_types:
-                config.unit_certificates.append(uc.create_keys(cert_type, password, node_id))
-    else:
-        config.supported_cert_types = uc.get_cert_types()
-        need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
-
-        password = generate_random_password()
-
-        for cert_type in config.supported_cert_types:
-            uc.clear(cert_type)
-
-        for cert_type in config.supported_cert_types:
-            uc.set_cert_owner(cert_type, password)
-
-        if need_disk_encryption:
-            uc.encrypt_disk(password)
-            config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
-            if config.protocol_version < 4:
-                uc.wait_for_connection()
-
-        for cert_type in config.supported_cert_types:
-            config.unit_certificates.append(uc.create_keys(cert_type, password))
-
-    register_payload = {
-        'hardware_id': config.system_id,
-        'system_uid': config.system_id,
-        'model_name': config.model_name,
-        'model_version': config.model_version,
-        'provisioning_software': "aos-provisioning:{version}".format(version=3.1),
-        'additional_csrs': []
-    }
-
-    for cert in config.unit_certificates:
-        if cert.cert_type == 'online':
-            register_payload['online_public_csr'] = cert.csr
-            if cert.node_id:
-                register_payload['online_public_node_id'] = cert.node_id
-        elif cert.cert_type == 'offline':
-            register_payload['offline_public_csr'] = cert.csr
-            if cert.node_id:
-                register_payload['offline_public_node_id'] = cert.node_id
-        else:
-            register_payload['additional_csrs'].append({
-                'cert_type': cert.cert_type,
-                'csr': cert.csr,
-                'node_id': cert.node_id,
-            })
-
-    response = cloud_api.register_device(register_payload)
-    system_uid = response.get('system_uid')
-    additional_certs = response.get('additional_certs', [])
-    for cert in config.unit_certificates:
-        if cert.cert_type == 'online':
-            cert.certificate = response.get('online_certificate')
-        elif cert.cert_type == 'offline':
-            cert.certificate = response.get('offline_certificate')
-        else:
-            for ac in additional_certs:
-                if ac['cert_type'] == cert.cert_type:
-                    if ac.get('node_id'):
-                        if ac.get('node_id') == cert.node_id:
-                            cert.certificate = ac['cert']
-                            break
-                    else:
-                        cert.certificate = ac['cert']
-                        cert.node_id = ac.get('node_id')
-                        break
-
-    for cert in config.unit_certificates:
-        uc.apply_certificate(cert)
-
-    claims = response.get('claim')
-
-    if claims:
-        if not hasattr(uc, 'need_set_users'):
-            uc.set_users([claims])
-        elif uc.need_set_users:
-            uc.set_users([claims])
-
-    uc.finish_provisioning()
-
-    print_message('[green]Finished successfully!')
-    link = cloud_api.get_unit_link_by_system_uid(system_uid)
-
-    if link:
-        print_message(f'You may find your unit on the cloud here: [green]{link}')
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+"""Provision unit."""
+
+import time
+
+from aos_prov.communication.cloud.cloud_api import CloudAPI
+from aos_prov.communication.unit.v4.unit_communication_v4 import UnitCommunicationV4
+from aos_prov.utils.common import generate_random_password, print_message
+from aos_prov.utils.config import Config
+from aos_prov.utils.errors import GrpcUnimplemented, UnitError
+
+COMMAND_TO_DECRYPT = 'diskencryption'
+
+
+def run_provision(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1):
+    """
+    Provision Unit. This function will try to provision starting from the newest to the oldest.
+
+    Args:
+         unit_address (str): Address of the Unit
+         cloud_api (CloudAPI): URL to download
+         reconnect_times (int): URL to download
+
+    Raises:
+        AosProvError: If provision fails.
+    """
+    config = Config()
+    uc = UnitCommunicationV4(unit_address)
+    model_name = ''
+    for retry in range(reconnect_times):
+        try:
+            print_message('Starting provisioning...')
+            config.system_id, model_name = uc.get_system_info()
+            config.protocol_version = uc.get_protocol_version()
+            break
+        except GrpcUnimplemented as gu:
+            print_message(f'[red]Grpc protocol error: {gu}.')
+            raise gu
+        except UnitError as be:
+            print_message('[yellow]Connection failed')
+            if retry + 1 < reconnect_times:
+                time.sleep(5)
+            else:
+                raise be
+
+    if config.system_id is None:
+        raise UnitError('Cannot read system_id')
+
+    config.set_model(model_name)
+    cloud_api.check_unit_is_not_provisioned(config.system_id)
+    if config.protocol_version >= 4:  # support of multi domains
+        config.node_ids = uc.get_all_node_ids()
+        for node_id in config.node_ids:
+            config.supported_cert_types = uc.get_cert_types(node_id)
+            need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
+
+            password = generate_random_password()
+
+            for cert_type in config.supported_cert_types:
+                uc.clear(cert_type, node_id)
+
+            for cert_type in config.supported_cert_types:
+                uc.set_cert_owner(cert_type, password, node_id)
+
+            if need_disk_encryption:
+                uc.encrypt_disk(password, node_id)
+                config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
+                if config.protocol_version < 4:
+                    uc.wait_for_connection()
+
+
+            for cert_type in config.supported_cert_types:
+                config.unit_certificates.append(uc.create_keys(cert_type, password, node_id))
+    else:
+        config.supported_cert_types = uc.get_cert_types()
+        need_disk_encryption = COMMAND_TO_DECRYPT in config.supported_cert_types
+
+        password = generate_random_password()
+
+        for cert_type in config.supported_cert_types:
+            uc.clear(cert_type)
+
+        for cert_type in config.supported_cert_types:
+            uc.set_cert_owner(cert_type, password)
+
+        if need_disk_encryption:
+            uc.encrypt_disk(password)
+            config.supported_cert_types.remove(COMMAND_TO_DECRYPT)
+            if config.protocol_version < 4:
+                uc.wait_for_connection()
+
+        for cert_type in config.supported_cert_types:
+            config.unit_certificates.append(uc.create_keys(cert_type, password))
+
+    register_payload = {
+        'hardware_id': config.system_id,
+        'system_uid': config.system_id,
+        'model_name': config.model_name,
+        'model_version': config.model_version,
+        'provisioning_software': "aos-provisioning:{version}".format(version=3.1),
+        'additional_csrs': []
+    }
+
+    for cert in config.unit_certificates:
+        if cert.cert_type == 'online':
+            register_payload['online_public_csr'] = cert.csr
+            if cert.node_id:
+                register_payload['online_public_node_id'] = cert.node_id
+        elif cert.cert_type == 'offline':
+            register_payload['offline_public_csr'] = cert.csr
+            if cert.node_id:
+                register_payload['offline_public_node_id'] = cert.node_id
+        else:
+            register_payload['additional_csrs'].append({
+                'cert_type': cert.cert_type,
+                'csr': cert.csr,
+                'node_id': cert.node_id,
+            })
+
+    response = cloud_api.register_device(register_payload)
+    system_uid = response.get('system_uid')
+    additional_certs = response.get('additional_certs', [])
+    for cert in config.unit_certificates:
+        if cert.cert_type == 'online':
+            cert.certificate = response.get('online_certificate')
+        elif cert.cert_type == 'offline':
+            cert.certificate = response.get('offline_certificate')
+        else:
+            for ac in additional_certs:
+                if ac['cert_type'] == cert.cert_type:
+                    if ac.get('node_id'):
+                        if ac.get('node_id') == cert.node_id:
+                            cert.certificate = ac['cert']
+                            break
+                    else:
+                        cert.certificate = ac['cert']
+                        cert.node_id = ac.get('node_id')
+                        break
+
+    for cert in config.unit_certificates:
+        uc.apply_certificate(cert)
+
+    claims = response.get('claim')
+
+    if claims:
+        if not hasattr(uc, 'need_set_users'):
+            uc.set_users([claims])
+        elif uc.need_set_users:
+            uc.set_users([claims])
+
+    uc.finish_provisioning()
+
+    print_message('[green]Finished successfully!')
+    link = cloud_api.get_unit_link_by_system_uid(system_uid)
+
+    if link:
+        print_message(f'You may find your unit on the cloud here: [green]{link}')
```

## aos_prov/commands/command_vm_multi_node_manage.py

```diff
@@ -1,404 +1,411 @@
-#
-#  Copyright (c) 2018-2023 Renesas Inc.
-#  Copyright (c) 2018-2023 EPAM Systems Inc.
-#
-
-import os
-import platform
-import socket
-import subprocess
-import uuid
-from pathlib import Path
-from random import randint
-from shutil import copyfile
-
-from aos_prov.commands.download import download_and_save_multinode
-from aos_prov.utils.common import (
-    DOWNLOADS_PATH,
-    AOS_DISKS_PATH,
-    DISK_IMAGE_DOWNLOAD_URL,
-    NODE0_IMAGE_FILENAME,
-    NODE1_IMAGE_FILENAME,
-    print_left,
-    print_success,
-    print_done,
-    print_error,
-    print_message
-)
-from aos_prov.utils.errors import AosProvError
-
-
-def _is_port_in_use(port):
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        return s.connect_ex(('localhost', port)) == 0
-
-
-def _delete_controller(vm_uuid: str, controller_name: str):
-    command = [
-        'VBoxManage', 'storagectl',
-        vm_uuid,
-        f'--name={controller_name}',
-        '--controller=',
-        '--remove',
-    ]
-    execute_command(command, catch_error=True)
-
-
-def _create_storage_controller(vm_uuid: str, controller_name: str):
-    """Create SATA controller for VM.
-        Args:
-             vm_uuid (str): UUID or Name of VM to attach controller.
-             controller_name (str): Name of the controller.
-    """
-    command = [
-        'VBoxManage', 'storagectl',
-        vm_uuid,
-        f'--name={controller_name}',
-        '--add=sata',
-        '--controller=IntelAhci',
-        '--portcount=1',
-        '--hostiocache=on',
-        '--bootable=on'
-    ]
-    execute_command(command)
-
-
-def _attach_disk(vm_uuid: str, attach_to_controller_name: str, disk_location: str):
-    """Attach disk file to the controller.
-        Args:
-             vm_uuid (str): UUID or Name of VM to attach controller.
-             attach_to_controller_name (str): Name of the controller where disk will be attached.
-             disk_location (str): path to the disk file.
-    """
-    command = [
-        'VBoxManage', 'storageattach',
-        vm_uuid,
-        '--storagectl', attach_to_controller_name,
-        '--port', '0',
-        '--type', 'hdd',
-        '--medium', disk_location
-    ]
-    execute_command(command)
-
-
-def _create_network(network_name: str):
-    print_left('Creating a network for the units...')
-    command = [
-        'VBoxManage',
-        'natnetwork',
-        'add',
-        '--netname',
-        network_name,
-        '--network',
-        '10.0.0.0/24',
-        '--enable',
-        '--dhcp',
-        'on'
-    ]
-    execute_command(command)
-    print_success(f'Network {network_name} has been created')
-
-
-def _remove_network(network_name: str):
-    print_left(f'Removing a network: {network_name} for the units...')
-    command = [
-        'VBoxManage',
-        'natnetwork',
-        'remove',
-        '--netname',
-        network_name,
-    ]
-    execute_command(command, catch_error=False)
-    print_message('Network has been removed')
-
-
-def _forward_port(network_name: str, forward_name: str, from_ip: str, from_port: int, to_port=None) -> int:
-    if to_port is None:
-        to_port = randint(8090, 8999)
-        while _is_port_in_use(to_port):
-            to_port = randint(8090, 8999)
-
-    command = [
-        'VBoxManage',
-        'natnetwork',
-        'modify',
-        '--netname',
-        network_name,
-        '--port-forward-4',
-        f"{forward_name}:tcp:[]:{to_port}:[{from_ip}]:{from_port}",
-    ]
-
-    execute_command(command)
-    return to_port
-
-
-def check_virtual_box():
-    print_left('Checking VirtualBox...')
-
-    if platform.machine().lower() not in ['amd64', 'x86_64']:
-        raise AosProvError('Only amd64 architecture is supported.')
-
-    try:
-        response = execute_command(['VBoxManage', '--version'], catch_error=False)
-    except AosProvError:
-        raise AosProvError('VirtualBox is not installed or it is not in the PATH')
-
-    if 'WARNING: The vboxdrv kernel module is not loaded' in response:
-        raise AosProvError('VirtualBox kernel modules is not installed.')
-
-    if not response.startswith('7'):
-        raise AosProvError('VirtualBox 7 is only supported')
-
-    print_success(response)
-
-
-def new_vm(vm_name: str, disk_location: str, nodes_count=2) -> ():
-    check_virtual_box()
-    print_message('Creating a new virtual machines...')
-
-    disk_location_path = Path(disk_location)
-
-    if not ((disk_location_path / NODE0_IMAGE_FILENAME).exists()) or \
-        not ((disk_location_path / NODE1_IMAGE_FILENAME).exists()):
-        if disk_location_path == AOS_DISKS_PATH:
-            print_message('Local images not found. Downloading...')
-            download_and_save_multinode(DISK_IMAGE_DOWNLOAD_URL, DOWNLOADS_PATH, False)
-            print_success('Download finished. You may find Unit images in: ' + str(DOWNLOADS_PATH.resolve()))
-        else:
-            raise AosProvError(f'Disk images not found in directory {disk_location}. Can\'t proceed!')
-
-    nodes = [
-        {
-            'name': 'node0',
-            'uuid': str(uuid.uuid4()),
-            'disk_name': NODE0_IMAGE_FILENAME,
-            'disk_location': Path(disk_location_path / NODE0_IMAGE_FILENAME)
-        }
-    ]
-
-    if nodes_count != 1:
-        nodes.append(
-            {
-                'name': 'node1',
-                'uuid': str(uuid.uuid4()),
-                'disk_name': NODE1_IMAGE_FILENAME,
-                'disk_location': Path(disk_location_path / NODE1_IMAGE_FILENAME)
-            }
-        )
-
-    units_network_name = f'aos-network-{vm_name}'
-    units_vm_group = f'/AosUnits/{vm_name}'
-    try:
-        _create_network(units_network_name)
-        print_left('Forwarding provisioning port...')
-        provisioning_port = _forward_port(
-            units_network_name,
-            forward_name='provisioningPortForward',
-            from_ip='10.0.0.100',
-            from_port=8089
-        )
-        print_success(provisioning_port)
-
-        print_left('Forwarding ssh port to node0...')
-        node0_ssh_port = _forward_port(
-            units_network_name,
-            forward_name='node0ssh',
-            from_ip='10.0.0.100',
-            from_port=22
-        )
-        print_success(node0_ssh_port)
-
-        print_left('Forwarding ssh port to node1...')
-        node1_ssh_port = _forward_port(
-            units_network_name,
-            forward_name='node1ssh',
-            from_ip='10.0.0.101',
-            from_port=22
-        )
-        print_success(node1_ssh_port)
-
-        for node in nodes:
-            print_left(f'Creating a new VM for {node["name"]}...')
-            create_node_vm(
-                node['name'],
-                node['uuid'],
-                units_vm_group,
-                node['disk_location'],
-                node['disk_name'],
-                units_network_name
-            )
-            print_done()
-
-        return provisioning_port, node0_ssh_port, node1_ssh_port
-    except AosProvError as error:
-        print_error('Cannot create VM. Clean up all related resources. Try again.')
-        remove_vms_in_group(vm_name)
-        raise error
-
-
-def create_node_vm(vm_name: str, vm_uuid: str, group: str, original_disk_path: Path, disk_name: str, network_name):
-    create_vm_command = [
-        'VBoxManage', 'createvm',
-        f'--name={vm_name}',
-        '--ostype=Linux_64',
-        f'--uuid={vm_uuid}',
-        f'--groups={group}',
-        '--default',
-        '--register'
-    ]
-
-    cpu_count = 1
-    if platform.system() == 'Windows':
-        cpu_count = 4
-
-    set_vm_params = [
-        'VBoxManage', 'modifyvm',
-        vm_uuid,
-        '--memory=1024',
-        '--firmware=efi',
-        f'--cpus={cpu_count}'
-    ]
-
-    set_vm_net = [
-        'VBoxManage', 'modifyvm',
-        vm_uuid,
-        '--nic1=natnetwork',
-        f'--nat-network1={network_name}'
-    ]
-
-    execute_command(create_vm_command)
-    execute_command(set_vm_params)
-    execute_command(set_vm_net)
-    _delete_controller(vm_uuid, 'SATA')
-    _delete_controller(vm_uuid, 'IDE')
-
-    _create_storage_controller(vm_uuid, 'SATA')
-
-    destination_image = str((_find_vm_location(vm_uuid) / disk_name).resolve())
-    copyfile(original_disk_path.absolute(), destination_image)
-
-    try:
-        _attach_disk(vm_uuid, 'SATA', disk_location=destination_image)
-    except AosProvError as error:
-        print_error(f'Cannot attach disk {destination_image} to VM. Clean up all related resources. Try again.')
-        os.remove(destination_image)
-        raise error
-
-
-def remove_vms_in_group(vm_name: str):
-    units_network_name = f'aos-network-{vm_name}'
-    vm_group = f'/AosUnits/{vm_name}'
-
-    print_message(f'Removing VMs in Groups: {vm_group} for the units...')
-
-    # find uuids of all VMs into the required Group
-    detailed_list_vms_command = [
-        'VBoxManage', 'list',
-        'vms',
-        '--long',
-    ]
-    detailed_list_vms_out = execute_command(detailed_list_vms_command, catch_error=True)
-    detailed_list_vms = dict(list())
-    processed_group_vm = ''
-    for output_line in detailed_list_vms_out.splitlines():
-        if output_line.startswith('Groups:'):
-            # line format is: 'Groups:                      /AosUnits/my-test-vm1'
-            if len(output_line.split()) == 2:
-                processed_group_vm = output_line.split()[1]
-        elif output_line.startswith('UUID:'):
-            # line format is: 'UUID:                        49f87eef-838b-43cb-b6eb-604989b15f9f'
-            if len(output_line.split()) == 2:
-                vm_uuid = output_line.split()[1]
-                list_of_uuids = []
-                if detailed_list_vms.get(processed_group_vm):
-                    list_of_uuids = detailed_list_vms[processed_group_vm]
-                if vm_uuid not in list_of_uuids:
-                    list_of_uuids.append(vm_uuid)
-                    detailed_list_vms[processed_group_vm] = list_of_uuids
-
-    _remove_network(units_network_name)
-
-    if not detailed_list_vms.get(vm_group):
-        print_error(f'VM Group: {vm_group} is not presented on system.')
-        return
-
-    for vm_uuid in detailed_list_vms[vm_group]:
-        delete_vm_command = [
-            'VBoxManage', 'unregistervm',
-            vm_uuid,
-            '--delete',
-        ]
-        execute_command(delete_vm_command, catch_error=False)
-    print_message('VMs have been deleted')
-
-
-def _find_vm_location(vm_uuid) -> Path:
-    set_vm_params = [
-        'VBoxManage', 'showvminfo',
-        vm_uuid,
-        '--machinereadable'
-    ]
-
-    response = execute_command(set_vm_params)
-
-    for row in response.splitlines():
-        param = row.split('=')
-        if param[0] == 'CfgFile':
-            return Path(param[1].replace('"', '')).parent
-
-
-def start_vms(group: str, check_virtualbox: bool = False, headless=False) -> None:
-    """Start all VMs in the group.
-
-    Args:
-        group (str): Name of the group to start
-        check_virtualbox (bool): Check VirtualBox status before execution
-        headless (bool): Start VM in headless mode if True
-    Raises:
-        AosProvError: If no VMs to start found.
-    Returns:
-        None
-    """
-    if check_virtualbox:
-        check_virtual_box()
-
-    message = f'Starting VMs in group [bold]{group}[/bold]'
-
-    if headless:
-        message += ' in headless mode'
-
-    print_message(message)
-    vms_to_start = []
-    vms = execute_command(['VBoxManage', 'list', 'vms'])
-
-    for vm in vms.splitlines():
-        guid = vm[vm.find('{')+1:vm.find('}')]
-        info_command = ['VBoxManage', 'showvminfo', guid, '--machinereadable']
-        info = execute_command(info_command)
-
-        for row in info.splitlines():
-            if row.startswith('groups='):
-                vm_group = row.replace('"', '').split('=')[1]
-                if group == vm_group:
-                    vms_to_start.append(guid)
-                    break
-
-    if len(vms_to_start) == 0:
-        raise AosProvError(f'No VMs found in group {group} to start!')
-
-    start_type = 'headless' if headless else 'gui'
-
-    for vm_guid in vms_to_start:
-        start_command = ['VBoxManage', 'startvm', vm_guid, f'--type={start_type}']
-        print_left(f'Starting VM {vm_guid}...')
-        execute_command(start_command)
-        print_done()
-
-
-def execute_command(command, catch_error=False) -> str:
-    execution_status = subprocess.run(command, shell=False, env=os.environ.copy(),  capture_output=True)
-    if execution_status.returncode == 0:
-        return execution_status.stdout.decode("utf-8")
-    else:
-        if not catch_error:
-            raise AosProvError(execution_status.stderr.decode("utf-8"))
+#
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
+#
+
+import os
+import platform
+import socket
+import subprocess
+import uuid
+from pathlib import Path
+from random import randint
+from shutil import copyfile
+
+from aos_prov.commands.download import download_and_save_multinode
+from aos_prov.utils.common import (
+    DOWNLOADS_PATH,
+    AOS_DISKS_PATH,
+    DISK_IMAGE_DOWNLOAD_URL,
+    NODE0_IMAGE_FILENAME,
+    NODE1_IMAGE_FILENAME,
+    print_left,
+    print_success,
+    print_done,
+    print_error,
+    print_message
+)
+from aos_prov.utils.errors import AosProvError
+
+
+def _is_port_in_use(port):
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        return s.connect_ex(('localhost', port)) == 0
+
+
+def _delete_controller(vm_uuid: str, controller_name: str):
+    command = [
+        'VBoxManage', 'storagectl',
+        vm_uuid,
+        f'--name={controller_name}',
+        '--controller=',
+        '--remove',
+    ]
+    execute_command(command, catch_error=True)
+
+
+def _create_storage_controller(vm_uuid: str, controller_name: str):
+    """Create SATA controller for VM.
+        Args:
+             vm_uuid (str): UUID or Name of VM to attach controller.
+             controller_name (str): Name of the controller.
+    """
+    command = [
+        'VBoxManage', 'storagectl',
+        vm_uuid,
+        f'--name={controller_name}',
+        '--add=sata',
+        '--controller=IntelAhci',
+        '--portcount=1',
+        '--hostiocache=on',
+        '--bootable=on'
+    ]
+    execute_command(command)
+
+
+def _attach_disk(vm_uuid: str, attach_to_controller_name: str, disk_location: str):
+    """Attach disk file to the controller.
+        Args:
+             vm_uuid (str): UUID or Name of VM to attach controller.
+             attach_to_controller_name (str): Name of the controller where disk will be attached.
+             disk_location (str): path to the disk file.
+    """
+    command = [
+        'VBoxManage', 'storageattach',
+        vm_uuid,
+        '--storagectl', attach_to_controller_name,
+        '--port', '0',
+        '--type', 'hdd',
+        '--medium', disk_location
+    ]
+    execute_command(command)
+
+
+def _create_network(network_name: str):
+    print_left('Creating a network for the units...')
+    command = [
+        'VBoxManage',
+        'natnetwork',
+        'add',
+        '--netname',
+        network_name,
+        '--network',
+        '10.0.0.0/24',
+        '--enable',
+        '--dhcp',
+        'on'
+    ]
+    execute_command(command)
+    print_success(f'Network {network_name} has been created')
+
+
+def _remove_network(network_name: str):
+    print_left(f'Removing a network: {network_name} for the units...')
+    command = [
+        'VBoxManage',
+        'natnetwork',
+        'remove',
+        '--netname',
+        network_name,
+    ]
+    execute_command(command, catch_error=False)
+    print_message('Network has been removed')
+
+
+def _forward_port(network_name: str, forward_name: str, from_ip: str, from_port: int, to_port=None) -> int:
+    if to_port is None:
+        to_port = randint(8090, 8999)
+        while _is_port_in_use(to_port):
+            to_port = randint(8090, 8999)
+
+    command = [
+        'VBoxManage',
+        'natnetwork',
+        'modify',
+        '--netname',
+        network_name,
+        '--port-forward-4',
+        f"{forward_name}:tcp:[]:{to_port}:[{from_ip}]:{from_port}",
+    ]
+
+    execute_command(command)
+    return to_port
+
+
+def check_virtual_box():
+    print_left('Checking VirtualBox...')
+
+    if platform.machine().lower() not in ['amd64', 'x86_64']:
+        raise AosProvError('Only amd64 architecture is supported.')
+
+    try:
+        response = execute_command(['VBoxManage', '--version'], catch_error=False)
+    except AosProvError:
+        raise AosProvError('VirtualBox is not installed or it is not in the PATH')
+
+    if 'WARNING: The vboxdrv kernel module is not loaded' in response:
+        raise AosProvError('VirtualBox kernel modules is not installed.')
+
+    if not response.startswith('7'):
+        raise AosProvError('VirtualBox 7 is only supported')
+
+    print_success(response)
+
+
+def new_vm(vm_name: str, disk_location: str, nodes_count=2) -> ():
+    check_virtual_box()
+    print_message('Creating a new virtual machines...')
+
+    disk_location_path = Path(disk_location)
+
+    if not ((disk_location_path / NODE0_IMAGE_FILENAME).exists()) or \
+        not ((disk_location_path / NODE1_IMAGE_FILENAME).exists()):
+        if disk_location_path == AOS_DISKS_PATH:
+            print_message('Local images not found. Downloading...')
+            download_and_save_multinode(DISK_IMAGE_DOWNLOAD_URL, DOWNLOADS_PATH, False)
+            print_success('Download finished. You may find Unit images in: ' + str(DOWNLOADS_PATH.resolve()))
+        else:
+            raise AosProvError(f'Disk images not found in directory {disk_location}. Can\'t proceed!')
+
+    nodes = [
+        {
+            'name': 'node0',
+            'uuid': str(uuid.uuid4()),
+            'disk_name': NODE0_IMAGE_FILENAME,
+            'disk_location': Path(disk_location_path / NODE0_IMAGE_FILENAME)
+        }
+    ]
+
+    if nodes_count != 1:
+        nodes.append(
+            {
+                'name': 'node1',
+                'uuid': str(uuid.uuid4()),
+                'disk_name': NODE1_IMAGE_FILENAME,
+                'disk_location': Path(disk_location_path / NODE1_IMAGE_FILENAME)
+            }
+        )
+
+    units_network_name = f'aos-network-{vm_name}'
+    units_vm_group = f'/AosUnits/{vm_name}'
+    try:
+        _create_network(units_network_name)
+        print_left('Forwarding provisioning port...')
+        provisioning_port = _forward_port(
+            units_network_name,
+            forward_name='provisioningPortForward',
+            from_ip='10.0.0.100',
+            from_port=8089
+        )
+        print_success(provisioning_port)
+
+        print_left('Forwarding ssh port to node0...')
+        node0_ssh_port = _forward_port(
+            units_network_name,
+            forward_name='node0ssh',
+            from_ip='10.0.0.100',
+            from_port=22
+        )
+        print_success(node0_ssh_port)
+
+        print_left('Forwarding ssh port to node1...')
+        node1_ssh_port = _forward_port(
+            units_network_name,
+            forward_name='node1ssh',
+            from_ip='10.0.0.101',
+            from_port=22
+        )
+        print_success(node1_ssh_port)
+
+        for node in nodes:
+            print_left(f'Creating a new VM for {node["name"]}...')
+            create_node_vm(
+                node['name'],
+                node['uuid'],
+                units_vm_group,
+                node['disk_location'],
+                node['disk_name'],
+                units_network_name
+            )
+            print_done()
+
+        return provisioning_port, node0_ssh_port, node1_ssh_port
+    except AosProvError as error:
+        print_error('Cannot create VM. Clean up all related resources. Try again.')
+        remove_vms_in_group(vm_name)
+        raise error
+
+
+def create_node_vm(vm_name: str, vm_uuid: str, group: str, original_disk_path: Path, disk_name: str, network_name):
+    create_vm_command = [
+        'VBoxManage', 'createvm',
+        f'--name={vm_name}',
+        '--ostype=Linux_64',
+        f'--uuid={vm_uuid}',
+        f'--groups={group}',
+        '--default',
+        '--register'
+    ]
+
+    cpu_count = 1
+    if platform.system() == 'Windows':
+        cpu_count = 4
+
+    set_vm_params = [
+        'VBoxManage', 'modifyvm',
+        vm_uuid,
+        '--memory=1024',
+        '--firmware=efi',
+        f'--cpus={cpu_count}'
+    ]
+
+    set_vm_net = [
+        'VBoxManage', 'modifyvm',
+        vm_uuid,
+        '--nic1=natnetwork',
+        f'--nat-network1={network_name}'
+    ]
+
+    execute_command(create_vm_command)
+    execute_command(set_vm_params)
+    execute_command(set_vm_net)
+    _delete_controller(vm_uuid, 'SATA')
+    _delete_controller(vm_uuid, 'IDE')
+
+    _create_storage_controller(vm_uuid, 'SATA')
+
+    destination_image = str((_find_vm_location(vm_uuid) / disk_name).resolve())
+    copyfile(original_disk_path.absolute(), destination_image)
+
+    try:
+        _attach_disk(vm_uuid, 'SATA', disk_location=destination_image)
+    except AosProvError as error:
+        print_error(f'Cannot attach disk {destination_image} to VM. Clean up all related resources. Try again.')
+        os.remove(destination_image)
+        raise error
+
+
+def remove_vms_in_group(vm_name: str):
+    units_network_name = f'aos-network-{vm_name}'
+    vm_group = f'/AosUnits/{vm_name}'
+
+    print_message(f'Removing VMs in Groups: {vm_group} for the units...')
+
+    # find uuids of all VMs into the required Group
+    detailed_list_vms_command = [
+        'VBoxManage', 'list',
+        'vms',
+        '--long',
+    ]
+    detailed_list_vms_out = execute_command(detailed_list_vms_command, catch_error=True)
+    detailed_list_vms = dict(list())
+    processed_group_vm = ''
+    for output_line in detailed_list_vms_out.splitlines():
+        if output_line.startswith('Groups:'):
+            # line format is: 'Groups:                      /AosUnits/my-test-vm1'
+            if len(output_line.split()) == 2:
+                processed_group_vm = output_line.split()[1]
+        elif output_line.startswith('UUID:'):
+            # line format is: 'UUID:                        49f87eef-838b-43cb-b6eb-604989b15f9f'
+            if len(output_line.split()) == 2:
+                vm_uuid = output_line.split()[1]
+                list_of_uuids = []
+                if detailed_list_vms.get(processed_group_vm):
+                    list_of_uuids = detailed_list_vms[processed_group_vm]
+                if vm_uuid not in list_of_uuids:
+                    list_of_uuids.append(vm_uuid)
+                    detailed_list_vms[processed_group_vm] = list_of_uuids
+
+    _remove_network(units_network_name)
+
+    if not detailed_list_vms.get(vm_group):
+        print_error(f'VM Group: {vm_group} is not presented on system.')
+        return
+
+    for vm_uuid in detailed_list_vms[vm_group]:
+        delete_vm_command = [
+            'VBoxManage', 'unregistervm',
+            vm_uuid,
+            '--delete',
+        ]
+        execute_command(delete_vm_command, catch_error=False)
+    print_message('VMs have been deleted')
+
+
+def _find_vm_location(vm_uuid) -> Path:
+    set_vm_params = [
+        'VBoxManage', 'showvminfo',
+        vm_uuid,
+        '--machinereadable'
+    ]
+
+    response = execute_command(set_vm_params)
+
+    for row in response.splitlines():
+        param = row.split('=')
+        if param[0] == 'CfgFile':
+            return Path(param[1].replace('"', '')).parent
+
+
+def start_vms(group: str, check_virtualbox: bool = False, headless=False) -> None:
+    """Start all VMs in the group.
+
+    Args:
+        group (str): Name of the group to start
+        check_virtualbox (bool): Check VirtualBox status before execution
+        headless (bool): Start VM in headless mode if True
+    Raises:
+        AosProvError: If no VMs to start found.
+    Returns:
+        None
+    """
+    if check_virtualbox:
+        check_virtual_box()
+
+    message = f'Starting VMs in group [bold]{group}[/bold]'
+
+    if headless:
+        message += ' in headless mode'
+
+    print_message(message)
+    vms_to_start = []
+    vms = execute_command(['VBoxManage', 'list', 'vms'])
+
+    for vm in vms.splitlines():
+        guid = vm[vm.find('{')+1:vm.find('}')]
+        info_command = ['VBoxManage', 'showvminfo', guid, '--machinereadable']
+        info = execute_command(info_command)
+
+        for row in info.splitlines():
+            if row.startswith('groups='):
+                vm_group = row.replace('"', '').split('=')[1]
+                if group == vm_group:
+                    vms_to_start.append(guid)
+                    break
+
+    if len(vms_to_start) == 0:
+        raise AosProvError(f'No VMs found in group {group} to start!')
+
+    start_type = 'headless' if headless else 'gui'
+
+    for vm_guid in vms_to_start:
+        start_command = ['VBoxManage', 'startvm', vm_guid, f'--type={start_type}']
+        print_left(f'Starting VM {vm_guid}...')
+        try:
+            execute_command(start_command, catch_error=True)
+        except AosProvError as e:
+            if 'is already locked by a session' in str(e):
+                print_message('[YELLOW]SKIPPING due to lock')
+            else:
+                print_message('[RED]ERROR')
+                print_error(str(e))
+        print_done()
+
+
+def execute_command(command, catch_error=False) -> str:
+    execution_status = subprocess.run(command, shell=False, env=os.environ.copy(),  capture_output=True)
+    if execution_status.returncode == 0:
+        return execution_status.stdout.decode("utf-8")
+    else:
+        if not catch_error:
+            raise AosProvError(execution_status.stderr.decode("utf-8"))
```

## aos_prov/commands/download.py

 * *Ordering differences only*

```diff
@@ -1,116 +1,116 @@
-#
-#  Copyright (c) 2018-2023 Renesas Inc.
-#  Copyright (c) 2018-2023 EPAM Systems Inc.
-#
-"""Download and save files command."""
-import gzip
-import tarfile
-from pathlib import Path
-
-import requests
-from rich.progress import Progress
-
-from aos_prov.utils.common import DOWNLOADS_PATH, NODE0_IMAGE_FILENAME, NODE1_IMAGE_FILENAME
-from aos_prov.utils.errors import AosProvError
-
-_SAVE_CHUNK = 8192
-
-
-def _create_downloads_directory():
-    Path(DOWNLOADS_PATH).mkdir(parents=True, exist_ok=True)
-
-
-def _is_gz_file(filepath):
-    with open(filepath, 'rb') as test_f:
-        return test_f.read(2) == b'\x1f\x8b'
-
-
-def download_and_save_multinode(download_url: str, save_path: Path, force_overwrite: bool = False) -> None:
-    """Download and save multi-node images.
-
-    Args:
-         download_url (str): URL to download
-         save_path (Path): Save destination url
-         force_overwrite (bool): Force to overwrite files
-
-    Raises:
-        AosProvError: If files exists and force_overwrite is false.
-    """
-    _create_downloads_directory()
-
-    node_files = [save_path / NODE0_IMAGE_FILENAME, save_path / NODE1_IMAGE_FILENAME]
-
-    for node_file in node_files:
-        if force_overwrite:
-            node_file.unlink(True)
-        elif node_file.exists():
-            raise AosProvError(f'Destination file {node_file} already exist. Delete it or download with -f key')
-
-    download_file_name = save_path / 'downloaded-multi-node-images.tar.gz'
-
-    with open(download_file_name, 'wb') as save_context:
-        response = requests.get(download_url, stream=True)
-        total_length = response.headers.get('content-length')
-
-        if total_length is None:  # no content length header
-            save_context.write(response.content)
-            return
-
-        with Progress() as progress:
-            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
-            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
-                progress.update(task_id, advance=len(received_data))
-                save_context.write(received_data)
-
-    with tarfile.open(download_file_name) as archive:
-        archive.extractall(save_path)
-
-    download_file_name.unlink()
-
-
-def download_and_save_file(
-    download_url: str,
-    save_path: Path,
-    force_overwrite: bool = False,
-    untargz: bool = False
-) -> None:
-    """Download and save file.
-
-    Args:
-         download_url (str): URL to download
-         save_path (Path): URL to download
-         force_overwrite (bool): URL to download
-
-    Raises:
-        AosProvError: If file exists and force_overwrite is false.
-    """
-    _create_downloads_directory()
-
-    if save_path.exists() and not force_overwrite:
-        raise AosProvError('Destination file already exist.')
-
-    with open(save_path, 'wb') as save_context:
-        response = requests.get(download_url, stream=True)
-        total_length = response.headers.get('content-length')
-
-        if total_length is None:  # no content length header
-            save_context.write(response.content)
-            return
-
-        with Progress() as progress:
-            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
-            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
-                progress.update(task_id, advance=len(received_data))
-                save_context.write(received_data)
-
-    if untargz:
-        with tarfile.open(save_path) as archive:
-            archive.extractall(save_path)
-
-    elif _is_gz_file(save_path):
-        with gzip.open(save_path, 'rb') as f:
-            with open(DOWNLOADS_PATH / 'tmp_unpacked', 'wb') as tmp_file:
-                tmp_file.write(f.read())
-
-        Path(save_path).unlink()
-        Path(DOWNLOADS_PATH / 'tmp_unpacked').rename(save_path)
+#
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
+#
+"""Download and save files command."""
+import gzip
+import tarfile
+from pathlib import Path
+
+import requests
+from rich.progress import Progress
+
+from aos_prov.utils.common import DOWNLOADS_PATH, NODE0_IMAGE_FILENAME, NODE1_IMAGE_FILENAME
+from aos_prov.utils.errors import AosProvError
+
+_SAVE_CHUNK = 8192
+
+
+def _create_downloads_directory():
+    Path(DOWNLOADS_PATH).mkdir(parents=True, exist_ok=True)
+
+
+def _is_gz_file(filepath):
+    with open(filepath, 'rb') as test_f:
+        return test_f.read(2) == b'\x1f\x8b'
+
+
+def download_and_save_multinode(download_url: str, save_path: Path, force_overwrite: bool = False) -> None:
+    """Download and save multi-node images.
+
+    Args:
+         download_url (str): URL to download
+         save_path (Path): Save destination url
+         force_overwrite (bool): Force to overwrite files
+
+    Raises:
+        AosProvError: If files exists and force_overwrite is false.
+    """
+    _create_downloads_directory()
+
+    node_files = [save_path / NODE0_IMAGE_FILENAME, save_path / NODE1_IMAGE_FILENAME]
+
+    for node_file in node_files:
+        if force_overwrite:
+            node_file.unlink(True)
+        elif node_file.exists():
+            raise AosProvError(f'Destination file {node_file} already exist. Delete it or download with -f key')
+
+    download_file_name = save_path / 'downloaded-multi-node-images.tar.gz'
+
+    with open(download_file_name, 'wb') as save_context:
+        response = requests.get(download_url, stream=True)
+        total_length = response.headers.get('content-length')
+
+        if total_length is None:  # no content length header
+            save_context.write(response.content)
+            return
+
+        with Progress() as progress:
+            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
+            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
+                progress.update(task_id, advance=len(received_data))
+                save_context.write(received_data)
+
+    with tarfile.open(download_file_name) as archive:
+        archive.extractall(save_path)
+
+    download_file_name.unlink()
+
+
+def download_and_save_file(
+    download_url: str,
+    save_path: Path,
+    force_overwrite: bool = False,
+    untargz: bool = False
+) -> None:
+    """Download and save file.
+
+    Args:
+         download_url (str): URL to download
+         save_path (Path): URL to download
+         force_overwrite (bool): URL to download
+
+    Raises:
+        AosProvError: If file exists and force_overwrite is false.
+    """
+    _create_downloads_directory()
+
+    if save_path.exists() and not force_overwrite:
+        raise AosProvError('Destination file already exist.')
+
+    with open(save_path, 'wb') as save_context:
+        response = requests.get(download_url, stream=True)
+        total_length = response.headers.get('content-length')
+
+        if total_length is None:  # no content length header
+            save_context.write(response.content)
+            return
+
+        with Progress() as progress:
+            task_id = progress.add_task('[cyan]Downloading...', total=int(total_length))
+            for received_data in response.iter_content(chunk_size=_SAVE_CHUNK):
+                progress.update(task_id, advance=len(received_data))
+                save_context.write(received_data)
+
+    if untargz:
+        with tarfile.open(save_path) as archive:
+            archive.extractall(save_path)
+
+    elif _is_gz_file(save_path):
+        with gzip.open(save_path, 'rb') as f:
+            with open(DOWNLOADS_PATH / 'tmp_unpacked', 'wb') as tmp_file:
+                tmp_file.write(f.read())
+
+        Path(save_path).unlink()
+        Path(DOWNLOADS_PATH / 'tmp_unpacked').rename(save_path)
```

## aos_prov/communication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/cloud/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
```

## aos_prov/communication/cloud/cloud_api.py

 * *Ordering differences only*

```diff
@@ -1,183 +1,183 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-import logging
-import sys
-from urllib.parse import urlencode
-
-import OpenSSL
-import requests
-
-from aos_prov.utils.common import print_message, print_left, print_success
-
-if sys.version_info > (3, 9):
-    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
-else:
-    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
-
-from aos_prov.utils.errors import DeviceRegisterError, CloudAccessError
-from aos_prov.utils.user_credentials import UserCredentials
-
-logger = logging.getLogger(__name__)
-
-DEFAULT_REGISTER_HOST = 'aoscloud.io'
-DEFAULT_REGISTER_PORT = 10000
-
-
-class CloudAPI:
-    __FILES_DIR = 'aos_prov'
-    __ROOT_CA_CERT_FILENAME = 'files/1rootCA.crt'
-    __REGISTER_URI_TPL = 'https://{}:{}/api/v1/units/provisioning/'
-    __USER_ME_URI_TPL = 'https://{}:{}/api/v1/users/me/'
-    __UNIT_STATUS_URL = 'https://{}:{}/api/v1/units/?{}'
-    __FIND_UNIT_TPL = 'https://{}:{}/api/v1/units/?{}'
-    __LINK_TO_THE_UNIT_ON_CLOUD_TPL = 'https://{}/oem/units/{}'
-
-    def __init__(self, user_credentials: UserCredentials, cloud_api_port: int = DEFAULT_REGISTER_PORT):
-        self._cloud_api_host = user_credentials.cloud_url
-        self._cloud_api_port = cloud_api_port if cloud_api_port else DEFAULT_REGISTER_PORT
-        self._user_credentials = user_credentials
-
-    def check_cloud_access(self) -> None:
-        """Check user access on the cloud and his role is OEM.
-
-        Raises:
-            CloudAccessError: If user haven't access to the cloud or his role is not OEM.
-        Returns:
-            None
-        """
-        try:
-            url = self.__USER_ME_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    resp = requests.get(url, verify=server_certificate_path,
-                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-
-                if resp.status_code != 200:
-                    print_message('[red]Received not HTTP 200 response. ' + str(resp.text))
-                    raise CloudAccessError('You do not have access to the cloud!')
-
-                user_info = resp.json()
-                if user_info['role'] != 'oem':
-                    print_message(f'[red]invalid user role: {resp.text}')
-                    raise CloudAccessError('You should use OEM account!')
-
-            print_left('Operation will be executed on domain:')
-            print_success(self._cloud_api_host)
-            print_left('OEM:')
-            print_success(user_info["oem"]["title"])
-            print_left('user:')
-            print_success(user_info["username"])
-        except ConnectionError as e:
-            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(e))
-        except (requests.exceptions.RequestException, ValueError, OSError, OpenSSL.SSL.Error) as e:
-            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(e) )
-
-
-    def register_device(self, payload):
-        """Registers device in cloud. Returns registered metadata.
-        :param: str - end_point for registering
-        :param: str - path to server pem that contains certs and a private one
-        :param: dict
-        :return: dict
-        """
-        logger.info('Registering the unit ...')
-        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-
-        try:
-            logger.debug('Sending to %s payload: %s', end_point, payload)
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    ret = requests.post(end_point, json=payload, verify=server_certificate_path,
-                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-
-                    if ret.status_code == 400:
-                        try:
-                            resp_content = ret.content.decode()
-                            print(str(resp_content))
-                            try:
-                                answer = ret.json()['non_field_errors'][0]
-                                logger.info('Registration error: ' + answer)
-                            except:
-                                pass
-
-                        except UnicodeDecodeError:
-                            resp_content = ret.content
-                            print(resp_content)
-                        logger.debug('Cloud response: {}'.format(resp_content))
-                    ret.raise_for_status()
-                    response = ret.json()
-        except (requests.exceptions.RequestException,
-                ValueError, OSError, OpenSSL.SSL.Error) as e:
-            logger.debug(e)
-            print(e)
-            raise DeviceRegisterError('Failed to register unit.')
-
-        return response
-
-    def check_unit_is_not_provisioned(self, system_uid):
-        print('Getting unit\'s status on the cloud ...')
-        try:
-            end_point = self.__UNIT_STATUS_URL.format(
-                self._cloud_api_host,
-                self._cloud_api_port,
-                urlencode({'system_uid': system_uid})
-            )
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    response = requests.get(end_point, verify=server_certificate_path,
-                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-
-        except (requests.exceptions.RequestException,
-                ValueError, OSError, OpenSSL.SSL.Error) as e:
-            print('Failed to check unit\'s status: %s', e)
-            raise DeviceRegisterError('Failed to HTTP GET: ', e)
-
-        response_json = response.json()
-
-        if 'results' not in response_json or 'count' not in response_json:
-            raise DeviceRegisterError('Invalid answer from the cloud. Please update current library')
-
-        if response_json['count'] == 0:
-            # There is no such unit on the cloud
-            return
-
-        status = response_json.get('results', [{}])[0].get('status')
-        if status is None:
-            return
-
-        if status != 'new':
-            raise DeviceRegisterError(f'Unit is in status "{status}". Please do deprovisioning first.')
-
-    def get_unit_link_by_system_uid(self, system_uid):
-        end_point = self.__FIND_UNIT_TPL.format(
-            self._cloud_api_host,
-            self._cloud_api_port,
-            urlencode({'system_uid': system_uid})
-        )
-        try:
-            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-            with pkg_resources.as_file(server_certificate) as server_certificate_path:
-                with self._user_credentials.user_credentials as temp_creds:
-                    response = requests.get(end_point, verify=server_certificate_path,
-                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-            unit_id = response.json()['results'][0]['id']
-            unit_domain = self._cloud_api_host
-            if not unit_domain.startswith('oem.'):
-                unit_domain = f'oem.{unit_domain}'
-            return self.__LINK_TO_THE_UNIT_ON_CLOUD_TPL.format(unit_domain, unit_id)
-        except Exception:
-            return None
-
-    def use_model_name_param(self) -> bool:
-        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
-        server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
-        with pkg_resources.as_file(server_certificate) as server_certificate_path:
-            with self._user_credentials.user_credentials as temp_creds:
-                resp = requests.options(end_point, verify=server_certificate_path,
-                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
-                return 'model_name' in resp.json()['actions']['POST']
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+import logging
+import sys
+from urllib.parse import urlencode
+
+import OpenSSL
+import requests
+
+from aos_prov.utils.common import print_message, print_left, print_success
+
+if sys.version_info > (3, 9):
+    from importlib import resources as pkg_resources  # noqa: WPS433, WPS440
+else:
+    import importlib_resources as pkg_resources  # noqa: WPS433, WPS440
+
+from aos_prov.utils.errors import DeviceRegisterError, CloudAccessError
+from aos_prov.utils.user_credentials import UserCredentials
+
+logger = logging.getLogger(__name__)
+
+DEFAULT_REGISTER_HOST = 'aoscloud.io'
+DEFAULT_REGISTER_PORT = 10000
+
+
+class CloudAPI:
+    __FILES_DIR = 'aos_prov'
+    __ROOT_CA_CERT_FILENAME = 'files/1rootCA.crt'
+    __REGISTER_URI_TPL = 'https://{}:{}/api/v1/units/provisioning/'
+    __USER_ME_URI_TPL = 'https://{}:{}/api/v1/users/me/'
+    __UNIT_STATUS_URL = 'https://{}:{}/api/v1/units/?{}'
+    __FIND_UNIT_TPL = 'https://{}:{}/api/v1/units/?{}'
+    __LINK_TO_THE_UNIT_ON_CLOUD_TPL = 'https://{}/oem/units/{}'
+
+    def __init__(self, user_credentials: UserCredentials, cloud_api_port: int = DEFAULT_REGISTER_PORT):
+        self._cloud_api_host = user_credentials.cloud_url
+        self._cloud_api_port = cloud_api_port if cloud_api_port else DEFAULT_REGISTER_PORT
+        self._user_credentials = user_credentials
+
+    def check_cloud_access(self) -> None:
+        """Check user access on the cloud and his role is OEM.
+
+        Raises:
+            CloudAccessError: If user haven't access to the cloud or his role is not OEM.
+        Returns:
+            None
+        """
+        try:
+            url = self.__USER_ME_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    resp = requests.get(url, verify=server_certificate_path,
+                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+
+                if resp.status_code != 200:
+                    print_message('[red]Received not HTTP 200 response. ' + str(resp.text))
+                    raise CloudAccessError('You do not have access to the cloud!')
+
+                user_info = resp.json()
+                if user_info['role'] != 'oem':
+                    print_message(f'[red]invalid user role: {resp.text}')
+                    raise CloudAccessError('You should use OEM account!')
+
+            print_left('Operation will be executed on domain:')
+            print_success(self._cloud_api_host)
+            print_left('OEM:')
+            print_success(user_info["oem"]["title"])
+            print_left('user:')
+            print_success(user_info["username"])
+        except ConnectionError as e:
+            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(e))
+        except (requests.exceptions.RequestException, ValueError, OSError, OpenSSL.SSL.Error) as e:
+            raise CloudAccessError('Failed to connect to the cloud with error: ' + str(e) )
+
+
+    def register_device(self, payload):
+        """Registers device in cloud. Returns registered metadata.
+        :param: str - end_point for registering
+        :param: str - path to server pem that contains certs and a private one
+        :param: dict
+        :return: dict
+        """
+        logger.info('Registering the unit ...')
+        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+
+        try:
+            logger.debug('Sending to %s payload: %s', end_point, payload)
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    ret = requests.post(end_point, json=payload, verify=server_certificate_path,
+                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+
+                    if ret.status_code == 400:
+                        try:
+                            resp_content = ret.content.decode()
+                            print(str(resp_content))
+                            try:
+                                answer = ret.json()['non_field_errors'][0]
+                                logger.info('Registration error: ' + answer)
+                            except:
+                                pass
+
+                        except UnicodeDecodeError:
+                            resp_content = ret.content
+                            print(resp_content)
+                        logger.debug('Cloud response: {}'.format(resp_content))
+                    ret.raise_for_status()
+                    response = ret.json()
+        except (requests.exceptions.RequestException,
+                ValueError, OSError, OpenSSL.SSL.Error) as e:
+            logger.debug(e)
+            print(e)
+            raise DeviceRegisterError('Failed to register unit.')
+
+        return response
+
+    def check_unit_is_not_provisioned(self, system_uid):
+        print('Getting unit\'s status on the cloud ...')
+        try:
+            end_point = self.__UNIT_STATUS_URL.format(
+                self._cloud_api_host,
+                self._cloud_api_port,
+                urlencode({'system_uid': system_uid})
+            )
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    response = requests.get(end_point, verify=server_certificate_path,
+                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+
+        except (requests.exceptions.RequestException,
+                ValueError, OSError, OpenSSL.SSL.Error) as e:
+            print('Failed to check unit\'s status: %s', e)
+            raise DeviceRegisterError('Failed to HTTP GET: ', e)
+
+        response_json = response.json()
+
+        if 'results' not in response_json or 'count' not in response_json:
+            raise DeviceRegisterError('Invalid answer from the cloud. Please update current library')
+
+        if response_json['count'] == 0:
+            # There is no such unit on the cloud
+            return
+
+        status = response_json.get('results', [{}])[0].get('status')
+        if status is None:
+            return
+
+        if status != 'new':
+            raise DeviceRegisterError(f'Unit is in status "{status}". Please do deprovisioning first.')
+
+    def get_unit_link_by_system_uid(self, system_uid):
+        end_point = self.__FIND_UNIT_TPL.format(
+            self._cloud_api_host,
+            self._cloud_api_port,
+            urlencode({'system_uid': system_uid})
+        )
+        try:
+            server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+            with pkg_resources.as_file(server_certificate) as server_certificate_path:
+                with self._user_credentials.user_credentials as temp_creds:
+                    response = requests.get(end_point, verify=server_certificate_path,
+                                            cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+            unit_id = response.json()['results'][0]['id']
+            unit_domain = self._cloud_api_host
+            if not unit_domain.startswith('oem.'):
+                unit_domain = f'oem.{unit_domain}'
+            return self.__LINK_TO_THE_UNIT_ON_CLOUD_TPL.format(unit_domain, unit_id)
+        except Exception:
+            return None
+
+    def use_model_name_param(self) -> bool:
+        end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
+        server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
+        with pkg_resources.as_file(server_certificate) as server_certificate_path:
+            with self._user_credentials.user_credentials as temp_creds:
+                resp = requests.options(end_point, verify=server_certificate_path,
+                                        cert=(temp_creds.cert_file_name, temp_creds.key_file_name))
+                return 'model_name' in resp.json()['actions']['POST']
```

## aos_prov/communication/unit/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v0/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v1/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
```

## aos_prov/communication/unit/v4/unit_communication_v4.py

 * *Ordering differences only*

```diff
@@ -1,221 +1,221 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-from contextlib import contextmanager
-
-import grpc
-from google.protobuf import empty_pb2
-
-from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iam_manager
-from aos_prov.communication.unit.v4.generated import iamanager_pb2_grpc as iam_manager_grpc
-from aos_prov.utils.common import print_message, print_done, print_left, print_success
-from aos_prov.utils.errors import UnitError, GrpcUnimplemented
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-UNIT_DEFAULT_PORT = 8089
-
-
-class UnitCommunicationV4:
-    def __init__(self, address: str = 'localhost:8089'):
-        self._need_set_users = False
-
-        if address is None:
-            address = 'localhost:8089'
-        parts = address.split(':')
-        if len(parts) == 2:
-            try:
-                port = int(parts[1])
-                if not 1 <= port <= 65535:
-                    raise UnitError('Unit port is invalid')
-            except ValueError:
-                raise UnitError('Unit port is invalid')
-        else:
-            address = address + ':' + str(UNIT_DEFAULT_PORT)
-        self.__unit_address = address
-        print_message(f'Will search unit on address: [green]{self.__unit_address}')
-
-    @property
-    def need_set_users(self):
-        return self._need_set_users
-
-    @need_set_users.setter
-    def need_set_users(self, value):
-        self._need_set_users = value
-
-    @contextmanager
-    def unit_certificate_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMCertificateServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
-
-    @contextmanager
-    def unit_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
-
-    @contextmanager
-    def unit_identify_stub(self):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicIdentityServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as e:
-            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
-                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
-            else:
-                raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
-
-    @contextmanager
-    def unit_provisioning_stub(self, catch_inactive=False, wait_for_close=False):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMProvisioningServiceStub(channel)
-                if wait_for_close:
-                    def _stop_wait(state):
-                        if state is grpc.ChannelConnectivity.SHUTDOWN:
-                            channel.unsubscribe(_stop_wait)
-                            return
-                    channel.subscribe(_stop_wait, try_to_connect=False)
-                yield stub
-
-        except grpc.RpcError as e:
-            if catch_inactive and \
-                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
-                return
-            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
-                return
-            raise UnitError(f"Error occurred: \n{e.code()}: {e.details()}")
-
-    @contextmanager
-    def unit_public_stub(self):
-        try:
-            with grpc.insecure_channel(self.__unit_address) as channel:
-                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
-                yield stub
-
-        except grpc.RpcError as e:
-            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
-                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
-            else:
-                raise UnitError(f"Error occurred: \n{e.code()}: {e.details()}")
-
-    def get_protocol_version(self) -> int:
-        with self.unit_public_stub() as stub:
-            print_left('Getting protocol version...')
-            response = stub.GetAPIVersion(empty_pb2.Empty())
-            print_success(str(response.version))
-            return int(response.version)
-
-    def get_system_info(self) -> (str, str):
-        with self.unit_identify_stub() as stub:
-            print_left('Getting System Info...')
-            response = stub.GetSystemInfo(empty_pb2.Empty())
-            print_done()
-            print_left('System ID:')
-            print_success(response.system_id)
-            print_left('Model name:')
-            print_success(response.board_model)
-            return response.system_id, response.board_model
-
-    def clear(self, certificate_type: str, node_id: str) -> None:
-        with self.unit_provisioning_stub() as stub:
-            print_left(f'Clearing certificate: {certificate_type} on Node ID: {node_id}...')
-            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type, node_id=node_id))
-            print_done()
-            return response
-
-    def set_cert_owner(self, certificate_type: str, password: str, node_id: str) -> None:
-        with self.unit_provisioning_stub() as stub:
-            print_left(f'Setting owner for: {certificate_type} on Node ID: {node_id}...')
-            response = stub.SetOwner(
-                iam_manager.SetOwnerRequest(type=certificate_type, password=password, node_id=node_id),
-            )
-            print_done()
-            return response
-
-    def get_all_node_ids(self) -> [str]:
-        with self.unit_provisioning_stub() as stub:
-            print_left('Getting Node IDs...')
-            response = stub.GetAllNodeIDs(empty_pb2.Empty())
-            print_success(response.ids)
-            return response.ids
-
-    def get_cert_types(self, node_id: str) -> [str]:
-        with self.unit_provisioning_stub() as stub:
-            print_left(f'Getting certificate types to renew on node {node_id}...')
-            response = stub.GetCertTypes(iam_manager.GetCertTypesRequest(node_id=node_id))
-            print_success(response.types)
-            return response.types
-
-    def create_keys(self, cert_type: str, password: str, node_id: str) -> UnitCertificate:
-        with self.unit_certificate_stub() as stub:
-            print_left(f'Generating key type: {cert_type} on Node: {node_id}...')
-            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password, node_id=node_id))
-            uc = UnitCertificate()
-            uc.cert_type = response.type
-            uc.node_id = response.node_id
-            uc.csr = response.csr
-            print_done()
-            return uc
-
-    def apply_certificate(self, unit_cert: UnitCertificate):
-        with self.unit_certificate_stub() as stub:
-            node_id = ''
-            if unit_cert.node_id:
-                node_id = str(unit_cert.node_id)
-            print_left(f'Applying certificate type: {unit_cert.cert_type} Node ID: {node_id}...')
-            stub.ApplyCert(iam_manager.ApplyCertRequest(
-                type=unit_cert.cert_type,
-                cert=unit_cert.certificate,
-                node_id=node_id,
-            ))
-            print_done()
-
-    def encrypt_disk(self, password: str, node_id: str):
-        print_left(f'Starting disk encryption on node {node_id}...')
-        try:
-            with self.unit_provisioning_stub(wait_for_close=False) as stub:
-                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password, node_id=node_id))
-                print_done()
-        except UnitError as be:
-            print_message(f'[red] Error.')
-            print_message(be)
-
-    def finish_provisioning(self):
-        with self.unit_provisioning_stub(True) as stub:
-            print_left('Finishing provisioning...')
-            stub.FinishProvisioning(empty_pb2.Empty())
-            print_done()
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+from contextlib import contextmanager
+
+import grpc
+from google.protobuf import empty_pb2
+
+from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iam_manager
+from aos_prov.communication.unit.v4.generated import iamanager_pb2_grpc as iam_manager_grpc
+from aos_prov.utils.common import print_message, print_done, print_left, print_success
+from aos_prov.utils.errors import UnitError, GrpcUnimplemented
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+UNIT_DEFAULT_PORT = 8089
+
+
+class UnitCommunicationV4:
+    def __init__(self, address: str = 'localhost:8089'):
+        self._need_set_users = False
+
+        if address is None:
+            address = 'localhost:8089'
+        parts = address.split(':')
+        if len(parts) == 2:
+            try:
+                port = int(parts[1])
+                if not 1 <= port <= 65535:
+                    raise UnitError('Unit port is invalid')
+            except ValueError:
+                raise UnitError('Unit port is invalid')
+        else:
+            address = address + ':' + str(UNIT_DEFAULT_PORT)
+        self.__unit_address = address
+        print_message(f'Will search unit on address: [green]{self.__unit_address}')
+
+    @property
+    def need_set_users(self):
+        return self._need_set_users
+
+    @need_set_users.setter
+    def need_set_users(self, value):
+        self._need_set_users = value
+
+    @contextmanager
+    def unit_certificate_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMCertificateServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_identify_stub(self):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicIdentityServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as e:
+            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
+            else:
+                raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_provisioning_stub(self, catch_inactive=False, wait_for_close=False):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMProvisioningServiceStub(channel)
+                if wait_for_close:
+                    def _stop_wait(state):
+                        if state is grpc.ChannelConnectivity.SHUTDOWN:
+                            channel.unsubscribe(_stop_wait)
+                            return
+                    channel.subscribe(_stop_wait, try_to_connect=False)
+                yield stub
+
+        except grpc.RpcError as e:
+            if catch_inactive and \
+                    not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
+                return
+            elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
+                return
+            raise UnitError(f"Error occurred: \n{e.code()}: {e.details()}")
+
+    @contextmanager
+    def unit_public_stub(self):
+        try:
+            with grpc.insecure_channel(self.__unit_address) as channel:
+                stub = iam_manager_grpc.IAMPublicServiceStub(channel)
+                yield stub
+
+        except grpc.RpcError as e:
+            if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
+                raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
+            else:
+                raise UnitError(f"Error occurred: \n{e.code()}: {e.details()}")
+
+    def get_protocol_version(self) -> int:
+        with self.unit_public_stub() as stub:
+            print_left('Getting protocol version...')
+            response = stub.GetAPIVersion(empty_pb2.Empty())
+            print_success(str(response.version))
+            return int(response.version)
+
+    def get_system_info(self) -> (str, str):
+        with self.unit_identify_stub() as stub:
+            print_left('Getting System Info...')
+            response = stub.GetSystemInfo(empty_pb2.Empty())
+            print_done()
+            print_left('System ID:')
+            print_success(response.system_id)
+            print_left('Model name:')
+            print_success(response.board_model)
+            return response.system_id, response.board_model
+
+    def clear(self, certificate_type: str, node_id: str) -> None:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Clearing certificate: {certificate_type} on Node ID: {node_id}...')
+            response = stub.Clear(iam_manager.ClearRequest(type=certificate_type, node_id=node_id))
+            print_done()
+            return response
+
+    def set_cert_owner(self, certificate_type: str, password: str, node_id: str) -> None:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Setting owner for: {certificate_type} on Node ID: {node_id}...')
+            response = stub.SetOwner(
+                iam_manager.SetOwnerRequest(type=certificate_type, password=password, node_id=node_id),
+            )
+            print_done()
+            return response
+
+    def get_all_node_ids(self) -> [str]:
+        with self.unit_provisioning_stub() as stub:
+            print_left('Getting Node IDs...')
+            response = stub.GetAllNodeIDs(empty_pb2.Empty())
+            print_success(response.ids)
+            return response.ids
+
+    def get_cert_types(self, node_id: str) -> [str]:
+        with self.unit_provisioning_stub() as stub:
+            print_left(f'Getting certificate types to renew on node {node_id}...')
+            response = stub.GetCertTypes(iam_manager.GetCertTypesRequest(node_id=node_id))
+            print_success(response.types)
+            return response.types
+
+    def create_keys(self, cert_type: str, password: str, node_id: str) -> UnitCertificate:
+        with self.unit_certificate_stub() as stub:
+            print_left(f'Generating key type: {cert_type} on Node: {node_id}...')
+            response = stub.CreateKey(iam_manager.CreateKeyRequest(type=cert_type, password=password, node_id=node_id))
+            uc = UnitCertificate()
+            uc.cert_type = response.type
+            uc.node_id = response.node_id
+            uc.csr = response.csr
+            print_done()
+            return uc
+
+    def apply_certificate(self, unit_cert: UnitCertificate):
+        with self.unit_certificate_stub() as stub:
+            node_id = ''
+            if unit_cert.node_id:
+                node_id = str(unit_cert.node_id)
+            print_left(f'Applying certificate type: {unit_cert.cert_type} Node ID: {node_id}...')
+            stub.ApplyCert(iam_manager.ApplyCertRequest(
+                type=unit_cert.cert_type,
+                cert=unit_cert.certificate,
+                node_id=node_id,
+            ))
+            print_done()
+
+    def encrypt_disk(self, password: str, node_id: str):
+        print_left(f'Starting disk encryption on node {node_id}...')
+        try:
+            with self.unit_provisioning_stub(wait_for_close=False) as stub:
+                stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password, node_id=node_id))
+                print_done()
+        except UnitError as be:
+            print_message(f'[red] Error.')
+            print_message(be)
+
+    def finish_provisioning(self):
+        with self.unit_provisioning_stub(True) as stub:
+            print_left('Finishing provisioning...')
+            stub.FinishProvisioning(empty_pb2.Empty())
+            print_done()
```

## aos_prov/communication/unit/v4/generated/iamanager_pb2.py

 * *Ordering differences only*

```diff
@@ -1,299 +1,299 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iamanager/v4/iamanager.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ciamanager/v4/iamanager.proto\x12\x0ciamanager.v4\x1a\x1bgoogle/protobuf/empty.proto\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\"\x19\n\x06NodeID\x12\x0f\n\x07node_id\x18\x01 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x08Subjects\x12\x10\n\x08subjects\x18\x01 \x03(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"I\n\rInstanceIdent\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x12\n\nsubject_id\x18\x02 \x01(\t\x12\x10\n\x08instance\x18\x03 \x01(\x04\"t\n\x13PermissionsResponse\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions\"\x16\n\x07NodesID\x12\x0b\n\x03ids\x18\x01 \x03(\t\"&\n\x13GetCertTypesRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"B\n\x0fSetOwnerRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"-\n\x0c\x43learRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"7\n\x12\x45ncryptDiskRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"T\n\x10\x43reateKeyRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"?\n\x11\x43reateKeyResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03\x63sr\x18\x03 \x01(\t\"?\n\x10\x41pplyCertRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x03 \x01(\t\"D\n\x11\x41pplyCertResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x03 \x01(\t\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v4.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x17RegisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12K\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x36.iamanager.v4.RegisterInstanceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions:\x02\x38\x01\"*\n\x18RegisterInstanceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\"J\n\x19UnregisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent2\xde\x01\n\x10IAMPublicService\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.APIVersion\"\x00\x12;\n\tGetNodeID\x12\x16.google.protobuf.Empty\x1a\x14.iamanager.v4.NodeID\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v4.GetCertRequest\x1a\x1d.iamanager.v4.GetCertResponse\"\x00\x32\xf0\x01\n\x18IAMPublicIdentityService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.SystemInfo\"\x00\x12?\n\x0bGetSubjects\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x12N\n\x18SubscribeSubjectsChanged\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x30\x01\x32v\n\x1bIAMPublicPermissionsService\x12W\n\x0eGetPermissions\x12 .iamanager.v4.PermissionsRequest\x1a!.iamanager.v4.PermissionsResponse\"\x00\x32\xbf\x03\n\x16IAMProvisioningService\x12@\n\rGetAllNodeIDs\x12\x16.google.protobuf.Empty\x1a\x15.iamanager.v4.NodesID\"\x00\x12L\n\x0cGetCertTypes\x12!.iamanager.v4.GetCertTypesRequest\x1a\x17.iamanager.v4.CertTypes\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v4.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v4.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v4.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x15IAMCertificateService\x12N\n\tCreateKey\x12\x1e.iamanager.v4.CreateKeyRequest\x1a\x1f.iamanager.v4.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v4.ApplyCertRequest\x1a\x1f.iamanager.v4.ApplyCertResponse\"\x00\x32\xd5\x01\n\x15IAMPermissionsService\x12\x63\n\x10RegisterInstance\x12%.iamanager.v4.RegisterInstanceRequest\x1a&.iamanager.v4.RegisterInstanceResponse\"\x00\x12W\n\x12UnregisterInstance\x12\'.iamanager.v4.UnregisterInstanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
-
-
-
-_APIVERSION = DESCRIPTOR.message_types_by_name['APIVersion']
-_NODEID = DESCRIPTOR.message_types_by_name['NodeID']
-_GETCERTREQUEST = DESCRIPTOR.message_types_by_name['GetCertRequest']
-_GETCERTRESPONSE = DESCRIPTOR.message_types_by_name['GetCertResponse']
-_SYSTEMINFO = DESCRIPTOR.message_types_by_name['SystemInfo']
-_SUBJECTS = DESCRIPTOR.message_types_by_name['Subjects']
-_PERMISSIONSREQUEST = DESCRIPTOR.message_types_by_name['PermissionsRequest']
-_INSTANCEIDENT = DESCRIPTOR.message_types_by_name['InstanceIdent']
-_PERMISSIONSRESPONSE = DESCRIPTOR.message_types_by_name['PermissionsResponse']
-_NODESID = DESCRIPTOR.message_types_by_name['NodesID']
-_GETCERTTYPESREQUEST = DESCRIPTOR.message_types_by_name['GetCertTypesRequest']
-_CERTTYPES = DESCRIPTOR.message_types_by_name['CertTypes']
-_SETOWNERREQUEST = DESCRIPTOR.message_types_by_name['SetOwnerRequest']
-_CLEARREQUEST = DESCRIPTOR.message_types_by_name['ClearRequest']
-_ENCRYPTDISKREQUEST = DESCRIPTOR.message_types_by_name['EncryptDiskRequest']
-_CREATEKEYREQUEST = DESCRIPTOR.message_types_by_name['CreateKeyRequest']
-_CREATEKEYRESPONSE = DESCRIPTOR.message_types_by_name['CreateKeyResponse']
-_APPLYCERTREQUEST = DESCRIPTOR.message_types_by_name['ApplyCertRequest']
-_APPLYCERTRESPONSE = DESCRIPTOR.message_types_by_name['ApplyCertResponse']
-_PERMISSIONS = DESCRIPTOR.message_types_by_name['Permissions']
-_PERMISSIONS_PERMISSIONSENTRY = _PERMISSIONS.nested_types_by_name['PermissionsEntry']
-_REGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['RegisterInstanceRequest']
-_REGISTERINSTANCEREQUEST_PERMISSIONSENTRY = _REGISTERINSTANCEREQUEST.nested_types_by_name['PermissionsEntry']
-_REGISTERINSTANCERESPONSE = DESCRIPTOR.message_types_by_name['RegisterInstanceResponse']
-_UNREGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['UnregisterInstanceRequest']
-APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
-  'DESCRIPTOR' : _APIVERSION,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.APIVersion)
-  })
-_sym_db.RegisterMessage(APIVersion)
-
-NodeID = _reflection.GeneratedProtocolMessageType('NodeID', (_message.Message,), {
-  'DESCRIPTOR' : _NODEID,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.NodeID)
-  })
-_sym_db.RegisterMessage(NodeID)
-
-GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertRequest)
-  })
-_sym_db.RegisterMessage(GetCertRequest)
-
-GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertResponse)
-  })
-_sym_db.RegisterMessage(GetCertResponse)
-
-SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMINFO,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.SystemInfo)
-  })
-_sym_db.RegisterMessage(SystemInfo)
-
-Subjects = _reflection.GeneratedProtocolMessageType('Subjects', (_message.Message,), {
-  'DESCRIPTOR' : _SUBJECTS,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.Subjects)
-  })
-_sym_db.RegisterMessage(Subjects)
-
-PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsRequest)
-  })
-_sym_db.RegisterMessage(PermissionsRequest)
-
-InstanceIdent = _reflection.GeneratedProtocolMessageType('InstanceIdent', (_message.Message,), {
-  'DESCRIPTOR' : _INSTANCEIDENT,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.InstanceIdent)
-  })
-_sym_db.RegisterMessage(InstanceIdent)
-
-PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsResponse)
-  })
-_sym_db.RegisterMessage(PermissionsResponse)
-
-NodesID = _reflection.GeneratedProtocolMessageType('NodesID', (_message.Message,), {
-  'DESCRIPTOR' : _NODESID,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.NodesID)
-  })
-_sym_db.RegisterMessage(NodesID)
-
-GetCertTypesRequest = _reflection.GeneratedProtocolMessageType('GetCertTypesRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCERTTYPESREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertTypesRequest)
-  })
-_sym_db.RegisterMessage(GetCertTypesRequest)
-
-CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
-  'DESCRIPTOR' : _CERTTYPES,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CertTypes)
-  })
-_sym_db.RegisterMessage(CertTypes)
-
-SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SETOWNERREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.SetOwnerRequest)
-  })
-_sym_db.RegisterMessage(SetOwnerRequest)
-
-ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CLEARREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ClearRequest)
-  })
-_sym_db.RegisterMessage(ClearRequest)
-
-EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.EncryptDiskRequest)
-  })
-_sym_db.RegisterMessage(EncryptDiskRequest)
-
-CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyRequest)
-  })
-_sym_db.RegisterMessage(CreateKeyRequest)
-
-CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEKEYRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyResponse)
-  })
-_sym_db.RegisterMessage(CreateKeyResponse)
-
-ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertRequest)
-  })
-_sym_db.RegisterMessage(ApplyCertRequest)
-
-ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTRESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertResponse)
-  })
-_sym_db.RegisterMessage(ApplyCertResponse)
-
-Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v4.iamanager_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _PERMISSIONS,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions)
-  })
-_sym_db.RegisterMessage(Permissions)
-_sym_db.RegisterMessage(Permissions.PermissionsEntry)
-
-RegisterInstanceRequest = _reflection.GeneratedProtocolMessageType('RegisterInstanceRequest', (_message.Message,), {
-
-  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY,
-    '__module__' : 'iamanager.v4.iamanager_pb2'
-    # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest.PermissionsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _REGISTERINSTANCEREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest)
-  })
-_sym_db.RegisterMessage(RegisterInstanceRequest)
-_sym_db.RegisterMessage(RegisterInstanceRequest.PermissionsEntry)
-
-RegisterInstanceResponse = _reflection.GeneratedProtocolMessageType('RegisterInstanceResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REGISTERINSTANCERESPONSE,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceResponse)
-  })
-_sym_db.RegisterMessage(RegisterInstanceResponse)
-
-UnregisterInstanceRequest = _reflection.GeneratedProtocolMessageType('UnregisterInstanceRequest', (_message.Message,), {
-  'DESCRIPTOR' : _UNREGISTERINSTANCEREQUEST,
-  '__module__' : 'iamanager.v4.iamanager_pb2'
-  # @@protoc_insertion_point(class_scope:iamanager.v4.UnregisterInstanceRequest)
-  })
-_sym_db.RegisterMessage(UnregisterInstanceRequest)
-
-_IAMPUBLICSERVICE = DESCRIPTOR.services_by_name['IAMPublicService']
-_IAMPUBLICIDENTITYSERVICE = DESCRIPTOR.services_by_name['IAMPublicIdentityService']
-_IAMPUBLICPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPublicPermissionsService']
-_IAMPROVISIONINGSERVICE = DESCRIPTOR.services_by_name['IAMProvisioningService']
-_IAMCERTIFICATESERVICE = DESCRIPTOR.services_by_name['IAMCertificateService']
-_IAMPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPermissionsService']
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _PERMISSIONS_PERMISSIONSENTRY._options = None
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_options = b'8\001'
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._options = None
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_options = b'8\001'
-  _APIVERSION._serialized_start=75
-  _APIVERSION._serialized_end=104
-  _NODEID._serialized_start=106
-  _NODEID._serialized_end=131
-  _GETCERTREQUEST._serialized_start=133
-  _GETCERTREQUEST._serialized_end=195
-  _GETCERTRESPONSE._serialized_start=197
-  _GETCERTRESPONSE._serialized_end=263
-  _SYSTEMINFO._serialized_start=265
-  _SYSTEMINFO._serialized_end=317
-  _SUBJECTS._serialized_start=319
-  _SUBJECTS._serialized_end=347
-  _PERMISSIONSREQUEST._serialized_start=349
-  _PERMISSIONSREQUEST._serialized_end=415
-  _INSTANCEIDENT._serialized_start=417
-  _INSTANCEIDENT._serialized_end=490
-  _PERMISSIONSRESPONSE._serialized_start=492
-  _PERMISSIONSRESPONSE._serialized_end=608
-  _NODESID._serialized_start=610
-  _NODESID._serialized_end=632
-  _GETCERTTYPESREQUEST._serialized_start=634
-  _GETCERTTYPESREQUEST._serialized_end=672
-  _CERTTYPES._serialized_start=674
-  _CERTTYPES._serialized_end=700
-  _SETOWNERREQUEST._serialized_start=702
-  _SETOWNERREQUEST._serialized_end=768
-  _CLEARREQUEST._serialized_start=770
-  _CLEARREQUEST._serialized_end=815
-  _ENCRYPTDISKREQUEST._serialized_start=817
-  _ENCRYPTDISKREQUEST._serialized_end=872
-  _CREATEKEYREQUEST._serialized_start=874
-  _CREATEKEYREQUEST._serialized_end=958
-  _CREATEKEYRESPONSE._serialized_start=960
-  _CREATEKEYRESPONSE._serialized_end=1023
-  _APPLYCERTREQUEST._serialized_start=1025
-  _APPLYCERTREQUEST._serialized_end=1088
-  _APPLYCERTRESPONSE._serialized_start=1090
-  _APPLYCERTRESPONSE._serialized_end=1158
-  _PERMISSIONS._serialized_start=1161
-  _PERMISSIONS._serialized_end=1291
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_start=1241
-  _PERMISSIONS_PERMISSIONSENTRY._serialized_end=1291
-  _REGISTERINSTANCEREQUEST._serialized_start=1294
-  _REGISTERINSTANCEREQUEST._serialized_end=1522
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_start=1445
-  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_end=1522
-  _REGISTERINSTANCERESPONSE._serialized_start=1524
-  _REGISTERINSTANCERESPONSE._serialized_end=1566
-  _UNREGISTERINSTANCEREQUEST._serialized_start=1568
-  _UNREGISTERINSTANCEREQUEST._serialized_end=1642
-  _IAMPUBLICSERVICE._serialized_start=1645
-  _IAMPUBLICSERVICE._serialized_end=1867
-  _IAMPUBLICIDENTITYSERVICE._serialized_start=1870
-  _IAMPUBLICIDENTITYSERVICE._serialized_end=2110
-  _IAMPUBLICPERMISSIONSSERVICE._serialized_start=2112
-  _IAMPUBLICPERMISSIONSSERVICE._serialized_end=2230
-  _IAMPROVISIONINGSERVICE._serialized_start=2233
-  _IAMPROVISIONINGSERVICE._serialized_end=2680
-  _IAMCERTIFICATESERVICE._serialized_start=2683
-  _IAMCERTIFICATESERVICE._serialized_end=2866
-  _IAMPERMISSIONSSERVICE._serialized_start=2869
-  _IAMPERMISSIONSSERVICE._serialized_end=3082
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: iamanager/v4/iamanager.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ciamanager/v4/iamanager.proto\x12\x0ciamanager.v4\x1a\x1bgoogle/protobuf/empty.proto\"\x1d\n\nAPIVersion\x12\x0f\n\x07version\x18\x01 \x01(\x04\"\x19\n\x06NodeID\x12\x0f\n\x07node_id\x18\x01 \x01(\t\">\n\x0eGetCertRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06issuer\x18\x02 \x01(\x0c\x12\x0e\n\x06serial\x18\x03 \x01(\t\"B\n\x0fGetCertResponse\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x02 \x01(\t\x12\x0f\n\x07key_url\x18\x03 \x01(\t\"4\n\nSystemInfo\x12\x11\n\tsystem_id\x18\x01 \x01(\t\x12\x13\n\x0b\x62oard_model\x18\x02 \x01(\t\"\x1c\n\x08Subjects\x12\x10\n\x08subjects\x18\x01 \x03(\t\"B\n\x12PermissionsRequest\x12\x0e\n\x06secret\x18\x01 \x01(\t\x12\x1c\n\x14\x66unctional_server_id\x18\x02 \x01(\t\"I\n\rInstanceIdent\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x12\n\nsubject_id\x18\x02 \x01(\t\x12\x10\n\x08instance\x18\x03 \x01(\x04\"t\n\x13PermissionsResponse\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12.\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions\"\x16\n\x07NodesID\x12\x0b\n\x03ids\x18\x01 \x03(\t\"&\n\x13GetCertTypesRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x1a\n\tCertTypes\x12\r\n\x05types\x18\x01 \x03(\t\"B\n\x0fSetOwnerRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"-\n\x0c\x43learRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"7\n\x12\x45ncryptDiskRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"T\n\x10\x43reateKeyRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"?\n\x11\x43reateKeyResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03\x63sr\x18\x03 \x01(\t\"?\n\x10\x41pplyCertRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04\x63\x65rt\x18\x03 \x01(\t\"D\n\x11\x41pplyCertResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08\x63\x65rt_url\x18\x03 \x01(\t\"\x82\x01\n\x0bPermissions\x12?\n\x0bpermissions\x18\x01 \x03(\x0b\x32*.iamanager.v4.Permissions.PermissionsEntry\x1a\x32\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe4\x01\n\x17RegisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent\x12K\n\x0bpermissions\x18\x02 \x03(\x0b\x32\x36.iamanager.v4.RegisterInstanceRequest.PermissionsEntry\x1aM\n\x10PermissionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.iamanager.v4.Permissions:\x02\x38\x01\"*\n\x18RegisterInstanceResponse\x12\x0e\n\x06secret\x18\x01 \x01(\t\"J\n\x19UnregisterInstanceRequest\x12-\n\x08instance\x18\x01 \x01(\x0b\x32\x1b.iamanager.v4.InstanceIdent2\xde\x01\n\x10IAMPublicService\x12\x43\n\rGetAPIVersion\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.APIVersion\"\x00\x12;\n\tGetNodeID\x12\x16.google.protobuf.Empty\x1a\x14.iamanager.v4.NodeID\"\x00\x12H\n\x07GetCert\x12\x1c.iamanager.v4.GetCertRequest\x1a\x1d.iamanager.v4.GetCertResponse\"\x00\x32\xf0\x01\n\x18IAMPublicIdentityService\x12\x43\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a\x18.iamanager.v4.SystemInfo\"\x00\x12?\n\x0bGetSubjects\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x12N\n\x18SubscribeSubjectsChanged\x12\x16.google.protobuf.Empty\x1a\x16.iamanager.v4.Subjects\"\x00\x30\x01\x32v\n\x1bIAMPublicPermissionsService\x12W\n\x0eGetPermissions\x12 .iamanager.v4.PermissionsRequest\x1a!.iamanager.v4.PermissionsResponse\"\x00\x32\xbf\x03\n\x16IAMProvisioningService\x12@\n\rGetAllNodeIDs\x12\x16.google.protobuf.Empty\x1a\x15.iamanager.v4.NodesID\"\x00\x12L\n\x0cGetCertTypes\x12!.iamanager.v4.GetCertTypesRequest\x1a\x17.iamanager.v4.CertTypes\"\x00\x12\x43\n\x08SetOwner\x12\x1d.iamanager.v4.SetOwnerRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x05\x43lear\x12\x1a.iamanager.v4.ClearRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0b\x45ncryptDisk\x12 .iamanager.v4.EncryptDiskRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x12\x46inishProvisioning\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x15IAMCertificateService\x12N\n\tCreateKey\x12\x1e.iamanager.v4.CreateKeyRequest\x1a\x1f.iamanager.v4.CreateKeyResponse\"\x00\x12N\n\tApplyCert\x12\x1e.iamanager.v4.ApplyCertRequest\x1a\x1f.iamanager.v4.ApplyCertResponse\"\x00\x32\xd5\x01\n\x15IAMPermissionsService\x12\x63\n\x10RegisterInstance\x12%.iamanager.v4.RegisterInstanceRequest\x1a&.iamanager.v4.RegisterInstanceResponse\"\x00\x12W\n\x12UnregisterInstance\x12\'.iamanager.v4.UnregisterInstanceRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
+
+
+
+_APIVERSION = DESCRIPTOR.message_types_by_name['APIVersion']
+_NODEID = DESCRIPTOR.message_types_by_name['NodeID']
+_GETCERTREQUEST = DESCRIPTOR.message_types_by_name['GetCertRequest']
+_GETCERTRESPONSE = DESCRIPTOR.message_types_by_name['GetCertResponse']
+_SYSTEMINFO = DESCRIPTOR.message_types_by_name['SystemInfo']
+_SUBJECTS = DESCRIPTOR.message_types_by_name['Subjects']
+_PERMISSIONSREQUEST = DESCRIPTOR.message_types_by_name['PermissionsRequest']
+_INSTANCEIDENT = DESCRIPTOR.message_types_by_name['InstanceIdent']
+_PERMISSIONSRESPONSE = DESCRIPTOR.message_types_by_name['PermissionsResponse']
+_NODESID = DESCRIPTOR.message_types_by_name['NodesID']
+_GETCERTTYPESREQUEST = DESCRIPTOR.message_types_by_name['GetCertTypesRequest']
+_CERTTYPES = DESCRIPTOR.message_types_by_name['CertTypes']
+_SETOWNERREQUEST = DESCRIPTOR.message_types_by_name['SetOwnerRequest']
+_CLEARREQUEST = DESCRIPTOR.message_types_by_name['ClearRequest']
+_ENCRYPTDISKREQUEST = DESCRIPTOR.message_types_by_name['EncryptDiskRequest']
+_CREATEKEYREQUEST = DESCRIPTOR.message_types_by_name['CreateKeyRequest']
+_CREATEKEYRESPONSE = DESCRIPTOR.message_types_by_name['CreateKeyResponse']
+_APPLYCERTREQUEST = DESCRIPTOR.message_types_by_name['ApplyCertRequest']
+_APPLYCERTRESPONSE = DESCRIPTOR.message_types_by_name['ApplyCertResponse']
+_PERMISSIONS = DESCRIPTOR.message_types_by_name['Permissions']
+_PERMISSIONS_PERMISSIONSENTRY = _PERMISSIONS.nested_types_by_name['PermissionsEntry']
+_REGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['RegisterInstanceRequest']
+_REGISTERINSTANCEREQUEST_PERMISSIONSENTRY = _REGISTERINSTANCEREQUEST.nested_types_by_name['PermissionsEntry']
+_REGISTERINSTANCERESPONSE = DESCRIPTOR.message_types_by_name['RegisterInstanceResponse']
+_UNREGISTERINSTANCEREQUEST = DESCRIPTOR.message_types_by_name['UnregisterInstanceRequest']
+APIVersion = _reflection.GeneratedProtocolMessageType('APIVersion', (_message.Message,), {
+  'DESCRIPTOR' : _APIVERSION,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.APIVersion)
+  })
+_sym_db.RegisterMessage(APIVersion)
+
+NodeID = _reflection.GeneratedProtocolMessageType('NodeID', (_message.Message,), {
+  'DESCRIPTOR' : _NODEID,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.NodeID)
+  })
+_sym_db.RegisterMessage(NodeID)
+
+GetCertRequest = _reflection.GeneratedProtocolMessageType('GetCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertRequest)
+  })
+_sym_db.RegisterMessage(GetCertRequest)
+
+GetCertResponse = _reflection.GeneratedProtocolMessageType('GetCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertResponse)
+  })
+_sym_db.RegisterMessage(GetCertResponse)
+
+SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMINFO,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.SystemInfo)
+  })
+_sym_db.RegisterMessage(SystemInfo)
+
+Subjects = _reflection.GeneratedProtocolMessageType('Subjects', (_message.Message,), {
+  'DESCRIPTOR' : _SUBJECTS,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.Subjects)
+  })
+_sym_db.RegisterMessage(Subjects)
+
+PermissionsRequest = _reflection.GeneratedProtocolMessageType('PermissionsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsRequest)
+  })
+_sym_db.RegisterMessage(PermissionsRequest)
+
+InstanceIdent = _reflection.GeneratedProtocolMessageType('InstanceIdent', (_message.Message,), {
+  'DESCRIPTOR' : _INSTANCEIDENT,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.InstanceIdent)
+  })
+_sym_db.RegisterMessage(InstanceIdent)
+
+PermissionsResponse = _reflection.GeneratedProtocolMessageType('PermissionsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSIONSRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.PermissionsResponse)
+  })
+_sym_db.RegisterMessage(PermissionsResponse)
+
+NodesID = _reflection.GeneratedProtocolMessageType('NodesID', (_message.Message,), {
+  'DESCRIPTOR' : _NODESID,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.NodesID)
+  })
+_sym_db.RegisterMessage(NodesID)
+
+GetCertTypesRequest = _reflection.GeneratedProtocolMessageType('GetCertTypesRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETCERTTYPESREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.GetCertTypesRequest)
+  })
+_sym_db.RegisterMessage(GetCertTypesRequest)
+
+CertTypes = _reflection.GeneratedProtocolMessageType('CertTypes', (_message.Message,), {
+  'DESCRIPTOR' : _CERTTYPES,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CertTypes)
+  })
+_sym_db.RegisterMessage(CertTypes)
+
+SetOwnerRequest = _reflection.GeneratedProtocolMessageType('SetOwnerRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETOWNERREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.SetOwnerRequest)
+  })
+_sym_db.RegisterMessage(SetOwnerRequest)
+
+ClearRequest = _reflection.GeneratedProtocolMessageType('ClearRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CLEARREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ClearRequest)
+  })
+_sym_db.RegisterMessage(ClearRequest)
+
+EncryptDiskRequest = _reflection.GeneratedProtocolMessageType('EncryptDiskRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ENCRYPTDISKREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.EncryptDiskRequest)
+  })
+_sym_db.RegisterMessage(EncryptDiskRequest)
+
+CreateKeyRequest = _reflection.GeneratedProtocolMessageType('CreateKeyRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyRequest)
+  })
+_sym_db.RegisterMessage(CreateKeyRequest)
+
+CreateKeyResponse = _reflection.GeneratedProtocolMessageType('CreateKeyResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEKEYRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.CreateKeyResponse)
+  })
+_sym_db.RegisterMessage(CreateKeyResponse)
+
+ApplyCertRequest = _reflection.GeneratedProtocolMessageType('ApplyCertRequest', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertRequest)
+  })
+_sym_db.RegisterMessage(ApplyCertRequest)
+
+ApplyCertResponse = _reflection.GeneratedProtocolMessageType('ApplyCertResponse', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTRESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.ApplyCertResponse)
+  })
+_sym_db.RegisterMessage(ApplyCertResponse)
+
+Permissions = _reflection.GeneratedProtocolMessageType('Permissions', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _PERMISSIONS_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v4.iamanager_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _PERMISSIONS,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.Permissions)
+  })
+_sym_db.RegisterMessage(Permissions)
+_sym_db.RegisterMessage(Permissions.PermissionsEntry)
+
+RegisterInstanceRequest = _reflection.GeneratedProtocolMessageType('RegisterInstanceRequest', (_message.Message,), {
+
+  'PermissionsEntry' : _reflection.GeneratedProtocolMessageType('PermissionsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY,
+    '__module__' : 'iamanager.v4.iamanager_pb2'
+    # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest.PermissionsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _REGISTERINSTANCEREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceRequest)
+  })
+_sym_db.RegisterMessage(RegisterInstanceRequest)
+_sym_db.RegisterMessage(RegisterInstanceRequest.PermissionsEntry)
+
+RegisterInstanceResponse = _reflection.GeneratedProtocolMessageType('RegisterInstanceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERINSTANCERESPONSE,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.RegisterInstanceResponse)
+  })
+_sym_db.RegisterMessage(RegisterInstanceResponse)
+
+UnregisterInstanceRequest = _reflection.GeneratedProtocolMessageType('UnregisterInstanceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _UNREGISTERINSTANCEREQUEST,
+  '__module__' : 'iamanager.v4.iamanager_pb2'
+  # @@protoc_insertion_point(class_scope:iamanager.v4.UnregisterInstanceRequest)
+  })
+_sym_db.RegisterMessage(UnregisterInstanceRequest)
+
+_IAMPUBLICSERVICE = DESCRIPTOR.services_by_name['IAMPublicService']
+_IAMPUBLICIDENTITYSERVICE = DESCRIPTOR.services_by_name['IAMPublicIdentityService']
+_IAMPUBLICPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPublicPermissionsService']
+_IAMPROVISIONINGSERVICE = DESCRIPTOR.services_by_name['IAMProvisioningService']
+_IAMCERTIFICATESERVICE = DESCRIPTOR.services_by_name['IAMCertificateService']
+_IAMPERMISSIONSSERVICE = DESCRIPTOR.services_by_name['IAMPermissionsService']
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _PERMISSIONS_PERMISSIONSENTRY._options = None
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_options = b'8\001'
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._options = None
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_options = b'8\001'
+  _APIVERSION._serialized_start=75
+  _APIVERSION._serialized_end=104
+  _NODEID._serialized_start=106
+  _NODEID._serialized_end=131
+  _GETCERTREQUEST._serialized_start=133
+  _GETCERTREQUEST._serialized_end=195
+  _GETCERTRESPONSE._serialized_start=197
+  _GETCERTRESPONSE._serialized_end=263
+  _SYSTEMINFO._serialized_start=265
+  _SYSTEMINFO._serialized_end=317
+  _SUBJECTS._serialized_start=319
+  _SUBJECTS._serialized_end=347
+  _PERMISSIONSREQUEST._serialized_start=349
+  _PERMISSIONSREQUEST._serialized_end=415
+  _INSTANCEIDENT._serialized_start=417
+  _INSTANCEIDENT._serialized_end=490
+  _PERMISSIONSRESPONSE._serialized_start=492
+  _PERMISSIONSRESPONSE._serialized_end=608
+  _NODESID._serialized_start=610
+  _NODESID._serialized_end=632
+  _GETCERTTYPESREQUEST._serialized_start=634
+  _GETCERTTYPESREQUEST._serialized_end=672
+  _CERTTYPES._serialized_start=674
+  _CERTTYPES._serialized_end=700
+  _SETOWNERREQUEST._serialized_start=702
+  _SETOWNERREQUEST._serialized_end=768
+  _CLEARREQUEST._serialized_start=770
+  _CLEARREQUEST._serialized_end=815
+  _ENCRYPTDISKREQUEST._serialized_start=817
+  _ENCRYPTDISKREQUEST._serialized_end=872
+  _CREATEKEYREQUEST._serialized_start=874
+  _CREATEKEYREQUEST._serialized_end=958
+  _CREATEKEYRESPONSE._serialized_start=960
+  _CREATEKEYRESPONSE._serialized_end=1023
+  _APPLYCERTREQUEST._serialized_start=1025
+  _APPLYCERTREQUEST._serialized_end=1088
+  _APPLYCERTRESPONSE._serialized_start=1090
+  _APPLYCERTRESPONSE._serialized_end=1158
+  _PERMISSIONS._serialized_start=1161
+  _PERMISSIONS._serialized_end=1291
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_start=1241
+  _PERMISSIONS_PERMISSIONSENTRY._serialized_end=1291
+  _REGISTERINSTANCEREQUEST._serialized_start=1294
+  _REGISTERINSTANCEREQUEST._serialized_end=1522
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_start=1445
+  _REGISTERINSTANCEREQUEST_PERMISSIONSENTRY._serialized_end=1522
+  _REGISTERINSTANCERESPONSE._serialized_start=1524
+  _REGISTERINSTANCERESPONSE._serialized_end=1566
+  _UNREGISTERINSTANCEREQUEST._serialized_start=1568
+  _UNREGISTERINSTANCEREQUEST._serialized_end=1642
+  _IAMPUBLICSERVICE._serialized_start=1645
+  _IAMPUBLICSERVICE._serialized_end=1867
+  _IAMPUBLICIDENTITYSERVICE._serialized_start=1870
+  _IAMPUBLICIDENTITYSERVICE._serialized_end=2110
+  _IAMPUBLICPERMISSIONSSERVICE._serialized_start=2112
+  _IAMPUBLICPERMISSIONSSERVICE._serialized_end=2230
+  _IAMPROVISIONINGSERVICE._serialized_start=2233
+  _IAMPROVISIONINGSERVICE._serialized_end=2680
+  _IAMCERTIFICATESERVICE._serialized_start=2683
+  _IAMCERTIFICATESERVICE._serialized_end=2866
+  _IAMPERMISSIONSSERVICE._serialized_start=2869
+  _IAMPERMISSIONSSERVICE._serialized_end=3082
+# @@protoc_insertion_point(module_scope)
```

## aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py

 * *Ordering differences only*

```diff
@@ -1,735 +1,735 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iamanager_dot_v4_dot_iamanager__pb2
-
-
-class IAMPublicServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetAPIVersion = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetAPIVersion',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
-                )
-        self.GetNodeID = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetNodeID',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
-                )
-        self.GetCert = channel.unary_unary(
-                '/iamanager.v4.IAMPublicService/GetCert',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
-                )
-
-
-class IAMPublicServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetAPIVersion(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetNodeID(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAPIVersion,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.SerializeToString,
-            ),
-            'GetNodeID': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetNodeID,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.SerializeToString,
-            ),
-            'GetCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCert,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetAPIVersion(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetAPIVersion',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetNodeID(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetNodeID',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetCert',
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPublicIdentityServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetSystemInfo = channel.unary_unary(
-                '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
-                )
-        self.GetSubjects = channel.unary_unary(
-                '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-                )
-        self.SubscribeSubjectsChanged = channel.unary_stream(
-                '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-                )
-
-
-class IAMPublicIdentityServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetSystemInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetSubjects(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SubscribeSubjectsChanged(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicIdentityServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSystemInfo,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.SerializeToString,
-            ),
-            'GetSubjects': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetSubjects,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
-            ),
-            'SubscribeSubjectsChanged': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeSubjectsChanged,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicIdentityService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicIdentityService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetSystemInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetSubjects(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SubscribeSubjectsChanged(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPublicPermissionsServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetPermissions = channel.unary_unary(
-                '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
-                )
-
-
-class IAMPublicPermissionsServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPublicPermissionsServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetPermissions': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetPermissions,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPublicPermissionsService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPublicPermissionsService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetPermissions(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
-            iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMProvisioningServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.GetAllNodeIDs = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
-                )
-        self.GetCertTypes = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/GetCertTypes',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
-                )
-        self.SetOwner = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/SetOwner',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.Clear = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/Clear',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.EncryptDisk = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/EncryptDisk',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.FinishProvisioning = channel.unary_unary(
-                '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMProvisioningServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def GetAllNodeIDs(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetCertTypes(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetOwner(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Clear(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EncryptDisk(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FinishProvisioning(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMProvisioningServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'GetAllNodeIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetAllNodeIDs,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.SerializeToString,
-            ),
-            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCertTypes,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.SerializeToString,
-            ),
-            'SetOwner': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetOwner,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'Clear': grpc.unary_unary_rpc_method_handler(
-                    servicer.Clear,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
-                    servicer.EncryptDisk,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
-                    servicer.FinishProvisioning,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMProvisioningService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMProvisioningService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def GetAllNodeIDs(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetCertTypes(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetCertTypes',
-            iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetOwner(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/SetOwner',
-            iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Clear(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/Clear',
-            iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EncryptDisk(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/EncryptDisk',
-            iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FinishProvisioning(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMCertificateServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.CreateKey = channel.unary_unary(
-                '/iamanager.v4.IAMCertificateService/CreateKey',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
-                )
-        self.ApplyCert = channel.unary_unary(
-                '/iamanager.v4.IAMCertificateService/ApplyCert',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
-                )
-
-
-class IAMCertificateServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def CreateKey(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ApplyCert(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMCertificateServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'CreateKey': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKey,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.SerializeToString,
-            ),
-            'ApplyCert': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApplyCert,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMCertificateService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMCertificateService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def CreateKey(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/CreateKey',
-            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApplyCert(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/ApplyCert',
-            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-
-class IAMPermissionsServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.RegisterInstance = channel.unary_unary(
-                '/iamanager.v4.IAMPermissionsService/RegisterInstance',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
-                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
-                )
-        self.UnregisterInstance = channel.unary_unary(
-                '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
-                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-
-
-class IAMPermissionsServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
-
-    def RegisterInstance(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def UnregisterInstance(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_IAMPermissionsServiceServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'RegisterInstance': grpc.unary_unary_rpc_method_handler(
-                    servicer.RegisterInstance,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.FromString,
-                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.SerializeToString,
-            ),
-            'UnregisterInstance': grpc.unary_unary_rpc_method_handler(
-                    servicer.UnregisterInstance,
-                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'iamanager.v4.IAMPermissionsService', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class IAMPermissionsService(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def RegisterInstance(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/RegisterInstance',
-            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
-            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UnregisterInstance(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
-            iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iamanager_dot_v4_dot_iamanager__pb2
+
+
+class IAMPublicServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetAPIVersion = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetAPIVersion',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
+                )
+        self.GetNodeID = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetNodeID',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
+                )
+        self.GetCert = channel.unary_unary(
+                '/iamanager.v4.IAMPublicService/GetCert',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
+                )
+
+
+class IAMPublicServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetAPIVersion(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetNodeID(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetAPIVersion': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAPIVersion,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.APIVersion.SerializeToString,
+            ),
+            'GetNodeID': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetNodeID,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodeID.SerializeToString,
+            ),
+            'GetCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCert,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetAPIVersion(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetAPIVersion',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.APIVersion.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetNodeID(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetNodeID',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.NodeID.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicService/GetCert',
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPublicIdentityServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetSystemInfo = channel.unary_unary(
+                '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
+                )
+        self.GetSubjects = channel.unary_unary(
+                '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+                )
+        self.SubscribeSubjectsChanged = channel.unary_stream(
+                '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+                )
+
+
+class IAMPublicIdentityServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetSystemInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSubjects(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeSubjectsChanged(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicIdentityServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetSystemInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSystemInfo,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.SerializeToString,
+            ),
+            'GetSubjects': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSubjects,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
+            ),
+            'SubscribeSubjectsChanged': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeSubjectsChanged,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.Subjects.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicIdentityService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicIdentityService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetSystemInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSystemInfo',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.SystemInfo.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSubjects(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicIdentityService/GetSubjects',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeSubjectsChanged(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/iamanager.v4.IAMPublicIdentityService/SubscribeSubjectsChanged',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.Subjects.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPublicPermissionsServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetPermissions = channel.unary_unary(
+                '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
+                )
+
+
+class IAMPublicPermissionsServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetPermissions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPublicPermissionsServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetPermissions': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPermissions,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPublicPermissionsService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPublicPermissionsService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetPermissions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPublicPermissionsService/GetPermissions',
+            iamanager_dot_v4_dot_iamanager__pb2.PermissionsRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.PermissionsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMProvisioningServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.GetAllNodeIDs = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
+                )
+        self.GetCertTypes = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/GetCertTypes',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
+                )
+        self.SetOwner = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/SetOwner',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.Clear = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/Clear',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.EncryptDisk = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/EncryptDisk',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+        self.FinishProvisioning = channel.unary_unary(
+                '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMProvisioningServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def GetAllNodeIDs(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCertTypes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetOwner(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Clear(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def EncryptDisk(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def FinishProvisioning(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMProvisioningServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'GetAllNodeIDs': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAllNodeIDs,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.NodesID.SerializeToString,
+            ),
+            'GetCertTypes': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCertTypes,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CertTypes.SerializeToString,
+            ),
+            'SetOwner': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetOwner,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'Clear': grpc.unary_unary_rpc_method_handler(
+                    servicer.Clear,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'EncryptDisk': grpc.unary_unary_rpc_method_handler(
+                    servicer.EncryptDisk,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+            'FinishProvisioning': grpc.unary_unary_rpc_method_handler(
+                    servicer.FinishProvisioning,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMProvisioningService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMProvisioningService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def GetAllNodeIDs(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetAllNodeIDs',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.NodesID.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCertTypes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/GetCertTypes',
+            iamanager_dot_v4_dot_iamanager__pb2.GetCertTypesRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.CertTypes.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetOwner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/SetOwner',
+            iamanager_dot_v4_dot_iamanager__pb2.SetOwnerRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Clear(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/Clear',
+            iamanager_dot_v4_dot_iamanager__pb2.ClearRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def EncryptDisk(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/EncryptDisk',
+            iamanager_dot_v4_dot_iamanager__pb2.EncryptDiskRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def FinishProvisioning(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMProvisioningService/FinishProvisioning',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMCertificateServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.CreateKey = channel.unary_unary(
+                '/iamanager.v4.IAMCertificateService/CreateKey',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
+                )
+        self.ApplyCert = channel.unary_unary(
+                '/iamanager.v4.IAMCertificateService/ApplyCert',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
+                )
+
+
+class IAMCertificateServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def CreateKey(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ApplyCert(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMCertificateServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'CreateKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKey,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.SerializeToString,
+            ),
+            'ApplyCert': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApplyCert,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMCertificateService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMCertificateService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def CreateKey(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/CreateKey',
+            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.CreateKeyResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApplyCert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMCertificateService/ApplyCert',
+            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.ApplyCertResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
+class IAMPermissionsServiceStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.RegisterInstance = channel.unary_unary(
+                '/iamanager.v4.IAMPermissionsService/RegisterInstance',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
+                response_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
+                )
+        self.UnregisterInstance = channel.unary_unary(
+                '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
+                request_serializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
+
+
+class IAMPermissionsServiceServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def RegisterInstance(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UnregisterInstance(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_IAMPermissionsServiceServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'RegisterInstance': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterInstance,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.FromString,
+                    response_serializer=iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.SerializeToString,
+            ),
+            'UnregisterInstance': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterInstance,
+                    request_deserializer=iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'iamanager.v4.IAMPermissionsService', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class IAMPermissionsService(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def RegisterInstance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/RegisterInstance',
+            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceRequest.SerializeToString,
+            iamanager_dot_v4_dot_iamanager__pb2.RegisterInstanceResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UnregisterInstance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/iamanager.v4.IAMPermissionsService/UnregisterInstance',
+            iamanager_dot_v4_dot_iamanager__pb2.UnregisterInstanceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## aos_prov/files/1rootCA.crt

```diff
@@ -1,170 +1,172 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2043 4552 5449  -----BEGIN CERTI
-00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4945  FICATE-----.MIIE
-00000020: 416a 4343 4175 7167 4177 4942 4167 494a  AjCCAuqgAwIBAgIJ
-00000030: 4150 776b 324e 4666 5344 506a 4d41 3047  APwk2NFfSDPjMA0G
-00000040: 4353 7147 5349 6233 4451 4542 4377 5541  CSqGSIb3DQEBCwUA
-00000050: 4d49 474e 4d52 6377 4651 5944 0a56 5151  MIGNMRcwFQYD.VQQ
-00000060: 4444 4135 4764 584e 7062 3234 6755 6d39  DDA5GdXNpb24gUm9
-00000070: 7664 4342 4451 5445 704d 4363 4743 5371  vdCBDQTEpMCcGCSq
-00000080: 4753 4962 3344 5145 4a41 5259 6164 6d39  GSIb3DQEJARYadm9
-00000090: 7362 3252 3562 586c 7958 324a 680a 596d  sb2R5bXlyX2Jh.Ym
-000000a0: 4e6f 6457 7441 5a58 4268 6253 356a 6232  NodWtAZXBhbS5jb2
-000000b0: 3078 4454 414c 4267 4e56 4241 6f4d 4245  0xDTALBgNVBAoMBE
-000000c0: 5651 5155 3078 4844 4161 4267 4e56 4241  VQQU0xHDAaBgNVBA
-000000d0: 734d 4530 3576 646e 567a 4945 3979 0a5a  sME05vdnVzIE9y.Z
-000000e0: 4738 6755 3256 6a62 4739 7964 5730 7844  G8gU2VjbG9ydW0xD
-000000f0: 5441 4c42 674e 5642 4163 4d42 4574 3561  TALBgNVBAcMBEt5a
-00000100: 5859 7843 7a41 4a42 674e 5642 4159 5441  XYxCzAJBgNVBAYTA
-00000110: 6c56 424d 4234 5844 5445 344d 4451 780a  lVBMB4XDTE4MDQx.
-00000120: 4d44 4578 4d7a 4d77 4d46 6f58 4454 4932  MDExMzMwMFoXDTI2
-00000130: 4d44 5979 4e7a 4578 4d7a 4d77 4d46 6f77  MDYyNzExMzMwMFow
-00000140: 6759 3078 467a 4156 4267 4e56 4241 4d4d  gY0xFzAVBgNVBAMM
-00000150: 446b 5a31 6332 6c76 6269 4253 6232 3930  DkZ1c2lvbiBSb290
-00000160: 0a49 454e 424d 536b 774a 7759 4a4b 6f5a  .IENBMSkwJwYJKoZ
-00000170: 4968 7663 4e41 516b 4246 6870 3262 3278  IhvcNAQkBFhp2b2x
-00000180: 765a 486c 7465 584a 6659 6d46 6959 3268  vZHlteXJfYmFiY2h
-00000190: 3161 3042 6c63 4746 744c 6d4e 7662 5445  1a0BlcGFtLmNvbTE
-000001a0: 4e0a 4d41 7347 4131 5545 4367 7745 5256  N.MAsGA1UECgwERV
-000001b0: 4242 5454 4563 4d42 6f47 4131 5545 4377  BBTTEcMBoGA1UECw
-000001c0: 7754 546d 3932 6458 4d67 5433 4a6b 6279  wTTm92dXMgT3Jkby
-000001d0: 4254 5a57 4e73 6233 4a31 6254 454e 4d41  BTZWNsb3J1bTENMA
-000001e0: 7347 0a41 3155 4542 7777 4553 336c 7064  sG.A1UEBwwES3lpd
-000001f0: 6a45 4c4d 416b 4741 3155 4542 684d 4356  jELMAkGA1UEBhMCV
-00000200: 5545 7767 6745 694d 4130 4743 5371 4753  UEwggEiMA0GCSqGS
-00000210: 4962 3344 5145 4241 5155 4141 3449 4244  Ib3DQEBAQUAA4IBD
-00000220: 7741 770a 6767 454b 416f 4942 4151 432b  wAw.ggEKAoIBAQC+
-00000230: 4b32 6f77 3248 4f37 2b53 5556 664f 7135  K2ow2HO7+SUVfOq5
-00000240: 7454 746d 486a 344c 5169 6a48 4a38 3033  tTtmHj4LQijHJ803
-00000250: 6d4c 6b39 706b 5065 662b 476c 6d65 7970  mLk9pkPef+Glmeyp
-00000260: 3948 5865 0a6a 446c 5143 3034 4d65 6f76  9HXe.jDlQC04Meov
-00000270: 4d42 654e 5461 7130 7769 6266 3771 6173  MBeNTaq0wibf7qas
-00000280: 396e 6958 6265 5852 567a 6865 5a49 467a  9niXbeXRVzheZIFz
-00000290: 694d 5871 5275 774c 7163 304b 5864 4478  iMXqRuwLqc0KXdDx
-000002a0: 4944 5054 620a 5457 334b 3048 4536 4d2f  IDPTb.TW3K0HE6M/
-000002b0: 6541 7454 666e 392b 5a2f 4c6e 6b57 7434  eAtTfn9+Z/LnkWt4
-000002c0: 7a4d 5861 7363 3032 6876 7566 736d 4956  zMXasc02hvufsmIV
-000002d0: 4575 4e62 6331 5668 7273 4a4a 6735 756b  EuNbc1VhrsJJg5uk
-000002e0: 3838 6c64 504d 0a4c 5346 376e 6666 3965  88ldPM.LSF7nff9e
-000002f0: 595a 5448 5967 4379 426b 7439 614c 2b66  YZTHYgCyBkt9aL+f
-00000300: 776f 584f 3665 5344 5341 686a 6f70 5833  woXO6eSDSAhjopX3
-00000310: 6c68 6469 646b 4d2b 6e69 3745 4f68 6c4e  lhdidkM+ni7EOhlN
-00000320: 3753 546d 6744 4d0a 574b 6839 6e4d 6a58  7STmgDM.WKh9nMjX
-00000330: 4435 6632 3850 4768 7457 2f64 5a76 6e34  D5f28PGhtW/dZvn4
-00000340: 537a 6173 5245 354d 6561 4578 496c 426d  SzasRE5MeaExIlBm
-00000350: 686b 5745 5567 5643 7950 374c 7675 5147  hkWEUgVCyP7LvuQG
-00000360: 5255 504b 2b4e 597a 0a46 4532 434c 5275  RUPK+NYz.FE2CLRu
-00000370: 6972 4c43 5779 3148 4974 396c 4c7a 6950  irLCWy1HIt9lLziP
-00000380: 6a6c 5a34 3336 316d 4e41 674d 4241 4147  jlZ4361mNAgMBAAG
-00000390: 6a59 7a42 684d 4230 4741 3155 6444 6751  jYzBhMB0GA1UdDgQ
-000003a0: 5742 4252 3053 6868 7a0a 4f75 4d39 3542  WBBR0Shhz.OuM95B
-000003b0: 6844 306d 5778 4331 6a2b 4b72 4536 556a  hD0mWxC1j+KrE6Uj
-000003c0: 414d 4267 4e56 4852 4d45 4254 4144 4151  AMBgNVHRMEBTADAQ
-000003d0: 482f 4d41 7347 4131 5564 4477 5145 4177  H/MAsGA1UdDwQEAw
-000003e0: 4942 426a 416c 4267 4e56 0a48 5245 4548  IBBjAlBgNV.HREEH
-000003f0: 6a41 6367 5270 3262 3278 765a 486c 7465  jAcgRp2b2xvZHlte
-00000400: 584a 6659 6d46 6959 3268 3161 3042 6c63  XJfYmFiY2h1a0Blc
-00000410: 4746 744c 6d4e 7662 5441 4e42 676b 7168  GFtLmNvbTANBgkqh
-00000420: 6b69 4739 7730 4241 5173 460a 4141 4f43  kiG9w0BAQsF.AAOC
-00000430: 4151 4541 6c38 6276 3148 5459 6533 6c34  AQEAl8bv1HTYe3l4
-00000440: 592b 6730 5456 5a52 3762 594c 3542 4e73  Y+g0TVZR7bYL5BNs
-00000450: 6e47 6771 7930 7153 3566 7539 3931 6b68  nGgqy0qS5fu991kh
-00000460: 5857 662b 5a77 6132 4d4c 566e 0a59 616b  XWf+Zwa2MLVn.Yak
-00000470: 4d6e 4c6b 6a76 6448 7155 7057 4d4a 2f53  MnLkjvdHqUpWMJ/S
-00000480: 3832 6f32 7a57 476d 6d75 7863 6135 3665  82o2zWGmmuxca56e
-00000490: 686a 7843 6950 2f6e 6b6d 344d 3734 7958  hjxCiP/nkm4M74yX
-000004a0: 7a32 5238 6375 3532 5778 596e 460a 794d  z2R8cu52WxYnF.yM
-000004b0: 7667 6177 7a51 3663 3179 6876 5a69 762f  vgawzQ6c1yhvZiv/
-000004c0: 6745 4537 4b64 6259 5256 4b4c 4850 6742  gEE7KdbYRVKLHPgB
-000004d0: 7a66 7975 7032 3169 356e 6753 6c54 634d  zfyup21i5ngSlTcM
-000004e0: 5252 5337 6f4f 426d 6f79 6534 7163 0a36  RRS7oOBmoye4qc.6
-000004f0: 6164 7136 4874 5936 582f 4f6e 5a39 4935  adq6HtY6X/OnZ9I5
-00000500: 786f 524e 3147 6376 614c 5567 5545 3669  xoRN1GcvaLUgUE6i
-00000510: 6754 6956 6131 7046 386b 6564 5768 4859  gTiVa1pF8kedWhHY
-00000520: 3777 7a54 5842 787a 5376 495a 6b43 550a  7wzTXBxzSvIZkCU.
-00000530: 5648 454f 7a76 6147 6b39 6d69 5036 6e42  VHEOzvaGk9miP6nB
-00000540: 7244 664e 7637 6d49 6b67 454b 4152 726a  rDfNv7mIkgEKARrj
-00000550: 6a53 706d 4a61 7349 4555 2b6d 4e74 7a65  jSpmJasIEU+mNtze
-00000560: 4f49 4569 4d74 5731 454d 5263 3435 376f  OIEiMtW1EMRc457o
-00000570: 0a30 5064 4649 336a 7365 794c 5650 5668  .0PdFI3jseyLVPVh
-00000580: 457a 556b 7543 376d 776a 6237 4365 513d  EzUkuC7mwjb7CeQ=
-00000590: 3d0a 2d2d 2d2d 2d45 4e44 2043 4552 5449  =.-----END CERTI
-000005a0: 4649 4341 5445 2d2d 2d2d 2d0a 2d2d 2d2d  FICATE-----.----
-000005b0: 2d42 4547 494e 2043 4552 5449 4649 4341  -BEGIN CERTIFICA
-000005c0: 5445 2d2d 2d2d 2d0a 4d49 4944 6354 4343  TE-----.MIIDcTCC
-000005d0: 416c 6d67 4177 4942 4167 4955 6141 6165  AlmgAwIBAgIUaAae
-000005e0: 392b 7657 6e4b 5674 514b 2f53 6c6c 5443  9+vWnKVtQK/SllTC
-000005f0: 6e69 6b4d 4366 6f77 4451 594a 4b6f 5a49  nikMCfowDQYJKoZI
-00000600: 6876 634e 4151 454c 0a42 5141 7751 6a45  hvcNAQEL.BQAwQjE
-00000610: 554d 4249 4741 3155 4541 7777 4c51 5739  UMBIGA1UEAwwLQW9
-00000620: 7a49 464a 7662 3351 6751 3045 7844 7a41  zIFJvb3QgQ0ExDzA
-00000630: 4e42 674e 5642 416f 4d42 6b35 3159 5735  NBgNVBAoMBk51YW5
-00000640: 6a5a 5445 4d4d 416f 470a 4131 5545 4377  jZTEMMAoG.A1UECw
-00000650: 7744 5157 397a 4d51 7377 4351 5944 5651  wDQW9zMQswCQYDVQ
-00000660: 5147 4577 4a56 557a 4167 4677 3079 4d44  QGEwJVUzAgFw0yMD
-00000670: 4578 4d54 6378 4d44 4934 4d44 4e61 4741  ExMTcxMDI4MDNaGA
-00000680: 3879 4d44 5577 4d54 4578 0a4d 4445 774d  8yMDUwMTEx.MDEwM
-00000690: 6a67 774d 316f 7751 6a45 554d 4249 4741  jgwM1owQjEUMBIGA
-000006a0: 3155 4541 7777 4c51 5739 7a49 464a 7662  1UEAwwLQW9zIFJvb
-000006b0: 3351 6751 3045 7844 7a41 4e42 674e 5642  3QgQ0ExDzANBgNVB
-000006c0: 416f 4d42 6b35 3159 5735 6a0a 5a54 454d  AoMBk51YW5j.ZTEM
-000006d0: 4d41 6f47 4131 5545 4377 7744 5157 397a  MAoGA1UECwwDQW9z
-000006e0: 4d51 7377 4351 5944 5651 5147 4577 4a56  MQswCQYDVQQGEwJV
-000006f0: 557a 4343 4153 4977 4451 594a 4b6f 5a49  UzCCASIwDQYJKoZI
-00000700: 6876 634e 4151 4542 4251 4144 0a67 6745  hvcNAQEBBQAD.ggE
-00000710: 5041 4443 4341 516f 4367 6745 4241 4e73  PADCCAQoCggEBANs
-00000720: 4a65 624b 4d6f 7232 7844 6c51 7241 3739  JebKMor2xDlQrA79
-00000730: 4566 4c51 3531 596e 6344 745a 6d78 4c4b  EfLQ51YncDtZmxLK
-00000740: 382b 5968 4c78 4c2f 3234 5853 420a 5844  8+YhLxL/24XSB.XD
-00000750: 546f 4447 4c61 7465 6372 7336 3145 5169  ToDGLatecrs61EQi
-00000760: 536f 744c 4f37 496c 5a77 4233 6766 5a55  SotLO7IlZwB3gfZU
-00000770: 4b6d 4c64 5179 5367 5741 6952 5369 686c  KmLdQySgWAiRSihl
-00000780: 7a76 7839 6d30 4348 7353 6648 3365 0a72  zvx9m0CHsSfH3e.r
-00000790: 704a 4c6a 6e6a 6953 365a 4a68 426b 5177  pJLjnjiS6ZJhBkQw
-000007a0: 732b 6241 5669 4e34 795a 7551 7063 4b73  s+bAViN4yZuQpcKs
-000007b0: 7879 6762 3177 7a37 6172 4f79 6c32 6e59  xygb1wz7arOyl2nY
-000007c0: 4544 4d7a 2b68 7964 3863 7337 5531 480a  EDMz+hyd8cs7U1H.
-000007d0: 304a 4a67 4931 7050 4255 4c63 4b65 4c66  0JJgI1pPBULcKeLf
-000007e0: 4347 5047 5a75 6642 3659 6549 6650 5455  CGPGZufB6YeIfPTU
-000007f0: 502f 4345 3439 6862 774d 7548 5868 7044  P/CE49hbwMuHXhpD
-00000800: 6335 4c73 3053 4258 5755 5666 6b42 4d45  c5Ls0SBXWUVfkBME
-00000810: 0a4a 7275 654d 497a 4a52 5177 5532 394e  .JrueMIzJRQwU29N
-00000820: 2b33 3250 6867 624c 5a75 776f 544a 5669  +32PhgbLZuwoTJVi
-00000830: 2b56 634b 5266 4632 4f62 7773 647a 6348  +VcKRfF2ObwsdzcH
-00000840: 3633 6454 4169 796a 4372 4d59 5934 6764  63dTAiyjCrMYY4gd
-00000850: 630a 3230 7562 6a64 796e 5737 7833 6778  c.20ubjdynW7x3gx
-00000860: 4f57 5168 304f 3269 6b6e 692f 4f54 786f  OWQh0O2ikni/OTxo
-00000870: 7a77 5837 386c 7243 4543 4177 4541 4161  zwX78lrCECAwEAAa
-00000880: 4e64 4d46 7377 4441 5944 5652 3054 4241  NdMFswDAYDVR0TBA
-00000890: 5577 0a41 7745 422f 7a41 6442 674e 5648  Uw.AwEB/zAdBgNVH
-000008a0: 5134 4546 6751 554f 656e 4436 5562 4f43  Q4EFgQUOenD6UbOC
-000008b0: 6c49 3344 4d67 4a36 3041 3266 5537 536a  lI3DMgJ60A2fU7Sj
-000008c0: 5938 7748 7759 4456 5230 6a42 4267 7746  Y8wHwYDVR0jBBgwF
-000008d0: 6f41 550a 4f65 6e44 3655 624f 436c 4933  oAU.OenD6UbOClI3
-000008e0: 444d 674a 3630 4132 6655 3753 6a59 3877  DMgJ60A2fU7SjY8w
-000008f0: 4377 5944 5652 3050 4241 5144 4167 4747  CwYDVR0PBAQDAgGG
-00000900: 4d41 3047 4353 7147 5349 6233 4451 4542  MA0GCSqGSIb3DQEB
-00000910: 4377 5541 0a41 3449 4241 5142 5151 6f69  CwUA.A4IBAQBQQoi
-00000920: 3638 6c6d 4541 506d 6373 4941 6958 3367  68lmEAPmcsIAiX3g
-00000930: 696c 6d76 7565 6164 6963 5a65 6f42 4b61  ilmvueadicZeoBKa
-00000940: 4b61 4846 4a6c 4c31 4341 7648 5748 544c  KaHFJlL1CAvHWHTL
-00000950: 6330 474c 720a 6f4c 3358 7156 5735 6971  c0GLr.oL3XqVW5iq
-00000960: 6547 4c38 6575 334f 6d69 6178 5049 5934  eGL8eu3OmiaxPIY4
-00000970: 6632 7a78 6f41 4847 4c54 5933 7572 2f4f  f2zxoAHGLTY3ur/O
-00000980: 3033 4742 5145 326a 4275 5636 754f 7058  03GBQE2jBuV6uOpX
-00000990: 744e 6330 6436 0a58 4470 342f 772f 704d  tNc0d6.XDp4/w/pM
-000009a0: 6345 6458 7337 5439 4f38 6c4c 496a 7976  cEdXs7T9O8lLIjyv
-000009b0: 532b 6866 6f53 4764 3958 346b 4e4b 694d  S+hfoSGd9X4kNKiM
-000009c0: 6135 536d 6f35 5530 566f 414c 4f4d 4667  a5Smo5U0VoALOMFg
-000009d0: 5245 3656 5a46 660a 5771 3245 7575 4154  RE6VZFf.Wq2EuuAT
-000009e0: 4578 3746 435a 6434 506b 634f 4c73 4666  Ex7FCZd4PkcOLsFf
-000009f0: 6f61 4c74 6545 6132 6c57 3435 6f57 4962  oaLteEa2lW45oWIb
-00000a00: 6c6c 4d6e 3365 5779 6f38 2b43 3251 3952  llMn3eWyo8+C2Q9R
-00000a10: 7733 6b62 7a49 6f74 0a32 5962 5059 6b50  w3kbzIot.2YbPYkP
-00000a20: 6273 4633 452f 6352 3455 5a46 386a 4742  bsF3E/cR4UZF8jGB
-00000a30: 6e65 4838 304d 746b 3034 4577 5635 6f62  neH80Mtk04EwV5ob
-00000a40: 6e67 4642 7174 3355 655a 796a 5658 4168  ngFBqt3UeZyjVXAh
-00000a50: 7775 6d5a 7436 522b 4a0a 7246 7a5a 6c64  wumZt6R+J.rFzZld
-00000a60: 4362 6d34 786a 2b70 5246 6879 3546 436b  Cbm4xj+pRFhy5FCk
-00000a70: 4849 7069 506a 0a2d 2d2d 2d2d 454e 4420  HIpiPj.-----END 
-00000a80: 4345 5254 4946 4943 4154 452d 2d2d 2d2d  CERTIFICATE-----
-00000a90: 0a                                       .
+00000010: 4649 4341 5445 2d2d 2d2d 2d0d 0a4d 4949  FICATE-----..MII
+00000020: 4541 6a43 4341 7571 6741 7749 4241 6749  EAjCCAuqgAwIBAgI
+00000030: 4a41 5077 6b32 4e46 6653 4450 6a4d 4130  JAPwk2NFfSDPjMA0
+00000040: 4743 5371 4753 4962 3344 5145 4243 7755  GCSqGSIb3DQEBCwU
+00000050: 414d 4947 4e4d 5263 7746 5159 440d 0a56  AMIGNMRcwFQYD..V
+00000060: 5151 4444 4135 4764 584e 7062 3234 6755  QQDDA5GdXNpb24gU
+00000070: 6d39 7664 4342 4451 5445 704d 4363 4743  m9vdCBDQTEpMCcGC
+00000080: 5371 4753 4962 3344 5145 4a41 5259 6164  SqGSIb3DQEJARYad
+00000090: 6d39 7362 3252 3562 586c 7958 324a 680d  m9sb2R5bXlyX2Jh.
+000000a0: 0a59 6d4e 6f64 5774 415a 5842 6862 5335  .YmNodWtAZXBhbS5
+000000b0: 6a62 3230 7844 5441 4c42 674e 5642 416f  jb20xDTALBgNVBAo
+000000c0: 4d42 4556 5151 5530 7848 4441 6142 674e  MBEVQQU0xHDAaBgN
+000000d0: 5642 4173 4d45 3035 7664 6e56 7a49 4539  VBAsME05vdnVzIE9
+000000e0: 790d 0a5a 4738 6755 3256 6a62 4739 7964  y..ZG8gU2VjbG9yd
+000000f0: 5730 7844 5441 4c42 674e 5642 4163 4d42  W0xDTALBgNVBAcMB
+00000100: 4574 3561 5859 7843 7a41 4a42 674e 5642  Et5aXYxCzAJBgNVB
+00000110: 4159 5441 6c56 424d 4234 5844 5445 344d  AYTAlVBMB4XDTE4M
+00000120: 4451 780d 0a4d 4445 784d 7a4d 774d 466f  DQx..MDExMzMwMFo
+00000130: 5844 5449 324d 4459 794e 7a45 784d 7a4d  XDTI2MDYyNzExMzM
+00000140: 774d 466f 7767 5930 7846 7a41 5642 674e  wMFowgY0xFzAVBgN
+00000150: 5642 414d 4d44 6b5a 3163 326c 7662 6942  VBAMMDkZ1c2lvbiB
+00000160: 5362 3239 300d 0a49 454e 424d 536b 774a  Sb290..IENBMSkwJ
+00000170: 7759 4a4b 6f5a 4968 7663 4e41 516b 4246  wYJKoZIhvcNAQkBF
+00000180: 6870 3262 3278 765a 486c 7465 584a 6659  hp2b2xvZHlteXJfY
+00000190: 6d46 6959 3268 3161 3042 6c63 4746 744c  mFiY2h1a0BlcGFtL
+000001a0: 6d4e 7662 5445 4e0d 0a4d 4173 4741 3155  mNvbTEN..MAsGA1U
+000001b0: 4543 6777 4552 5642 4254 5445 634d 426f  ECgwERVBBTTEcMBo
+000001c0: 4741 3155 4543 7777 5454 6d39 3264 584d  GA1UECwwTTm92dXM
+000001d0: 6754 334a 6b62 7942 545a 574e 7362 334a  gT3JkbyBTZWNsb3J
+000001e0: 3162 5445 4e4d 4173 470d 0a41 3155 4542  1bTENMAsG..A1UEB
+000001f0: 7777 4553 336c 7064 6a45 4c4d 416b 4741  wwES3lpdjELMAkGA
+00000200: 3155 4542 684d 4356 5545 7767 6745 694d  1UEBhMCVUEwggEiM
+00000210: 4130 4743 5371 4753 4962 3344 5145 4241  A0GCSqGSIb3DQEBA
+00000220: 5155 4141 3449 4244 7741 770d 0a67 6745  QUAA4IBDwAw..ggE
+00000230: 4b41 6f49 4241 5143 2b4b 326f 7732 484f  KAoIBAQC+K2ow2HO
+00000240: 372b 5355 5666 4f71 3574 5474 6d48 6a34  7+SUVfOq5tTtmHj4
+00000250: 4c51 696a 484a 3830 336d 4c6b 3970 6b50  LQijHJ803mLk9pkP
+00000260: 6566 2b47 6c6d 6579 7039 4858 650d 0a6a  ef+Glmeyp9HXe..j
+00000270: 446c 5143 3034 4d65 6f76 4d42 654e 5461  DlQC04MeovMBeNTa
+00000280: 7130 7769 6266 3771 6173 396e 6958 6265  q0wibf7qas9niXbe
+00000290: 5852 567a 6865 5a49 467a 694d 5871 5275  XRVzheZIFziMXqRu
+000002a0: 774c 7163 304b 5864 4478 4944 5054 620d  wLqc0KXdDxIDPTb.
+000002b0: 0a54 5733 4b30 4845 364d 2f65 4174 5466  .TW3K0HE6M/eAtTf
+000002c0: 6e39 2b5a 2f4c 6e6b 5774 347a 4d58 6173  n9+Z/LnkWt4zMXas
+000002d0: 6330 3268 7675 6673 6d49 5645 754e 6263  c02hvufsmIVEuNbc
+000002e0: 3156 6872 734a 4a67 3575 6b38 386c 6450  1VhrsJJg5uk88ldP
+000002f0: 4d0d 0a4c 5346 376e 6666 3965 595a 5448  M..LSF7nff9eYZTH
+00000300: 5967 4379 426b 7439 614c 2b66 776f 584f  YgCyBkt9aL+fwoXO
+00000310: 3665 5344 5341 686a 6f70 5833 6c68 6469  6eSDSAhjopX3lhdi
+00000320: 646b 4d2b 6e69 3745 4f68 6c4e 3753 546d  dkM+ni7EOhlN7STm
+00000330: 6744 4d0d 0a57 4b68 396e 4d6a 5844 3566  gDM..WKh9nMjXD5f
+00000340: 3238 5047 6874 572f 645a 766e 3453 7a61  28PGhtW/dZvn4Sza
+00000350: 7352 4535 4d65 6145 7849 6c42 6d68 6b57  sRE5MeaExIlBmhkW
+00000360: 4555 6756 4379 5037 4c76 7551 4752 5550  EUgVCyP7LvuQGRUP
+00000370: 4b2b 4e59 7a0d 0a46 4532 434c 5275 6972  K+NYz..FE2CLRuir
+00000380: 4c43 5779 3148 4974 396c 4c7a 6950 6a6c  LCWy1HIt9lLziPjl
+00000390: 5a34 3336 316d 4e41 674d 4241 4147 6a59  Z4361mNAgMBAAGjY
+000003a0: 7a42 684d 4230 4741 3155 6444 6751 5742  zBhMB0GA1UdDgQWB
+000003b0: 4252 3053 6868 7a0d 0a4f 754d 3935 4268  BR0Shhz..OuM95Bh
+000003c0: 4430 6d57 7843 316a 2b4b 7245 3655 6a41  D0mWxC1j+KrE6UjA
+000003d0: 4d42 674e 5648 524d 4542 5441 4441 5148  MBgNVHRMEBTADAQH
+000003e0: 2f4d 4173 4741 3155 6444 7751 4541 7749  /MAsGA1UdDwQEAwI
+000003f0: 4242 6a41 6c42 674e 560d 0a48 5245 4548  BBjAlBgNV..HREEH
+00000400: 6a41 6367 5270 3262 3278 765a 486c 7465  jAcgRp2b2xvZHlte
+00000410: 584a 6659 6d46 6959 3268 3161 3042 6c63  XJfYmFiY2h1a0Blc
+00000420: 4746 744c 6d4e 7662 5441 4e42 676b 7168  GFtLmNvbTANBgkqh
+00000430: 6b69 4739 7730 4241 5173 460d 0a41 414f  kiG9w0BAQsF..AAO
+00000440: 4341 5145 416c 3862 7631 4854 5965 336c  CAQEAl8bv1HTYe3l
+00000450: 3459 2b67 3054 565a 5237 6259 4c35 424e  4Y+g0TVZR7bYL5BN
+00000460: 736e 4767 7179 3071 5335 6675 3939 316b  snGgqy0qS5fu991k
+00000470: 6858 5766 2b5a 7761 324d 4c56 6e0d 0a59  hXWf+Zwa2MLVn..Y
+00000480: 616b 4d6e 4c6b 6a76 6448 7155 7057 4d4a  akMnLkjvdHqUpWMJ
+00000490: 2f53 3832 6f32 7a57 476d 6d75 7863 6135  /S82o2zWGmmuxca5
+000004a0: 3665 686a 7843 6950 2f6e 6b6d 344d 3734  6ehjxCiP/nkm4M74
+000004b0: 7958 7a32 5238 6375 3532 5778 596e 460d  yXz2R8cu52WxYnF.
+000004c0: 0a79 4d76 6761 777a 5136 6331 7968 765a  .yMvgawzQ6c1yhvZ
+000004d0: 6976 2f67 4545 374b 6462 5952 564b 4c48  iv/gEE7KdbYRVKLH
+000004e0: 5067 427a 6679 7570 3231 6935 6e67 536c  PgBzfyup21i5ngSl
+000004f0: 5463 4d52 5253 376f 4f42 6d6f 7965 3471  TcMRRS7oOBmoye4q
+00000500: 630d 0a36 6164 7136 4874 5936 582f 4f6e  c..6adq6HtY6X/On
+00000510: 5a39 4935 786f 524e 3147 6376 614c 5567  Z9I5xoRN1GcvaLUg
+00000520: 5545 3669 6754 6956 6131 7046 386b 6564  UE6igTiVa1pF8ked
+00000530: 5768 4859 3777 7a54 5842 787a 5376 495a  WhHY7wzTXBxzSvIZ
+00000540: 6b43 550d 0a56 4845 4f7a 7661 476b 396d  kCU..VHEOzvaGk9m
+00000550: 6950 366e 4272 4466 4e76 376d 496b 6745  iP6nBrDfNv7mIkgE
+00000560: 4b41 5272 6a6a 5370 6d4a 6173 4945 552b  KARrjjSpmJasIEU+
+00000570: 6d4e 747a 654f 4945 694d 7457 3145 4d52  mNtzeOIEiMtW1EMR
+00000580: 6334 3537 6f0d 0a30 5064 4649 336a 7365  c457o..0PdFI3jse
+00000590: 794c 5650 5668 457a 556b 7543 376d 776a  yLVPVhEzUkuC7mwj
+000005a0: 6237 4365 513d 3d0d 0a2d 2d2d 2d2d 454e  b7CeQ==..-----EN
+000005b0: 4420 4345 5254 4946 4943 4154 452d 2d2d  D CERTIFICATE---
+000005c0: 2d2d 0d0a 2d2d 2d2d 2d42 4547 494e 2043  --..-----BEGIN C
+000005d0: 4552 5449 4649 4341 5445 2d2d 2d2d 2d0d  ERTIFICATE-----.
+000005e0: 0a4d 4949 4463 5443 4341 6c6d 6741 7749  .MIIDcTCCAlmgAwI
+000005f0: 4241 6749 5561 4161 6539 2b76 576e 4b56  BAgIUaAae9+vWnKV
+00000600: 7451 4b2f 536c 6c54 436e 696b 4d43 666f  tQK/SllTCnikMCfo
+00000610: 7744 5159 4a4b 6f5a 4968 7663 4e41 5145  wDQYJKoZIhvcNAQE
+00000620: 4c0d 0a42 5141 7751 6a45 554d 4249 4741  L..BQAwQjEUMBIGA
+00000630: 3155 4541 7777 4c51 5739 7a49 464a 7662  1UEAwwLQW9zIFJvb
+00000640: 3351 6751 3045 7844 7a41 4e42 674e 5642  3QgQ0ExDzANBgNVB
+00000650: 416f 4d42 6b35 3159 5735 6a5a 5445 4d4d  AoMBk51YW5jZTEMM
+00000660: 416f 470d 0a41 3155 4543 7777 4451 5739  AoG..A1UECwwDQW9
+00000670: 7a4d 5173 7743 5159 4456 5151 4745 774a  zMQswCQYDVQQGEwJ
+00000680: 5655 7a41 6746 7730 794d 4445 784d 5463  VUzAgFw0yMDExMTc
+00000690: 784d 4449 344d 444e 6147 4138 794d 4455  xMDI4MDNaGA8yMDU
+000006a0: 774d 5445 780d 0a4d 4445 774d 6a67 774d  wMTEx..MDEwMjgwM
+000006b0: 316f 7751 6a45 554d 4249 4741 3155 4541  1owQjEUMBIGA1UEA
+000006c0: 7777 4c51 5739 7a49 464a 7662 3351 6751  wwLQW9zIFJvb3QgQ
+000006d0: 3045 7844 7a41 4e42 674e 5642 416f 4d42  0ExDzANBgNVBAoMB
+000006e0: 6b35 3159 5735 6a0d 0a5a 5445 4d4d 416f  k51YW5j..ZTEMMAo
+000006f0: 4741 3155 4543 7777 4451 5739 7a4d 5173  GA1UECwwDQW9zMQs
+00000700: 7743 5159 4456 5151 4745 774a 5655 7a43  wCQYDVQQGEwJVUzC
+00000710: 4341 5349 7744 5159 4a4b 6f5a 4968 7663  CASIwDQYJKoZIhvc
+00000720: 4e41 5145 4242 5141 440d 0a67 6745 5041  NAQEBBQAD..ggEPA
+00000730: 4443 4341 516f 4367 6745 4241 4e73 4a65  DCCAQoCggEBANsJe
+00000740: 624b 4d6f 7232 7844 6c51 7241 3739 4566  bKMor2xDlQrA79Ef
+00000750: 4c51 3531 596e 6344 745a 6d78 4c4b 382b  LQ51YncDtZmxLK8+
+00000760: 5968 4c78 4c2f 3234 5853 420d 0a58 4454  YhLxL/24XSB..XDT
+00000770: 6f44 474c 6174 6563 7273 3631 4551 6953  oDGLatecrs61EQiS
+00000780: 6f74 4c4f 3749 6c5a 7742 3367 665a 554b  otLO7IlZwB3gfZUK
+00000790: 6d4c 6451 7953 6757 4169 5253 6968 6c7a  mLdQySgWAiRSihlz
+000007a0: 7678 396d 3043 4873 5366 4833 650d 0a72  vx9m0CHsSfH3e..r
+000007b0: 704a 4c6a 6e6a 6953 365a 4a68 426b 5177  pJLjnjiS6ZJhBkQw
+000007c0: 732b 6241 5669 4e34 795a 7551 7063 4b73  s+bAViN4yZuQpcKs
+000007d0: 7879 6762 3177 7a37 6172 4f79 6c32 6e59  xygb1wz7arOyl2nY
+000007e0: 4544 4d7a 2b68 7964 3863 7337 5531 480d  EDMz+hyd8cs7U1H.
+000007f0: 0a30 4a4a 6749 3170 5042 554c 634b 654c  .0JJgI1pPBULcKeL
+00000800: 6643 4750 475a 7566 4236 5965 4966 5054  fCGPGZufB6YeIfPT
+00000810: 5550 2f43 4534 3968 6277 4d75 4858 6870  UP/CE49hbwMuHXhp
+00000820: 4463 354c 7330 5342 5857 5556 666b 424d  Dc5Ls0SBXWUVfkBM
+00000830: 450d 0a4a 7275 654d 497a 4a52 5177 5532  E..JrueMIzJRQwU2
+00000840: 394e 2b33 3250 6867 624c 5a75 776f 544a  9N+32PhgbLZuwoTJ
+00000850: 5669 2b56 634b 5266 4632 4f62 7773 647a  Vi+VcKRfF2Obwsdz
+00000860: 6348 3633 6454 4169 796a 4372 4d59 5934  cH63dTAiyjCrMYY4
+00000870: 6764 630d 0a32 3075 626a 6479 6e57 3778  gdc..20ubjdynW7x
+00000880: 3367 784f 5751 6830 4f32 696b 6e69 2f4f  3gxOWQh0O2ikni/O
+00000890: 5478 6f7a 7758 3738 6c72 4345 4341 7745  TxozwX78lrCECAwE
+000008a0: 4141 614e 644d 4673 7744 4159 4456 5230  AAaNdMFswDAYDVR0
+000008b0: 5442 4155 770d 0a41 7745 422f 7a41 6442  TBAUw..AwEB/zAdB
+000008c0: 674e 5648 5134 4546 6751 554f 656e 4436  gNVHQ4EFgQUOenD6
+000008d0: 5562 4f43 6c49 3344 4d67 4a36 3041 3266  UbOClI3DMgJ60A2f
+000008e0: 5537 536a 5938 7748 7759 4456 5230 6a42  U7SjY8wHwYDVR0jB
+000008f0: 4267 7746 6f41 550d 0a4f 656e 4436 5562  BgwFoAU..OenD6Ub
+00000900: 4f43 6c49 3344 4d67 4a36 3041 3266 5537  OClI3DMgJ60A2fU7
+00000910: 536a 5938 7743 7759 4456 5230 5042 4151  SjY8wCwYDVR0PBAQ
+00000920: 4441 6747 474d 4130 4743 5371 4753 4962  DAgGGMA0GCSqGSIb
+00000930: 3344 5145 4243 7755 410d 0a41 3449 4241  3DQEBCwUA..A4IBA
+00000940: 5142 5151 6f69 3638 6c6d 4541 506d 6373  QBQQoi68lmEAPmcs
+00000950: 4941 6958 3367 696c 6d76 7565 6164 6963  IAiX3gilmvueadic
+00000960: 5a65 6f42 4b61 4b61 4846 4a6c 4c31 4341  ZeoBKaKaHFJlL1CA
+00000970: 7648 5748 544c 6330 474c 720d 0a6f 4c33  vHWHTLc0GLr..oL3
+00000980: 5871 5657 3569 7165 474c 3865 7533 4f6d  XqVW5iqeGL8eu3Om
+00000990: 6961 7850 4959 3466 327a 786f 4148 474c  iaxPIY4f2zxoAHGL
+000009a0: 5459 3375 722f 4f30 3347 4251 4532 6a42  TY3ur/O03GBQE2jB
+000009b0: 7556 3675 4f70 5874 4e63 3064 360d 0a58  uV6uOpXtNc0d6..X
+000009c0: 4470 342f 772f 704d 6345 6458 7337 5439  Dp4/w/pMcEdXs7T9
+000009d0: 4f38 6c4c 496a 7976 532b 6866 6f53 4764  O8lLIjyvS+hfoSGd
+000009e0: 3958 346b 4e4b 694d 6135 536d 6f35 5530  9X4kNKiMa5Smo5U0
+000009f0: 566f 414c 4f4d 4667 5245 3656 5a46 660d  VoALOMFgRE6VZFf.
+00000a00: 0a57 7132 4575 7541 5445 7837 4643 5a64  .Wq2EuuATEx7FCZd
+00000a10: 3450 6b63 4f4c 7346 666f 614c 7465 4561  4PkcOLsFfoaLteEa
+00000a20: 326c 5734 356f 5749 626c 6c4d 6e33 6557  2lW45oWIbllMn3eW
+00000a30: 796f 382b 4332 5139 5277 336b 627a 496f  yo8+C2Q9Rw3kbzIo
+00000a40: 740d 0a32 5962 5059 6b50 6273 4633 452f  t..2YbPYkPbsF3E/
+00000a50: 6352 3455 5a46 386a 4742 6e65 4838 304d  cR4UZF8jGBneH80M
+00000a60: 746b 3034 4577 5635 6f62 6e67 4642 7174  tk04EwV5obngFBqt
+00000a70: 3355 655a 796a 5658 4168 7775 6d5a 7436  3UeZyjVXAhwumZt6
+00000a80: 522b 4a0d 0a72 467a 5a6c 6443 626d 3478  R+J..rFzZldCbm4x
+00000a90: 6a2b 7052 4668 7935 4643 6b48 4970 6950  j+pRFhy5FCkHIpiP
+00000aa0: 6a0d 0a2d 2d2d 2d2d 454e 4420 4345 5254  j..-----END CERT
+00000ab0: 4946 4943 4154 452d 2d2d 2d2d 0d0a       IFICATE-----..
```

## aos_prov/utils/__init__.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-
-import os
-
-# SDK home directory name
-SDK_TOOL_DIR_NAME = '.aos'
-# SDK home directory full path
-SDK_FULL_PATH = os.path.join(os.path.expanduser("~"), SDK_TOOL_DIR_NAME)
-# Default directory with user keys and certificates
-SDK_SECURITY_PATH = os.path.join(SDK_FULL_PATH, 'security')
-
-# Default user certificate filename
-USER_CERTIFICATE_FILE_NAME = 'oem-client.pem'
-# Default user key filename
-USER_KEY_FILE_NAME = 'private_key.pem'
-
-# Default user certificate full path
-DEFAULT_USER_CERT_PATH = os.path.join(SDK_SECURITY_PATH, USER_CERTIFICATE_FILE_NAME)
-# Default user key full path
-DEFAULT_USER_KEY_PATH = os.path.join(SDK_SECURITY_PATH, USER_KEY_FILE_NAME)
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+
+import os
+
+# SDK home directory name
+SDK_TOOL_DIR_NAME = '.aos'
+# SDK home directory full path
+SDK_FULL_PATH = os.path.join(os.path.expanduser("~"), SDK_TOOL_DIR_NAME)
+# Default directory with user keys and certificates
+SDK_SECURITY_PATH = os.path.join(SDK_FULL_PATH, 'security')
+
+# Default user certificate filename
+USER_CERTIFICATE_FILE_NAME = 'oem-client.pem'
+# Default user key filename
+USER_KEY_FILE_NAME = 'private_key.pem'
+
+# Default user certificate full path
+DEFAULT_USER_CERT_PATH = os.path.join(SDK_SECURITY_PATH, USER_CERTIFICATE_FILE_NAME)
+# Default user key full path
+DEFAULT_USER_KEY_PATH = os.path.join(SDK_SECURITY_PATH, USER_KEY_FILE_NAME)
```

## aos_prov/utils/common.py

 * *Ordering differences only*

```diff
@@ -1,54 +1,54 @@
-#
-#  Copyright (c) 2018-2023 Renesas Inc.
-#  Copyright (c) 2018-2023 EPAM Systems Inc.
-#
-
-import random
-import string
-from pathlib import Path
-
-from rich.console import Console
-
-CONTENT_ENCRYPTION_ALGORITHM = 'aes256_cbc'
-DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
-AOS_DISKS_PATH = DOWNLOADS_PATH
-NODE0_IMAGE_FILENAME = 'aos-vm-node0-genericx86-64.wic.vmdk'
-NODE1_IMAGE_FILENAME = 'aos-vm-node1-genericx86-64.wic.vmdk'
-
-DISK_IMAGE_DOWNLOAD_URL = 'https://aos-prod-cdn-endpoint.azureedge.net/vm/R4.0.5.tar.gz?' \
-                          '0b4212dd0fd3cf5e29e44f35e2b3fafa474156bf99a8b9399de3b40bb0586a' \
-                          '0822e3a9396e05a96aed7f8e79650aeabdd0abe0d1876b2a621c37e28ebc' \
-
-console = Console()
-error_console = Console(stderr=True, style='red')
-allow_print = True
-
-def print_message(formatted_text, end="\n", ljust: int = 0):
-    if allow_print:
-        if ljust > 0:
-            formatted_text = formatted_text.ljust(ljust)
-        console.print(formatted_text, end=end)
-
-def print_left(formatted_text, ljust=60):
-    print_message(formatted_text, end='', ljust = ljust)
-
-def print_done():
-    print_message('[green]DONE')
-
-def print_success(message):
-    print_message(f'[green]{str(message)}')
-
-def print_error(message):
-    if allow_print:
-        error_console.print(message)
-
-def generate_random_password() -> str:
-    """
-    Generate random password from letters and digits.
-
-    Returns:
-        str: Random string password
-    """
-    dictionary = string.ascii_letters + string.digits
-    password_length = random.randint(10, 15)
-    return ''.join(random.choice(dictionary) for _ in range(password_length))
+#
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
+#
+
+import random
+import string
+from pathlib import Path
+
+from rich.console import Console
+
+CONTENT_ENCRYPTION_ALGORITHM = 'aes256_cbc'
+DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
+AOS_DISKS_PATH = DOWNLOADS_PATH
+NODE0_IMAGE_FILENAME = 'aos-vm-node0-genericx86-64.wic.vmdk'
+NODE1_IMAGE_FILENAME = 'aos-vm-node1-genericx86-64.wic.vmdk'
+
+DISK_IMAGE_DOWNLOAD_URL = 'https://aos-prod-cdn-endpoint.azureedge.net/vm/R4.0.5.tar.gz?' \
+                          '0b4212dd0fd3cf5e29e44f35e2b3fafa474156bf99a8b9399de3b40bb0586a' \
+                          '0822e3a9396e05a96aed7f8e79650aeabdd0abe0d1876b2a621c37e28ebc' \
+
+console = Console()
+error_console = Console(stderr=True, style='red')
+allow_print = True
+
+def print_message(formatted_text, end="\n", ljust: int = 0):
+    if allow_print:
+        if ljust > 0:
+            formatted_text = formatted_text.ljust(ljust)
+        console.print(formatted_text, end=end)
+
+def print_left(formatted_text, ljust=60):
+    print_message(formatted_text, end='', ljust = ljust)
+
+def print_done():
+    print_message('[green]DONE')
+
+def print_success(message):
+    print_message(f'[green]{str(message)}')
+
+def print_error(message):
+    if allow_print:
+        error_console.print(message)
+
+def generate_random_password() -> str:
+    """
+    Generate random password from letters and digits.
+
+    Returns:
+        str: Random string password
+    """
+    dictionary = string.ascii_letters + string.digits
+    password_length = random.randint(10, 15)
+    return ''.join(random.choice(dictionary) for _ in range(password_length))
```

## aos_prov/utils/config.py

 * *Ordering differences only*

```diff
@@ -1,88 +1,88 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-
-class Config(object):
-    """Contains a provisioning procedure configuration."""
-
-    def __init__(self):
-        self._system_id = None
-        self._model_name = None
-        self._model_version = None
-        self._user_claim = None
-        self._supported_cert_types = None
-        self._protocol_version = None
-        self._node_ids = None
-        self._unit_certificates = []
-
-    @property
-    def system_id(self) -> str:
-        """Return System ID of the Unit."""
-        return self._system_id
-
-    @system_id.setter
-    def system_id(self, sys_id):
-        self._system_id = sys_id
-
-    @property
-    def model_name(self) -> str:
-        """Return Model Name of the Unit. It is defined by the manufacturer."""
-        return self._model_name
-
-    @property
-    def model_version(self) -> str:
-        """Return Model Version or Revision of the Unit. It is defined by the manufacturer."""
-        return self._model_version
-
-    @property
-    def supported_cert_types(self) -> [str]:
-        """Return list of certificate names to be set on the Unit."""
-        return self._supported_cert_types
-
-    @supported_cert_types.setter
-    def supported_cert_types(self, cert_types):
-        self._supported_cert_types = cert_types
-
-    @property
-    def protocol_version(self) -> int:
-        """Return api version."""
-        return self._protocol_version
-
-    @protocol_version.setter
-    def protocol_version(self, protocol_version):
-        self._protocol_version = protocol_version
-
-    @property
-    def node_ids(self) -> [str]:
-        """Return list of node Ids."""
-        return self._node_ids
-
-    @node_ids.setter
-    def node_ids(self, node_ids):
-        self._node_ids = node_ids
-
-    @property
-    def unit_certificates(self) -> [UnitCertificate]:
-        """Return list of Unit certificates objects."""
-        return self._unit_certificates
-
-    @unit_certificates.setter
-    def unit_certificates(self, unit_certs):
-        self._unit_certificates = unit_certs
-
-    def set_model(self, model_string):
-        """Parse model name and version received from the Unit.
-
-        Args:
-            model_string: model info returned by Unit.
-        """
-        model_chunks = model_string.strip().split(';')
-        self._model_name = model_chunks[0].strip()
-        if len(model_chunks) > 1:
-            self._model_version = model_chunks[1].strip()
-        else:
-            self._model_version = 'Unknown'
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+
+class Config(object):
+    """Contains a provisioning procedure configuration."""
+
+    def __init__(self):
+        self._system_id = None
+        self._model_name = None
+        self._model_version = None
+        self._user_claim = None
+        self._supported_cert_types = None
+        self._protocol_version = None
+        self._node_ids = None
+        self._unit_certificates = []
+
+    @property
+    def system_id(self) -> str:
+        """Return System ID of the Unit."""
+        return self._system_id
+
+    @system_id.setter
+    def system_id(self, sys_id):
+        self._system_id = sys_id
+
+    @property
+    def model_name(self) -> str:
+        """Return Model Name of the Unit. It is defined by the manufacturer."""
+        return self._model_name
+
+    @property
+    def model_version(self) -> str:
+        """Return Model Version or Revision of the Unit. It is defined by the manufacturer."""
+        return self._model_version
+
+    @property
+    def supported_cert_types(self) -> [str]:
+        """Return list of certificate names to be set on the Unit."""
+        return self._supported_cert_types
+
+    @supported_cert_types.setter
+    def supported_cert_types(self, cert_types):
+        self._supported_cert_types = cert_types
+
+    @property
+    def protocol_version(self) -> int:
+        """Return api version."""
+        return self._protocol_version
+
+    @protocol_version.setter
+    def protocol_version(self, protocol_version):
+        self._protocol_version = protocol_version
+
+    @property
+    def node_ids(self) -> [str]:
+        """Return list of node Ids."""
+        return self._node_ids
+
+    @node_ids.setter
+    def node_ids(self, node_ids):
+        self._node_ids = node_ids
+
+    @property
+    def unit_certificates(self) -> [UnitCertificate]:
+        """Return list of Unit certificates objects."""
+        return self._unit_certificates
+
+    @unit_certificates.setter
+    def unit_certificates(self, unit_certs):
+        self._unit_certificates = unit_certs
+
+    def set_model(self, model_string):
+        """Parse model name and version received from the Unit.
+
+        Args:
+            model_string: model info returned by Unit.
+        """
+        model_chunks = model_string.strip().split(';')
+        self._model_name = model_chunks[0].strip()
+        if len(model_chunks) > 1:
+            self._model_version = model_chunks[1].strip()
+        else:
+            self._model_version = 'Unknown'
```

## aos_prov/utils/errors.py

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-
-
-class OnUnitError(Exception):
-    pass
-
-
-class UserCredentialsError(OnUnitError):
-    pass
-
-
-class DeviceRegisterError(OnUnitError):
-    pass
-
-
-class DeviceDeregisterError(OnUnitError):
-    pass
-
-
-class UnitError(OnUnitError):
-    pass
-
-
-class GrpcUnimplemented(OnUnitError):
-    pass
-
-
-class CloudAccessError(OnUnitError):
-    pass
-
-
-class AosProvError(OnUnitError):
-    pass
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+
+
+class OnUnitError(Exception):
+    pass
+
+
+class UserCredentialsError(OnUnitError):
+    pass
+
+
+class DeviceRegisterError(OnUnitError):
+    pass
+
+
+class DeviceDeregisterError(OnUnitError):
+    pass
+
+
+class UnitError(OnUnitError):
+    pass
+
+
+class GrpcUnimplemented(OnUnitError):
+    pass
+
+
+class CloudAccessError(OnUnitError):
+    pass
+
+
+class AosProvError(OnUnitError):
+    pass
```

## aos_prov/utils/unit_certificate.py

 * *Ordering differences only*

```diff
@@ -1,53 +1,53 @@
-#
-#  Copyright (c) 2018-2022 Renesas Inc.
-#  Copyright (c) 2018-2022 EPAM Systems Inc.
-#
-
-"""Unit certificate object."""
-
-
-class UnitCertificate:
-    """Unit certificate object."""
-
-    def __init__(self):
-        """Unit certificate object."""
-        self._cert_type = None
-        self._csr = None
-        self._node_id = None
-        self._certificate = None
-
-    @property
-    def cert_type(self) -> str:
-        """Certificate type (Required type list is taken from unit)."""
-        return self._cert_type
-
-    @cert_type.setter
-    def cert_type(self, cert_type):
-        self._cert_type = cert_type
-
-    @property
-    def csr(self) -> str:
-        """Certificate Signing Request."""
-        return self._csr
-
-    @csr.setter
-    def csr(self, csr_value):
-        self._csr = csr_value
-
-    @property
-    def node_id(self) -> str:
-        """Node ID."""
-        return self._node_id
-
-    @node_id.setter
-    def node_id(self, node_id):
-        self._node_id = node_id
-
-    @property
-    def certificate(self) -> str:
-        """Certificate."""
-        return self._certificate
-
-    @certificate.setter
-    def certificate(self, cert):
-        self._certificate = cert
+#
+#  Copyright (c) 2018-2022 Renesas Inc.
+#  Copyright (c) 2018-2022 EPAM Systems Inc.
+#
+
+"""Unit certificate object."""
+
+
+class UnitCertificate:
+    """Unit certificate object."""
+
+    def __init__(self):
+        """Unit certificate object."""
+        self._cert_type = None
+        self._csr = None
+        self._node_id = None
+        self._certificate = None
+
+    @property
+    def cert_type(self) -> str:
+        """Certificate type (Required type list is taken from unit)."""
+        return self._cert_type
+
+    @cert_type.setter
+    def cert_type(self, cert_type):
+        self._cert_type = cert_type
+
+    @property
+    def csr(self) -> str:
+        """Certificate Signing Request."""
+        return self._csr
+
+    @csr.setter
+    def csr(self, csr_value):
+        self._csr = csr_value
+
+    @property
+    def node_id(self) -> str:
+        """Node ID."""
+        return self._node_id
+
+    @node_id.setter
+    def node_id(self, node_id):
+        self._node_id = node_id
+
+    @property
+    def certificate(self) -> str:
+        """Certificate."""
+        return self._certificate
+
+    @certificate.setter
+    def certificate(self, cert):
+        self._certificate = cert
```

## aos_prov/utils/user_credentials.py

 * *Ordering differences only*

```diff
@@ -1,184 +1,184 @@
-#
-#  Copyright (c) 2018-2021 Renesas Inc.
-#  Copyright (c) 2018-2021 EPAM Systems Inc.
-#
-import os
-import tempfile
-from os.path import isfile
-from pathlib import Path
-from typing import Optional
-
-import OpenSSL
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives._serialization import Encoding, PrivateFormat, NoEncryption
-from cryptography.hazmat.primitives.serialization.pkcs12 import load_key_and_certificates
-from cryptography.x509.oid import NameOID
-
-from aos_prov.utils import SDK_SECURITY_PATH
-from aos_prov.utils.errors import UserCredentialsError
-
-
-def _extract_cloud_domain_from_cert(cert_bytes: bytes) -> str:
-    """Get the Cloud domain name from user certificate."""
-    private_key, certificate, additional_certificates = load_key_and_certificates(cert_bytes, None)
-    return certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)[0].value
-
-
-def _pkcs12_to_pem(pkcs12_bytes: bytes):
-    private_key, certificate, additional_certificates = \
-        load_key_and_certificates(pkcs12_bytes, ''.encode('utf8'), default_backend())
-
-    cert_bytes = bytearray(certificate.public_bytes(Encoding.PEM))
-    for add_cert in additional_certificates:
-        cert_bytes += add_cert.public_bytes(Encoding.PEM)
-    key_bytes = private_key.private_bytes(Encoding.PEM, PrivateFormat.PKCS8, NoEncryption())
-    cert_bytes = bytes(cert_bytes)
-    return cert_bytes, key_bytes
-
-
-def _create_temp_file(data: bytes):
-    tmp_file = tempfile.NamedTemporaryFile(delete=False)
-    tmp_file.write(data)
-    tmp_file.close()
-    return tmp_file.name
-
-
-class TempCredentials:
-    def __init__(self, certificate: Optional[bytes], key: Optional[bytes],
-                 cert_file_name: Optional[str], key_file_name: Optional[str]):
-        self._key_file_name = key_file_name
-        self._cert_file_name = cert_file_name
-
-        self._key = None
-        self._certificate = None
-
-        if certificate and key:
-            self._key = key
-            self._certificate = certificate
-
-    def __enter__(self):
-        if not self._key_file_name:
-            self._key_file_name = _create_temp_file(self._key)
-        if not self._cert_file_name:
-            self._cert_file_name = _create_temp_file(self._certificate)
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._key:
-            os.unlink(self._key_file_name)
-            self._key_file_name = None
-        if self._certificate:
-            os.unlink(self._cert_file_name)
-            self._cert_file_name = None
-
-    @property
-    def key_file_name(self):
-        return self._key_file_name
-
-    @property
-    def cert_file_name(self):
-        return self._cert_file_name
-
-
-class UserCredentials:
-
-    def __init__(self, cert_file_path: Optional[str], key_file_path: Optional[str], pkcs12: Optional[str]):
-        self._cert_file_path = cert_file_path
-        self._key_file_path = key_file_path
-        self._cloud_url = None
-        if pkcs12:
-            if Path(pkcs12).exists():
-                with open(pkcs12, 'rb') as pkcs12_file:
-                    pkcs12_file_content = pkcs12_file.read()
-                    cert_bytes, key_bytes = _pkcs12_to_pem(pkcs12_file_content)
-                    self._user_credentials = TempCredentials(certificate=cert_bytes, key=key_bytes,
-                                                             cert_file_name=None, key_file_name=None)
-                    self._cloud_url = _extract_cloud_domain_from_cert(pkcs12_file_content)
-            else:
-                if not Path(cert_file_path).exists() or not Path(key_file_path).exists():
-                    raise UserCredentialsError(f'User credentials file {pkcs12} not found.')
-                else:
-                    self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
-                                                             certificate=None, key=None)
-                    self._validate_credentials_format()
-                    self._cloud_url = self._extract_cloud_url()
-
-        else:
-            if not Path(cert_file_path).exists():
-                raise UserCredentialsError(f'User credentials file {cert_file_path} not found.')
-            elif not Path(key_file_path).exists():
-                raise UserCredentialsError(f'User credentials file {key_file_path} not found.')
-            else:
-                self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
-                                                         certificate=None, key=None)
-                self._validate_credentials_format()
-                self._cloud_url = self._extract_cloud_url()
-
-    @property
-    def cloud_url(self):
-        return self._cloud_url
-
-    @property
-    def user_credentials(self):
-        return self._user_credentials
-
-    def _check_credentials_access(self):
-        """ Validate existence and access to user credential files
-
-            Raises:
-                UserCredentialsError: If credentials files are not found
-            Returns:
-                None
-        """
-
-        if not isfile(self._cert_file_path):
-            text = (f"[red]Can't find user certificate file...[/red]\n\n"
-                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
-                    f"or set path to the certificate file with argument: --cert \n"
-                    f"(Example: aos-prov -u 127.0.0.1 --cert /path/to/certfile) \n")
-            raise UserCredentialsError(text)
-
-        if not isfile(self._key_file_path):
-            text = (f"[red]Can't find user key file...[/red]\n\n"
-                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
-                    f"or set path to the key file with argument: --key \n"
-                    f"(Example: aos-prov -u 127.0.0.1 --key /path/to/keyfile) \n")
-            raise UserCredentialsError(text)
-
-    def _validate_credentials_format(self):
-        """ Validate format of user credential files
-
-            Raises:
-                UserCredentialsError: If credentials files are in wrong format or with errors
-            Returns:
-                None
-        """
-        with open(self._cert_file_path, "rb") as c, open(self._key_file_path, "r") as k:
-            cert_content = c.read()
-            key_content = k.read()
-
-        try:
-            private_key_obj = OpenSSL.crypto.load_privatekey(OpenSSL.crypto.FILETYPE_PEM, key_content)
-        except OpenSSL.crypto.Error:
-            raise UserCredentialsError('private key is not correct')
-
-        try:
-            cert_obj = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, cert_content)
-        except OpenSSL.crypto.Error:
-            raise UserCredentialsError('Certificate is not correct: %s' % key_content)
-
-        context = OpenSSL.SSL.Context(OpenSSL.SSL.TLSv1_2_METHOD)
-        context.use_privatekey(private_key_obj)
-        context.use_certificate(cert_obj)
-        try:
-            context.check_privatekey()
-        except OpenSSL.SSL.Error:
-            raise UserCredentialsError('User private key does not match certificate')
-
-    def _extract_cloud_url(self):
-        """Get the Cloud domain name from user certificate"""
-        with open(self._cert_file_path, "rb") as cert:
-            return OpenSSL.crypto.load_certificate(
-                OpenSSL.crypto.FILETYPE_PEM,
-                cert.read()
-            ).get_subject().organizationName
+#
+#  Copyright (c) 2018-2021 Renesas Inc.
+#  Copyright (c) 2018-2021 EPAM Systems Inc.
+#
+import os
+import tempfile
+from os.path import isfile
+from pathlib import Path
+from typing import Optional
+
+import OpenSSL
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives._serialization import Encoding, PrivateFormat, NoEncryption
+from cryptography.hazmat.primitives.serialization.pkcs12 import load_key_and_certificates
+from cryptography.x509.oid import NameOID
+
+from aos_prov.utils import SDK_SECURITY_PATH
+from aos_prov.utils.errors import UserCredentialsError
+
+
+def _extract_cloud_domain_from_cert(cert_bytes: bytes) -> str:
+    """Get the Cloud domain name from user certificate."""
+    private_key, certificate, additional_certificates = load_key_and_certificates(cert_bytes, None)
+    return certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)[0].value
+
+
+def _pkcs12_to_pem(pkcs12_bytes: bytes):
+    private_key, certificate, additional_certificates = \
+        load_key_and_certificates(pkcs12_bytes, ''.encode('utf8'), default_backend())
+
+    cert_bytes = bytearray(certificate.public_bytes(Encoding.PEM))
+    for add_cert in additional_certificates:
+        cert_bytes += add_cert.public_bytes(Encoding.PEM)
+    key_bytes = private_key.private_bytes(Encoding.PEM, PrivateFormat.PKCS8, NoEncryption())
+    cert_bytes = bytes(cert_bytes)
+    return cert_bytes, key_bytes
+
+
+def _create_temp_file(data: bytes):
+    tmp_file = tempfile.NamedTemporaryFile(delete=False)
+    tmp_file.write(data)
+    tmp_file.close()
+    return tmp_file.name
+
+
+class TempCredentials:
+    def __init__(self, certificate: Optional[bytes], key: Optional[bytes],
+                 cert_file_name: Optional[str], key_file_name: Optional[str]):
+        self._key_file_name = key_file_name
+        self._cert_file_name = cert_file_name
+
+        self._key = None
+        self._certificate = None
+
+        if certificate and key:
+            self._key = key
+            self._certificate = certificate
+
+    def __enter__(self):
+        if not self._key_file_name:
+            self._key_file_name = _create_temp_file(self._key)
+        if not self._cert_file_name:
+            self._cert_file_name = _create_temp_file(self._certificate)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self._key:
+            os.unlink(self._key_file_name)
+            self._key_file_name = None
+        if self._certificate:
+            os.unlink(self._cert_file_name)
+            self._cert_file_name = None
+
+    @property
+    def key_file_name(self):
+        return self._key_file_name
+
+    @property
+    def cert_file_name(self):
+        return self._cert_file_name
+
+
+class UserCredentials:
+
+    def __init__(self, cert_file_path: Optional[str], key_file_path: Optional[str], pkcs12: Optional[str]):
+        self._cert_file_path = cert_file_path
+        self._key_file_path = key_file_path
+        self._cloud_url = None
+        if pkcs12:
+            if Path(pkcs12).exists():
+                with open(pkcs12, 'rb') as pkcs12_file:
+                    pkcs12_file_content = pkcs12_file.read()
+                    cert_bytes, key_bytes = _pkcs12_to_pem(pkcs12_file_content)
+                    self._user_credentials = TempCredentials(certificate=cert_bytes, key=key_bytes,
+                                                             cert_file_name=None, key_file_name=None)
+                    self._cloud_url = _extract_cloud_domain_from_cert(pkcs12_file_content)
+            else:
+                if not Path(cert_file_path).exists() or not Path(key_file_path).exists():
+                    raise UserCredentialsError(f'User credentials file {pkcs12} not found.')
+                else:
+                    self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
+                                                             certificate=None, key=None)
+                    self._validate_credentials_format()
+                    self._cloud_url = self._extract_cloud_url()
+
+        else:
+            if not Path(cert_file_path).exists():
+                raise UserCredentialsError(f'User credentials file {cert_file_path} not found.')
+            elif not Path(key_file_path).exists():
+                raise UserCredentialsError(f'User credentials file {key_file_path} not found.')
+            else:
+                self._user_credentials = TempCredentials(cert_file_name=cert_file_path, key_file_name=key_file_path,
+                                                         certificate=None, key=None)
+                self._validate_credentials_format()
+                self._cloud_url = self._extract_cloud_url()
+
+    @property
+    def cloud_url(self):
+        return self._cloud_url
+
+    @property
+    def user_credentials(self):
+        return self._user_credentials
+
+    def _check_credentials_access(self):
+        """ Validate existence and access to user credential files
+
+            Raises:
+                UserCredentialsError: If credentials files are not found
+            Returns:
+                None
+        """
+
+        if not isfile(self._cert_file_path):
+            text = (f"[red]Can't find user certificate file...[/red]\n\n"
+                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
+                    f"or set path to the certificate file with argument: --cert \n"
+                    f"(Example: aos-prov -u 127.0.0.1 --cert /path/to/certfile) \n")
+            raise UserCredentialsError(text)
+
+        if not isfile(self._key_file_path):
+            text = (f"[red]Can't find user key file...[/red]\n\n"
+                    f"Copy file to the default directory: [{SDK_SECURITY_PATH}] \n"
+                    f"or set path to the key file with argument: --key \n"
+                    f"(Example: aos-prov -u 127.0.0.1 --key /path/to/keyfile) \n")
+            raise UserCredentialsError(text)
+
+    def _validate_credentials_format(self):
+        """ Validate format of user credential files
+
+            Raises:
+                UserCredentialsError: If credentials files are in wrong format or with errors
+            Returns:
+                None
+        """
+        with open(self._cert_file_path, "rb") as c, open(self._key_file_path, "r") as k:
+            cert_content = c.read()
+            key_content = k.read()
+
+        try:
+            private_key_obj = OpenSSL.crypto.load_privatekey(OpenSSL.crypto.FILETYPE_PEM, key_content)
+        except OpenSSL.crypto.Error:
+            raise UserCredentialsError('private key is not correct')
+
+        try:
+            cert_obj = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM, cert_content)
+        except OpenSSL.crypto.Error:
+            raise UserCredentialsError('Certificate is not correct: %s' % key_content)
+
+        context = OpenSSL.SSL.Context(OpenSSL.SSL.TLSv1_2_METHOD)
+        context.use_privatekey(private_key_obj)
+        context.use_certificate(cert_obj)
+        try:
+            context.check_privatekey()
+        except OpenSSL.SSL.Error:
+            raise UserCredentialsError('User private key does not match certificate')
+
+    def _extract_cloud_url(self):
+        """Get the Cloud domain name from user certificate"""
+        with open(self._cert_file_path, "rb") as cert:
+            return OpenSSL.crypto.load_certificate(
+                OpenSSL.crypto.FILETYPE_PEM,
+                cert.read()
+            ).get_subject().organizationName
```

## test/utils/test_config.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-import unittest
-from aos_prov.utils.config import Config
-
-
-class TestConfig(unittest.TestCase):
-    def test_config_can_be_created(self):
-        c = Config()
-        self.assertIsInstance(c, Config)
-
-    def test_setters_and_getters(self):
-        c = Config()
-        c.system_id = 'some system id'
-        self.assertEqual(c.system_id, 'some system id')
-
-        c.protocol_version = 5
-        self.assertEqual(c.protocol_version, 5)
-
-        c.node_ids = ['dom0', 'dom1']
-        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
-
-        c.supported_cert_types = ['um', 'sm']
-        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
-
+import unittest
+from aos_prov.utils.config import Config
+
+
+class TestConfig(unittest.TestCase):
+    def test_config_can_be_created(self):
+        c = Config()
+        self.assertIsInstance(c, Config)
+
+    def test_setters_and_getters(self):
+        c = Config()
+        c.system_id = 'some system id'
+        self.assertEqual(c.system_id, 'some system id')
+
+        c.protocol_version = 5
+        self.assertEqual(c.protocol_version, 5)
+
+        c.node_ids = ['dom0', 'dom1']
+        self.assertEqual(c.node_ids, ['dom0', 'dom1'])
+
+        c.supported_cert_types = ['um', 'sm']
+        self.assertEqual(c.supported_cert_types, ['um', 'sm'])
+
```

## test/utils/test_unit_certificate.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-import unittest
-
-from aos_prov.utils.unit_certificate import UnitCertificate
-
-
-class TestUnitCertificate(unittest.TestCase):
-    def test_object_can_be_created(self):
-        uc = UnitCertificate()
-        self.assertIsInstance(uc, UnitCertificate)
-
-    def test_attributes(self):
-        uc = UnitCertificate()
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.node_id = 'node_id'
-        self.assertEqual(uc.node_id, 'node_id')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
+import unittest
+
+from aos_prov.utils.unit_certificate import UnitCertificate
+
+
+class TestUnitCertificate(unittest.TestCase):
+    def test_object_can_be_created(self):
+        uc = UnitCertificate()
+        self.assertIsInstance(uc, UnitCertificate)
+
+    def test_attributes(self):
+        uc = UnitCertificate()
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.node_id = 'node_id'
+        self.assertEqual(uc.node_id, 'node_id')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
```

## test/utils/test_user_credentials.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-import unittest
-
-from aos_prov.utils.user_credentials import UserCredentials
-
-
-class TestUserCredentials(unittest.TestCase):
-    def test_attributes(self):
-        uc = UserCredentials('zzz', 'zz1')
-
-        uc.cert_type = 'type1'
-        self.assertEqual(uc.cert_type, 'type1')
-
-        uc.certificate = 'some cert 1'
-        self.assertEqual(uc.certificate, 'some cert 1')
-
-        uc.csr = 'csr'
-        self.assertEqual(uc.csr, 'csr')
+import unittest
+
+from aos_prov.utils.user_credentials import UserCredentials
+
+
+class TestUserCredentials(unittest.TestCase):
+    def test_attributes(self):
+        uc = UserCredentials('zzz', 'zz1')
+
+        uc.cert_type = 'type1'
+        self.assertEqual(uc.cert_type, 'type1')
+
+        uc.certificate = 'some cert 1'
+        self.assertEqual(uc.certificate, 'some cert 1')
+
+        uc.csr = 'csr'
+        self.assertEqual(uc.csr, 'csr')
```

## Comparing `aos_prov-4.2.0b1.dist-info/METADATA` & `aos_prov-4.2.0b2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: aos-prov
-Version: 4.2.0b1
+Version: 4.2.0b2
 Summary: AosEdge Unit provisioning tool
+Home-page: UNKNOWN
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -99,7 +100,9 @@
 aos-prov vm-remove --name {vm-name}
 ```
 
 ### Start Unit VMs:
 ```bash
 aos-prov vm-start --name {vm-name}
 ```
+
+
```

