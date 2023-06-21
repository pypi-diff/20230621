# Comparing `tmp/braincube-aws-core-0.0.1.tar.gz` & `tmp/braincube-aws-core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-0.0.1.tar", last modified: Tue Jun 20 17:06:05 2023, max compression
+gzip compressed data, was "braincube-aws-core-0.0.2.tar", last modified: Wed Jun 21 20:21:58 2023, max compression
```

## Comparing `braincube-aws-core-0.0.1.tar` & `braincube-aws-core-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.742397 braincube-aws-core-0.0.1/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8843 2023-06-20 17:06:05.742647 braincube-aws-core-0.0.1/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8097 2023-06-20 17:05:54.000000 braincube-aws-core-0.0.1/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-20 17:06:05.744159 braincube-aws-core-0.0.1/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.721331 braincube-aws-core-0.0.1/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.726583 braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8843 2023-06-20 17:06:05.000000 braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      841 2023-06-20 17:06:05.000000 braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-20 17:06:05.000000 braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-20 17:06:05.000000 braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-20 17:06:05.000000 braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.727072 braincube-aws-core-0.0.1/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.729782 braincube-aws-core-0.0.1/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.1/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.1/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.1/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-0.0.1/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.732252 braincube-aws-core-0.0.1/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.1/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.1/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.735118 braincube-aws-core-0.0.1/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.1/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-0.0.1/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-0.0.1/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.739822 braincube-aws-core-0.0.1/src/core/rules_engine/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/src/core/rules_engine/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.1/src/core/rules_engine/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.1/src/core/rules_engine/exceptions.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.1/src/core/rules_engine/rule_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-20 17:06:05.741808 braincube-aws-core-0.0.1/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.1/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.1/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.1/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.892466 braincube-aws-core-0.0.2/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8761 2023-06-21 20:21:58.892617 braincube-aws-core-0.0.2/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8015 2023-06-21 20:10:09.000000 braincube-aws-core-0.0.2/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-21 20:21:58.893230 braincube-aws-core-0.0.2/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.874910 braincube-aws-core-0.0.2/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.878912 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8761 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.879192 braincube-aws-core-0.0.2/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.882194 braincube-aws-core-0.0.2/src/core/app/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/app/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.2/src/core/app/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.2/src/core/app/app_event.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6203 2023-06-21 20:01:55.000000 braincube-aws-core-0.0.2/src/core/app/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-21 13:21:21.000000 braincube-aws-core-0.0.2/src/core/app/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.2/src/core/app/exception_handler.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.886295 braincube-aws-core-0.0.2/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.2/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.2/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.2/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-0.0.2/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.888123 braincube-aws-core-0.0.2/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.2/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.2/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.890224 braincube-aws-core-0.0.2/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.2/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.2/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.2/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.891925 braincube-aws-core-0.0.2/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.2/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.2/src/core/utils/data.py
```

### Comparing `braincube-aws-core-0.0.1/LICENSE` & `braincube-aws-core-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/PKG-INFO` & `braincube-aws-core-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 License-File: LICENSE
 
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
-[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core-alpha/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Installation
 
 ```bash
 pip install braincube-aws-core
 ```
@@ -42,17 +42,17 @@
 
 ```python
 import asyncio
 
 from uuid import uuid4
 from http import HTTPStatus
 
-from core.rest.data import HTTPRequest, HTTPResponse
-from core.rest.app_module import AppModule
-from core.rest.app_controller import AppController
+from core.app.data import HTTPRequest, HTTPResponse
+from core.app.app_module import AppModule
+from core.app.app_controller import AppController
 
 from pydantic import BaseModel
 
 
 class AccountDto(BaseModel):
     iban: str
     bban: str
@@ -64,15 +64,15 @@
 }
 
 app = AppController("/accounts")
 
 
 @app.get("/{id}")
 async def get_account(request: HTTPRequest) -> HTTPResponse:
-    account = data.get(request.path_parameters["id"])
+    account = data.get(request.path_params["id"])
     return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
 
 
 @app.post()
 async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
     data[uuid4()] = request.body
     return HTTPResponse(HTTPStatus.CREATED)
@@ -105,15 +105,15 @@
     def __init__(self, pool: Pool):
         self._pool = pool
 ```
 
 ### Postgres Repository Example
 
 ```python
-from core.rest.data import HTTPRequest
+from core.app.data import HTTPRequest
 from core.utils.data import Order, OrderType
 from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
 from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
 
 # schema definition
 equities = Schema(
@@ -165,41 +165,41 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_pk(Key(request.path_parameters["id"]), request.query_parameters.fields)
+await repo.find_by_pk(Key(request.path_params["id"]), request.query_params.fields)
 
 await repo.exists_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    order=request.query_params.order)
 
 await repo.find_all(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    order=request.query_params.order)
 
 await repo.find_all_by_pk(
     [
         Key("9448a57b-f686-4935-b152-566baab712db"),
         Key("43c8ec37-9a59-44eb-be90-def391ba2f02")
     ],
-    aliases=request.query_parameters.fields,
-    order=request.query_parameters.order)
+    aliases=request.query_params.fields,
+    order=request.query_params.order)
 
 await repo.find_many(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    page=request.query_parameters.page,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    page=request.query_params.page,
+    order=request.query_params.order)
 
 await repo.insert({
     "name": "Bursa de Valori Bucuresti SA",
     "type": 1,
     "industrySector": 40,
     "isin": "ROBVBAACNOR0",
     "bloombergCode": "BBG000BBWMC5",
@@ -216,22 +216,22 @@
         ["Coca-Cola HBC AG", 1, 49, "CH0198251305", "BBG004HJV2T1", "EEE GA Equity", "EUR", "GR"],
     ]
 )
 
 await repo.update({
     "type": 1,
     "isin": 40,
-}, request.query_parameters.conditions, request.query_parameters.fields)
+}, request.query_params.conditions, request.query_params.fields)
 
 await repo.update_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), {
     "type": 1,
     "isin": 40
 })
 
-await repo.delete(request.query_parameters.conditions, ["id", "name", "type"])
+await repo.delete(request.query_params.conditions, ["id", "name", "type"])
 
 await repo.delete_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), ["id", "name", "type"])
 
 await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
```

### Comparing `braincube-aws-core-0.0.1/README.md` & `braincube-aws-core-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
-[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core-alpha/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Installation
 
 ```bash
 pip install braincube-aws-core
 ```
@@ -22,17 +22,17 @@
 
 ```python
 import asyncio
 
 from uuid import uuid4
 from http import HTTPStatus
 
-from core.rest.data import HTTPRequest, HTTPResponse
-from core.rest.app_module import AppModule
-from core.rest.app_controller import AppController
+from core.app.data import HTTPRequest, HTTPResponse
+from core.app.app_module import AppModule
+from core.app.app_controller import AppController
 
 from pydantic import BaseModel
 
 
 class AccountDto(BaseModel):
     iban: str
     bban: str
@@ -44,15 +44,15 @@
 }
 
 app = AppController("/accounts")
 
 
 @app.get("/{id}")
 async def get_account(request: HTTPRequest) -> HTTPResponse:
-    account = data.get(request.path_parameters["id"])
+    account = data.get(request.path_params["id"])
     return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
 
 
 @app.post()
 async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
     data[uuid4()] = request.body
     return HTTPResponse(HTTPStatus.CREATED)
@@ -85,15 +85,15 @@
     def __init__(self, pool: Pool):
         self._pool = pool
 ```
 
 ### Postgres Repository Example
 
 ```python
-from core.rest.data import HTTPRequest
+from core.app.data import HTTPRequest
 from core.utils.data import Order, OrderType
 from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
 from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
 
 # schema definition
 equities = Schema(
@@ -145,41 +145,41 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_pk(Key(request.path_parameters["id"]), request.query_parameters.fields)
+await repo.find_by_pk(Key(request.path_params["id"]), request.query_params.fields)
 
 await repo.exists_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    order=request.query_params.order)
 
 await repo.find_all(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    order=request.query_params.order)
 
 await repo.find_all_by_pk(
     [
         Key("9448a57b-f686-4935-b152-566baab712db"),
         Key("43c8ec37-9a59-44eb-be90-def391ba2f02")
     ],
-    aliases=request.query_parameters.fields,
-    order=request.query_parameters.order)
+    aliases=request.query_params.fields,
+    order=request.query_params.order)
 
 await repo.find_many(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    page=request.query_parameters.page,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    page=request.query_params.page,
+    order=request.query_params.order)
 
 await repo.insert({
     "name": "Bursa de Valori Bucuresti SA",
     "type": 1,
     "industrySector": 40,
     "isin": "ROBVBAACNOR0",
     "bloombergCode": "BBG000BBWMC5",
@@ -196,22 +196,22 @@
         ["Coca-Cola HBC AG", 1, 49, "CH0198251305", "BBG004HJV2T1", "EEE GA Equity", "EUR", "GR"],
     ]
 )
 
 await repo.update({
     "type": 1,
     "isin": 40,
-}, request.query_parameters.conditions, request.query_parameters.fields)
+}, request.query_params.conditions, request.query_params.fields)
 
 await repo.update_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), {
     "type": 1,
     "isin": 40
 })
 
-await repo.delete(request.query_parameters.conditions, ["id", "name", "type"])
+await repo.delete(request.query_params.conditions, ["id", "name", "type"])
 
 await repo.delete_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), ["id", "name", "type"])
 
 await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
```

### Comparing `braincube-aws-core-0.0.1/setup.cfg` & `braincube-aws-core-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core
-version = 0.0.1
+version = 0.0.2
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/PKG-INFO` & `braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 License-File: LICENSE
 
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
-[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core-alpha/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Installation
 
 ```bash
 pip install braincube-aws-core
 ```
@@ -42,17 +42,17 @@
 
 ```python
 import asyncio
 
 from uuid import uuid4
 from http import HTTPStatus
 
-from core.rest.data import HTTPRequest, HTTPResponse
-from core.rest.app_module import AppModule
-from core.rest.app_controller import AppController
+from core.app.data import HTTPRequest, HTTPResponse
+from core.app.app_module import AppModule
+from core.app.app_controller import AppController
 
 from pydantic import BaseModel
 
 
 class AccountDto(BaseModel):
     iban: str
     bban: str
@@ -64,15 +64,15 @@
 }
 
 app = AppController("/accounts")
 
 
 @app.get("/{id}")
 async def get_account(request: HTTPRequest) -> HTTPResponse:
-    account = data.get(request.path_parameters["id"])
+    account = data.get(request.path_params["id"])
     return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
 
 
 @app.post()
 async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
     data[uuid4()] = request.body
     return HTTPResponse(HTTPStatus.CREATED)
@@ -105,15 +105,15 @@
     def __init__(self, pool: Pool):
         self._pool = pool
 ```
 
 ### Postgres Repository Example
 
 ```python
-from core.rest.data import HTTPRequest
+from core.app.data import HTTPRequest
 from core.utils.data import Order, OrderType
 from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
 from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
 
 # schema definition
 equities = Schema(
@@ -165,41 +165,41 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_pk(Key(request.path_parameters["id"]), request.query_parameters.fields)
+await repo.find_by_pk(Key(request.path_params["id"]), request.query_params.fields)
 
 await repo.exists_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    order=request.query_params.order)
 
 await repo.find_all(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    order=request.query_params.order)
 
 await repo.find_all_by_pk(
     [
         Key("9448a57b-f686-4935-b152-566baab712db"),
         Key("43c8ec37-9a59-44eb-be90-def391ba2f02")
     ],
-    aliases=request.query_parameters.fields,
-    order=request.query_parameters.order)
+    aliases=request.query_params.fields,
+    order=request.query_params.order)
 
 await repo.find_many(
-    request.query_parameters.fields,
-    conditions=request.query_parameters.conditions,
-    page=request.query_parameters.page,
-    order=request.query_parameters.order)
+    request.query_params.fields,
+    conditions=request.query_params.conditions,
+    page=request.query_params.page,
+    order=request.query_params.order)
 
 await repo.insert({
     "name": "Bursa de Valori Bucuresti SA",
     "type": 1,
     "industrySector": 40,
     "isin": "ROBVBAACNOR0",
     "bloombergCode": "BBG000BBWMC5",
@@ -216,22 +216,22 @@
         ["Coca-Cola HBC AG", 1, 49, "CH0198251305", "BBG004HJV2T1", "EEE GA Equity", "EUR", "GR"],
     ]
 )
 
 await repo.update({
     "type": 1,
     "isin": 40,
-}, request.query_parameters.conditions, request.query_parameters.fields)
+}, request.query_params.conditions, request.query_params.fields)
 
 await repo.update_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), {
     "type": 1,
     "isin": 40
 })
 
-await repo.delete(request.query_parameters.conditions, ["id", "name", "type"])
+await repo.delete(request.query_params.conditions, ["id", "name", "type"])
 
 await repo.delete_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), ["id", "name", "type"])
 
 await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
```

### Comparing `braincube-aws-core-0.0.1/src/braincube_aws_core.egg-info/SOURCES.txt` & `braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 setup.py
 src/braincube_aws_core.egg-info/PKG-INFO
 src/braincube_aws_core.egg-info/SOURCES.txt
 src/braincube_aws_core.egg-info/dependency_links.txt
 src/braincube_aws_core.egg-info/requires.txt
 src/braincube_aws_core.egg-info/top_level.txt
 src/core/__init__.py
+src/core/app/__init__.py
+src/core/app/app_controller.py
+src/core/app/app_event.py
+src/core/app/app_module.py
+src/core/app/data.py
+src/core/app/exception_handler.py
 src/core/dal/__init__.py
 src/core/dal/data.py
 src/core/dal/database_errors.py
 src/core/dal/postgres_connection.py
 src/core/dal/postgres_repository.py
 src/core/di/__init__.py
 src/core/di/data.py
 src/core/di/injector.py
-src/core/rest/__init__.py
-src/core/rest/app_controller.py
-src/core/rest/app_module.py
-src/core/rest/data.py
 src/core/rules_engine/__init__.py
 src/core/rules_engine/data.py
 src/core/rules_engine/exceptions.py
 src/core/rules_engine/rule_manager.py
 src/core/utils/__init__.py
 src/core/utils/convert.py
 src/core/utils/data.py
```

### Comparing `braincube-aws-core-0.0.1/src/core/dal/data.py` & `braincube-aws-core-0.0.2/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/dal/postgres_connection.py` & `braincube-aws-core-0.0.2/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/dal/postgres_repository.py` & `braincube-aws-core-0.0.2/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/di/data.py` & `braincube-aws-core-0.0.2/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/di/injector.py` & `braincube-aws-core-0.0.2/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/rest/app_controller.py` & `braincube-aws-core-0.0.2/src/core/app/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/rules_engine/data.py` & `braincube-aws-core-0.0.2/src/core/rules_engine/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/rules_engine/rule_manager.py` & `braincube-aws-core-0.0.2/src/core/rules_engine/rule_manager.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/utils/convert.py` & `braincube-aws-core-0.0.2/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.1/src/core/utils/data.py` & `braincube-aws-core-0.0.2/src/core/utils/data.py`

 * *Files identical despite different names*

