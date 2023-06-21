# Comparing `tmp/betfair_parser-0.4.1.tar.gz` & `tmp/betfair_parser-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.4.1.tar", max compression
+gzip compressed data, was "betfair_parser-0.4.2.tar", max compression
```

## Comparing `betfair_parser-0.4.1.tar` & `betfair_parser-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1286 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0     3277 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/__init__.py
--rw-r--r--   0        0        0     2054 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/client.py
--rw-r--r--   0        0        0     2417 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/endpoints.py
--rw-r--r--   0        0        0      741 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3177 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    21951 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9634 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8860 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    32923 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0      238 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/__init__.py
--rw-r--r--   0        0        0     9771 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/enums.py
--rw-r--r--   0        0        0     4734 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/messages.py
--rw-r--r--   0        0        0     1493 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/common/type_definitions.py
--rw-r--r--   0        0        0     2773 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     8653 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/identity.py
--rw-r--r--   0        0        0     3645 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     3172 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      399 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     5989 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-06-18 09:38:31.222552 betfair_parser-0.4.1/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2507 2023-06-18 09:38:31.226552 betfair_parser-0.4.1/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2319 2023-06-18 09:38:31.226552 betfair_parser-0.4.1/betfair_parser/strenums.py
--rw-r--r--   0        0        0      902 2023-06-18 09:38:31.226552 betfair_parser-0.4.1/betfair_parser/util.py
--rw-r--r--   0        0        0     1731 2023-06-18 09:38:46.874497 betfair_parser-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     3277 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     2054 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/client.py
+-rw-r--r--   0        0        0     2417 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      741 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3278 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21951 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9634 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8860 2023-06-21 01:29:35.311172 betfair_parser-0.4.2/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    32923 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      238 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9771 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     4740 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1493 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0     2773 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8653 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3645 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3172 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      399 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     5989 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2507 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2319 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      902 2023-06-21 01:29:35.315172 betfair_parser-0.4.2/betfair_parser/util.py
+-rw-r--r--   0        0        0     1731 2023-06-21 01:29:52.455450 betfair_parser-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.2/PKG-INFO
```

### Comparing `betfair_parser-0.4.1/LICENSE.txt` & `betfair_parser-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/README.md` & `betfair_parser-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/client.py` & `betfair_parser-0.4.2/betfair_parser/client.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/endpoints.py` & `betfair_parser-0.4.2/betfair_parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/exceptions.py` & `betfair_parser-0.4.2/betfair_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.4.2/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.4.2/betfair_parser/spec/accounts/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,31 @@
     throws = AccountAPINGException  # type: ignore
 
 
 class _GetAccountFundsParams(Params, frozen=True):
     wallet: Optional[Wallet] = None  # Name of the wallet in question. Global wallet is returned by default
 
 
+class _GetAccountDetailsParams(Params, frozen=True):
+    pass
+
+
 class GetAccountFunds(AccountRequest, kw_only=True, frozen=True):
     """Returns the available to bet amount, exposure and commission information."""
 
     method = "AccountAPING/v1.0/getAccountFunds"
     params: _GetAccountFundsParams
     return_type = Response[AccountFundsResponse]
 
 
 class GetAccountDetails(AccountRequest, kw_only=True, frozen=True):
     """Returns the details relating your account, including your discount rate and Betfair point balance."""
 
     method = "AccountAPING/v1.0/getAccountDetails"
+    params: _GetAccountDetailsParams
     return_type = Response[AccountDetailsResponse]
 
 
 class _GetAccountStatementParams(Params, frozen=True):
     locale: Optional[str] = None  # The language to be used where applicable. Defaults to account settings
     from_record: Optional[int] = None  # Specifies the first record that will be returned, defaults to 0
     record_count: Optional[int] = None  # Specifies the maximum number of records to be returned. Maximum 100
```

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.4.2/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.4.2/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.4.2/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.4.2/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.4.2/betfair_parser/spec/betting/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/common/enums.py` & `betfair_parser-0.4.2/betfair_parser/spec/common/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/common/messages.py` & `betfair_parser-0.4.2/betfair_parser/spec/common/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Generic, Literal, Optional, TypeVar
+from typing import Any, Generic, Literal, Optional, TypeVar, get_type_hints
 
 import msgspec
 
 from betfair_parser.exceptions import APIError, APINGException, JSONError
 from betfair_parser.spec.common.enums import (
     AccountAPINGExceptionCode,
     APINGExceptionCode,
@@ -114,15 +114,15 @@
     method: str = ""
     params: ParamsType = {}  # type: ignore
     return_type = Response  # not to be serialized, so no type definition
     throws = APINGException  # JSON error definition
 
     @classmethod
     def with_params(cls, request_id=1, **kwargs):
-        params_cls = cls.__annotations__.get("params", dict)
+        params_cls = get_type_hints(cls)["params"]
         return cls(
             params=params_cls(**kwargs),
             method=cls.method,
             id=request_id,
         )
 
     @staticmethod
```

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/common/type_definitions.py` & `betfair_parser-0.4.2/betfair_parser/spec/common/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.4.2/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/identity.py` & `betfair_parser-0.4.2/betfair_parser/spec/identity.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/navigation.py` & `betfair_parser-0.4.2/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/race_status.py` & `betfair_parser-0.4.2/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.4.2/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.4.2/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.4.2/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/strenums.py` & `betfair_parser-0.4.2/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/betfair_parser/util.py` & `betfair_parser-0.4.2/betfair_parser/util.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.1/pyproject.toml` & `betfair_parser-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "betfair_parser"
-version = "0.4.1"
+version = "0.4.2"
 description = "A betfair parser"
 readme = "README.md"
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 msgspec = "^0.16.0"
```

### Comparing `betfair_parser-0.4.1/PKG-INFO` & `betfair_parser-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfair-parser
-Version: 0.4.1
+Version: 0.4.2
 Summary: A betfair parser
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

