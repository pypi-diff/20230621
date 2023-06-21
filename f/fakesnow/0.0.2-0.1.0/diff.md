# Comparing `tmp/fakesnow-0.0.2.tar.gz` & `tmp/fakesnow-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.0.2.tar", last modified: Wed Mar 15 05:13:52 2023, max compression
+gzip compressed data, was "fakesnow-0.1.0.tar", last modified: Wed Jun 21 02:35:59 2023, max compression
```

## Comparing `fakesnow-0.0.2.tar` & `fakesnow-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:13:52.749509 fakesnow-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-15 05:12:46.000000 fakesnow-0.0.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:13:52.745509 fakesnow-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:13:52.745509 fakesnow-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-15 05:12:46.000000 fakesnow-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-15 05:12:46.000000 fakesnow-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-15 05:12:46.000000 fakesnow-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-15 05:12:46.000000 fakesnow-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-15 05:12:46.000000 fakesnow-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-15 05:12:46.000000 fakesnow-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-15 05:12:46.000000 fakesnow-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-15 05:12:46.000000 fakesnow-0.0.2/Makefile-common.mk
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-15 05:13:52.749509 fakesnow-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-15 05:12:46.000000 fakesnow-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:13:52.745509 fakesnow-0.0.2/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-03-15 05:12:46.000000 fakesnow-0.0.2/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-15 05:12:46.000000 fakesnow-0.0.2/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-15 05:12:46.000000 fakesnow-0.0.2/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-03-15 05:12:46.000000 fakesnow-0.0.2/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-15 05:12:46.000000 fakesnow-0.0.2/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-15 05:12:46.000000 fakesnow-0.0.2/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-03-15 05:12:46.000000 fakesnow-0.0.2/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:13:52.749509 fakesnow-0.0.2/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-15 05:13:52.000000 fakesnow-0.0.2/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-15 05:13:52.000000 fakesnow-0.0.2/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 05:13:52.000000 fakesnow-0.0.2/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-15 05:13:52.000000 fakesnow-0.0.2/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-15 05:13:52.000000 fakesnow-0.0.2/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-15 05:12:46.000000 fakesnow-0.0.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-15 05:12:46.000000 fakesnow-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-15 05:12:46.000000 fakesnow-0.0.2/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 05:13:52.749509 fakesnow-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-15 05:12:46.000000 fakesnow-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 05:13:52.749509 fakesnow-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/patch_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-03-15 05:12:46.000000 fakesnow-0.0.2/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.426805 fakesnow-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 02:35:51.000000 fakesnow-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 02:35:51.000000 fakesnow-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-21 02:35:59.422805 fakesnow-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-21 02:35:51.000000 fakesnow-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.422805 fakesnow-0.1.0/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19240 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.422805 fakesnow-0.1.0/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-21 02:35:51.000000 fakesnow-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 02:35:59.426805 fakesnow-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 02:35:51.000000 fakesnow-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.422805 fakesnow-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_transforms.py
```

### Comparing `fakesnow-0.0.2/LICENSE` & `fakesnow-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.0.2/PKG-INFO` & `fakesnow-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.0.2
+Version: 0.1.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -30,32 +30,49 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: notebook
 License-File: LICENSE
 
 # fakesnow ❄️
 
-Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run Snowflake DB locally.
+Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
+
+## Install
+
+```
+pip install fakesnow
+```
 
 ## Usage
 
 ```python
 import fakesnow
 import snowflake.connector
 
 with fakesnow.patch():
     conn = snowflake.connector.connect()
 
     print(conn.cursor().execute("SELECT 'Hello fake world!'").fetchone())
 ```
 
-Standard imports (eg: `snowflake.connector.connect`) are patched. To patch additional imports, eg:
+The following imports are automatically patched:
+
+- `import snowflake.connector.connect`
+- `import  snowflake.connector.pandas_tools.write_pandas`
+
+To patch modules that use the `from ... import` syntax, manually specify them, eg: if _mymodule.py_ has the import:
 
 ```python
-with fakesnow.patch("mymodule.connect"):
+from snowflake.connector.pandas_tools import write_pandas
+```
+
+Then patch it using:
+
+```python
+with fakesnow.patch("mymodule.write_pandas"):
     ...
 ```
 
 pytest [fixtures](fakesnow/fixtures.py) are provided for testing. Example _conftest.py_:
 
 ```python
 from typing import Iterator
@@ -68,27 +85,44 @@
 @pytest.fixture(scope="session", autouse=True)
 def setup(_fakesnow_session: None) -> Iterator[None]:
     # the standard imports are now patched
     ...
     yield
 ```
 
+Or with `from ... import` patch targets:
+
+```python
+from typing import Iterator
+
+import fakesnow
+import pytest
+
+@pytest.fixture(scope="session", autouse=True)
+def _fakesnow_session() -> Iterator[None]:
+    with fakesnow.patch("mymodule.write_pandas"):
+        yield
+```
+
 ## Implementation coverage
 
 - [x] multiple databases
 - [x] cursors
 - [x] [get_result_batches()](https://docs.snowflake.com/en/user-guide/python-connector-api#get_result_batches)
 - [x] [write_pandas(..)](https://docs.snowflake.com/en/user-guide/python-connector-api#write_pandas)
 - [x] table comments
 - [x] [qmark binding](https://docs.snowflake.com/en/user-guide/python-connector-example#binding-data)
 - [ ] [access control](https://docs.snowflake.com/en/user-guide/security-access-control-overview)
 - [ ] standalone/out of process api/support for faking non-python connectors
 - [ ] [stored procedures](https://docs.snowflake.com/en/sql-reference/stored-procedures)
 
 Partial support
+
 - [x] date functions
 - [x] tags
 - [x] semi-structured data
 
+For more detail see [tests/test_fakes.py](tests/test_fakes.py)
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) to get started and develop in this repo.
```

### Comparing `fakesnow-0.0.2/README.md` & `fakesnow-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 # fakesnow ❄️
 
-Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run Snowflake DB locally.
+Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
+
+## Install
+
+```
+pip install fakesnow
+```
 
 ## Usage
 
 ```python
 import fakesnow
 import snowflake.connector
 
 with fakesnow.patch():
     conn = snowflake.connector.connect()
 
     print(conn.cursor().execute("SELECT 'Hello fake world!'").fetchone())
 ```
 
-Standard imports (eg: `snowflake.connector.connect`) are patched. To patch additional imports, eg:
+The following imports are automatically patched:
+
+- `import snowflake.connector.connect`
+- `import  snowflake.connector.pandas_tools.write_pandas`
+
+To patch modules that use the `from ... import` syntax, manually specify them, eg: if _mymodule.py_ has the import:
 
 ```python
-with fakesnow.patch("mymodule.connect"):
+from snowflake.connector.pandas_tools import write_pandas
+```
+
+Then patch it using:
+
+```python
+with fakesnow.patch("mymodule.write_pandas"):
     ...
 ```
 
 pytest [fixtures](fakesnow/fixtures.py) are provided for testing. Example _conftest.py_:
 
 ```python
 from typing import Iterator
@@ -34,27 +51,44 @@
 @pytest.fixture(scope="session", autouse=True)
 def setup(_fakesnow_session: None) -> Iterator[None]:
     # the standard imports are now patched
     ...
     yield
 ```
 
+Or with `from ... import` patch targets:
+
+```python
+from typing import Iterator
+
+import fakesnow
+import pytest
+
+@pytest.fixture(scope="session", autouse=True)
+def _fakesnow_session() -> Iterator[None]:
+    with fakesnow.patch("mymodule.write_pandas"):
+        yield
+```
+
 ## Implementation coverage
 
 - [x] multiple databases
 - [x] cursors
 - [x] [get_result_batches()](https://docs.snowflake.com/en/user-guide/python-connector-api#get_result_batches)
 - [x] [write_pandas(..)](https://docs.snowflake.com/en/user-guide/python-connector-api#write_pandas)
 - [x] table comments
 - [x] [qmark binding](https://docs.snowflake.com/en/user-guide/python-connector-example#binding-data)
 - [ ] [access control](https://docs.snowflake.com/en/user-guide/security-access-control-overview)
 - [ ] standalone/out of process api/support for faking non-python connectors
 - [ ] [stored procedures](https://docs.snowflake.com/en/sql-reference/stored-procedures)
 
 Partial support
+
 - [x] date functions
 - [x] tags
 - [x] semi-structured data
 
+For more detail see [tests/test_fakes.py](tests/test_fakes.py)
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) to get started and develop in this repo.
```

### Comparing `fakesnow-0.0.2/fakesnow/__init__.py` & `fakesnow-0.1.0/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.0.2/fakesnow/checks.py` & `fakesnow-0.1.0/fakesnow/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
     if not (node := expression.find(exp.Table)):
         return False, False
 
     assert node.parent, f"No parent for table expression {node.sql()}"
 
     if (parent_kind := node.parent.args.get("kind")) and isinstance(parent_kind, str):
-
         if parent_kind.upper() == "DATABASE":
             # "CREATE/DROP DATABASE"
             no_database = False
             no_schema = False
         elif parent_kind.upper() == "SCHEMA":
             # "CREATE/DROP SCHEMA"
             no_database = not node.args.get("db")
@@ -49,15 +48,14 @@
 
     elif (
         node.parent.key == "use"
         and (parent_kind := node.parent.args.get("kind"))
         and isinstance(parent_kind, exp.Var)
         and parent_kind.name
     ):
-
         if parent_kind.name.upper() == "DATABASE":
             # "USE DATABASE"
             no_database = False
             no_schema = False
         elif parent_kind.name.upper() == "SCHEMA":
             # "USE SCHEMA"
             no_database = not node.args.get("db")
```

### Comparing `fakesnow-0.0.2/fakesnow/expr.py` & `fakesnow-0.1.0/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.0.2/fakesnow/fakes.py` & `fakesnow-0.1.0/fakesnow/fakes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import re
 from string import Template
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, Iterable, Iterator, Literal, Optional, Sequence, Type, Union, cast
+from typing import Any, Iterable, Iterator, Literal, Optional, Sequence, Type, Union, cast
 
 import duckdb
+import pandas as pd
 import pyarrow
 import pyarrow.lib
 import pyarrow.types
 import snowflake.connector.errors
 import sqlglot
 from duckdb import DuckDBPyConnection
 from snowflake.connector.cursor import DictCursor, ResultMetadata, SnowflakeCursor
@@ -17,17 +18,14 @@
 from sqlglot import exp, parse_one
 from typing_extensions import Self
 
 import fakesnow.checks as checks
 import fakesnow.expr as expr
 import fakesnow.transforms as transforms
 
-if TYPE_CHECKING:
-    import pandas as pd
-
 SCHEMA_UNSET = "schema_unset"
 
 # use ext prefix in columns to disambiguate when joining with information_schema.tables
 SQL_CREATE_INFORMATION_SCHEMA_TABLES_EXT = Template(
     """
 create table ${catalog}.information_schema.tables_ext (
     ext_table_catalog varchar,
@@ -54,14 +52,15 @@
             duck_conn (DuckDBPyConnection): DuckDB connection.
             use_dict_result (bool, optional): If true rows are returned as dicts otherwise they
                 are returned as tuples. Defaults to False.
         """
         self._conn = conn
         self._duck_conn = duck_conn
         self._use_dict_result = use_dict_result
+        self._last_sql = None
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]] = ...,
@@ -75,71 +74,46 @@
 
         Takes the same arguments as execute
 
         Returns:
             list[ResultMetadata]: _description_
         """
 
-        # fmt: off
-        def as_result_metadata(column_name: str, column_type: str, _: str) -> ResultMetadata:
-            # see https://docs.snowflake.com/en/user-guide/python-connector-api.html#type-codes
-            # and https://arrow.apache.org/docs/python/api/datatypes.html#type-checking
-            # type ignore because of https://github.com/snowflakedb/snowflake-connector-python/issues/1423
-            if column_type == "INTEGER":
-                return ResultMetadata(
-                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True                    # type: ignore # noqa: E501
-                )
-            elif column_type.startswith("DECIMAL"):
-                match = re.search(r'\((\d+),(\d+)\)', column_type)
-                if match:
-                    precision = int(match[1])
-                    scale = int(match[2])
-                else:
-                    precision = scale = None
-                return ResultMetadata(
-                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=precision, scale=scale, is_nullable=True # type: ignore # noqa: E501
-                )
-            elif column_type == "VARCHAR":
-                return ResultMetadata(
-                    name=column_name, type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True   # type: ignore # noqa: E501
-                )
-            elif column_type == "FLOAT":
-                return ResultMetadata(
-                    name=column_name, type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True       # type: ignore # noqa: E501
-                )
-            elif column_type == "TIMESTAMP":
-                return ResultMetadata(
-                    name=column_name, type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True             # type: ignore # noqa: E501
-                )
-            else:
-                # TODO handle more types
-                raise NotImplementedError(f"for column type {column_type}")
-
-        # fmt: on
-
         describe = transforms.as_describe(parse_one(command, read="snowflake"))
         self.execute(describe, *args, **kwargs)
+        return FakeSnowflakeCursor._describe_as_result_metadata(self._duck_conn.fetchall())  # noqa: SLF001
 
-        meta = [
-            as_result_metadata(column_name, column_type, null)
-            for (column_name, column_type, null, _, _, _) in self._duck_conn.fetchall()
-        ]
+    @property
+    def description(self) -> list[ResultMetadata]:
+        # use a cursor to avoid destroying an unfetched result on the main connection
+        with self._duck_conn.cursor() as cur:
+            assert self._conn.database, "Not implemented when database is None"
+            assert self._conn.schema, "Not implemented when database is None"
+
+            # match database and schema used on the main connection
+            cur.execute(f"SET SCHEMA = '{self._conn.database}.{self._conn.schema}'")
+            cur.execute(f"DESCRIBE {self._last_sql}")
+            meta = FakeSnowflakeCursor._describe_as_result_metadata(cur.fetchall())  # noqa: SLF001
 
-        return meta
+        return meta  # type: ignore see https://github.com/duckdb/duckdb/issues/7816
 
     def execute(
         self,
         command: str | exp.Expression,
         params: Sequence[Any] | dict[Any, Any] | None = None,
         *args: Any,
         **kwargs: Any,
     ) -> FakeSnowflakeCursor:
         self._arrow_table = None
 
-        expression = command if isinstance(command, exp.Expression) else parse_one(command, read="snowflake")
+        if isinstance(command, exp.Expression):
+            expression = command
+        else:
+            expression = parse_one(self._rewrite_params(command, params), read="snowflake")
+
         cmd = expr.key_command(expression)
 
         no_database, no_schema = checks.is_unqualified_table_expression(expression)
 
         if no_database and not self._conn.database_set:
             raise snowflake.connector.errors.ProgrammingError(
                 msg=f"Cannot perform {cmd}. This session does not have a current database. Call 'USE DATABASE', or use a qualified name.",  # noqa: E501
@@ -164,20 +138,22 @@
             .transform(transforms.regex)
             .transform(transforms.semi_structured_types)
             .transform(transforms.parse_json)
             .transform(transforms.indices_to_array)
             .transform(transforms.indices_to_object)
             .transform(transforms.values_columns)
             .transform(transforms.to_date)
+            .transform(transforms.object_construct)
         )
 
         sql = transformed.sql(dialect="duckdb")
 
         if cmd != "COMMENT TABLE":
             try:
+                self._last_sql = sql
                 self._duck_conn.execute(sql, params)
             except duckdb.BinderException as e:
                 msg = e.args[0]
                 raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2043, sqlstate="02000") from None
             except duckdb.CatalogException as e:
                 # minimal processing to make it look like a snowflake exception, message content may differ
                 msg = cast(str, e.args[0]).split("\n")[0]
@@ -208,14 +184,33 @@
                 ON CONFLICT (ext_table_catalog, ext_table_schema, ext_table_name)
                 DO UPDATE SET comment = excluded.comment
                 """
             )
 
         return self
 
+    def executemany(
+        self,
+        command: str,
+        seqparams: Sequence[Any] | dict[str, Any],
+        **kwargs: Any,
+    ) -> FakeSnowflakeCursor:
+        if isinstance(seqparams, dict):
+            # see https://docs.snowflake.com/en/developer-guide/python-connector/python-connector-api
+            raise NotImplementedError("dict params not supported yet")
+
+        # TODO: support insert optimisations
+        # the snowflake connector will optimise inserts into a single query
+        # unless num_statements != 1 .. but for simplicity we execute each
+        # query one by one, which means the response differs
+        for p in seqparams:
+            self.execute(command, p)
+
+        return self
+
     def fetchall(self) -> list[tuple] | list[dict]:
         if self._use_dict_result:
             return self._duck_conn.fetch_arrow_table().to_pylist()
         else:
             return self._duck_conn.fetchall()
 
     def fetch_pandas_all(self, **kwargs: dict[str, Any]) -> pd.DataFrame:
@@ -233,27 +228,96 @@
 
         try:
             return self._arrow_table.take([self._arrow_table_fetch_one_index]).to_pylist()
         except pyarrow.lib.ArrowIndexError:
             return None
 
     def get_result_batches(self) -> list[ResultBatch] | None:
-        # chunk_size is multiple of 1024
+        # rows_per_batch is approximate
         # see https://github.com/duckdb/duckdb/issues/4755
-        reader = self._duck_conn.fetch_record_batch(chunk_size=1024)
+        reader = self._duck_conn.fetch_record_batch(rows_per_batch=1000)
 
         batches = []
         while True:
             try:
-                batches.append(DuckResultBatch(self._use_dict_result, reader.read_next_batch()))
+                batches.append(FakeResultBatch(self._use_dict_result, reader.read_next_batch()))
             except StopIteration:
                 break
 
         return batches
 
+    @staticmethod
+    def _describe_as_result_metadata(describe_results: list) -> list[ResultMetadata]:
+        # fmt: off
+        def as_result_metadata(column_name: str, column_type: str, _: str) -> ResultMetadata:
+            # see https://docs.snowflake.com/en/user-guide/python-connector-api.html#type-codes
+            # and https://arrow.apache.org/docs/python/api/datatypes.html#type-checking
+            # type ignore because of https://github.com/snowflakedb/snowflake-connector-python/issues/1423
+            if column_type == "INTEGER":
+                return ResultMetadata(
+                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True                    # type: ignore # noqa: E501
+                )
+            elif column_type.startswith("DECIMAL"):
+                match = re.search(r'\((\d+),(\d+)\)', column_type)
+                if match:
+                    precision = int(match[1])
+                    scale = int(match[2])
+                else:
+                    precision = scale = None
+                return ResultMetadata(
+                    name=column_name, type_code=0, display_size=None, internal_size=None, precision=precision, scale=scale, is_nullable=True # type: ignore # noqa: E501
+                )
+            elif column_type == "VARCHAR":
+                # TODO: fetch internal_size from varchar size
+                return ResultMetadata(
+                    name=column_name, type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True   # type: ignore # noqa: E501
+                )
+            elif column_type == "FLOAT":
+                return ResultMetadata(
+                    name=column_name, type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True       # type: ignore # noqa: E501
+                )
+            elif column_type == "BOOLEAN":
+                return ResultMetadata(
+                    name=column_name, type_code=13, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True      # type: ignore # noqa: E501
+                )
+            elif column_type == "DATE":
+                return ResultMetadata(
+                    name=column_name, type_code=3, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True       # type: ignore # noqa: E501
+                )
+            elif column_type in ["TIMESTAMP", "TIMESTAMP_NS"]:
+                return ResultMetadata(
+                    name=column_name, type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True             # type: ignore # noqa: E501
+                )
+            else:
+                # TODO handle more types
+                raise NotImplementedError(f"for column type {column_type}")
+
+        # fmt: on
+
+        meta = [
+            as_result_metadata(column_name, column_type, null)
+            for (column_name, column_type, null, _, _, _) in describe_results
+        ]
+        return meta
+
+    def _rewrite_params(
+        self,
+        command: str,
+        params: Sequence[Any] | dict[Any, Any] | None = None,
+    ) -> str:
+        if isinstance(params, dict):
+            # see https://docs.snowflake.com/en/developer-guide/python-connector/python-connector-api
+            raise NotImplementedError("dict params not supported yet")
+
+        if params and self._conn._paramstyle in ("pyformat", "format"):  # noqa: SLF001
+            # duckdb uses question mark style params
+            return command.replace("%s", "?")
+
+        return command
+
 
 class FakeSnowflakeConnection:
     def __init__(
         self,
         duck_conn: DuckDBPyConnection,
         database: Optional[str] = None,
         schema: Optional[str] = None,
@@ -343,29 +407,34 @@
         cursors = [
             self.cursor(cursor_class).execute(e.sql(dialect="snowflake"))
             for e in sqlglot.parse(sql_text, read="snowflake")
             if e
         ]
         return cursors if return_cursors else []
 
-    def insert_df(
+    def _insert_df(
         self, df: pd.DataFrame, table_name: str, database: str | None = None, schema: str | None = None
     ) -> int:
-        self._duck_conn.execute(f"INSERT INTO {table_name} SELECT * FROM df")
+        # dicts in dataframes are written as parquet structs, and snowflake loads parquet structs as json strings
+        # whereas duckdb loads them as a struct, so we convert them to json here
+        cols = [f"TO_JSON({c})" if isinstance(df[c][0], dict) else c for c in df.columns]
+        cols = ",".join(cols)
+
+        self._duck_conn.execute(f"INSERT INTO {table_name}({','.join(df.columns.to_list())}) SELECT {cols} FROM df")
         return self._duck_conn.fetchall()[0][0]
 
 
-class DuckResultBatch(ResultBatch):
+class FakeResultBatch(ResultBatch):
     def __init__(self, use_dict_result: bool, batch: pyarrow.RecordBatch):
         self._use_dict_result = use_dict_result
         self._batch = batch
 
     def create_iter(
         self, **kwargs: dict[str, Any]
-    ) -> (Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[pyarrow.Table] | Iterator[pd.DataFrame]):
+    ) -> Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[pyarrow.Table] | Iterator[pd.DataFrame]:
         if self._use_dict_result:
             return iter(self._batch.to_pylist())
 
         return iter(tuple(d.values()) for d in self._batch.to_pylist())
 
     @property
     def rowcount(self) -> int:
@@ -412,14 +481,14 @@
     quote_identifiers: bool = True,
     auto_create_table: bool = False,
     create_temp_table: bool = False,
     overwrite: bool = False,
     table_type: Literal["", "temp", "temporary", "transient"] = "",
     **kwargs: Any,
 ) -> WritePandasResult:
-    count = conn.insert_df(df, table_name, database, schema)
+    count = conn._insert_df(df, table_name, database, schema)  # noqa: SLF001
 
     # mocks https://docs.snowflake.com/en/sql-reference/sql/copy-into-table.html#output
     mock_copy_results = [("fakesnow/file0.txt", "LOADED", count, count, 1, 0, None, None, None, None)]
 
     # return success
     return (True, len(mock_copy_results), count, mock_copy_results)
```

### Comparing `fakesnow-0.0.2/fakesnow/transforms.py` & `fakesnow-0.1.0/fakesnow/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     """
 
     if isinstance(expression, exp.Create):
         comment = None
         if props := cast(exp.Properties, expression.args.get("properties")):
             other_props = []
             for p in props.expressions:
-                if isinstance(p, exp.SchemaCommentProperty) and (isinstance(p.this, (exp.Literal, exp.Var))):
+                if isinstance(p, exp.SchemaCommentProperty) and (isinstance(p.this, (exp.Literal, exp.Identifier))):
                     comment = p.this.this
                 else:
                     other_props.append(p)
 
             new = expression.copy()
             new_props: exp.Properties = new.args["properties"]
             new_props.args["expressions"] = other_props
@@ -140,15 +140,15 @@
         >>> sqlglot.parse_one("SELECT myarray[0] FROM table1").transform(indices_to_array).sql()
         'SELECT myarray[1] FROM table1'
     Args:
         expression (exp.Expression): the expression that will be transformed.
 
     Returns:
         exp.Expression: The transformed expression.
-    """  # noqa: E501
+    """
     if (
         isinstance(expression, exp.Bracket)
         and len(expression.expressions) == 1
         and (index := expression.expressions[0])
         and isinstance(index, exp.Literal)
         and index.this
         and not index.is_string
@@ -214,24 +214,48 @@
         and (tbl_exp := expression.find(exp.Table))
         and tbl_exp.name.upper() == "TABLES"
         and tbl_exp.db.upper() == "INFORMATION_SCHEMA"
     ):
         return expression.join(
             "information_schema.tables_ext",
             on=(
-                "tables.table_catalog = tables_ext.ext_table_catalog",
-                "tables.table_schema = tables_ext.ext_table_schema",
-                "tables.table_name = tables_ext.ext_table_name",
+                """
+                tables.table_catalog = tables_ext.ext_table_catalog AND
+                tables.table_schema = tables_ext.ext_table_schema AND
+                tables.table_name = tables_ext.ext_table_name
+                """
             ),
             join_type="left",
         )
 
     return expression
 
 
+def object_construct(expression: exp.Expression) -> exp.Expression:
+    """Convert object_construct to return a json string
+
+    Because internally snowflake stores OBJECT types as a json string.
+
+    Example:
+        >>> import sqlglot
+        >>> sqlglot.parse_one("SELECT OBJECT_CONSTRUCT('a',1,'b','BBBB', 'c',null)", read="snowflake").transform(object_construct).sql(dialect="duckdb")
+        "SELECT TO_JSON({'a': 1, 'b': 'BBBB', 'c': NULL})"
+    Args:
+        expression (exp.Expression): the expression that will be transformed.
+
+    Returns:
+        exp.Expression: The transformed expression.
+    """  # noqa: E501
+
+    if isinstance(expression, exp.Struct):
+        return exp.Anonymous(this="TO_JSON", expressions=[expression])
+
+    return expression
+
+
 def parse_json(expression: exp.Expression) -> exp.Expression:
     """Convert parse_json() to json().
 
     Example:
         >>> import sqlglot
         >>> sqlglot.parse_one("insert into table1 (name) select parse_json('{}')").transform(parse_json).sql()
         "CREATE TABLE table1 (name JSON)"
@@ -385,29 +409,31 @@
     """Convert to_date() to a cast.
 
     See https://docs.snowflake.com/en/sql-reference/functions/to_date
 
     Example:
         >>> import sqlglot
         >>> sqlglot.parse_one("SELECT to_date(to_timestamp(0))").transform(to_date).sql()
-        "SELECT CAST(TO_TIMESTAMP(0) AS DATE)"
+        "SELECT CAST(DATE_TRUNC('day', TO_TIMESTAMP(0)) AS DATE)"
     Args:
         expression (exp.Expression): the expression that will be transformed.
 
     Returns:
         exp.Expression: The transformed expression.
     """
 
     if (
         isinstance(expression, exp.Anonymous)
         and isinstance(expression.this, str)
         and expression.this.upper() == "TO_DATE"
     ):
         return exp.Cast(
-            this=expression.expressions[0],
+            # add datetrunc to handle timestamp_ns (aka timestamp(9)) columns
+            # and avoid https://github.com/duckdb/duckdb/issues/7672
+            this=exp.DateTrunc(unit=exp.Literal(this="day", is_string=True), this=expression.expressions[0]),
             to=exp.DataType(this=exp.DataType.Type.DATE, nested=False, prefix=False),
         )
     return expression
 
 
 def semi_structured_types(expression: exp.Expression) -> exp.Expression:
     """Convert OBJECT, ARRAY, and VARIANT types to duckdb compatible types.
```

### Comparing `fakesnow-0.0.2/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.1.0/fakesnow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.0.2
+Version: 0.1.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -30,32 +30,49 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: notebook
 License-File: LICENSE
 
 # fakesnow ❄️
 
-Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run Snowflake DB locally.
+Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
+
+## Install
+
+```
+pip install fakesnow
+```
 
 ## Usage
 
 ```python
 import fakesnow
 import snowflake.connector
 
 with fakesnow.patch():
     conn = snowflake.connector.connect()
 
     print(conn.cursor().execute("SELECT 'Hello fake world!'").fetchone())
 ```
 
-Standard imports (eg: `snowflake.connector.connect`) are patched. To patch additional imports, eg:
+The following imports are automatically patched:
+
+- `import snowflake.connector.connect`
+- `import  snowflake.connector.pandas_tools.write_pandas`
+
+To patch modules that use the `from ... import` syntax, manually specify them, eg: if _mymodule.py_ has the import:
 
 ```python
-with fakesnow.patch("mymodule.connect"):
+from snowflake.connector.pandas_tools import write_pandas
+```
+
+Then patch it using:
+
+```python
+with fakesnow.patch("mymodule.write_pandas"):
     ...
 ```
 
 pytest [fixtures](fakesnow/fixtures.py) are provided for testing. Example _conftest.py_:
 
 ```python
 from typing import Iterator
@@ -68,27 +85,44 @@
 @pytest.fixture(scope="session", autouse=True)
 def setup(_fakesnow_session: None) -> Iterator[None]:
     # the standard imports are now patched
     ...
     yield
 ```
 
+Or with `from ... import` patch targets:
+
+```python
+from typing import Iterator
+
+import fakesnow
+import pytest
+
+@pytest.fixture(scope="session", autouse=True)
+def _fakesnow_session() -> Iterator[None]:
+    with fakesnow.patch("mymodule.write_pandas"):
+        yield
+```
+
 ## Implementation coverage
 
 - [x] multiple databases
 - [x] cursors
 - [x] [get_result_batches()](https://docs.snowflake.com/en/user-guide/python-connector-api#get_result_batches)
 - [x] [write_pandas(..)](https://docs.snowflake.com/en/user-guide/python-connector-api#write_pandas)
 - [x] table comments
 - [x] [qmark binding](https://docs.snowflake.com/en/user-guide/python-connector-example#binding-data)
 - [ ] [access control](https://docs.snowflake.com/en/user-guide/security-access-control-overview)
 - [ ] standalone/out of process api/support for faking non-python connectors
 - [ ] [stored procedures](https://docs.snowflake.com/en/sql-reference/stored-procedures)
 
 Partial support
+
 - [x] date functions
 - [x] tags
 - [x] semi-structured data
 
+For more detail see [tests/test_fakes.py](tests/test_fakes.py)
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) to get started and develop in this repo.
```

### Comparing `fakesnow-0.0.2/pyproject.toml` & `fakesnow-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run Snowflake DB locally."
-dynamic = ["version"]
+version = "0.1.0"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
-    "duckdb~=0.7.0",
+    "duckdb~=0.8.0",
     # include the pandas extra to get compatible version of pyarrow
     "snowflake-connector-python[pandas]",
-    "sqlglot~=11.3.6",
+    "sqlglot~=15.0.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/tekumara/fakesnow"
 
 [project.optional-dependencies]
 dev = [
-    "black~=22.12",
+    "black~=23.3",
     "build~=0.10",
-    "docformatter~=1.5",
-    # exclude 3.0.1 because of https://github.com/snowflakedb/snowflake-connector-python/issues/1464
-    "snowflake-connector-python!=3.0.1",
     # include the secure-local-storage extra for token caching
     "snowflake-connector-python[secure-local-storage]",
-    "pandas",
-    "pre-commit~=3.0",
-    "pytest~=7.2",
-    "ruff~=0.0.235",
+    "pre-commit~=3.2",
+    "pytest~=7.3",
+    "ruff~=0.0.263",
     "twine~=4.0",
 ]
 # for debugging, see https://duckdb.org/docs/guides/python/jupyter.html
 notebook = ["duckdb-engine", "ipykernel", "jupysql", "snowflake-sqlalchemy"]
 
 [build-system]
-requires = ["setuptools~=67.6", "setuptools_scm[toml]~=7.1", "wheel~=0.40"]
+requires = ["setuptools~=67.6", "wheel~=0.40"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["tests*"]
 
-# pyproject.toml
-[tool.setuptools_scm]
-
 # use PyCharm default line length of 120
 [tool.black]
 line-length = 120
 
 [tool.docformatter]
 pre-summary-newline = true
 recursive = true
@@ -69,29 +62,35 @@
     "ANN",
     # pep8-naming
     "N",
     # bugbear
     "B",
     # isort
     "I",
+    # flake8-unused-arguments - disabled because our fakes don't use all arguments
+    # "ARG",
+    # flake8-self
+    "SLF",
+    # ruff-specific
+    "RUF",
 ]
 ignore = [
     # allow untyped self and cls args, and no return type from dunder methods
     "ANN101",
     "ANN102",
     "ANN204",
     # allow == True because pandas dataframes overload equality
     "E712",
     # only relevant for python >= 3.10
     "B905",
 ]
 # first-party imports for sorting
 src = ["."]
-
 fix = true
+show-fixes = true
 
 [tool.ruff.per-file-ignores]
 # test functions don't need return types
 "tests/*" = ["ANN201", "ANN202"]
 
 [tool.ruff.flake8-annotations]
 # allow *args: Any, **kwargs: Any
```

### Comparing `fakesnow-0.0.2/tests/test_checks.py` & `fakesnow-0.1.0/tests/test_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,42 +8,38 @@
 
     assert is_unqualified_table_expression(sqlglot.parse_one("SELECT * FROM jaffles.customers")) == (True, False)
 
     assert is_unqualified_table_expression(sqlglot.parse_one("SELECT * FROM marts.jaffles.customers")) == (False, False)
 
 
 def test_check_unqualified_create_table() -> None:
-
     assert is_unqualified_table_expression(sqlglot.parse_one("CREATE TABLE customers (ID INT)")) == (True, True)
 
     assert is_unqualified_table_expression(sqlglot.parse_one("CREATE TABLE jaffles.customers (ID INT)")) == (
         True,
         False,
     )
 
 
 def test_check_unqualified_drop_table() -> None:
-
     assert is_unqualified_table_expression(sqlglot.parse_one("DROP TABLE customers")) == (True, True)
 
     assert is_unqualified_table_expression(sqlglot.parse_one("DROP TABLE jaffles.customers")) == (
         True,
         False,
     )
 
 
 def test_check_unqualified_schema() -> None:
-
     # assert is_unqualified_table_expression(sqlglot.parse_one("CREATE SCHEMA jaffles")) == (True, False)
 
     # assert is_unqualified_table_expression(sqlglot.parse_one("CREATE SCHEMA marts.jaffles")) ==  (False, False)
 
     assert is_unqualified_table_expression(sqlglot.parse_one("USE SCHEMA jaffles")) == (True, False)
 
     assert is_unqualified_table_expression(sqlglot.parse_one("USE SCHEMA marts.jaffles")) == (False, False)
 
 
 def test_check_unqualified_database() -> None:
-
     assert is_unqualified_table_expression(sqlglot.parse_one("CREATE DATABASE marts")) == (False, False)
 
     assert is_unqualified_table_expression(sqlglot.parse_one("USE DATABASE marts")) == (False, False)
```

### Comparing `fakesnow-0.0.2/tests/test_expr.py` & `fakesnow-0.1.0/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.0.2/tests/test_fakes.py` & `fakesnow-0.1.0/tests/test_fakes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import datetime
+import json
 
 import pandas as pd
 import pytest
 import snowflake.connector
 import snowflake.connector.cursor
 import snowflake.connector.pandas_tools
 from pandas.testing import assert_frame_equal
 
 
 def test_binding_default_paramstyle(conn: snowflake.connector.SnowflakeConnection):
-    assert conn._paramstyle == "pyformat"
+    assert conn._paramstyle == "pyformat"  # noqa: SLF001
+    with conn.cursor() as cur:
+        cur.execute("create table customers (ID int, FIRST_NAME varchar, ACTIVE boolean)")
+        cur.execute("insert into customers values (%s, %s, %s)", (1, "Jenny", True))
+        cur.execute("select * from customers")
+        assert cur.fetchall() == [(1, "Jenny", True)]
 
 
 def test_binding_qmark(conn: snowflake.connector.SnowflakeConnection):
-    conn._paramstyle = "qmark"
+    conn._paramstyle = "qmark"  # noqa: SLF001
     with conn.cursor() as cur:
         cur.execute("create table customers (ID int, FIRST_NAME varchar, ACTIVE boolean)")
         cur.execute("insert into customers values (?, ?, ?)", (1, "Jenny", True))
         cur.execute("select * from customers")
         assert cur.fetchall() == [(1, "Jenny", True)]
 
 
@@ -29,15 +35,14 @@
     with snowflake.connector.connect(database="db1", schema="schema1"):
         # connects again and reuses db1 and schema1
         pass
 
 
 def test_connect_without_database(_fakesnow_no_auto_create: None):
     with snowflake.connector.connect() as conn, conn.cursor() as cur:
-
         with pytest.raises(snowflake.connector.errors.ProgrammingError) as excinfo:
             cur.execute("SELECT * FROM customers")
 
         # actual snowflake error message is:
         #
         # 002003 (42S02): SQL compilation error:
         # Object 'CUSTOMERS' does not exist or not authorized.
@@ -127,15 +132,14 @@
         cur.execute("select id, first_name, last_name from customers")
         assert cur.fetchall() == [(1, "Jenny", "P"), (2, "Jasper", "M")]
 
 
 def test_connect_with_non_existent_db_or_schema(_fakesnow_no_auto_create: None):
     # can connect with db that doesn't exist
     with snowflake.connector.connect(database="marts") as conn, conn.cursor() as cur:
-
         # but no valid database set
         with pytest.raises(snowflake.connector.errors.ProgrammingError) as excinfo:
             cur.execute("create table foobar (i int)")
 
         assert (
             "090105 (22000): Cannot perform CREATE TABLE. This session does not have a current database. Call 'USE DATABASE', or use a qualified name."  # noqa: E501
             in str(excinfo.value)
@@ -144,15 +148,14 @@
         # database still present on connection
         assert conn.database == "MARTS"
 
         cur.execute("CREATE database marts")
 
     # can connect with schema that doesn't exist
     with snowflake.connector.connect(database="marts", schema="jaffles") as conn, conn.cursor() as cur:
-
         # but no valid schema set
         with pytest.raises(snowflake.connector.errors.ProgrammingError) as excinfo:
             cur.execute("create table foobar (i int)")
 
         assert (
             "090106 (22000): Cannot perform CREATE TABLE. This session does not have a current schema. Call 'USE SCHEMA', or use a qualified name."  # noqa: E501
             in str(excinfo.value)
@@ -168,37 +171,66 @@
 
         assert cur.fetchall() == [
             {"current_database()": "DB1", "current_schema()": "SCHEMA1"},
         ]
 
 
 def test_describe(cur: snowflake.connector.cursor.SnowflakeCursor):
-    cur.execute("create table customers (ID int, CNAME varchar, AMOUNT decimal(10,2), PCT real, UPDATE_AT timestamp)")
-    metadata = cur.describe("select * from customers")
-
+    cur.execute(
+        """
+        create table customers (
+            ID int, CNAME varchar, AMOUNT decimal(10,2), PCT real, ACTIVE boolean,
+            UPDATE_AT timestamp, UPDATE_AT_NTZ timestamp_ntz(9), INSERTIONDATE DATE
+        )
+        """
+    )
     # fmt: off
-    assert metadata == [
+    expected_metadata = [
+        snowflake.connector.cursor.ResultMetadata(
+            name="ID", type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True                  # type: ignore # noqa: E501
+        ),
         snowflake.connector.cursor.ResultMetadata(
-            name="ID", type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True              # type: ignore # noqa: E501
+            name="CNAME", type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True,     # type: ignore # noqa: E501
         ),
         snowflake.connector.cursor.ResultMetadata(
-            name="CNAME", type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True, # type: ignore # noqa: E501
+            name="AMOUNT", type_code=0, display_size=None, internal_size=None, precision=10, scale=2, is_nullable=True,             # type: ignore # noqa: E501
         ),
         snowflake.connector.cursor.ResultMetadata(
-            name="AMOUNT", type_code=0, display_size=None, internal_size=None, precision=10, scale=2, is_nullable=True,         # type: ignore # noqa: E501
+            name="PCT", type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True,           # type: ignore # noqa: E501
         ),
         snowflake.connector.cursor.ResultMetadata(
-            name="PCT", type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True,       # type: ignore # noqa: E501
+            name="ACTIVE", type_code=13, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True,       # type: ignore # noqa: E501
         ),
         snowflake.connector.cursor.ResultMetadata(
-            name='UPDATE_AT', type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True        # type: ignore # noqa: E501
+            name='UPDATE_AT', type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True            # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name='UPDATE_AT_NTZ', type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True        # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name='INSERTIONDATE', type_code=3, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True  # type: ignore # noqa: E501
         ),
     ]
     # fmt: on
 
+    assert cur.describe("select * from customers") == expected_metadata
+
+    cur.execute("select * from customers")
+    assert cur.description == expected_metadata
+
+
+def test_executemany(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
+
+    customers = [(1, "Jenny", "P"), (2, "Jasper", "M")]
+    cur.executemany("insert into customers (id, first_name, last_name) values (%s,%s,%s)", customers)
+
+    cur.execute("select id, first_name, last_name from customers")
+    assert cur.fetchall() == customers
+
 
 def test_execute_string(conn: snowflake.connector.SnowflakeConnection):
     [_, cur2] = conn.execute_string(
         """ create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar);
             select count(*) customers """
     )
     assert [(1,)] == cur2.fetchall()
@@ -299,14 +331,26 @@
 
 
 def test_non_existent_table_throws_snowflake_exception(cur: snowflake.connector.cursor.SnowflakeCursor):
     with pytest.raises(snowflake.connector.errors.ProgrammingError) as _:
         cur.execute("select * from this_table_does_not_exist")
 
 
+def test_object_construct(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute("SELECT OBJECT_CONSTRUCT('a',1,'b','BBBB', 'c',null)")
+
+    # TODO: strip null within duckdb via python UDF
+    def strip_none_values(d: dict) -> dict:
+        return {k: v for k, v in d.items() if v}
+
+    result = cur.fetchone()
+    assert isinstance(result, tuple)
+    assert strip_none_values(json.loads(result[0])) == json.loads('{\n  "a": 1,\n  "b": "BBBB"\n}')
+
+
 def test_regex(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("select regexp_replace('abc123', '\\\\D', '')")
     assert cur.fetchone() == ("123",)
 
 
 def test_schema_create_and_use(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create schema jaffles")
@@ -321,27 +365,27 @@
     cur.execute("create schema jaffles")
     cur.execute("create table jaffles.customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
     # dropping schema drops its contents
     cur.execute("drop schema jaffles")
 
 
 def test_semi_structured_types(cur: snowflake.connector.cursor.SnowflakeCursor):
-    cur.execute("create table semi (emails array, name object, notes variant)")
+    cur.execute("create table semis (emails array, name object, notes variant)")
     cur.execute(
-        """insert into semi(emails, name, notes) SELECT [1, 2], parse_json('{"k": "v1"}'), parse_json('["foo"]')"""
+        """insert into semis(emails, name, notes) SELECT [1, 2], parse_json('{"k": "v1"}'), parse_json('["foo"]')"""
     )
     cur.execute(
-        """insert into semi(emails, name, notes) VALUES ([3,4], parse_json('{"k": "v2"}'), parse_json('["bar"]'))"""  # noqa: E501
+        """insert into semis(emails, name, notes) VALUES ([3,4], parse_json('{"k": "v2"}'), parse_json('["bar"]'))"""  # noqa: E501
     )
 
-    cur.execute("select emails[0] from semi")
+    cur.execute("select emails[0] from semis")
     # returned as strings, because the underlying type is JSON (duckdb) / VARIANT (snowflake)
     assert cur.fetchall() == [("1",), ("3",)]
 
-    cur.execute("select name['k'] from semi")
+    cur.execute("select name['k'] from semis")
     # returned as json strings, because the underlying type is JSON (duckdb) / VARIANT (snowflake)
     assert cur.fetchall() == [('"v1"',), ('"v2"',)]
 
 
 def test_table_comments(cur: snowflake.connector.cursor.SnowflakeCursor):
     def read_comment() -> str:
         cur.execute(
@@ -366,16 +410,16 @@
 
 def test_timestamp(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("SELECT to_timestamp(0)")
     assert cur.fetchall() == [(datetime.datetime(1970, 1, 1, 0, 0),)]
 
 
 def test_timestamp_to_date(cur: snowflake.connector.cursor.SnowflakeCursor):
-    cur.execute("SELECT to_date(to_timestamp(0))")
-    assert cur.fetchall() == [(datetime.date(1970, 1, 1),)]
+    cur.execute("SELECT to_date(to_timestamp(0)), to_date(cast(to_timestamp(0) as timestamp(9)))")
+    assert cur.fetchall() == [(datetime.date(1970, 1, 1), datetime.date(1970, 1, 1))]
 
 
 def test_unquoted_identifiers_are_upper_cased(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor(snowflake.connector.cursor.DictCursor) as cur:
         cur.execute("create table customers (id int, first_name varchar, last_name varchar)")
         cur.execute("insert into customers values (1, 'Jenny', 'P')")
         cur.execute("select first_name, first_name as fname from customers")
@@ -391,15 +435,14 @@
         rows = [row for batch in batches for row in batch]
         assert rows == [
             {"FIRST_NAME": "Jenny", "FNAME": "Jenny"},
         ]
 
 
 def test_use_invalid_schema(_fakesnow: None):
-
     # database will be created but not schema
     with snowflake.connector.connect(database="marts") as conn, conn.cursor() as cur:
         with pytest.raises(snowflake.connector.errors.ProgrammingError) as _:
             cur.execute("use schema this_does_not_exist")
 
         # assert (
         #     "002043 (02000): SQL compilation error:\nObject does not exist, or operation cannot be performed."
@@ -446,7 +489,41 @@
             ]
         )
         snowflake.connector.pandas_tools.write_pandas(conn, df, "customers")
 
         cur.execute("select id, first_name, last_name from customers")
 
         assert cur.fetchall() == [(1, "Jenny", "P"), (2, "Jasper", "M")]
+
+
+def test_write_pandas_partial_columns(conn: snowflake.connector.SnowflakeConnection):
+    with conn.cursor() as cur:
+        cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
+
+        df = pd.DataFrame.from_records(
+            [
+                {"ID": 1, "FIRST_NAME": "Jenny"},
+                {"ID": 2, "FIRST_NAME": "Jasper"},
+            ]
+        )
+        snowflake.connector.pandas_tools.write_pandas(conn, df, "customers")
+
+        cur.execute("select id, first_name, last_name from customers")
+
+        # columns not in dataframe will receive their default value
+        assert cur.fetchall() == [(1, "Jenny", None), (2, "Jasper", None)]
+
+
+def test_write_pandas_dict_column_as_varchar(conn: snowflake.connector.SnowflakeConnection):
+    with conn.cursor() as cur:
+        cur.execute("create table example (id str, vc varchar, o object)")
+
+        df = pd.DataFrame(
+            [("abc", {"kind": "vc", "count": 1}, {"kind": "obj", "amount": 2})], columns=["ID", "VC", "O"]
+        )
+        snowflake.connector.pandas_tools.write_pandas(conn, df, "EXAMPLE")
+
+        cur.execute("select * from example")
+
+        # returned values are valid json strings
+        # TODO: order object keys alphabetically like snowflake does
+        assert cur.fetchall() == [("abc", '{"kind":"vc","count":1}', '{"kind":"obj","amount":2}')]
```

### Comparing `fakesnow-0.0.2/tests/test_patch.py` & `fakesnow-0.1.0/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.0.2/tests/test_transforms.py` & `fakesnow-0.1.0/tests/test_transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     as_describe,
     create_database,
     drop_schema_cascade,
     extract_comment,
     indices_to_array,
     indices_to_object,
     join_information_schema_ext,
+    object_construct,
     parse_json,
     regex,
     semi_structured_types,
     set_schema,
     tag,
     to_date,
     upper_case_unquoted_identifiers,
@@ -70,14 +71,23 @@
 def test_information_schema_ext() -> None:
     assert (
         sqlglot.parse_one("SELECT * FROM INFORMATION_SCHEMA.TABLES").transform(join_information_schema_ext).sql()
         == "SELECT * FROM INFORMATION_SCHEMA.TABLES LEFT JOIN information_schema.tables_ext ON tables.table_catalog = tables_ext.ext_table_catalog AND tables.table_schema = tables_ext.ext_table_schema AND tables.table_name = tables_ext.ext_table_name"  # noqa: e501
     )
 
 
+def test_object_construct() -> None:
+    assert (
+        sqlglot.parse_one("SELECT OBJECT_CONSTRUCT('a',1,'b','BBBB', 'c',null)", read="snowflake")
+        .transform(object_construct)
+        .sql(dialect="duckdb")
+        == "SELECT TO_JSON({'a': 1, 'b': 'BBBB', 'c': NULL})"
+    )
+
+
 def test_parse_json() -> None:
     assert (
         sqlglot.parse_one("""insert into table1 (name) select parse_json('{"first":"foo", "last":"bar"}')""")
         .transform(parse_json)
         .sql()
         == """INSERT INTO table1 (name) SELECT JSON('{"first":"foo", "last":"bar"}')"""
     )
@@ -86,21 +96,14 @@
 def test_regex() -> None:
     assert (
         sqlglot.parse_one("SELECT regexp_replace('abc123', '\\\\D', '')").transform(regex).sql()
         == "SELECT REGEXP_REPLACE('abc123', '\\D', '', 'g')"
     )
 
 
-def test_to_date() -> None:
-    assert (
-        sqlglot.parse_one("SELECT to_date(to_timestamp(0))").transform(to_date).sql()
-        == "SELECT CAST(TO_TIMESTAMP(0) AS DATE)"
-    )
-
-
 def test_semi_structured_types() -> None:
     assert (
         sqlglot.parse_one("CREATE TABLE table1 (name object)").transform(semi_structured_types).sql()
         == "CREATE TABLE table1 (name JSON)"
     )
 
     assert (
@@ -114,14 +117,21 @@
     )
 
 
 def test_tag() -> None:
     assert sqlglot.parse_one("ALTER TABLE table1 SET TAG foo='bar'", read="snowflake").transform(tag) == SUCCESS_NO_OP
 
 
+def test_to_date() -> None:
+    assert (
+        sqlglot.parse_one("SELECT to_date(to_timestamp(0))").transform(to_date).sql()
+        == "SELECT CAST(DATE_TRUNC('day', TO_TIMESTAMP(0)) AS DATE)"
+    )
+
+
 def test_use() -> None:
     assert (
         sqlglot.parse_one("use database marts").transform(set_schema, current_database=None).sql()
         == "SET schema = 'marts.main'"
     )
 
     assert (
```

