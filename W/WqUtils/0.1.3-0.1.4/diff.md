# Comparing `tmp/WqUtils-0.1.3-py3-none-any.whl.zip` & `tmp/WqUtils-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9482 bytes, number of entries: 10
+Zip file size: 9492 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     5333 b- defN 23-Jun-19 08:15 WqUtils/Utils.py
--rw-r--r--  2.0 unx      292 b- defN 23-Jun-19 15:54 WqUtils/__init__.py
+-rw-r--r--  2.0 unx      334 b- defN 23-Jun-21 05:54 WqUtils/__init__.py
 -rw-r--r--  2.0 unx     7635 b- defN 23-Jun-21 05:40 WqUtils/DB_Utils/ExecPgSql.py
 -rw-r--r--  2.0 unx     6557 b- defN 23-Jun-19 16:59 WqUtils/DB_Utils/SqlServer_DB.py
 -rw-r--r--  2.0 unx      267 b- defN 23-Jun-19 06:58 WqUtils/DB_Utils/__init__.py
 -rw-r--r--  2.0 unx      457 b- defN 23-Jun-21 02:48 WqUtils/DB_Utils/db_config.toml
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      790 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/RECORD
-10 files, 21639 bytes uncompressed, 8134 bytes compressed:  62.4%
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      790 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/RECORD
+10 files, 21681 bytes uncompressed, 8144 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: WqUtils/DB_Utils/__init__.py
 Comment: 
 
 Filename: WqUtils/DB_Utils/db_config.toml
 Comment: 
 
-Filename: WqUtils-0.1.3.dist-info/METADATA
+Filename: WqUtils-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.1.3.dist-info/WHEEL
+Filename: WqUtils-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.1.3.dist-info/top_level.txt
+Filename: WqUtils-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.1.3.dist-info/RECORD
+Filename: WqUtils-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/__init__.py

```diff
@@ -5,8 +5,9 @@
 @ Date: 2022-11-25 16:55
 @ Email: stephen.wan@colourdata.com.cn
 @ LastEditors: stephen.wan
 @ LastEditTime: 2022-11-25 16:55
 @ ProjectName: model_testing
 @ Description: to do
 """
-from .DB_Utils.SqlServer_DB import ExecSql
+from .DB_Utils.SqlServer_DB import ExecSql
+from .DB_Utils.ExecPgSql import ExecPgSql
```

