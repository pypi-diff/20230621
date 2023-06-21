# Comparing `tmp/redb-odm-1.2.2.tar.gz` & `tmp/redb-odm-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.2.2.tar", last modified: Thu Jun  8 18:15:57 2023, max compression
+gzip compressed data, was "redb-odm-1.2.3.tar", last modified: Wed Jun 21 01:05:07 2023, max compression
```

## Comparing `redb-odm-1.2.2.tar` & `redb-odm-1.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.255736 redb-odm-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 18:15:38.000000 redb-odm-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 18:15:57.255736 redb-odm-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 18:15:38.000000 redb-odm-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.243736 redb-odm-1.2.2/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.247736 redb-odm-1.2.2/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/behaviors/i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.247736 redb-odm-1.2.2/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 18:15:38.000000 redb-odm-1.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 18:15:38.000000 redb-odm-1.2.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 18:15:38.000000 redb-odm-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:15:57.255736 redb-odm-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-08 18:15:38.000000 redb-odm-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.255736 redb-odm-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_soft_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_unique_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 01:04:51.000000 redb-odm-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 01:05:07.649717 redb-odm-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 01:04:51.000000 redb-odm-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.645717 redb-odm-1.2.3/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.645717 redb-odm-1.2.3/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/behaviors/i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.645717 redb-odm-1.2.3/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 01:04:51.000000 redb-odm-1.2.3/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 01:05:07.000000 redb-odm-1.2.3/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 01:04:51.000000 redb-odm-1.2.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 01:04:51.000000 redb-odm-1.2.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 01:04:51.000000 redb-odm-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:05:07.653717 redb-odm-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-21 01:04:51.000000 redb-odm-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:05:07.649717 redb-odm-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_soft_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-21 01:04:51.000000 redb-odm-1.2.3/tests/test_unique_constraints.py
```

### Comparing `redb-odm-1.2.2/redb/behaviors/i_remember.py` & `redb-odm-1.2.3/redb/behaviors/i_remember.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,17 @@
 
         out = super().dict(*args, **kwargs)
         return out
 
     @classmethod
     def get_hashable_fields(cls) -> list[ClassField]:
         all_fields = super().get_hashable_fields()
-        return list(filter(lambda x: x.model_field.name not in HISTORY_FIELDS, all_fields))
+        return list(
+            filter(lambda x: x.model_field.name not in HISTORY_FIELDS, all_fields)
+        )
 
     @classmethod
     def historical_find_one(
         cls: Type[T],
         filter: OptionalDocumentData = None,
         fields: IncludeColumns = None,
         skip: int = 0,
@@ -175,15 +177,15 @@
         update: DocumentData,
         upsert: bool = False,
         operator: str | None = "$set",
         allow_new_fields: bool = False,
         user_info: Any = None,
     ) -> UpdateOneResult:
         original_doc = super().find_one(filter=filter)
-        new_history = cls.__build_history_from_ref(user_info, original_doc)
+        new_history = cls._build_history_from_ref(user_info, original_doc)
         update_result = cls.update_one(
             filter={"_id": original_doc.id},
             update=update,
             upsert=upsert,
             operator=operator,
             allow_new_fields=allow_new_fields,
         )
@@ -191,52 +193,54 @@
         return update_result
 
     @classmethod
     def historical_replace_one(
         cls, filter: DocumentData, replacement: DocumentData, user_info: Any = None
     ) -> ReplaceOneResult:
         original_doc = super().find_one(filter=filter)
-        new_history = cls.__build_history_from_ref(user_info, original_doc)
+        new_history = cls._build_history_from_ref(user_info, original_doc)
         replace_result = cls.replace_one(
             filter={"_id": original_doc.id},
             replacement=replacement,
         )
         cls._historical_insert_one(new_history)
         return replace_result
 
-
     @classmethod
     def historical_delete_one(
         cls,
         filter: DocumentData,
         user_info: Any = None,
     ) -> DeleteOneResult:
         original_doc = super().find_one(filter=filter)
-        new_history = cls.__build_history_from_ref(user_info, original_doc)
+        new_history = cls._build_history_from_ref(user_info, original_doc)
         delete_result = cls.delete_one(filter={"_id": original_doc.id})
         cls._historical_insert_one(new_history)
         return delete_result
 
     @classmethod
-    def __build_history_from_ref(
+    def _build_history_from_ref(
         cls,
         user_info: Any,
         referenced_doc: "IRememberDoc",
     ) -> Dict:
         history_filter = {"ref_id": referenced_doc.id}
         try:
-            history = cls.historical_find_one(filter=history_filter, fields=["version"])
+            histories = cls.historical_find_many(filter=history_filter, fields=["version"], limit=1)
+            history = histories[0]
             version = history["version"] + 1  # type: ignore
-        except DocumentNotFound:
+        except (DocumentNotFound, IndexError):
             version = 1
 
         new_history = referenced_doc.dict(
             ignored_history_fields=False,
             exclude={"id"},
             exclude_none=True,
         )
         new_history["version"] = version
-        new_history["retired_by"] = user_info.dict() if hasattr(user_info, "dict") else str(user_info)
+        new_history["retired_by"] = (
+            user_info.dict() if hasattr(user_info, "dict") else str(user_info)
+        )
         new_history["retired_at"] = pytz.UTC.localize(datetime.utcnow()).isoformat()
         new_history["ref_id"] = referenced_doc.id
         new_history["_id"] = f"{referenced_doc.id}_v{version}"
         return new_history
```

### Comparing `redb-odm-1.2.2/redb/behaviors/soft_deletion.py` & `redb-odm-1.2.3/redb/behaviors/soft_deletion.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,33 +16,33 @@
         all_fields = super().get_hashable_fields()
         return list(filter(lambda x: x.model_field.name != "is_deleted", all_fields))
 
     @classmethod
     def soft_delete_one(cls, filters):
         result = cls.update_one(filters, dict(is_deleted=True))
         if not result.matched_count:
-            raise DocumentNotFound
+            raise DocumentNotFound(collection_name=cls.collection_name())
 
     @classmethod
     def soft_undelete_one(cls, filters):
         result = cls.update_one(filters, dict(is_deleted=False))
         if not result.matched_count:
-            raise DocumentNotFound
+            raise DocumentNotFound(collection_name=cls.collection_name())
 
     @classmethod
     def soft_delete_many(cls, filters):
         result = cls.update_many(filters, dict(is_deleted=True))
         if not result.matched_count:
-            raise DocumentNotFound
+            raise DocumentNotFound(collection_name=cls.collection_name())
 
     @classmethod
     def soft_undelete_many(cls, filters):
         result = cls.update_many(filters, dict(is_deleted=False))
         if not result.matched_count:
-            raise DocumentNotFound
+            raise DocumentNotFound(collection_name=cls.collection_name())
 
     @classmethod
     def find_one(
         cls: Type[T],
         filter: OptionalDocumentData = None,
         fields: IncludeColumns = None,
         skip: int = 0,
```

### Comparing `redb-odm-1.2.2/redb/core/base.py` & `redb-odm-1.2.3/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/core/document.py` & `redb-odm-1.2.3/redb/core/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from pathlib import Path
 from typing import Any, Dict, Sequence, Type, TypeAlias, TypeVar, Union, cast
 
 import pytz
 from pymongo.errors import DuplicateKeyError
 from redb.interface.errors import (
     CannotUpdateIdentifyingField,
     UniqueConstraintViolation,
@@ -42,14 +43,15 @@
     created_at: datetime = Field(default_factory=lambda: datetime.now(pytz.UTC))  # type: ignore
     updated_at: datetime = Field(default_factory=lambda: datetime.now(pytz.UTC))  # type: ignore
 
     class Config:
         json_encoders = {
             datetime: lambda d: d.isoformat(),
             DBRef: lambda ref: dict(ref.as_doc()),
+            Path: str,
             ObjectId: str,
         }
         smart_union = True
 
     def __init__(self, **data: Any) -> None:
         calculate_hash = False
         if "id" in data:
```

### Comparing `redb-odm-1.2.2/redb/core/instance.py` & `redb-odm-1.2.3/redb/core/instance.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/core/transaction.py` & `redb-odm-1.2.3/redb/core/transaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import contextlib
 from datetime import datetime
 from typing import Any, ContextManager, Dict, Sequence, Type, TypeVar, overload
 
 import pytz
 from pymongo.errors import DuplicateKeyError
+from redb.behaviors import IRememberDoc
 
 from redb.core.document import (
     Document,
     DocumentData,
     IncludeColumns,
     OptionalDocumentData,
     SortColumns,
@@ -41,16 +42,17 @@
 )
 from redb.interface.errors import UniqueConstraintViolation
 
 T = TypeVar("T", bound=Document)
 
 
 class CollectionWrapper:
-    def __init__(self, collection: Collection, collection_class: T) -> None:
+    def __init__(self, collection: Collection, history_collection: Collection, collection_class: T) -> None:
         self.__collection = collection
+        self.__history_collection = history_collection
         self.__collection_class = collection_class
 
     def _get_driver_collection(self) -> Any:
         return self.__collection._get_driver_collection()
 
     def create_indexes(self) -> None:
         indexes = self.__collection_class.get_indexes()
@@ -134,14 +136,30 @@
         try:
             return self.__collection.insert_one(
                 cls=self.__collection_class,
                 data=data,
             )
         except DuplicateKeyError as e:
             raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
+        
+    def _historical_insert_one(self,data: DocumentData) -> InsertOneResult:
+        if self.__history_collection is None:
+            raise ValueError("Base class does not inherit from IRememberDoc")
+
+        data = _format_document_data(data)
+        try:
+            return self.__history_collection.insert_one(
+                cls=self.__collection_class,
+                data=data,
+            )
+        except DuplicateKeyError as e:
+            raise UniqueConstraintViolation(
+                dup_keys=e.details["keyValue"],  # type: ignore
+                collection_name=self.__collection_class.history_collection_name(),
+            )
 
     def insert_vectors(self, data: Dict[str, list[Any]]) -> InsertManyResult:
         keys = list(data.keys())
         values_size = len(data[keys[0]])
         instances = [None] * values_size
         instances = [{key: data[key][i] for key in keys} for i in range(values_size)]
 
@@ -218,14 +236,38 @@
         self.__collection.update_one(
             cls=self.__collection_class,
             filter=filter,
             update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
         )
         return result
 
+    def historical_update_one(
+        self,
+        filter: DocumentData,
+        update: DocumentData,
+        upsert: bool = False,
+        operator: str | None = "$set",
+        allow_new_fields: bool = False,
+        user_info: Any = None,
+    ) -> UpdateOneResult:
+        if self.__history_collection is None:
+            raise ValueError("Base class does not inherit from IRememberDoc")
+        
+        original_doc = self.find_one(filter=filter)
+        new_history = self.__collection_class._build_history_from_ref(user_info, original_doc)
+        update_result = self.update_one(
+            filter={"_id": original_doc.id},
+            update=update,
+            upsert=upsert,
+            operator=operator,
+            allow_new_fields=allow_new_fields,
+        )
+        self._historical_insert_one(new_history)
+        return update_result
+
     def update_many(
         self,
         filter: DocumentData,
         update: DocumentData,
         upsert: bool = False,
         operator: str | None = "$set",
         allow_new_fields: bool = False,
@@ -258,14 +300,28 @@
 
     def delete_one(self, filter: DocumentData) -> DeleteOneResult:
         filter = _format_document_data(filter)
         return self.__collection.delete_one(
             cls=self.__collection_class,
             filter=filter,
         )
+    
+    def historical_delete_one(
+        self,
+        filter: DocumentData,
+        user_info: Any = None,
+    ) -> DeleteOneResult:
+        if self.__history_collection is None:
+            raise ValueError("Base class does not inherit from IRememberDoc")
+        
+        original_doc = self.find_one(filter=filter)
+        new_history = self.__collection_class._build_history_from_ref(user_info, original_doc)
+        delete_result = self.delete_one(filter={"_id": original_doc.id})
+        self._historical_insert_one(new_history)
+        return delete_result
 
     def delete_many(self, filter: DocumentData) -> DeleteManyResult:
         filter = _format_document_data(filter)
         return self.__collection.delete_many(
             cls=self.__collection_class,
             filter=filter,
         )
@@ -305,16 +361,21 @@
     else:
         database = client.get_database(db_name)
 
     if isinstance(collection, str):
         collection = database.get_collection(collection)
     else:
         collection_name = collection.collection_name()
+        driver_history_collection = None
+        if issubclass(collection, IRememberDoc):
+            history_collection_name = collection.history_collection_name()
+            driver_history_collection = database.get_collection(history_collection_name)
+        
         driver_collection = database.get_collection(collection_name)
-        collection = CollectionWrapper(driver_collection, collection)
+        collection = CollectionWrapper(driver_collection, driver_history_collection, collection)
 
     yield collection
 
     if new_client:
         client.close()
```

### Comparing `redb-odm-1.2.2/redb/core/utils.py` & `redb-odm-1.2.3/redb/core/utils.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/interface/client.py` & `redb-odm-1.2.3/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/interface/collection.py` & `redb-odm-1.2.3/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/interface/configs.py` & `redb-odm-1.2.3/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/interface/database.py` & `redb-odm-1.2.3/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/interface/errors.py` & `redb-odm-1.2.3/redb/interface/errors.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/interface/fields.py` & `redb-odm-1.2.3/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/interface/results.py` & `redb-odm-1.2.3/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/json_system/client.py` & `redb-odm-1.2.3/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/json_system/collection.py` & `redb-odm-1.2.3/redb/json_system/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         update: Json,
         upsert: bool = False,
     ) -> UpdateOneResult:
         doc: dict = self.find_one(cls, return_cls=dict, filter=filter)
         update = update.pop(next(iter(update.keys())))  # { $set: {...} }
         if doc is None:
             if not upsert:
-                raise DocumentNotFound
+                raise DocumentNotFound(collection_name=cls.collection_name())
             result = self.insert_one(cls, data=update)
             return UpdateOneResult(
                 matched_count=1,
                 modified_count=1,
                 upserted_id=result.inserted_id,
             )
         doc_path = self.__collection / Path(f"{doc['_id']}.json")
```

### Comparing `redb-odm-1.2.2/redb/json_system/database.py` & `redb-odm-1.2.3/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/migo_system/client.py` & `redb-odm-1.2.3/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/migo_system/collection.py` & `redb-odm-1.2.3/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/migo_system/database.py` & `redb-odm-1.2.3/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/mongo_system/client.py` & `redb-odm-1.2.3/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb/mongo_system/collection.py` & `redb-odm-1.2.3/redb/mongo_system/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         result = self.__collection.find_one(
             filter=filter,
             projection=fields,
             skip=skip,
         )
         if not result:
             m = f"Document not found with filters {filter} in collection {self.__collection.name}."
-            raise DocumentNotFound(m)
+            raise DocumentNotFound(m, collection_name=self.__collection.name)
         return return_cls(**result)
 
     def distinct(
         self,
         cls: ReturnType,
         key: str,
         filter: OptionalJson = None,
```

### Comparing `redb-odm-1.2.2/redb/mongo_system/database.py` & `redb-odm-1.2.3/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.2.3/redb_odm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/setup.py` & `redb-odm-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_bson_objs.py` & `redb-odm-1.2.3/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_hashing.py` & `redb-odm-1.2.3/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_i_remember.py` & `redb-odm-1.2.3/tests/test_i_remember.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_json_client.py` & `redb-odm-1.2.3/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_mongo_system.py` & `redb-odm-1.2.3/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_return_cls.py` & `redb-odm-1.2.3/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_soft_deletion.py` & `redb-odm-1.2.3/tests/test_soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.2/tests/test_unique_constraints.py` & `redb-odm-1.2.3/tests/test_unique_constraints.py`

 * *Files identical despite different names*

