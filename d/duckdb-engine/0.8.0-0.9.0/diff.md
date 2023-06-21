# Comparing `tmp/duckdb_engine-0.8.0.tar.gz` & `tmp/duckdb_engine-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdb_engine-0.8.0.tar", max compression
+gzip compressed data, was "duckdb_engine-0.9.0.tar", max compression
```

## Comparing `duckdb_engine-0.8.0.tar` & `duckdb_engine-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     5953 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/README.md
--rw-r--r--   0        0        0        4 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
--rw-r--r--   0        0        0        1 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
--rw-r--r--   0        0        0    20688 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
--rw-r--r--   0        0        0    11754 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/__init__.py
--rw-r--r--   0        0        0     1096 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/config.py
--rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/conftest.py
--rw-r--r--   0        0        0     5731 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/datatypes.py
--rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/py.typed
--rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/__init__.py
--rw-r--r--   0        0        0     1209 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      338 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/snapshots/snap_test_basic.py
--rw-r--r--   0        0        0    11218 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_basic.py
--rw-r--r--   0        0        0     4016 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_datatypes.py
--rw-r--r--   0        0        0      948 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_ibis.py
--rw-r--r--   0        0        0     1740 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_integration.py
--rw-r--r--   0        0        0     3946 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_pandas.py
--rw-r--r--   0        0        0      257 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/util.py
--rw-r--r--   0        0        0     1403 2023-06-20 15:20:50.026194 duckdb_engine-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-21 03:45:37.107242 duckdb_engine-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     5953 2023-06-21 03:45:37.107242 duckdb_engine-0.9.0/README.md
+-rw-r--r--   0        0        0        4 2023-06-21 03:45:37.107242 duckdb_engine-0.9.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
+-rw-r--r--   0        0        0        1 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
+-rw-r--r--   0        0        0    20688 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
+-rw-r--r--   0        0        0    12277 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/__init__.py
+-rw-r--r--   0        0        0     1096 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/config.py
+-rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/conftest.py
+-rw-r--r--   0        0        0     5731 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/datatypes.py
+-rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/py.typed
+-rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/__init__.py
+-rw-r--r--   0        0        0     1209 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/snapshots/snap_test_basic.py
+-rw-r--r--   0        0        0    11631 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_basic.py
+-rw-r--r--   0        0        0     4016 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_datatypes.py
+-rw-r--r--   0        0        0      948 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_ibis.py
+-rw-r--r--   0        0        0     1740 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_integration.py
+-rw-r--r--   0        0        0     3946 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_pandas.py
+-rw-r--r--   0        0        0      257 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/util.py
+-rw-r--r--   0        0        0     1403 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.9.0/PKG-INFO
```

### Comparing `duckdb_engine-0.8.0/LICENSE.txt` & `duckdb_engine-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/README.md` & `duckdb_engine-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz` & `duckdb_engine-0.9.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/__init__.py` & `duckdb_engine-0.9.0/duckdb_engine/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,29 @@
     Set,
     Tuple,
     Type,
     cast,
 )
 
 import duckdb
+import sqlalchemy
 from sqlalchemy import pool, text
 from sqlalchemy import types as sqltypes
 from sqlalchemy import util
 from sqlalchemy.dialects.postgresql import UUID
-from sqlalchemy.dialects.postgresql.base import PGDialect, PGInspector
+from sqlalchemy.dialects.postgresql.base import PGDialect, PGInspector, PGTypeCompiler
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.url import URL
+from sqlalchemy.ext.compiler import compiles
 
 from .config import apply_config, get_core_config
 from .datatypes import ISCHEMA_NAMES, register_extension_types
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 if TYPE_CHECKING:
     from sqlalchemy.base import Connection
     from sqlalchemy.engine.interfaces import _IndexDict
 
 
 register_extension_types()
@@ -353,7 +355,22 @@
                 connection, schema="*", info_cache=kw.get("info_cache")
             )
         )
 
         columns = self._get_columns_info(rows, domains, enums, schema)  # type: ignore[attr-defined]
 
         return columns.items()
+
+
+if sqlalchemy.__version__ >= "2.0.14":
+    from sqlalchemy import TryCast  # type: ignore[attr-defined]
+
+    @compiles(TryCast, "duckdb")  # type: ignore[misc]
+    def visit_try_cast(
+        instance: TryCast,
+        compiler: PGTypeCompiler,
+        **kw: Any,
+    ) -> str:
+        return "TRY_CAST({} AS {})".format(
+            compiler.process(instance.clause, **kw),
+            compiler.process(instance.typeclause, **kw),
+        )
```

### Comparing `duckdb_engine-0.8.0/duckdb_engine/config.py` & `duckdb_engine-0.9.0/duckdb_engine/config.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/datatypes.py` & `duckdb_engine-0.9.0/duckdb_engine/datatypes.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/tests/conftest.py` & `duckdb_engine-0.9.0/duckdb_engine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/tests/test_basic.py` & `duckdb_engine-0.9.0/duckdb_engine/tests/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import logging
 import os
 import zlib
-from datetime import timedelta
+from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Any, Generic, Optional, TypeVar, cast
 
 import duckdb
 import sqlalchemy
 from hypothesis import assume, given, settings
 from hypothesis.strategies import text as text_strat
 from packaging.version import Version
 from pytest import LogCaptureFixture, fixture, importorskip, mark, raises
 from sqlalchemy import (
     Column,
+    DateTime,
     ForeignKey,
     Integer,
     Interval,
     MetaData,
     Sequence,
     String,
     Table,
     create_engine,
     inspect,
+    select,
     text,
     types,
 )
 from sqlalchemy.dialects import registry  # type: ignore
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.exc import DBAPIError
@@ -404,7 +406,18 @@
         assert (
             engine.connect() is not None
         )  # grab the "stale" connection, which will cause a ping
 
         assert any(
             "Pool pre-ping on connection" in message for message in caplog.messages
         )
+
+
+def test_try_cast(engine: Engine) -> None:
+    try_cast = importorskip("sqlalchemy", "2.0.14").try_cast
+
+    with engine.connect() as conn:
+        query = select(try_cast("2022-01-01", DateTime))
+        assert conn.execute(query).one() == (datetime(2022, 1, 1),)
+
+        query = select(try_cast("not a date", DateTime))
+        assert conn.execute(query).one() == (None,)
```

### Comparing `duckdb_engine-0.8.0/duckdb_engine/tests/test_datatypes.py` & `duckdb_engine-0.9.0/duckdb_engine/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/tests/test_ibis.py` & `duckdb_engine-0.9.0/duckdb_engine/tests/test_ibis.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/tests/test_integration.py` & `duckdb_engine-0.9.0/duckdb_engine/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/duckdb_engine/tests/test_pandas.py` & `duckdb_engine-0.9.0/duckdb_engine/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.8.0/pyproject.toml` & `duckdb_engine-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duckdb_engine"
-version = "0.8.0"
+version = "0.9.0"
 description = "SQLAlchemy driver for duckdb"
 authors = ["Elliana <me@mause.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Mause/duckdb_engine"
 
 [tool.poetry.urls]
@@ -17,15 +17,15 @@
 sqlalchemy = ">=1.3.22"
 numpy = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pre-commit = "^2.21.0"
 pdbpp = "^0.10.3"
-mypy = "^1.3"
+mypy = "^1.4"
 hypothesis = "^6.75.2"
 pandas = "^1"
 jupysql = "^0.7.8"
 sqlalchemy = {version="^1.3.19", extras=['mypy']}
 pytest-cov = {extras = ["coverage"], version = "^4.0.0"}
 snapshottest = "^0.6.0"
 pytest-remotedata = "^0.4.0"
```

### Comparing `duckdb_engine-0.8.0/PKG-INFO` & `duckdb_engine-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb-engine
-Version: 0.8.0
+Version: 0.9.0
 Summary: SQLAlchemy driver for duckdb
 Home-page: https://github.com/Mause/duckdb_engine
 License: MIT
 Author: Elliana
 Author-email: me@mause.me
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

