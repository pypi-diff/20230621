# Comparing `tmp/mypy-boto3-mq-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-mq-1.26.158.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mq-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:46 2022, max compression
+gzip compressed data, was "mypy-boto3-mq-1.26.158.tar", last modified: Wed Jun 21 19:33:01 2023, max compression
```

## Comparing `mypy-boto3-mq-1.26.0.post1.tar` & `mypy-boto3-mq-1.26.158.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:46.892837 mypy-boto3-mq-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14644 2022-11-01 21:43:46.892837 mypy-boto3-mq-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13223 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:46.888837 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16467 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    16437 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8340 2022-11-01 21:38:27.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8338 2022-11-01 21:38:27.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    25981 2022-11-01 21:38:27.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    25936 2022-11-01 21:38:27.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:46.892837 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14644 2022-11-01 21:43:46.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-11-01 21:43:46.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:46.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:46.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:46.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-01 21:43:46.000000 mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:46.892837 mypy-boto3-mq-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-11-01 21:38:26.000000 mypy-boto3-mq-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/mypy_boto3_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-06-21 19:32:25.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27972 2023-06-21 19:32:25.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/setup.py
```

### Comparing `mypy-boto3-mq-1.26.0.post1/LICENSE` & `mypy-boto3-mq-1.26.158/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-mq-1.26.0.post1/PKG-INFO` & `mypy-boto3-mq-1.26.158/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MQ 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.158
+Summary: Type annotations for boto3.MQ 1.26.158 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-mq"></a>
 
 # mypy-boto3-mq
 
 [![PyPI - mypy-boto3-mq](https://img.shields.io/pypi/v/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.26.158](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,18 +299,20 @@
 
 ```python
 from mypy_boto3_mq.literals import (
     AuthenticationStrategyType,
     BrokerStateType,
     BrokerStorageTypeType,
     ChangeTypeType,
+    DataReplicationModeType,
     DayOfWeekType,
     DeploymentModeType,
     EngineTypeType,
     ListBrokersPaginatorName,
+    PromoteModeType,
     SanitizationWarningReasonType,
     MQServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -340,14 +343,15 @@
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
     ResponseMetadataTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
     LdapServerMetadataOutputTypeDef,
@@ -359,14 +363,15 @@
     PaginatorConfigTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     PendingLogsTypeDef,
+    PromoteRequestRequestTypeDef,
     RebootBrokerRequestRequestTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
     ConfigurationsTypeDef,
@@ -378,23 +383,25 @@
     DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListTagsResponseTypeDef,
-    UpdateBrokerResponseTypeDef,
+    PromoteResponseTypeDef,
+    DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
     ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
+    UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
 )
 
 
 def get_structure() -> ActionRequiredTypeDef:
     return {...}
 ```
@@ -402,42 +409,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-mq-1.26.0.post1/README.md` & `mypy-boto3-mq-1.26.158/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mq"></a>
 
 # mypy-boto3-mq
 
 [![PyPI - mypy-boto3-mq](https://img.shields.io/pypi/v/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.26.158](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,18 +267,20 @@
 
 ```python
 from mypy_boto3_mq.literals import (
     AuthenticationStrategyType,
     BrokerStateType,
     BrokerStorageTypeType,
     ChangeTypeType,
+    DataReplicationModeType,
     DayOfWeekType,
     DeploymentModeType,
     EngineTypeType,
     ListBrokersPaginatorName,
+    PromoteModeType,
     SanitizationWarningReasonType,
     MQServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -309,14 +311,15 @@
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
     ResponseMetadataTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
     LdapServerMetadataOutputTypeDef,
@@ -328,14 +331,15 @@
     PaginatorConfigTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     PendingLogsTypeDef,
+    PromoteRequestRequestTypeDef,
     RebootBrokerRequestRequestTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
     ConfigurationsTypeDef,
@@ -347,23 +351,25 @@
     DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListTagsResponseTypeDef,
-    UpdateBrokerResponseTypeDef,
+    PromoteResponseTypeDef,
+    DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
     ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
+    UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
 )
 
 
 def get_structure() -> ActionRequiredTypeDef:
     return {...}
 ```
@@ -371,42 +377,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/__init__.py` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/__init__.pyi` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/__main__.py` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MQ 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.MQ 1.26.158\nVersion:         1.26.158\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.158")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/client.py` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthenticationStrategyType,
     BrokerStorageTypeType,
+    DataReplicationModeType,
     DeploymentModeType,
     EngineTypeType,
+    PromoteModeType,
 )
 from .paginator import ListBrokersPaginator
 from .type_defs import (
     ConfigurationIdTypeDef,
     CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     DeleteBrokerResponseTypeDef,
@@ -41,14 +43,15 @@
     LdapServerMetadataInputTypeDef,
     ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListTagsResponseTypeDef,
     ListUsersResponseTypeDef,
     LogsTypeDef,
+    PromoteResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -128,15 +131,17 @@
         EncryptionOptions: EncryptionOptionsTypeDef = ...,
         LdapServerMetadata: LdapServerMetadataInputTypeDef = ...,
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
         SecurityGroups: Sequence[str] = ...,
         StorageType: BrokerStorageTypeType = ...,
         SubnetIds: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
+        DataReplicationMode: DataReplicationModeType = ...,
+        DataReplicationPrimaryBrokerArn: str = ...
     ) -> CreateBrokerResponseTypeDef:
         """
         Creates a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#create_broker)
         """
@@ -170,15 +175,16 @@
     def create_user(
         self,
         *,
         BrokerId: str,
         Password: str,
         Username: str,
         ConsoleAccess: bool = ...,
-        Groups: Sequence[str] = ...
+        Groups: Sequence[str] = ...,
+        ReplicationUser: bool = ...
     ) -> Dict[str, Any]:
         """
         Creates an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#create_user)
         """
@@ -329,14 +335,22 @@
         """
         Returns a list of all ActiveMQ users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#list_users)
         """
 
+    def promote(self, *, BrokerId: str, Mode: PromoteModeType) -> PromoteResponseTypeDef:
+        """
+        Promotes a data replication replica broker to the primary broker role.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.promote)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#promote)
+        """
+
     def reboot_broker(self, *, BrokerId: str) -> Dict[str, Any]:
         """
         Reboots a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.reboot_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#reboot_broker)
         """
@@ -349,15 +363,16 @@
         AutoMinorVersionUpgrade: bool = ...,
         Configuration: ConfigurationIdTypeDef = ...,
         EngineVersion: str = ...,
         HostInstanceType: str = ...,
         LdapServerMetadata: LdapServerMetadataInputTypeDef = ...,
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
-        SecurityGroups: Sequence[str] = ...
+        SecurityGroups: Sequence[str] = ...,
+        DataReplicationMode: DataReplicationModeType = ...
     ) -> UpdateBrokerResponseTypeDef:
         """
         Adds a pending configuration change to a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#update_broker)
         """
@@ -375,15 +390,16 @@
     def update_user(
         self,
         *,
         BrokerId: str,
         Username: str,
         ConsoleAccess: bool = ...,
         Groups: Sequence[str] = ...,
-        Password: str = ...
+        Password: str = ...,
+        ReplicationUser: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the information for an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#update_user)
         """
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/client.pyi` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthenticationStrategyType,
     BrokerStorageTypeType,
+    DataReplicationModeType,
     DeploymentModeType,
     EngineTypeType,
+    PromoteModeType,
 )
 from .paginator import ListBrokersPaginator
 from .type_defs import (
     ConfigurationIdTypeDef,
     CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     DeleteBrokerResponseTypeDef,
@@ -41,14 +43,15 @@
     LdapServerMetadataInputTypeDef,
     ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListTagsResponseTypeDef,
     ListUsersResponseTypeDef,
     LogsTypeDef,
+    PromoteResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -121,15 +124,17 @@
         EncryptionOptions: EncryptionOptionsTypeDef = ...,
         LdapServerMetadata: LdapServerMetadataInputTypeDef = ...,
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
         SecurityGroups: Sequence[str] = ...,
         StorageType: BrokerStorageTypeType = ...,
         SubnetIds: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
+        DataReplicationMode: DataReplicationModeType = ...,
+        DataReplicationPrimaryBrokerArn: str = ...
     ) -> CreateBrokerResponseTypeDef:
         """
         Creates a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#create_broker)
         """
@@ -160,15 +165,16 @@
     def create_user(
         self,
         *,
         BrokerId: str,
         Password: str,
         Username: str,
         ConsoleAccess: bool = ...,
-        Groups: Sequence[str] = ...
+        Groups: Sequence[str] = ...,
+        ReplicationUser: bool = ...
     ) -> Dict[str, Any]:
         """
         Creates an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#create_user)
         """
@@ -303,14 +309,21 @@
     ) -> ListUsersResponseTypeDef:
         """
         Returns a list of all ActiveMQ users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#list_users)
         """
+    def promote(self, *, BrokerId: str, Mode: PromoteModeType) -> PromoteResponseTypeDef:
+        """
+        Promotes a data replication replica broker to the primary broker role.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.promote)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#promote)
+        """
     def reboot_broker(self, *, BrokerId: str) -> Dict[str, Any]:
         """
         Reboots a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.reboot_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#reboot_broker)
         """
@@ -322,15 +335,16 @@
         AutoMinorVersionUpgrade: bool = ...,
         Configuration: ConfigurationIdTypeDef = ...,
         EngineVersion: str = ...,
         HostInstanceType: str = ...,
         LdapServerMetadata: LdapServerMetadataInputTypeDef = ...,
         Logs: LogsTypeDef = ...,
         MaintenanceWindowStartTime: WeeklyStartTimeTypeDef = ...,
-        SecurityGroups: Sequence[str] = ...
+        SecurityGroups: Sequence[str] = ...,
+        DataReplicationMode: DataReplicationModeType = ...
     ) -> UpdateBrokerResponseTypeDef:
         """
         Adds a pending configuration change to a broker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#update_broker)
         """
@@ -346,15 +360,16 @@
     def update_user(
         self,
         *,
         BrokerId: str,
         Username: str,
         ConsoleAccess: bool = ...,
         Groups: Sequence[str] = ...,
-        Password: str = ...
+        Password: str = ...,
+        ReplicationUser: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the information for an ActiveMQ user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/client/#update_user)
         """
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/literals.py` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 
 
 __all__ = (
     "AuthenticationStrategyType",
     "BrokerStateType",
     "BrokerStorageTypeType",
     "ChangeTypeType",
+    "DataReplicationModeType",
     "DayOfWeekType",
     "DeploymentModeType",
     "EngineTypeType",
     "ListBrokersPaginatorName",
+    "PromoteModeType",
     "SanitizationWarningReasonType",
     "MQServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -40,24 +42,27 @@
 AuthenticationStrategyType = Literal["LDAP", "SIMPLE"]
 BrokerStateType = Literal[
     "CREATION_FAILED",
     "CREATION_IN_PROGRESS",
     "CRITICAL_ACTION_REQUIRED",
     "DELETION_IN_PROGRESS",
     "REBOOT_IN_PROGRESS",
+    "REPLICA",
     "RUNNING",
 ]
 BrokerStorageTypeType = Literal["EBS", "EFS"]
 ChangeTypeType = Literal["CREATE", "DELETE", "UPDATE"]
+DataReplicationModeType = Literal["CRDR", "NONE"]
 DayOfWeekType = Literal[
     "FRIDAY", "MONDAY", "SATURDAY", "SUNDAY", "THURSDAY", "TUESDAY", "WEDNESDAY"
 ]
 DeploymentModeType = Literal["ACTIVE_STANDBY_MULTI_AZ", "CLUSTER_MULTI_AZ", "SINGLE_INSTANCE"]
 EngineTypeType = Literal["ACTIVEMQ", "RABBITMQ"]
 ListBrokersPaginatorName = Literal["list_brokers"]
+PromoteModeType = Literal["FAILOVER", "SWITCHOVER"]
 SanitizationWarningReasonType = Literal[
     "DISALLOWED_ATTRIBUTE_REMOVED", "DISALLOWED_ELEMENT_REMOVED", "INVALID_ATTRIBUTE_VALUE_REMOVED"
 ]
 MQServiceName = Literal["mq"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -78,14 +83,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -95,30 +101,35 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -144,14 +155,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -196,51 +208,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -253,14 +271,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -272,28 +291,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -302,14 +328,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -320,55 +347,64 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -394,24 +430,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/literals.pyi` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,20 @@
     from typing_extensions import Literal
 
 __all__ = (
     "AuthenticationStrategyType",
     "BrokerStateType",
     "BrokerStorageTypeType",
     "ChangeTypeType",
+    "DataReplicationModeType",
     "DayOfWeekType",
     "DeploymentModeType",
     "EngineTypeType",
     "ListBrokersPaginatorName",
+    "PromoteModeType",
     "SanitizationWarningReasonType",
     "MQServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -38,24 +40,27 @@
 AuthenticationStrategyType = Literal["LDAP", "SIMPLE"]
 BrokerStateType = Literal[
     "CREATION_FAILED",
     "CREATION_IN_PROGRESS",
     "CRITICAL_ACTION_REQUIRED",
     "DELETION_IN_PROGRESS",
     "REBOOT_IN_PROGRESS",
+    "REPLICA",
     "RUNNING",
 ]
 BrokerStorageTypeType = Literal["EBS", "EFS"]
 ChangeTypeType = Literal["CREATE", "DELETE", "UPDATE"]
+DataReplicationModeType = Literal["CRDR", "NONE"]
 DayOfWeekType = Literal[
     "FRIDAY", "MONDAY", "SATURDAY", "SUNDAY", "THURSDAY", "TUESDAY", "WEDNESDAY"
 ]
 DeploymentModeType = Literal["ACTIVE_STANDBY_MULTI_AZ", "CLUSTER_MULTI_AZ", "SINGLE_INSTANCE"]
 EngineTypeType = Literal["ACTIVEMQ", "RABBITMQ"]
 ListBrokersPaginatorName = Literal["list_brokers"]
+PromoteModeType = Literal["FAILOVER", "SWITCHOVER"]
 SanitizationWarningReasonType = Literal[
     "DISALLOWED_ATTRIBUTE_REMOVED", "DISALLOWED_ELEMENT_REMOVED", "INVALID_ATTRIBUTE_VALUE_REMOVED"
 ]
 MQServiceName = Literal["mq"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -76,14 +81,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -93,30 +99,35 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -142,14 +153,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -194,51 +206,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -251,14 +269,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -270,28 +289,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -300,14 +326,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -318,55 +345,64 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -392,24 +428,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/paginator.py` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/paginator.pyi` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/type_defs.py` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AuthenticationStrategyType,
     BrokerStateType,
     BrokerStorageTypeType,
     ChangeTypeType,
+    DataReplicationModeType,
     DayOfWeekType,
     DeploymentModeType,
     EngineTypeType,
+    PromoteModeType,
     SanitizationWarningReasonType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -45,14 +47,15 @@
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
     "ResponseMetadataTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DataReplicationCounterpartTypeDef",
     "DeleteBrokerRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
     "LdapServerMetadataOutputTypeDef",
@@ -64,14 +67,15 @@
     "PaginatorConfigTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "PendingLogsTypeDef",
+    "PromoteRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "SanitizationWarningTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "BrokerInstanceOptionTypeDef",
     "BrokerEngineTypeTypeDef",
     "ConfigurationsTypeDef",
@@ -83,23 +87,25 @@
     "DeleteBrokerResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListBrokersResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "ListTagsResponseTypeDef",
-    "UpdateBrokerResponseTypeDef",
+    "PromoteResponseTypeDef",
+    "DataReplicationMetadataOutputTypeDef",
     "ListUsersResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ListBrokersRequestListBrokersPaginateTypeDef",
     "LogsSummaryTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     "DescribeBrokerEngineTypesResponseTypeDef",
     "ListConfigurationsResponseTypeDef",
+    "UpdateBrokerResponseTypeDef",
     "DescribeBrokerResponseTypeDef",
 )
 
 ActionRequiredTypeDef = TypedDict(
     "ActionRequiredTypeDef",
     {
         "ActionRequiredCode": str,
@@ -268,14 +274,15 @@
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "ConsoleAccess": bool,
         "Groups": Sequence[str],
+        "ReplicationUser": bool,
     },
     total=False,
 )
 
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
@@ -367,25 +374,34 @@
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
     "_OptionalCreateUserRequestRequestTypeDef",
     {
         "ConsoleAccess": bool,
         "Groups": Sequence[str],
+        "ReplicationUser": bool,
     },
     total=False,
 )
 
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
+DataReplicationCounterpartTypeDef = TypedDict(
+    "DataReplicationCounterpartTypeDef",
+    {
+        "BrokerId": str,
+        "Region": str,
+    },
+)
+
 DeleteBrokerRequestRequestTypeDef = TypedDict(
     "DeleteBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
@@ -612,14 +628,22 @@
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
 )
 
+PromoteRequestRequestTypeDef = TypedDict(
+    "PromoteRequestRequestTypeDef",
+    {
+        "BrokerId": str,
+        "Mode": PromoteModeType,
+    },
+)
+
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
@@ -677,14 +701,15 @@
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateUserRequestRequestTypeDef",
     {
         "ConsoleAccess": bool,
         "Groups": Sequence[str],
         "Password": str,
+        "ReplicationUser": bool,
     },
     total=False,
 )
 
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
@@ -774,14 +799,16 @@
         "LdapServerMetadata": LdapServerMetadataInputTypeDef,
         "Logs": LogsTypeDef,
         "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": Sequence[str],
         "StorageType": BrokerStorageTypeType,
         "SubnetIds": Sequence[str],
         "Tags": Mapping[str, str],
+        "DataReplicationMode": DataReplicationModeType,
+        "DataReplicationPrimaryBrokerArn": str,
     },
     total=False,
 )
 
 
 class CreateBrokerRequestRequestTypeDef(
     _RequiredCreateBrokerRequestRequestTypeDef, _OptionalCreateBrokerRequestRequestTypeDef
@@ -803,14 +830,15 @@
         "Configuration": ConfigurationIdTypeDef,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataInputTypeDef,
         "Logs": LogsTypeDef,
         "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": Sequence[str],
+        "DataReplicationMode": DataReplicationModeType,
     },
     total=False,
 )
 
 
 class UpdateBrokerRequestRequestTypeDef(
     _RequiredUpdateBrokerRequestRequestTypeDef, _OptionalUpdateBrokerRequestRequestTypeDef
@@ -907,31 +935,43 @@
     "ListTagsResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBrokerResponseTypeDef = TypedDict(
-    "UpdateBrokerResponseTypeDef",
+PromoteResponseTypeDef = TypedDict(
+    "PromoteResponseTypeDef",
     {
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "AutoMinorVersionUpgrade": bool,
         "BrokerId": str,
-        "Configuration": ConfigurationIdTypeDef,
-        "EngineVersion": str,
-        "HostInstanceType": str,
-        "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
-        "Logs": LogsTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
-        "SecurityGroups": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDataReplicationMetadataOutputTypeDef = TypedDict(
+    "_RequiredDataReplicationMetadataOutputTypeDef",
+    {
+        "DataReplicationRole": str,
+    },
+)
+_OptionalDataReplicationMetadataOutputTypeDef = TypedDict(
+    "_OptionalDataReplicationMetadataOutputTypeDef",
+    {
+        "DataReplicationCounterpart": DataReplicationCounterpartTypeDef,
+    },
+    total=False,
+)
+
+
+class DataReplicationMetadataOutputTypeDef(
+    _RequiredDataReplicationMetadataOutputTypeDef, _OptionalDataReplicationMetadataOutputTypeDef
+):
+    pass
+
+
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "BrokerId": str,
         "MaxResults": int,
         "NextToken": str,
         "Users": List[UserSummaryTypeDef],
@@ -943,14 +983,15 @@
     "DescribeUserResponseTypeDef",
     {
         "BrokerId": str,
         "ConsoleAccess": bool,
         "Groups": List[str],
         "Pending": UserPendingChangesTypeDef,
         "Username": str,
+        "ReplicationUser": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
     "ListBrokersRequestListBrokersPaginateTypeDef",
     {
@@ -1020,14 +1061,35 @@
         "Configurations": List[ConfigurationTypeDef],
         "MaxResults": int,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBrokerResponseTypeDef = TypedDict(
+    "UpdateBrokerResponseTypeDef",
+    {
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "AutoMinorVersionUpgrade": bool,
+        "BrokerId": str,
+        "Configuration": ConfigurationIdTypeDef,
+        "EngineVersion": str,
+        "HostInstanceType": str,
+        "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
+        "Logs": LogsTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
+        "SecurityGroups": List[str],
+        "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "DataReplicationMode": DataReplicationModeType,
+        "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "PendingDataReplicationMode": DataReplicationModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeBrokerResponseTypeDef = TypedDict(
     "DescribeBrokerResponseTypeDef",
     {
         "ActionsRequired": List[ActionRequiredTypeDef],
         "AuthenticationStrategy": AuthenticationStrategyType,
         "AutoMinorVersionUpgrade": bool,
         "BrokerArn": str,
@@ -1052,10 +1114,14 @@
         "PendingSecurityGroups": List[str],
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
         "StorageType": BrokerStorageTypeType,
         "SubnetIds": List[str],
         "Tags": Dict[str, str],
         "Users": List[UserSummaryTypeDef],
+        "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "DataReplicationMode": DataReplicationModeType,
+        "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "PendingDataReplicationMode": DataReplicationModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq/type_defs.pyi` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AuthenticationStrategyType,
     BrokerStateType,
     BrokerStorageTypeType,
     ChangeTypeType,
+    DataReplicationModeType,
     DayOfWeekType,
     DeploymentModeType,
     EngineTypeType,
+    PromoteModeType,
     SanitizationWarningReasonType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -44,14 +46,15 @@
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
     "ResponseMetadataTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DataReplicationCounterpartTypeDef",
     "DeleteBrokerRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
     "LdapServerMetadataOutputTypeDef",
@@ -63,14 +66,15 @@
     "PaginatorConfigTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "PendingLogsTypeDef",
+    "PromoteRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "SanitizationWarningTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "BrokerInstanceOptionTypeDef",
     "BrokerEngineTypeTypeDef",
     "ConfigurationsTypeDef",
@@ -82,23 +86,25 @@
     "DeleteBrokerResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListBrokersResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "ListTagsResponseTypeDef",
-    "UpdateBrokerResponseTypeDef",
+    "PromoteResponseTypeDef",
+    "DataReplicationMetadataOutputTypeDef",
     "ListUsersResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ListBrokersRequestListBrokersPaginateTypeDef",
     "LogsSummaryTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     "DescribeBrokerEngineTypesResponseTypeDef",
     "ListConfigurationsResponseTypeDef",
+    "UpdateBrokerResponseTypeDef",
     "DescribeBrokerResponseTypeDef",
 )
 
 ActionRequiredTypeDef = TypedDict(
     "ActionRequiredTypeDef",
     {
         "ActionRequiredCode": str,
@@ -257,14 +263,15 @@
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "ConsoleAccess": bool,
         "Groups": Sequence[str],
+        "ReplicationUser": bool,
     },
     total=False,
 )
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
@@ -348,23 +355,32 @@
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
     "_OptionalCreateUserRequestRequestTypeDef",
     {
         "ConsoleAccess": bool,
         "Groups": Sequence[str],
+        "ReplicationUser": bool,
     },
     total=False,
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+DataReplicationCounterpartTypeDef = TypedDict(
+    "DataReplicationCounterpartTypeDef",
+    {
+        "BrokerId": str,
+        "Region": str,
+    },
+)
+
 DeleteBrokerRequestRequestTypeDef = TypedDict(
     "DeleteBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
@@ -581,14 +597,22 @@
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
 )
 
+PromoteRequestRequestTypeDef = TypedDict(
+    "PromoteRequestRequestTypeDef",
+    {
+        "BrokerId": str,
+        "Mode": PromoteModeType,
+    },
+)
+
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
@@ -642,14 +666,15 @@
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateUserRequestRequestTypeDef",
     {
         "ConsoleAccess": bool,
         "Groups": Sequence[str],
         "Password": str,
+        "ReplicationUser": bool,
     },
     total=False,
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
@@ -735,14 +760,16 @@
         "LdapServerMetadata": LdapServerMetadataInputTypeDef,
         "Logs": LogsTypeDef,
         "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": Sequence[str],
         "StorageType": BrokerStorageTypeType,
         "SubnetIds": Sequence[str],
         "Tags": Mapping[str, str],
+        "DataReplicationMode": DataReplicationModeType,
+        "DataReplicationPrimaryBrokerArn": str,
     },
     total=False,
 )
 
 class CreateBrokerRequestRequestTypeDef(
     _RequiredCreateBrokerRequestRequestTypeDef, _OptionalCreateBrokerRequestRequestTypeDef
 ):
@@ -762,14 +789,15 @@
         "Configuration": ConfigurationIdTypeDef,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataInputTypeDef,
         "Logs": LogsTypeDef,
         "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": Sequence[str],
+        "DataReplicationMode": DataReplicationModeType,
     },
     total=False,
 )
 
 class UpdateBrokerRequestRequestTypeDef(
     _RequiredUpdateBrokerRequestRequestTypeDef, _OptionalUpdateBrokerRequestRequestTypeDef
 ):
@@ -864,31 +892,41 @@
     "ListTagsResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBrokerResponseTypeDef = TypedDict(
-    "UpdateBrokerResponseTypeDef",
+PromoteResponseTypeDef = TypedDict(
+    "PromoteResponseTypeDef",
     {
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "AutoMinorVersionUpgrade": bool,
         "BrokerId": str,
-        "Configuration": ConfigurationIdTypeDef,
-        "EngineVersion": str,
-        "HostInstanceType": str,
-        "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
-        "Logs": LogsTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
-        "SecurityGroups": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDataReplicationMetadataOutputTypeDef = TypedDict(
+    "_RequiredDataReplicationMetadataOutputTypeDef",
+    {
+        "DataReplicationRole": str,
+    },
+)
+_OptionalDataReplicationMetadataOutputTypeDef = TypedDict(
+    "_OptionalDataReplicationMetadataOutputTypeDef",
+    {
+        "DataReplicationCounterpart": DataReplicationCounterpartTypeDef,
+    },
+    total=False,
+)
+
+class DataReplicationMetadataOutputTypeDef(
+    _RequiredDataReplicationMetadataOutputTypeDef, _OptionalDataReplicationMetadataOutputTypeDef
+):
+    pass
+
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "BrokerId": str,
         "MaxResults": int,
         "NextToken": str,
         "Users": List[UserSummaryTypeDef],
@@ -900,14 +938,15 @@
     "DescribeUserResponseTypeDef",
     {
         "BrokerId": str,
         "ConsoleAccess": bool,
         "Groups": List[str],
         "Pending": UserPendingChangesTypeDef,
         "Username": str,
+        "ReplicationUser": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
     "ListBrokersRequestListBrokersPaginateTypeDef",
     {
@@ -975,14 +1014,35 @@
         "Configurations": List[ConfigurationTypeDef],
         "MaxResults": int,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBrokerResponseTypeDef = TypedDict(
+    "UpdateBrokerResponseTypeDef",
+    {
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "AutoMinorVersionUpgrade": bool,
+        "BrokerId": str,
+        "Configuration": ConfigurationIdTypeDef,
+        "EngineVersion": str,
+        "HostInstanceType": str,
+        "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
+        "Logs": LogsTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
+        "SecurityGroups": List[str],
+        "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "DataReplicationMode": DataReplicationModeType,
+        "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "PendingDataReplicationMode": DataReplicationModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeBrokerResponseTypeDef = TypedDict(
     "DescribeBrokerResponseTypeDef",
     {
         "ActionsRequired": List[ActionRequiredTypeDef],
         "AuthenticationStrategy": AuthenticationStrategyType,
         "AutoMinorVersionUpgrade": bool,
         "BrokerArn": str,
@@ -1007,10 +1067,14 @@
         "PendingSecurityGroups": List[str],
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
         "StorageType": BrokerStorageTypeType,
         "SubnetIds": List[str],
         "Tags": Dict[str, str],
         "Users": List[UserSummaryTypeDef],
+        "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "DataReplicationMode": DataReplicationModeType,
+        "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
+        "PendingDataReplicationMode": DataReplicationModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/PKG-INFO` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MQ 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.158
+Summary: Type annotations for boto3.MQ 1.26.158 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-mq"></a>
 
 # mypy-boto3-mq
 
 [![PyPI - mypy-boto3-mq](https://img.shields.io/pypi/v/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.26.158](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,18 +299,20 @@
 
 ```python
 from mypy_boto3_mq.literals import (
     AuthenticationStrategyType,
     BrokerStateType,
     BrokerStorageTypeType,
     ChangeTypeType,
+    DataReplicationModeType,
     DayOfWeekType,
     DeploymentModeType,
     EngineTypeType,
     ListBrokersPaginatorName,
+    PromoteModeType,
     SanitizationWarningReasonType,
     MQServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -340,14 +343,15 @@
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
     ResponseMetadataTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
     LdapServerMetadataOutputTypeDef,
@@ -359,14 +363,15 @@
     PaginatorConfigTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     PendingLogsTypeDef,
+    PromoteRequestRequestTypeDef,
     RebootBrokerRequestRequestTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
     ConfigurationsTypeDef,
@@ -378,23 +383,25 @@
     DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListTagsResponseTypeDef,
-    UpdateBrokerResponseTypeDef,
+    PromoteResponseTypeDef,
+    DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
     ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
+    UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
 )
 
 
 def get_structure() -> ActionRequiredTypeDef:
     return {...}
 ```
@@ -402,42 +409,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-mq-1.26.0.post1/mypy_boto3_mq.egg-info/SOURCES.txt` & `mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.0.post1/setup.py` & `mypy-boto3-mq-1.26.158/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-mq.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mq",
-    version="1.26.0.post1",
+    version="1.26.158",
     packages=["mypy_boto3_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MQ 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.MQ 1.26.158 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 mq type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_mq": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_mq": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

