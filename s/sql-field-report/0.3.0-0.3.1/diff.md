# Comparing `tmp/sql_field_report-0.3.0.tar.gz` & `tmp/sql_field_report-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.3.0.tar", max compression
+gzip compressed data, was "sql_field_report-0.3.1.tar", max compression
```

## Comparing `sql_field_report-0.3.0.tar` & `sql_field_report-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      764 2023-06-21 10:20:01.660767 sql_field_report-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.3.0/README.md
--rw-r--r--   0        0        0       83 2023-06-21 10:20:40.824766 sql_field_report-0.3.0/sql_field_report/__init__.py
--rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.3.0/sql_field_report/__main__.py
--rw-r--r--   0        0        0     4069 2023-06-21 10:20:27.440753 sql_field_report-0.3.0/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.3.0/sql_field_report/utils/__init__.py
--rw-r--r--   0        0        0     7534 2023-06-21 10:20:27.455742 sql_field_report-0.3.0/sql_field_report/utils/analysis.py
--rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-0.3.0/sql_field_report/utils/databases.py
--rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-0.3.0/sql_field_report/utils/excel.py
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 sql_field_report-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      764 2023-06-21 10:41:51.859474 sql_field_report-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.3.1/README.md
+-rw-r--r--   0        0        0       83 2023-06-21 10:20:40.824766 sql_field_report-0.3.1/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.3.1/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     4069 2023-06-21 10:20:27.440753 sql_field_report-0.3.1/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.3.1/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0     7548 2023-06-21 10:40:58.011842 sql_field_report-0.3.1/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-0.3.1/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-0.3.1/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 sql_field_report-0.3.1/PKG-INFO
```

### Comparing `sql_field_report-0.3.0/pyproject.toml` & `sql_field_report-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sql_field_report-0.3.0/README.md` & `sql_field_report-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.3.0/sql_field_report/sql_field_report.py` & `sql_field_report-0.3.1/sql_field_report/sql_field_report.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.3.0/sql_field_report/utils/analysis.py` & `sql_field_report-0.3.1/sql_field_report/utils/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
         with Pool() as p:
             file_shape = p.map(review_column, data)
     except:
         data = pd.DataFrame.from_records(
             data=[["ERROR", "ERROR"]], columns=["ERROR", "ERROR2"]
         )
-        data = get_series(data)
+        data = get_series(table, data)
         file_shape = tuple((review_column(h) for h in data))
 
     return file_shape
 
 
 def analyze_dataframe(table: str, get_data: Callable[[str], pd.DataFrame]) -> tuple:
     """Analyze a dataframe
@@ -188,15 +188,15 @@
         with Pool() as p:
             file_shape = p.map(review_column, data)
     except:
         traceback.print_exc()
         data = pd.DataFrame.from_records(
             data=[["ERROR", "ERROR"]], columns=["ERROR", "ERROR2"]
         )
-        data = get_series(data)
+        data = get_series(table, data)
         file_shape = tuple((review_column(h) for h in data))
     return file_shape
 
 
 def analyze_sql_tables(objects: list, conn: Connection) -> pd.DataFrame:
     """
     Analyze SQL Tables
```

### Comparing `sql_field_report-0.3.0/sql_field_report/utils/databases.py` & `sql_field_report-0.3.1/sql_field_report/utils/databases.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.3.0/sql_field_report/utils/excel.py` & `sql_field_report-0.3.1/sql_field_report/utils/excel.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.3.0/PKG-INFO` & `sql_field_report-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

