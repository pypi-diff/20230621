# Comparing `tmp/airflow-provider-duckdb-0.1.1a1.tar.gz` & `tmp/airflow-provider-duckdb-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-duckdb-0.1.1a1.tar", last modified: Wed Jun 21 17:16:23 2023, max compression
+gzip compressed data, was "airflow-provider-duckdb-0.1.1a2.tar", last modified: Wed Jun 21 17:35:16 2023, max compression
```

## Comparing `airflow-provider-duckdb-0.1.1a1.tar` & `airflow-provider-duckdb-0.1.1a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.348516 airflow-provider-duckdb-0.1.1a1/
--rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a1/LICENSE
--rw-r--r--   0 julian     (502) staff       (20)     2728 2023-06-21 17:16:23.348282 airflow-provider-duckdb-0.1.1a1/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)     2306 2023-02-02 17:24:37.000000 airflow-provider-duckdb-0.1.1a1/README.md
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.347054 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/
--rw-r--r--   0 julian     (502) staff       (20)     2728 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/requires.txt
--rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-21 17:16:23.000000 airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.347264 airflow-provider-duckdb-0.1.1a1/duckdb_provider/
--rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a1/duckdb_provider/__init__.py
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:16:23.347838 airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/
--rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/__init__.py
--rw-r--r--   0 julian     (502) staff       (20)     1748 2023-06-21 17:14:39.000000 airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/duckdb_hook.py
--rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-21 17:16:23.348588 airflow-provider-duckdb-0.1.1a1/setup.cfg
--rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-21 17:15:17.000000 airflow-provider-duckdb-0.1.1a1/setup.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:35:16.539845 airflow-provider-duckdb-0.1.1a2/
+-rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a2/LICENSE
+-rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 17:35:16.539622 airflow-provider-duckdb-0.1.1a2/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)     2655 2023-06-21 17:25:11.000000 airflow-provider-duckdb-0.1.1a2/README.md
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:35:16.538359 airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/
+-rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-21 17:35:16.000000 airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-21 17:35:16.000000 airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-21 17:35:16.000000 airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-21 17:35:16.000000 airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-21 17:35:16.000000 airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/requires.txt
+-rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-21 17:35:16.000000 airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:35:16.538528 airflow-provider-duckdb-0.1.1a2/duckdb_provider/
+-rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a2/duckdb_provider/__init__.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-21 17:35:16.539185 airflow-provider-duckdb-0.1.1a2/duckdb_provider/hooks/
+-rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a2/duckdb_provider/hooks/__init__.py
+-rw-r--r--   0 julian     (502) staff       (20)     1780 2023-06-21 17:34:43.000000 airflow-provider-duckdb-0.1.1a2/duckdb_provider/hooks/duckdb_hook.py
+-rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-21 17:35:16.539911 airflow-provider-duckdb-0.1.1a2/setup.cfg
+-rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-21 17:34:50.000000 airflow-provider-duckdb-0.1.1a2/setup.py
```

### Comparing `airflow-provider-duckdb-0.1.1a1/LICENSE` & `airflow-provider-duckdb-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.1a1/PKG-INFO` & `airflow-provider-duckdb-0.1.1a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -12,30 +12,40 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # airflow-provider-duckdb
 
 A DuckDB provider for Airflow. This provider exposes a hook/connection that returns a DuckDB connection.
 
+This works for either local or MotherDuck connections.
+
 ## Installation
 
 ```bash
 pip install airflow-provider-duckdb
 ```
 
 ## Connection
 
 The connection type is `duckdb`. It supports setting the following parameters:
 
-- `file` (optional): The path to the DuckDB database file. If not set, operations will be done in-memory.
+- `host` (optional): Path to local file or MotherDuck database (leave blank for in-memory database)
+- `password` (optional): MotherDuck Service token (leave blank for local database)
+
+These have been relabeled in the Airflow UI for clarity.
+
+For example, if you want to connect to a local file:
+
+- `host`: `/path/to/file.db`
+- `password`: (leave blank)
 
-Example connection strings:
+If you want to connect to a MotherDuck database:
 
-- `duckdb://:memory:`
-- `duckdb:///tmp/duckdb.db`
+- `host`: `<YOUR_DB_NAME>`
+- `password`: `<YOUR_MOTHERDUCK_SERVICE_TOKEN>`
 
 ## Usage
 
 ```python
 import pandas as pd
 import pendulum
```

### Comparing `airflow-provider-duckdb-0.1.1a1/README.md` & `airflow-provider-duckdb-0.1.1a2/airflow_provider_duckdb.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,51 @@
+Metadata-Version: 2.1
+Name: airflow-provider-duckdb
+Version: 0.1.1a2
+Summary: DuckDB (duckdb.org) provider for Apache Airflow
+Home-page: http://astronomer.io/
+Author: Julian LaNeve
+Author-email: julian@astronomer.io
+License: Apache License 2.0
+Classifier: Framework :: Apache Airflow
+Classifier: Framework :: Apache Airflow :: Provider
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # airflow-provider-duckdb
 
 A DuckDB provider for Airflow. This provider exposes a hook/connection that returns a DuckDB connection.
 
+This works for either local or MotherDuck connections.
+
 ## Installation
 
 ```bash
 pip install airflow-provider-duckdb
 ```
 
 ## Connection
 
 The connection type is `duckdb`. It supports setting the following parameters:
 
-- `file` (optional): The path to the DuckDB database file. If not set, operations will be done in-memory.
+- `host` (optional): Path to local file or MotherDuck database (leave blank for in-memory database)
+- `password` (optional): MotherDuck Service token (leave blank for local database)
+
+These have been relabeled in the Airflow UI for clarity.
+
+For example, if you want to connect to a local file:
+
+- `host`: `/path/to/file.db`
+- `password`: (leave blank)
 
-Example connection strings:
+If you want to connect to a MotherDuck database:
 
-- `duckdb://:memory:`
-- `duckdb:///tmp/duckdb.db`
+- `host`: `<YOUR_DB_NAME>`
+- `password`: `<YOUR_MOTHERDUCK_SERVICE_TOKEN>`
 
 ## Usage
 
 ```python
 import pandas as pd
 import pendulum
```

### Comparing `airflow-provider-duckdb-0.1.1a1/airflow_provider_duckdb.egg-info/PKG-INFO` & `airflow-provider-duckdb-0.1.1a2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-Metadata-Version: 2.1
-Name: airflow-provider-duckdb
-Version: 0.1.1a1
-Summary: DuckDB (duckdb.org) provider for Apache Airflow
-Home-page: http://astronomer.io/
-Author: Julian LaNeve
-Author-email: julian@astronomer.io
-License: Apache License 2.0
-Classifier: Framework :: Apache Airflow
-Classifier: Framework :: Apache Airflow :: Provider
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # airflow-provider-duckdb
 
 A DuckDB provider for Airflow. This provider exposes a hook/connection that returns a DuckDB connection.
 
+This works for either local or MotherDuck connections.
+
 ## Installation
 
 ```bash
 pip install airflow-provider-duckdb
 ```
 
 ## Connection
 
 The connection type is `duckdb`. It supports setting the following parameters:
 
-- `file` (optional): The path to the DuckDB database file. If not set, operations will be done in-memory.
+- `host` (optional): Path to local file or MotherDuck database (leave blank for in-memory database)
+- `password` (optional): MotherDuck Service token (leave blank for local database)
+
+These have been relabeled in the Airflow UI for clarity.
+
+For example, if you want to connect to a local file:
+
+- `host`: `/path/to/file.db`
+- `password`: (leave blank)
 
-Example connection strings:
+If you want to connect to a MotherDuck database:
 
-- `duckdb://:memory:`
-- `duckdb:///tmp/duckdb.db`
+- `host`: `<YOUR_DB_NAME>`
+- `password`: `<YOUR_MOTHERDUCK_SERVICE_TOKEN>`
 
 ## Usage
 
 ```python
 import pandas as pd
 import pendulum
```

### Comparing `airflow-provider-duckdb-0.1.1a1/duckdb_provider/hooks/duckdb_hook.py` & `airflow-provider-duckdb-0.1.1a2/duckdb_provider/hooks/duckdb_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         airflow_conn = self.get_connection(conn_id)
 
         host = ""
         if airflow_conn.host:
             host = airflow_conn.host
 
         # if a token was given, return a MotherDuck URI
-        if airflow_conn.password:
+        if airflow_conn.password and airflow_conn.password != "":
             return f"motherduck:{host}?token={airflow_conn.password}"
 
         # if we don't have a host, assume we're using an in-memory database
         if not airflow_conn.host:
             return "duckdb:///:memory:"
 
         # otherwise return the host
```

### Comparing `airflow-provider-duckdb-0.1.1a1/setup.py` & `airflow-provider-duckdb-0.1.1a2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-provider-duckdb",
-    version="0.1.1a1",
+    version="0.1.1a2",
     description="DuckDB (duckdb.org) provider for Apache Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "apache_airflow_provider": [
             "provider_info=duckdb_provider.__init__:get_provider_info"
         ]
```

