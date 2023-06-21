# Comparing `tmp/airflow-provider-duckdb-0.1.1a3.tar.gz` & `tmp/airflow-provider-duckdb-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-duckdb-0.1.1a3.tar", last modified: Wed Jun 21 18:17:23 2023, max compression
+gzip compressed data, was "airflow-provider-duckdb-0.1.1a4.tar", last modified: Wed Jun 21 18:35:57 2023, max compression
```

## Comparing `airflow-provider-duckdb-0.1.1a3.tar` & `airflow-provider-duckdb-0.1.1a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:17:23.633666 airflow-provider-duckdb-0.1.1a3/
--rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a3/LICENSE
--rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 18:17:23.633455 airflow-provider-duckdb-0.1.1a3/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)     2655 2023-06-21 17:25:11.000000 airflow-provider-duckdb-0.1.1a3/README.md
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:17:23.632254 airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/
--rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 18:17:23.000000 airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-21 18:17:23.000000 airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-21 18:17:23.000000 airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-21 18:17:23.000000 airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-21 18:17:23.000000 airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/requires.txt
--rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-21 18:17:23.000000 airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:17:23.632427 airflow-provider-duckdb-0.1.1a3/duckdb_provider/
--rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a3/duckdb_provider/__init__.py
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:17:23.633075 airflow-provider-duckdb-0.1.1a3/duckdb_provider/hooks/
--rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a3/duckdb_provider/hooks/__init__.py
--rw-r--r--   0 julian     (502) staff       (20)     2163 2023-06-21 18:14:24.000000 airflow-provider-duckdb-0.1.1a3/duckdb_provider/hooks/duckdb_hook.py
--rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-21 18:17:23.633725 airflow-provider-duckdb-0.1.1a3/setup.cfg
--rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-21 18:17:01.000000 airflow-provider-duckdb-0.1.1a3/setup.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:35:57.068959 airflow-provider-duckdb-0.1.1a4/
+-rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a4/LICENSE
+-rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 18:35:57.068789 airflow-provider-duckdb-0.1.1a4/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)     2655 2023-06-21 17:25:11.000000 airflow-provider-duckdb-0.1.1a4/README.md
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:35:57.067620 airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/
+-rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 18:35:57.000000 airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-21 18:35:57.000000 airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-21 18:35:57.000000 airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-21 18:35:57.000000 airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-21 18:35:57.000000 airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/requires.txt
+-rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-21 18:35:57.000000 airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:35:57.067793 airflow-provider-duckdb-0.1.1a4/duckdb_provider/
+-rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a4/duckdb_provider/__init__.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 18:35:57.068446 airflow-provider-duckdb-0.1.1a4/duckdb_provider/hooks/
+-rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a4/duckdb_provider/hooks/__init__.py
+-rw-r--r--   0 julian     (502) staff       (20)     2164 2023-06-21 18:35:19.000000 airflow-provider-duckdb-0.1.1a4/duckdb_provider/hooks/duckdb_hook.py
+-rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-21 18:35:57.069006 airflow-provider-duckdb-0.1.1a4/setup.cfg
+-rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-21 18:35:51.000000 airflow-provider-duckdb-0.1.1a4/setup.py
```

### Comparing `airflow-provider-duckdb-0.1.1a3/LICENSE` & `airflow-provider-duckdb-0.1.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.1a3/PKG-INFO` & `airflow-provider-duckdb-0.1.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.1.1a3/README.md` & `airflow-provider-duckdb-0.1.1a4/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.1a3/airflow_provider_duckdb.egg-info/PKG-INFO` & `airflow-provider-duckdb-0.1.1a4/airflow_provider_duckdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.1.1a3/duckdb_provider/hooks/duckdb_hook.py` & `airflow-provider-duckdb-0.1.1a4/duckdb_provider/hooks/duckdb_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         # if a user gave a host, use a connection to a local file
         if airflow_conn.host:
             return f"duckdb:///{airflow_conn.host}"
 
         # if a user gave a password, use a connection to a MotherDuck instance
         if airflow_conn.password:
             db_name = airflow_conn.schema or ""
-            return f"duckdb:///md:{db_name}?motherduck_token{airflow_conn.password}&token={airflow_conn.password}"
+            return f"duckdb:///md:{db_name}?motherduck_token={airflow_conn.password}&token={airflow_conn.password}"
 
         # otherwise use an in-memory connection
         return f"duckdb:///:memory:"
 
     @staticmethod
     def get_ui_field_behaviour() -> Dict:
         """Returns custom field behaviour"""
```

### Comparing `airflow-provider-duckdb-0.1.1a3/setup.py` & `airflow-provider-duckdb-0.1.1a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-provider-duckdb",
-    version="0.1.1a3",
+    version="0.1.1a4",
     description="DuckDB (duckdb.org) provider for Apache Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "apache_airflow_provider": [
             "provider_info=duckdb_provider.__init__:get_provider_info"
         ]
```

