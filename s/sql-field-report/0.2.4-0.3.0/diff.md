# Comparing `tmp/sql_field_report-0.2.4.tar.gz` & `tmp/sql_field_report-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.2.4.tar", max compression
+gzip compressed data, was "sql_field_report-0.3.0.tar", max compression
```

## Comparing `sql_field_report-0.2.4.tar` & `sql_field_report-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      717 2023-06-20 16:59:24.080891 sql_field_report-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.2.4/README.md
--rw-r--r--   0        0        0      116 2023-06-12 09:54:08.238167 sql_field_report-0.2.4/sql_field_report/__init__.py
--rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.2.4/sql_field_report/__main__.py
--rw-r--r--   0        0        0     4069 2023-06-12 10:03:44.017730 sql_field_report-0.2.4/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.2.4/sql_field_report/utils/__init__.py
--rw-r--r--   0        0        0     6919 2023-06-12 09:54:08.250421 sql_field_report-0.2.4/sql_field_report/utils/analysis.py
--rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-0.2.4/sql_field_report/utils/databases.py
--rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-0.2.4/sql_field_report/utils/excel.py
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 sql_field_report-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      764 2023-06-21 10:20:01.660767 sql_field_report-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.3.0/README.md
+-rw-r--r--   0        0        0       83 2023-06-21 10:20:40.824766 sql_field_report-0.3.0/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.3.0/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     4069 2023-06-21 10:20:27.440753 sql_field_report-0.3.0/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.3.0/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0     7534 2023-06-21 10:20:27.455742 sql_field_report-0.3.0/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-0.3.0/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-0.3.0/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 sql_field_report-0.3.0/PKG-INFO
```

### Comparing `sql_field_report-0.2.4/pyproject.toml` & `sql_field_report-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "0.2.4"
+version = "0.3.0"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -13,14 +13,16 @@
 sqlalchemy = "^2.0.11"
 python-dotenv = "^1.0.0"
 regex = "^2023.3.23"
 pyodbc = "^4.0.39"
 typer = {extras = ["all"], version = "^0.7.0"}
 coloredlogs = "^15.0.1"
 mysql-connector-python = "^8.0.33"
+pytest = "^7.3.2"
+faust-cchardet = "^2.1.18"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [tool.poetry.scripts]
 sql-field-report = "sql_field_report.sql_field_report:app"
```

### Comparing `sql_field_report-0.2.4/README.md` & `sql_field_report-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.4/sql_field_report/sql_field_report.py` & `sql_field_report-0.3.0/sql_field_report/sql_field_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Callable
 
 import coloredlogs
 import pandas as pd
 import typer
-from sqlalchemy import text, Connection
+from sqlalchemy import Connection, text
 
 from .utils.analysis import analyze_dataframes, analyze_sql_tables
 from .utils.databases import MSSQLConnection, MySQLConnection
 from .utils.excel import generate_excel_report
 
 
 def build_sql_field_report(output_file_name: str, objects: list, conn: Connection):
```

### Comparing `sql_field_report-0.2.4/sql_field_report/utils/analysis.py` & `sql_field_report-0.3.0/sql_field_report/utils/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 import logging
+import sys
+import time
+import traceback
+from multiprocessing import Pool
 from typing import Callable
 
 import pandas as pd
 import regex as re
 from sqlalchemy import text
 from sqlalchemy.engine import Connection
 
@@ -81,41 +85,42 @@
         and (not float(count) == float(distinct_count))
     ):
         return True
     else:
         return False
 
 
-def review_column(file: str, data: pd.DataFrame, column: str):
+def review_column(column_data: tuple[str, str, pd.Series]):
     """
     Review a column of data in a data set to return field report metadata
 
     Params:
     str: file - The source file/table
-    pd.DataFrame: data - the data
-    str: column - the column being analyzed
+    tuple[str, pd.Series]: column - a tuple containing the column name and the column in a pd.Series
 
     Return:
     tuple: analysis - the column analysis
     """
 
+    file, column, data = column_data
+
     if data.shape[0] != 0:
         length = len(data)
-        values = data[column].dropna().to_list()
+        values = data.dropna().to_list()
         populated = len(values)
         unique = len(set(values))
 
         if length > 0:
             choice_ratio = float(unique) / float(length)
         else:
             choice_ratio = length
 
         choice_flag = get_choice_flag(unique, choice_ratio, length)
 
-        values = data[column].to_list()
+        values = data.to_list()
 
         types = list([estimate_dealcloud_datatype(v, choice_flag) for v in set(values)])
 
         datatype = most_common(types)
 
         analysis = (file, column, length, populated, unique, datatype)
 
@@ -123,33 +128,49 @@
 
     else:
         analysis = (file, column, 0, 0, 0, "EMPTY")
 
     return analysis
 
 
+def get_series(table: str, data: pd.DataFrame) -> list[tuple[str, pd.Series]]:
+    """Accepts a dataframe and returns a list of series
+
+    Args:
+        data (pd.DataFrame): Dataframe to be broken down
+
+    Returns:
+        list[pd.Series]: List of series for each dataframe column
+    """
+    return list([(table, c, data[c]) for c in data.columns])
+
+
 def analyze_sql_table(table: str, conn: Connection):
     """
     Take in a file path and return an overview of the shape of that file
 
     Params:
     str: table - the database table to query
 
     Returns:
     Tuple: file_shape - a tuple of tuples containing the file name, field name, row count for each field
     """
     try:
         data = pd.read_sql(text(f"SELECT * FROM {table}"), conn)
 
-        file_shape = tuple((review_column(table, data, h) for h in data.columns))
+        data = get_series(table, data)
+
+        with Pool() as p:
+            file_shape = p.map(review_column, data)
     except:
         data = pd.DataFrame.from_records(
             data=[["ERROR", "ERROR"]], columns=["ERROR", "ERROR2"]
         )
-        file_shape = tuple((review_column(table, data, h) for h in data.columns))
+        data = get_series(data)
+        file_shape = tuple((review_column(h) for h in data))
 
     return file_shape
 
 
 def analyze_dataframe(table: str, get_data: Callable[[str], pd.DataFrame]) -> tuple:
     """Analyze a dataframe
 
@@ -158,22 +179,25 @@
         get_data (Callable[[str], pd.DataFrame]): A function that will take in a table name and return a Dataframe
 
     Returns:
         tuple: A tuple describing the shape of the data
     """
     try:
         data = get_data(table)
+        data = get_series(table, data)
 
-        file_shape = tuple((review_column(table, data, h) for h in data.columns))
+        with Pool() as p:
+            file_shape = p.map(review_column, data)
     except:
+        traceback.print_exc()
         data = pd.DataFrame.from_records(
             data=[["ERROR", "ERROR"]], columns=["ERROR", "ERROR2"]
         )
-        file_shape = tuple((review_column(table, data, h) for h in data.columns))
-
+        data = get_series(data)
+        file_shape = tuple((review_column(h) for h in data))
     return file_shape
 
 
 def analyze_sql_tables(objects: list, conn: Connection) -> pd.DataFrame:
     """
     Analyze SQL Tables
```

### Comparing `sql_field_report-0.2.4/sql_field_report/utils/databases.py` & `sql_field_report-0.3.0/sql_field_report/utils/databases.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.4/sql_field_report/utils/excel.py` & `sql_field_report-0.3.0/sql_field_report/utils/excel.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.4/PKG-INFO` & `sql_field_report-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 0.2.4
+Version: 0.3.0
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
+Requires-Dist: faust-cchardet (>=2.1.18,<3.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyodbc (>=4.0.39,<5.0.0)
+Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: regex (>=2023.3.23,<2024.0.0)
 Requires-Dist: sqlalchemy (>=2.0.11,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # SQL Field Report
```

