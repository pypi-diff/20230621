# Comparing `tmp/iam_actions-1.2.20230620.tar.gz` & `tmp/iam_actions-1.2.20230621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230620.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230621.tar", max compression
```

## Comparing `iam_actions-1.2.20230620.tar` & `iam_actions-1.2.20230621.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/README.md
--rw-r--r--   0        0        0      228 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/__init__.py
--rw-r--r--   0        0        0  4334986 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/services.py
--rw-r--r--   0        0        0   557555 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/policies.json
--rw-r--r--   0        0        0   196395 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   540781 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-20 02:33:42.768792 iam_actions-1.2.20230620/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230620/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230620/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/README.md
+-rw-r--r--   0        0        0      228 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4337071 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-21 02:31:55.952532 iam_actions-1.2.20230621/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   557686 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/policies.json
+-rw-r--r--   0        0        0   196535 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   540907 2023-06-21 02:33:30.119694 iam_actions-1.2.20230621/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-21 02:33:31.071767 iam_actions-1.2.20230621/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230621/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230621/PKG-INFO
```

### Comparing `iam_actions-1.2.20230620/LICENSE` & `iam_actions-1.2.20230621/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/README.md` & `iam_actions-1.2.20230621/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/iam_actions/actions.json` & `iam_actions-1.2.20230621/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998027035960337%*

 * *Differences: {"'auditmanager'": "{'GetEvidenceFileUploadUrl': OrderedDict([('access_level', 'Undocumented'), "*

 * *                   "('action', 'GetEvidenceFileUploadUrl'), ('condition_keys', []), "*

 * *                   "('description', 'Not Documented by AWS'), ('orphan', False), ('resources', "*

 * *                   '[])])}',*

 * * "'mgn'": "{'ListManagedAccounts': OrderedDict([('access_level', 'List'), ('action', "*

 * *          "'ListManagedAccounts'), ('condition_keys', []), ('description', 'Grants permission to "*

 * *          "list  […]*

```diff
@@ -9043,14 +9043,22 @@
             "condition_keys": [],
             "description": "Grants permission to get all the evidence from an evidence folder in AWS Audit Manager",
             "orphan": false,
             "resources": [
                 "assessmentControlSet"
             ]
         },
+        "GetEvidenceFileUploadUrl": {
+            "access_level": "Undocumented",
+            "action": "GetEvidenceFileUploadUrl",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetEvidenceFolder": {
             "access_level": "Read",
             "action": "GetEvidenceFolder",
             "condition_keys": [],
             "description": "Grants permission to get the evidence folder from AWS Audit Manager",
             "orphan": false,
             "resources": [
@@ -98215,14 +98223,22 @@
             "access_level": "List",
             "action": "ListImports",
             "condition_keys": [],
             "description": "Grants permission to list the import tasks",
             "orphan": false,
             "resources": []
         },
+        "ListManagedAccounts": {
+            "access_level": "List",
+            "action": "ListManagedAccounts",
+            "condition_keys": [],
+            "description": "Grants permission to list managed accounts",
+            "orphan": false,
+            "resources": []
+        },
         "ListSourceServerActions": {
             "access_level": "List",
             "action": "ListSourceServerActions",
             "condition_keys": [],
             "description": "Grants permission to list source server action documents",
             "orphan": false,
             "resources": [
@@ -98311,14 +98327,24 @@
             "condition_keys": [],
             "description": "Grants permission to notify vcenter client started",
             "orphan": false,
             "resources": [
                 "VcenterClientResource"
             ]
         },
+        "PauseReplication": {
+            "access_level": "Write",
+            "action": "PauseReplication",
+            "condition_keys": [],
+            "description": "Grants permission to pause replication",
+            "orphan": false,
+            "resources": [
+                "SourceServerResource"
+            ]
+        },
         "PutSourceServerAction": {
             "access_level": "Write",
             "action": "PutSourceServerAction",
             "condition_keys": [],
             "description": "Grants permission to put source server action document",
             "orphan": false,
             "resources": [
@@ -98362,14 +98388,24 @@
             "condition_keys": [],
             "description": "Grants permission to remove launch configuration template action document",
             "orphan": false,
             "resources": [
                 "LaunchConfigurationTemplateResource"
             ]
         },
+        "ResumeReplication": {
+            "access_level": "Write",
+            "action": "ResumeReplication",
+            "condition_keys": [],
+            "description": "Grants permission to resume replication",
+            "orphan": false,
+            "resources": [
+                "SourceServerResource"
+            ]
+        },
         "RetryDataReplication": {
             "access_level": "Write",
             "action": "RetryDataReplication",
             "condition_keys": [],
             "description": "Grants permission to retry replication",
             "orphan": false,
             "resources": [
@@ -98498,14 +98534,24 @@
             ],
             "description": "Grants permission to start test",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
+        "StopReplication": {
+            "access_level": "Write",
+            "action": "StopReplication",
+            "condition_keys": [],
+            "description": "Grants permission to stop replication",
+            "orphan": false,
+            "resources": [
+                "SourceServerResource"
+            ]
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "mgn:CreateAction"
@@ -110017,122 +110063,172 @@
             "resources": []
         }
     },
     "purchase-orders": {
         "AddPurchaseOrder": {
             "access_level": "Write",
             "action": "AddPurchaseOrder",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to add a new purchase order",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "DeletePurchaseOrder": {
             "access_level": "Write",
             "action": "DeletePurchaseOrder",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to delete a purchase order",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "GetConsoleActionSetEnforced": {
             "access_level": "Read",
             "action": "GetConsoleActionSetEnforced",
             "condition_keys": [],
             "description": "Grants permission to view whether existing or fine-grained IAM actions are being used to control authorization to Billing, Cost Management, and Account consoles",
             "orphan": false,
             "resources": []
         },
         "GetPurchaseOrder": {
             "access_level": "Read",
             "action": "GetPurchaseOrder",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to get a purchase order",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "ListPurchaseOrderInvoices": {
             "access_level": "List",
             "action": "ListPurchaseOrderInvoices",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to list purchase order invoices",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "ListPurchaseOrders": {
             "access_level": "List",
             "action": "ListPurchaseOrders",
             "condition_keys": [],
-            "description": "Grants permission to get all available purchase orders",
+            "description": "Grants permission to list all purchase orders for an account",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListTagsForResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to list tags for a purchase order",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "ModifyPurchaseOrders": {
             "access_level": "Write",
             "action": "ModifyPurchaseOrders",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to modify purchase orders and details",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "TagResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "TagResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to tag purchase orders with given key value pairs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "UntagResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "UntagResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to remove tags from a purchase order",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "UpdateConsoleActionSetEnforced": {
             "access_level": "Write",
             "action": "UpdateConsoleActionSetEnforced",
             "condition_keys": [],
             "description": "Grants permission to change whether existing or fine-grained IAM actions will be used to control authorization to Billing, Cost Management, and Account consoles",
             "orphan": false,
             "resources": []
         },
         "UpdatePurchaseOrder": {
             "access_level": "Write",
             "action": "UpdatePurchaseOrder",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to update an existing purchase order",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "UpdatePurchaseOrderStatus": {
             "access_level": "Write",
             "action": "UpdatePurchaseOrderStatus",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to set purchase order status",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         },
         "ViewPurchaseOrders": {
             "access_level": "Read",
             "action": "ViewPurchaseOrders",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to view purchase orders and details",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "purchase-order"
+            ]
         }
     },
     "qldb": {
         "CancelJournalKinesisStream": {
             "access_level": "Write",
             "action": "CancelJournalKinesisStream",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230620/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230621/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230621/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/iam_actions/generate/generate.py` & `iam_actions-1.2.20230621/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230621/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230621/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/iam_actions/generate/services.py` & `iam_actions-1.2.20230621/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230620/iam_actions/policies.json` & `iam_actions-1.2.20230621/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993784842495%*

 * *Differences: {"'serviceMap'": "{'AWS Application Migration Service': {'Actions': {insert: [(48, "*

 * *                 "'ListManagedAccounts'), (59, 'PauseReplication'), (65, 'ResumeReplication'), "*

 * *                 "(80, 'StopReplication')]}}, 'AWS Audit Manager': {'Actions': {insert: [(27, "*

 * *                 "'GetEvidenceFileUploadUrl')]}}}"}*

```diff
@@ -741,43 +741,47 @@
                 "InitializeService",
                 "IssueClientCertificateForMgn",
                 "ListApplications",
                 "ListExportErrors",
                 "ListExports",
                 "ListImportErrors",
                 "ListImports",
+                "ListManagedAccounts",
                 "ListSourceServerActions",
                 "ListTagsForResource",
                 "ListTemplateActions",
                 "ListWaves",
                 "MarkAsArchived",
                 "NotifyAgentAuthenticationForMgn",
                 "NotifyAgentConnectedForMgn",
                 "NotifyAgentDisconnectedForMgn",
                 "NotifyAgentReplicationProgressForMgn",
                 "NotifyVcenterClientStartedForMgn",
+                "PauseReplication",
                 "PutSourceServerAction",
                 "PutTemplateAction",
                 "RegisterAgentForMgn",
                 "RemoveSourceServerAction",
                 "RemoveTemplateAction",
+                "ResumeReplication",
                 "RetryDataReplication",
                 "SendAgentLogsForMgn",
                 "SendAgentMetricsForMgn",
                 "SendChannelCommandResultForMgn",
                 "SendClientLogsForMgn",
                 "SendClientMetricsForMgn",
                 "SendVcenterClientCommandResultForMgn",
                 "SendVcenterClientLogsForMgn",
                 "SendVcenterClientMetricsForMgn",
                 "StartCutover",
                 "StartExport",
                 "StartImport",
                 "StartReplication",
                 "StartTest",
+                "StopReplication",
                 "TagResource",
                 "TerminateTargetInstances",
                 "UnarchiveApplication",
                 "UnarchiveWave",
                 "UntagResource",
                 "UpdateAgentBacklogForMgn",
                 "UpdateAgentConversionInfoForMgn",
@@ -845,14 +849,15 @@
                 "GetAssessmentFramework",
                 "GetAssessmentReportUrl",
                 "GetChangeLogs",
                 "GetControl",
                 "GetDelegations",
                 "GetEvidence",
                 "GetEvidenceByEvidenceFolder",
+                "GetEvidenceFileUploadUrl",
                 "GetEvidenceFolder",
                 "GetEvidenceFoldersByAssessment",
                 "GetEvidenceFoldersByAssessmentControl",
                 "GetInsights",
                 "GetInsightsByAssessment",
                 "GetOrganizationAdminAccount",
                 "GetServicesInScope",
```

### Comparing `iam_actions-1.2.20230620/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230621/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986187845303868%*

 * *Differences: {"'purchase-orders'": "{replace: OrderedDict([('purchase-order', OrderedDict([('arn_pattern', "*

 * *                      "'arn:*:purchase-orders::*:purchase-order/*'), ('condition_keys', "*

 * *                      "'aws:ResourceTag/${TagKey}')]))])}"}*

```diff
@@ -4886,15 +4886,20 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "service-template-version": {
             "arn_pattern": "arn:*:proton:*:*:service-template/*:*.*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
-    "purchase-orders": {},
+    "purchase-orders": {
+        "purchase-order": {
+            "arn_pattern": "arn:*:purchase-orders::*:purchase-order/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        }
+    },
     "qldb": {
         "catalog": {
             "arn_pattern": "arn:*:qldb:*:*:ledger/*/information_schema/user_tables",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "ledger": {
             "arn_pattern": "arn:*:qldb:*:*:ledger/*",
```

### Comparing `iam_actions-1.2.20230620/iam_actions/services.json` & `iam_actions-1.2.20230621/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999934929704579%*

 * *Differences: {"'auditmanager'": "{'Actions': {insert: [(27, 'GetEvidenceFileUploadUrl')]}}",*

 * * "'mgn'": "{'Actions': {insert: [(48, 'ListManagedAccounts'), (59, 'PauseReplication'), (65, "*

 * *          "'ResumeReplication'), (80, 'StopReplication')]}}"}*

```diff
@@ -1427,14 +1427,15 @@
             "GetAssessmentFramework",
             "GetAssessmentReportUrl",
             "GetChangeLogs",
             "GetControl",
             "GetDelegations",
             "GetEvidence",
             "GetEvidenceByEvidenceFolder",
+            "GetEvidenceFileUploadUrl",
             "GetEvidenceFolder",
             "GetEvidenceFoldersByAssessment",
             "GetEvidenceFoldersByAssessmentControl",
             "GetInsights",
             "GetInsightsByAssessment",
             "GetOrganizationAdminAccount",
             "GetServicesInScope",
@@ -13723,43 +13724,47 @@
             "InitializeService",
             "IssueClientCertificateForMgn",
             "ListApplications",
             "ListExportErrors",
             "ListExports",
             "ListImportErrors",
             "ListImports",
+            "ListManagedAccounts",
             "ListSourceServerActions",
             "ListTagsForResource",
             "ListTemplateActions",
             "ListWaves",
             "MarkAsArchived",
             "NotifyAgentAuthenticationForMgn",
             "NotifyAgentConnectedForMgn",
             "NotifyAgentDisconnectedForMgn",
             "NotifyAgentReplicationProgressForMgn",
             "NotifyVcenterClientStartedForMgn",
+            "PauseReplication",
             "PutSourceServerAction",
             "PutTemplateAction",
             "RegisterAgentForMgn",
             "RemoveSourceServerAction",
             "RemoveTemplateAction",
+            "ResumeReplication",
             "RetryDataReplication",
             "SendAgentLogsForMgn",
             "SendAgentMetricsForMgn",
             "SendChannelCommandResultForMgn",
             "SendClientLogsForMgn",
             "SendClientMetricsForMgn",
             "SendVcenterClientCommandResultForMgn",
             "SendVcenterClientLogsForMgn",
             "SendVcenterClientMetricsForMgn",
             "StartCutover",
             "StartExport",
             "StartImport",
             "StartReplication",
             "StartTest",
+            "StopReplication",
             "TagResource",
             "TerminateTargetInstances",
             "UnarchiveApplication",
             "UnarchiveWave",
             "UntagResource",
             "UpdateAgentBacklogForMgn",
             "UpdateAgentConversionInfoForMgn",
```

### Comparing `iam_actions-1.2.20230620/pyproject.toml` & `iam_actions-1.2.20230621/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230620"
+version = "1.2.20230621"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230620/setup.py` & `iam_actions-1.2.20230621/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230620',
+    'version': '1.2.20230621',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230620/PKG-INFO` & `iam_actions-1.2.20230621/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230620
+Version: 1.2.20230621
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

