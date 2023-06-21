# Comparing `tmp/sqlite_dataset-0.5.0.tar.gz` & `tmp/sqlite_dataset-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_dataset-0.5.0.tar", max compression
+gzip compressed data, was "sqlite_dataset-0.5.1.tar", max compression
```

## Comparing `sqlite_dataset-0.5.0.tar` & `sqlite_dataset-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1089 2023-06-09 11:39:25.599908 sqlite_dataset-0.5.0/LICENSE
--rw-r--r--   0        0        0      528 2023-06-12 16:10:55.983467 sqlite_dataset-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5374 2023-06-09 15:11:27.339707 sqlite_dataset-0.5.0/README.md
--rw-r--r--   0        0        0       89 2023-06-09 13:45:27.347401 sqlite_dataset-0.5.0/sqlite_dataset/__init__.py
--rw-r--r--   0        0        0     5873 2023-06-12 13:08:36.472992 sqlite_dataset-0.5.0/sqlite_dataset/dataset.py
--rw-r--r--   0        0        0      702 2023-06-12 12:56:44.150591 sqlite_dataset-0.5.0/sqlite_dataset/fields.py
--rw-r--r--   0        0        0     1536 2023-06-12 13:15:21.856534 sqlite_dataset-0.5.0/sqlite_dataset/test.py
--rw-r--r--   0        0        0      308 2023-03-27 09:27:16.270611 sqlite_dataset-0.5.0/sqlite_dataset/utils.py
--rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 sqlite_dataset-0.5.0/setup.py
--rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 sqlite_dataset-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-11 19:35:01.090281 sqlite_dataset-0.5.1/LICENSE
+-rw-r--r--   0        0        0      528 2023-06-21 20:53:57.886266 sqlite_dataset-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5374 2023-06-09 18:41:19.289218 sqlite_dataset-0.5.1/README.md
+-rw-r--r--   0        0        0       89 2023-06-09 18:41:19.297903 sqlite_dataset-0.5.1/sqlite_dataset/__init__.py
+-rw-r--r--   0        0        0     5988 2023-06-21 20:51:41.145320 sqlite_dataset-0.5.1/sqlite_dataset/dataset.py
+-rw-r--r--   0        0        0      727 2023-06-12 20:13:45.118264 sqlite_dataset-0.5.1/sqlite_dataset/fields.py
+-rw-r--r--   0        0        0     2072 2023-06-21 20:53:15.797329 sqlite_dataset-0.5.1/sqlite_dataset/test.py
+-rw-r--r--   0        0        0      308 2023-03-27 07:17:29.704114 sqlite_dataset-0.5.1/sqlite_dataset/utils.py
+-rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 sqlite_dataset-0.5.1/PKG-INFO
```

### Comparing `sqlite_dataset-0.5.0/LICENSE` & `sqlite_dataset-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_dataset-0.5.0/pyproject.toml` & `sqlite_dataset-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlite-dataset"
-version = "0.5.0"
+version = "0.5.1"
 description = "Use SQLite database to store datasets."
 authors = ["Jinshuai Ma <mayazureee@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sqlite_dataset"}]
 license = "MIT"
 repository = "https://github.com/Mayazure/sqlite-dataset"
```

### Comparing `sqlite_dataset-0.5.0/README.md` & `sqlite_dataset-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlite_dataset-0.5.0/sqlite_dataset/dataset.py` & `sqlite_dataset-0.5.1/sqlite_dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,17 @@
 def _get_table_fields(attrs):
     table_fields = []
     for table_name, table_value in attrs.items():
         if is_table_class(table_value):
             use_tablename = table_value.tablename or table_name
             for (field_name, field_value) in table_value.fields:
                 field_value.tablename = use_tablename
-                table_fields.append((field_name, field_value))
+                if field_value.name is None:
+                    field_value.name = field_name
+                table_fields.append((f'{table_name}_{field_name}', field_value))
     return table_fields
 
 
 class DatasetMeta(type):
 
     def __new__(mcs, name, bases, attrs):
         __defaulttable__ = attrs.get('__defaulttable__', 'data')
```

### Comparing `sqlite_dataset-0.5.0/sqlite_dataset/test.py` & `sqlite_dataset-0.5.1/sqlite_dataset/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import pandas as pd
+# import pandas as pd
+from sqlalchemy import Integer, BLOB
 
 from sqlite_dataset import SQLiteDataset, Field, String, Float
 from sqlite_dataset.fields import DataTable
 
 
 class MyBaseIrisDataset(SQLiteDataset):
     __defaulttable__ = 'sentence'
@@ -58,7 +59,25 @@
 #     df.to_sql('iris', ds.connection)
 #     ds.connection.commit()
 #     # res = pd.read_sql(
 #     #     ds.get_table('iris').select(),
 #     #     ds.connection
 #     # )
 #     # print(res)
+
+
+class YelpAnnotationDataset(SQLiteDataset):
+    examples = DataTable(
+        record_id=Field(Integer, primary_key=True, autoincrement=True, tablename='examples'),
+        test=Field(String, default='test'),
+        id=Field(Integer),
+        review_id=Field(String),
+        text=Field(String),
+    )
+    annotations = DataTable(
+        record_id=Field(Integer, primary_key=True),
+        annotation=Field(BLOB)
+    )
+
+
+with YelpAnnotationDataset('yelp.db') as ds:
+    pass
```

### Comparing `sqlite_dataset-0.5.0/PKG-INFO` & `sqlite_dataset-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-dataset
-Version: 0.5.0
+Version: 0.5.1
 Summary: Use SQLite database to store datasets.
 Home-page: https://github.com/Mayazure/sqlite-dataset
 License: MIT
 Author: Jinshuai Ma
 Author-email: mayazureee@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

