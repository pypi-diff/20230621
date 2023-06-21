# Comparing `tmp/airflow-provider-duckdb-0.1.0.tar.gz` & `tmp/airflow-provider-duckdb-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-duckdb-0.1.0.tar", last modified: Tue May  2 14:54:57 2023, max compression
+gzip compressed data, was "airflow-provider-duckdb-0.1.1a1.tar", last modified: Wed Jun 21 17:16:23 2023, max compression
```

## Comparing `airflow-provider-duckdb-0.1.0.tar` & `airflow-provider-duckdb-0.1.1a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.291730 airflow-provider-duckdb-0.1.0/
--rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.0/LICENSE
--rw-r--r--   0 julian     (502) staff       (20)     2726 2023-05-02 14:54:57.291531 airflow-provider-duckdb-0.1.0/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)     2306 2023-02-02 17:24:37.000000 airflow-provider-duckdb-0.1.0/README.md
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.290421 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/
--rw-r--r--   0 julian     (502) staff       (20)     2726 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)      409 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (502) staff       (20)        1 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 julian     (502) staff       (20)       85 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 julian     (502) staff       (20)       48 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/requires.txt
--rw-r--r--   0 julian     (502) staff       (20)       16 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.290588 airflow-provider-duckdb-0.1.0/duckdb_provider/
--rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.0/duckdb_provider/__init__.py
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.291143 airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/
--rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/__init__.py
--rw-r--r--   0 julian     (502) staff       (20)     1799 2022-10-31 14:37:54.000000 airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/duckdb_hook.py
--rw-r--r--   0 julian     (502) staff       (20)       38 2023-05-02 14:54:57.291778 airflow-provider-duckdb-0.1.0/setup.cfg
--rw-r--r--   0 julian     (502) staff       (20)      944 2023-05-02 14:54:30.000000 airflow-provider-duckdb-0.1.0/setup.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.348516 airflow-provider-duckdb-0.1.1a1/
+-rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a1/LICENSE
+-rw-r--r--   0 julian     (502) staff       (20)     2728 2023-06-21 17:16:23.348282 airflow-provider-duckdb-0.1.1a1/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)     2306 2023-02-02 17:24:37.000000 airflow-provider-duckdb-0.1.1a1/README.md
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.347054 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/
+-rw-r--r--   0 julian     (502) staff       (20)     2728 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/requires.txt
+-rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.347264 airflow-provider-duckdb-0.1.1a1/duckdb_provider/
+-rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a1/duckdb_provider/__init__.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.347838 airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/
+-rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/__init__.py
+-rw-r--r--   0 julian     (502) staff       (20)     1748 2023-06-21 17:14:39.000000 airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/duckdb_hook.py
+-rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-21 17:16:23.348588 airflow-provider-duckdb-0.1.1a1/setup.cfg
+-rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-21 17:15:17.000000 airflow-provider-duckdb-0.1.1a1/setup.py
```

### Comparing `airflow-provider-duckdb-0.1.0/LICENSE` & `airflow-provider-duckdb-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.0/PKG-INFO` & `airflow-provider-duckdb-0.1.1a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.1.0/README.md` & `airflow-provider-duckdb-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/PKG-INFO` & `airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/duckdb_hook.py` & `airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/duckdb_hook.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,45 +13,43 @@
     default_conn_name = "duckdb_default"
     conn_type = "duckdb"
     hook_name = "DuckDB"
     placeholder = "?"
 
     def get_conn(self) -> duckdb.DuckDBPyConnection:
         """Returns a duckdb connection object"""
-        # get the conn_id from the hook
-        conn_id = getattr(self, self.conn_name_attr)
-
-        # get the airflow connection object with config
-        airflow_conn = self.get_connection(conn_id)
-
-        # return the duckdb connection
-        # either in memory if we don't have a host
-        if not airflow_conn.host:
-            return duckdb.connect(":memory:")
-
-        # or from a file specified by the host field
-        return duckdb.connect(airflow_conn.host)
+        uri = self.get_uri()
+        return duckdb.connect(uri)
 
     def get_uri(self) -> str:
         """Override DbApiHook get_uri method for get_sqlalchemy_engine()"""
         # get the conn_id from the hook
         conn_id = getattr(self, self.conn_name_attr)
 
         # get the airflow connection object with config
         airflow_conn = self.get_connection(conn_id)
 
+        host = ""
+        if airflow_conn.host:
+            host = airflow_conn.host
+
+        # if a token was given, return a MotherDuck URI
+        if airflow_conn.password:
+            return f"motherduck:{host}?token={airflow_conn.password}"
+
         # if we don't have a host, assume we're using an in-memory database
         if not airflow_conn.host:
             return "duckdb:///:memory:"
 
         # otherwise return the host
         return f"duckdb:///{airflow_conn.host}"
 
     @staticmethod
     def get_ui_field_behaviour() -> Dict:
         """Returns custom field behaviour"""
         return {
-            "hidden_fields": ["login", "password", "schema", "port", "extra"],
+            "hidden_fields": ["login", "schema", "port", "extra"],
             "relabeling": {
-                "host": "File (leave blank for in-memory database)",
+                "host": "Path to local file or MotherDuck database (leave blank for in-memory database)",
+                "password": "MotherDuck Service token (leave blank for local database)",
             },
         }
```

### Comparing `airflow-provider-duckdb-0.1.0/setup.py` & `airflow-provider-duckdb-0.1.1a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-provider-duckdb",
-    version="0.1.0",
+    version="0.1.1a1",
     description="DuckDB (duckdb.org) provider for Apache Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "apache_airflow_provider": [
             "provider_info=duckdb_provider.__init__:get_provider_info"
         ]
```

