# Comparing `tmp/WqUtils-0.1.2-py3-none-any.whl.zip` & `tmp/WqUtils-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6666 bytes, number of entries: 9
+Zip file size: 9482 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     5333 b- defN 23-Jun-19 08:15 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Jun-19 15:54 WqUtils/__init__.py
+-rw-r--r--  2.0 unx     7635 b- defN 23-Jun-21 05:40 WqUtils/DB_Utils/ExecPgSql.py
 -rw-r--r--  2.0 unx     6557 b- defN 23-Jun-19 16:59 WqUtils/DB_Utils/SqlServer_DB.py
 -rw-r--r--  2.0 unx      267 b- defN 23-Jun-19 06:58 WqUtils/DB_Utils/__init__.py
--rw-r--r--  2.0 unx      255 b- defN 23-Jun-19 07:32 WqUtils/DB_Utils/db_config.toml
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      704 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/RECORD
-9 files, 13716 bytes uncompressed, 5452 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx      457 b- defN 23-Jun-21 02:48 WqUtils/DB_Utils/db_config.toml
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      790 b- defN 23-Jun-21 05:52 WqUtils-0.1.3.dist-info/RECORD
+10 files, 21639 bytes uncompressed, 8134 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: WqUtils/Utils.py
 Comment: 
 
 Filename: WqUtils/__init__.py
 Comment: 
 
+Filename: WqUtils/DB_Utils/ExecPgSql.py
+Comment: 
+
 Filename: WqUtils/DB_Utils/SqlServer_DB.py
 Comment: 
 
 Filename: WqUtils/DB_Utils/__init__.py
 Comment: 
 
 Filename: WqUtils/DB_Utils/db_config.toml
 Comment: 
 
-Filename: WqUtils-0.1.2.dist-info/METADATA
+Filename: WqUtils-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.1.2.dist-info/WHEEL
+Filename: WqUtils-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.1.2.dist-info/top_level.txt
+Filename: WqUtils-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.1.2.dist-info/RECORD
+Filename: WqUtils-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/DB_Utils/db_config.toml

```diff
@@ -5,8 +5,16 @@
 port = 9200
 
 [sqlserver_database]
 HOST = '123.57.241.126'
 PORT = 1433
 USERNAME = 'wanqiang'
 PASSWORD = 'wq2022'
-DB = 'YiliPOC'
+DB = 'YiliPOC'
+
+[pg_database]
+HOST = "gp-uf6xpccjt4kem37d4o-master.gpdb.rds.aliyuncs.com"
+PORT = "5432"
+USERNAME = "colourdata"
+PASSWORD = "Colourdata110!"
+DB = "CD_Research_DB"
+options = "-c search_path=dbo,public"
```

