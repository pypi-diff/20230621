# Comparing `tmp/pg_force_execute-0.0.9.tar.gz` & `tmp/pg_force_execute-0.0.dev0.tar.gz`

## Comparing `pg_force_execute-0.0.9.tar` & `pg_force_execute-0.0.dev0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pg_force_execute-0.0.9/pg_force_execute.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.9/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.9/LICENSE
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 pg_force_execute-0.0.9/README.md
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pg_force_execute-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 pg_force_execute-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 pg_force_execute-0.0.dev0/pg_force_execute.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.dev0/LICENSE
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pg_force_execute-0.0.dev0/README.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pg_force_execute-0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 pg_force_execute-0.0.dev0/PKG-INFO
```

### Comparing `pg_force_execute-0.0.9/pg_force_execute.py` & `pg_force_execute-0.0.dev0/pg_force_execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sqlalchemy as sa
 
 
 @contextlib.contextmanager
 def pg_force_execute(conn,
                      delay=datetime.timedelta(minutes=5),
                      check_interval=datetime.timedelta(seconds=1),
-                     termination_thread_timeout=datetime.timedelta(seconds=10),
+                     cleanup_timeout=datetime.timedelta(seconds=10),
                      logger=logging.getLogger("pg_force_execute"),
 ):
     cancel_exception = None
 
     def force_unblock(pid, exit):
         nonlocal cancel_exception
 
@@ -58,10 +58,10 @@
     t = Thread(target=force_unblock, args=(pid, exit))
     t.start()
 
     try:
         yield
     finally:
         exit.set()
-        t.join(timeout=termination_thread_timeout.total_seconds())
+        t.join(timeout=cleanup_timeout.total_seconds())
         if cancel_exception is not None:
             raise cancel_exception
```

### Comparing `pg_force_execute-0.0.9/.gitignore` & `pg_force_execute-0.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.9/LICENSE` & `pg_force_execute-0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.9/README.md` & `pg_force_execute-0.0.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that continue to block it after a configurable delay.
 
 Using this to wrap queries is somewhat of a last resort, but is useful in certain Extract Transform Load (ETL) pipeline contexts. For example, if it is more important to replace one table with another than to allow running queries on the table to complete, then this can be used to run the relevant `ALTER TABLE RENAME TO` query.
 
 
 ## Installation
 
+`pg-force-execute` can be installed from PyPI using pip. `psycopg2` or `psycopg` (Psycopg 3) must also be explicitly installed.
+
 ```bash
-pip install pg-force-execute
+pip install pg-force-execute psycopg
 ```
 
 
 ## Example usage
 
 ```python
 import datetime
@@ -33,39 +35,43 @@
         ):
 
     results = conn.execute(sa.text(query))
     print(results.fetchall())
 ```
 
 
-## Compatibility
-
-- Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
-- psycopg2 >= 2.9.2 or Psycopg 3 >= 3.1.4
-- SQLAlchemy >= 1.4.0 (tested on 1.4.0 and 2.0.0)
-- PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, and 15.0)
-
-
 ## API
 
 The API a single context manager `pg_force_execute`.
 
-`pg_force_execute`(conn, engine, delay=datetime.timedelta(minutes=5), check_interval=datetime.timedelta(seconds=1), termination_thread_timeout=datetime.timedelta(seconds=10), logger=logging.getLogger("pg_force_execute"))
+`pg_force_execute`(conn, delay=datetime.timedelta(minutes=5), check_interval=datetime.timedelta(seconds=1), cleanup_timeout=datetime.timedelta(seconds=10), logger=logging.getLogger("pg_force_execute"))
 
 - `conn` - A [SQLAlchemy connection](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Connection) that will be unblocked
 
 - `delay` (optional) - How long to wait before attempting to terminate backends blocking `conn`
 
-- `check_interval` (optional) - The interval between repeated attempted to terminate backends blocking `conn`
+- `check_interval` (optional) - The interval between repeated attempts to terminate backends blocking `conn`
+
+- `cleanup_timeout` (optional) - How long to wait for resources to be cleaned up before allowing exit of the context manager
 
-- `termination_thread_timeout` (optional) - How long to wait for the termination to complete
+    For usual operation this parameter shouldn't need to be changed.
 
 - `logger` (optional) The Python logger instance through which to log
 
 
+## Compatibility
+
+- Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
+- psycopg2 >= 2.9.2 or Psycopg 3 >= 3.1.4
+- SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
+- PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, and 15.0)
+
+Note that SQLAlchemy < 2 does not support Psycopg 3.
+
+
 ## Running tests locally
 
 ```bash
-pip install -e ".[dev]"  # Only needed once
-./start-services.sh      # Only needed once
+python -m pip install -e ".[dev]"  # Only needed once
+./start-services.sh                # Only needed once
 pytest
 ```
```

### Comparing `pg_force_execute-0.0.9/pyproject.toml` & `pg_force_execute-0.0.dev0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-force-execute"
-version = "0.0.9"
+version = "0.0.dev0"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that block them"
 readme = "README.md"
 requires-python = ">=3.7.1"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "sqlalchemy>=1.4.0",
+    "sqlalchemy>=1.4.24",
 ]
 
 [project.optional-dependencies]
 dev = [
     "psycopg>=3.1.4",
     "psycopg2>=2.9.2",
     "pytest>=7.2.1",
 ]
 ci = [
     "pytest==7.2.1",
 ]
 ci-psycopg2-sqlalchemy1 = [
     "psycopg2==2.9.2",
-    "sqlalchemy==1.4.0",
+    "sqlalchemy==1.4.24",
 ]
 ci-psycopg2-sqlalchemy2 = [
     "psycopg2==2.9.2",
     "sqlalchemy==2.0.0",
 ]
 ci-psycopg3-sqlalchemy2 = [
     "psycopg==3.1.4",
```

### Comparing `pg_force_execute-0.0.9/PKG-INFO` & `pg_force_execute-0.0.dev0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pg-force-execute
-Version: 0.0.9
+Version: 0.0.dev0
 Summary: Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that block them
 Project-URL: Source, https://github.com/uktrade/pg-force-execute
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.1
-Requires-Dist: sqlalchemy>=1.4.0
+Requires-Dist: sqlalchemy>=1.4.24
 Provides-Extra: ci
 Requires-Dist: pytest==7.2.1; extra == 'ci'
 Provides-Extra: ci-psycopg2-sqlalchemy1
 Requires-Dist: psycopg2==2.9.2; extra == 'ci-psycopg2-sqlalchemy1'
-Requires-Dist: sqlalchemy==1.4.0; extra == 'ci-psycopg2-sqlalchemy1'
+Requires-Dist: sqlalchemy==1.4.24; extra == 'ci-psycopg2-sqlalchemy1'
 Provides-Extra: ci-psycopg2-sqlalchemy2
 Requires-Dist: psycopg2==2.9.2; extra == 'ci-psycopg2-sqlalchemy2'
 Requires-Dist: sqlalchemy==2.0.0; extra == 'ci-psycopg2-sqlalchemy2'
 Provides-Extra: ci-psycopg3-sqlalchemy2
 Requires-Dist: psycopg==3.1.4; extra == 'ci-psycopg3-sqlalchemy2'
 Requires-Dist: sqlalchemy==2.0.0; extra == 'ci-psycopg3-sqlalchemy2'
 Provides-Extra: dev
@@ -32,16 +32,18 @@
 Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that continue to block it after a configurable delay.
 
 Using this to wrap queries is somewhat of a last resort, but is useful in certain Extract Transform Load (ETL) pipeline contexts. For example, if it is more important to replace one table with another than to allow running queries on the table to complete, then this can be used to run the relevant `ALTER TABLE RENAME TO` query.
 
 
 ## Installation
 
+`pg-force-execute` can be installed from PyPI using pip. `psycopg2` or `psycopg` (Psycopg 3) must also be explicitly installed.
+
 ```bash
-pip install pg-force-execute
+pip install pg-force-execute psycopg
 ```
 
 
 ## Example usage
 
 ```python
 import datetime
@@ -62,39 +64,43 @@
         ):
 
     results = conn.execute(sa.text(query))
     print(results.fetchall())
 ```
 
 
-## Compatibility
-
-- Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
-- psycopg2 >= 2.9.2 or Psycopg 3 >= 3.1.4
-- SQLAlchemy >= 1.4.0 (tested on 1.4.0 and 2.0.0)
-- PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, and 15.0)
-
-
 ## API
 
 The API a single context manager `pg_force_execute`.
 
-`pg_force_execute`(conn, engine, delay=datetime.timedelta(minutes=5), check_interval=datetime.timedelta(seconds=1), termination_thread_timeout=datetime.timedelta(seconds=10), logger=logging.getLogger("pg_force_execute"))
+`pg_force_execute`(conn, delay=datetime.timedelta(minutes=5), check_interval=datetime.timedelta(seconds=1), cleanup_timeout=datetime.timedelta(seconds=10), logger=logging.getLogger("pg_force_execute"))
 
 - `conn` - A [SQLAlchemy connection](https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Connection) that will be unblocked
 
 - `delay` (optional) - How long to wait before attempting to terminate backends blocking `conn`
 
-- `check_interval` (optional) - The interval between repeated attempted to terminate backends blocking `conn`
+- `check_interval` (optional) - The interval between repeated attempts to terminate backends blocking `conn`
+
+- `cleanup_timeout` (optional) - How long to wait for resources to be cleaned up before allowing exit of the context manager
 
-- `termination_thread_timeout` (optional) - How long to wait for the termination to complete
+    For usual operation this parameter shouldn't need to be changed.
 
 - `logger` (optional) The Python logger instance through which to log
 
 
+## Compatibility
+
+- Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
+- psycopg2 >= 2.9.2 or Psycopg 3 >= 3.1.4
+- SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
+- PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, and 15.0)
+
+Note that SQLAlchemy < 2 does not support Psycopg 3.
+
+
 ## Running tests locally
 
 ```bash
-pip install -e ".[dev]"  # Only needed once
-./start-services.sh      # Only needed once
+python -m pip install -e ".[dev]"  # Only needed once
+./start-services.sh                # Only needed once
 pytest
 ```
```

