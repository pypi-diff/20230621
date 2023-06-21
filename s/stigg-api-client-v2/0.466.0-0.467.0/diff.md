# Comparing `tmp/stigg_api_client_v2-0.466.0.tar.gz` & `tmp/stigg_api_client_v2-0.467.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.466.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.467.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.466.0.tar` & `stigg_api_client_v2-0.467.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-06-19 12:32:55.301117 stigg_api_client_v2-0.466.0/README.md
--rw-r--r--   0        0        0      653 2023-06-19 12:33:40.768710 stigg_api_client_v2-0.466.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-19 12:32:55.301117 stigg_api_client_v2-0.466.0/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-19 12:32:55.301117 stigg_api_client_v2-0.466.0/stigg/client.py
--rw-r--r--   0        0        0    39611 2023-06-19 12:33:39.148727 stigg_api_client_v2-0.466.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-19 12:33:37.828741 stigg_api_client_v2-0.466.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-19 12:33:37.848740 stigg_api_client_v2-0.466.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70260 2023-06-19 12:33:38.924729 stigg_api_client_v2-0.466.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-19 12:33:37.872740 stigg_api_client_v2-0.466.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-19 12:33:37.956739 stigg_api_client_v2-0.466.0/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23730 2023-06-19 12:33:35.640763 stigg_api_client_v2-0.466.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-19 12:33:37.836741 stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-19 12:33:37.840741 stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53605 2023-06-19 12:33:38.608733 stigg_api_client_v2-0.466.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-19 12:33:37.892740 stigg_api_client_v2-0.466.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-19 12:33:37.900740 stigg_api_client_v2-0.466.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-19 12:33:37.884740 stigg_api_client_v2-0.466.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-19 12:33:37.936740 stigg_api_client_v2-0.466.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-19 12:33:37.916740 stigg_api_client_v2-0.466.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-19 12:33:37.908740 stigg_api_client_v2-0.466.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-19 12:33:37.948739 stigg_api_client_v2-0.466.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-19 12:33:37.904740 stigg_api_client_v2-0.466.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-19 12:33:37.920740 stigg_api_client_v2-0.466.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-19 12:33:37.932740 stigg_api_client_v2-0.466.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-19 12:33:37.796741 stigg_api_client_v2-0.466.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-19 12:33:37.792741 stigg_api_client_v2-0.466.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-19 12:33:37.816741 stigg_api_client_v2-0.466.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   125303 2023-06-19 12:33:37.776741 stigg_api_client_v2-0.466.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-19 12:33:37.876740 stigg_api_client_v2-0.466.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-19 12:33:37.784741 stigg_api_client_v2-0.466.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-19 12:33:37.812741 stigg_api_client_v2-0.466.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-19 12:33:37.864740 stigg_api_client_v2-0.466.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-06-19 12:33:37.860740 stigg_api_client_v2-0.466.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-06-19 12:33:37.856740 stigg_api_client_v2-0.466.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-19 12:33:38.716731 stigg_api_client_v2-0.466.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-19 12:33:37.800741 stigg_api_client_v2-0.466.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-19 12:33:37.824741 stigg_api_client_v2-0.466.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-06-19 12:33:37.952739 stigg_api_client_v2-0.466.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0      451 2023-06-19 12:33:37.964739 stigg_api_client_v2-0.466.0/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.466.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-21 15:05:31.473351 stigg_api_client_v2-0.467.0/README.md
+-rw-r--r--   0        0        0      653 2023-06-21 15:06:09.017465 stigg_api_client_v2-0.467.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-21 15:05:31.473351 stigg_api_client_v2-0.467.0/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-21 15:05:31.473351 stigg_api_client_v2-0.467.0/stigg/client.py
+-rw-r--r--   0        0        0    39611 2023-06-21 15:06:07.357472 stigg_api_client_v2-0.467.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-21 15:06:06.985474 stigg_api_client_v2-0.467.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-21 15:06:06.985474 stigg_api_client_v2-0.467.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-21 15:06:06.117478 stigg_api_client_v2-0.467.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-21 15:06:06.133478 stigg_api_client_v2-0.467.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70260 2023-06-21 15:06:07.201473 stigg_api_client_v2-0.467.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-21 15:06:06.157478 stigg_api_client_v2-0.467.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-21 15:06:06.245477 stigg_api_client_v2-0.467.0/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23730 2023-06-21 15:06:04.005487 stigg_api_client_v2-0.467.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-21 15:06:06.125478 stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-21 15:06:06.129478 stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-21 15:06:06.989474 stigg_api_client_v2-0.467.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53605 2023-06-21 15:06:06.985474 stigg_api_client_v2-0.467.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-21 15:06:06.177477 stigg_api_client_v2-0.467.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-21 15:06:06.185478 stigg_api_client_v2-0.467.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-21 15:06:06.173478 stigg_api_client_v2-0.467.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-21 15:06:06.225477 stigg_api_client_v2-0.467.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-21 15:06:06.201477 stigg_api_client_v2-0.467.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-21 15:06:06.197477 stigg_api_client_v2-0.467.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-21 15:06:06.233477 stigg_api_client_v2-0.467.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-21 15:06:06.193477 stigg_api_client_v2-0.467.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-21 15:06:06.209478 stigg_api_client_v2-0.467.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-21 15:06:06.217477 stigg_api_client_v2-0.467.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-21 15:06:06.085478 stigg_api_client_v2-0.467.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-21 15:06:06.077478 stigg_api_client_v2-0.467.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-21 15:06:06.105478 stigg_api_client_v2-0.467.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   125523 2023-06-21 15:06:06.061478 stigg_api_client_v2-0.467.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-21 15:06:06.165478 stigg_api_client_v2-0.467.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-21 15:06:06.073478 stigg_api_client_v2-0.467.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-21 15:06:06.101478 stigg_api_client_v2-0.467.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-21 15:06:06.153478 stigg_api_client_v2-0.467.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-06-21 15:06:06.149478 stigg_api_client_v2-0.467.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-06-21 15:06:06.141478 stigg_api_client_v2-0.467.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-21 15:06:06.993474 stigg_api_client_v2-0.467.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-21 15:06:06.089478 stigg_api_client_v2-0.467.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-21 15:06:06.109478 stigg_api_client_v2-0.467.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-06-21 15:06:06.237477 stigg_api_client_v2-0.467.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0      451 2023-06-21 15:06:06.249477 stigg_api_client_v2-0.467.0/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.467.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.466.0/README.md` & `stigg_api_client_v2-0.467.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.466.0/pyproject.toml` & `stigg_api_client_v2-0.467.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.466.0"
+version = "0.467.0"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.467.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.467.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.467.0/stigg/generated/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.467.0/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/client.py` & `stigg_api_client_v2-0.467.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import SlimSubscriptionFragment
+from .fragments import SubscriptionPreviewFragment
 
 
-class CreateSubscription(BaseModel):
-    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
-        alias="createSubscription"
+class EstimateSubscription(BaseModel):
+    estimate_subscription: "EstimateSubscriptionEstimateSubscription" = Field(
+        alias="estimateSubscription"
     )
 
 
-class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
+class EstimateSubscriptionEstimateSubscription(SubscriptionPreviewFragment):
     pass
 
 
-CreateSubscription.update_forward_refs()
-CreateSubscriptionCreateSubscription.update_forward_refs()
+EstimateSubscription.update_forward_refs()
+EstimateSubscriptionEstimateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.467.0/stigg/generated/entitlements_updated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.467.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.467.0/stigg/generated/update_subscription.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import SubscriptionPreviewFragment
+from .fragments import SlimSubscriptionFragment
 
 
-class EstimateSubscription(BaseModel):
-    estimate_subscription: "EstimateSubscriptionEstimateSubscription" = Field(
-        alias="estimateSubscription"
+class UpdateSubscription(BaseModel):
+    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
+        alias="updateSubscription"
     )
 
 
-class EstimateSubscriptionEstimateSubscription(SubscriptionPreviewFragment):
+class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
     pass
 
 
-EstimateSubscription.update_forward_refs()
-EstimateSubscriptionEstimateSubscription.update_forward_refs()
+UpdateSubscription.update_forward_refs()
+UpdateSubscriptionUpdateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.467.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.467.0/stigg/generated/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.467.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,36 +32,14 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -77,14 +55,36 @@
 class PriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -328,34 +328,14 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -399,14 +379,21 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
     trial_remaining_days: Optional[int] = Field(alias="trialRemainingDays")
     billing_period_range: Optional[
@@ -475,14 +462,27 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -532,65 +532,14 @@
 
 
 class TotalPriceFragmentTotal(BaseModel):
     amount: float
     currency: Currency
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -655,14 +604,65 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -813,14 +813,34 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -835,34 +855,14 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1282,19 +1282,19 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
@@ -1317,59 +1317,59 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
@@ -1385,19 +1385,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.467.0/stigg/generated/get_active_subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.467.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.467.0/stigg/generated/get_customer_by_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.467.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.467.0/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.467.0/stigg/generated/get_sdk_configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.467.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -888,14 +888,17 @@
     direction: SortDirection
     field: EnvironmentSortFields
     nulls: Optional[SortNulls]
 
 
 class EstimateSubscriptionInput(BaseModel):
     addons: Optional[List["SubscriptionAddonInput"]]
+    billable_features: Optional[List["BillableFeatureInput"]] = Field(
+        alias="billableFeatures"
+    )
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
     billing_information: Optional["SubscriptionBillingInfo"] = Field(
         alias="billingInformation"
     )
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     customer_id: str = Field(alias="customerId")
     environment_id: Optional[str] = Field(alias="environmentId")
@@ -906,14 +909,17 @@
     skip_trial: Optional[bool] = Field(alias="skipTrial", default=False)
     start_date: Optional[Any] = Field(alias="startDate")
     unit_quantity: Optional[float] = Field(alias="unitQuantity", default=-1)
 
 
 class EstimateSubscriptionUpdateInput(BaseModel):
     addons: Optional[List["SubscriptionAddonInput"]]
+    billable_features: Optional[List["BillableFeatureInput"]] = Field(
+        alias="billableFeatures"
+    )
     environment_id: Optional[str] = Field(alias="environmentId")
     promotion_code: Optional[str] = Field(alias="promotionCode")
     subscription_id: str = Field(alias="subscriptionId")
     unit_quantity: Optional[float] = Field(alias="unitQuantity")
 
 
 class ExperimentFilter(BaseModel):
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.467.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.467.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.467.0/stigg/generated/provision_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.467.0/stigg/generated/report_usage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.466.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.467.0/stigg/generated/create_subscription.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-06-19 12:33
+# Generated by ariadne-codegen on 2023-06-21 15:06
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class UpdateSubscription(BaseModel):
-    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
-        alias="updateSubscription"
+class CreateSubscription(BaseModel):
+    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
+        alias="createSubscription"
     )
 
 
-class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
+class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
     pass
 
 
-UpdateSubscription.update_forward_refs()
-UpdateSubscriptionUpdateSubscription.update_forward_refs()
+CreateSubscription.update_forward_refs()
+CreateSubscriptionCreateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.466.0/PKG-INFO` & `stigg_api_client_v2-0.467.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.466.0
+Version: 0.467.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

