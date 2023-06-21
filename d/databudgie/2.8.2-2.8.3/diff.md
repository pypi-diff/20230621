# Comparing `tmp/databudgie-2.8.2.tar.gz` & `tmp/databudgie-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databudgie-2.8.2.tar", max compression
+gzip compressed data, was "databudgie-2.8.3.tar", max compression
```

## Comparing `databudgie-2.8.2.tar` & `databudgie-2.8.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     5139 2023-06-12 14:36:28.294923 databudgie-2.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     1973 2023-06-12 14:36:28.294923 databudgie-2.8.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1053 2023-06-12 14:36:28.294923 databudgie-2.8.2/LICENSE
--rw-r--r--   0        0        0     1310 2023-06-12 14:36:28.294923 databudgie-2.8.2/README.md
--rw-r--r--   0        0        0     2883 2023-06-12 14:36:28.298923 databudgie-2.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/__init__.py
--rw-r--r--   0        0        0       69 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/__main__.py
--rw-r--r--   0        0        0       74 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/adapter/__init__.py
--rw-r--r--   0        0        0     7162 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/adapter/base.py
--rw-r--r--   0        0        0    10638 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/adapter/postgres.py
--rw-r--r--   0        0        0     7361 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/backup.py
--rw-r--r--   0        0        0      105 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/cli/__init__.py
--rw-r--r--   0        0        0     3071 2023-06-12 14:36:28.298923 databudgie-2.8.2/src/databudgie/cli/base.py
--rw-r--r--   0        0        0     6728 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/cli/commands.py
--rw-r--r--   0        0        0     4730 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/cli/config.py
--rw-r--r--   0        0        0     1112 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/compression.py
--rw-r--r--   0        0        0    11753 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/config.py
--rw-r--r--   0        0        0      105 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/manifest/__init__.py
--rw-r--r--   0        0        0     2348 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/manifest/manager.py
--rw-r--r--   0        0        0     1602 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/manifest/sqlalchemy.py
--rw-r--r--   0        0        0      565 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/match.py
--rw-r--r--   0        0        0     1564 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/output.py
--rw-r--r--   0        0        0        0 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/py.typed
--rw-r--r--   0        0        0     8408 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/restore.py
--rw-r--r--   0        0        0     1948 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/s3.py
--rw-r--r--   0        0        0    11806 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/storage.py
--rw-r--r--   0        0        0     4586 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/table_op.py
--rw-r--r--   0        0        0     2462 2023-06-12 14:36:28.302923 databudgie-2.8.2/src/databudgie/utils.py
--rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 databudgie-2.8.2/setup.py
--rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 databudgie-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     5139 2023-06-21 20:25:54.906850 databudgie-2.8.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1973 2023-06-21 20:25:54.906850 databudgie-2.8.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1053 2023-06-21 20:25:54.906850 databudgie-2.8.3/LICENSE
+-rw-r--r--   0        0        0     1310 2023-06-21 20:25:54.906850 databudgie-2.8.3/README.md
+-rw-r--r--   0        0        0     2883 2023-06-21 20:25:54.910850 databudgie-2.8.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/__init__.py
+-rw-r--r--   0        0        0       69 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/__main__.py
+-rw-r--r--   0        0        0       74 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/adapter/__init__.py
+-rw-r--r--   0        0        0     7584 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/adapter/base.py
+-rw-r--r--   0        0        0    11357 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/adapter/postgres.py
+-rw-r--r--   0        0        0     7545 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/backup.py
+-rw-r--r--   0        0        0      105 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/__init__.py
+-rw-r--r--   0        0        0     3071 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/base.py
+-rw-r--r--   0        0        0     6738 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/commands.py
+-rw-r--r--   0        0        0     4944 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/config.py
+-rw-r--r--   0        0        0     1112 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/compression.py
+-rw-r--r--   0        0        0    11855 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/config.py
+-rw-r--r--   0        0        0      105 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/manifest/__init__.py
+-rw-r--r--   0        0        0     2348 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/manifest/manager.py
+-rw-r--r--   0        0        0     1602 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/manifest/sqlalchemy.py
+-rw-r--r--   0        0        0      565 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/match.py
+-rw-r--r--   0        0        0     1564 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/output.py
+-rw-r--r--   0        0        0        0 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/py.typed
+-rw-r--r--   0        0        0     8014 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/restore.py
+-rw-r--r--   0        0        0     1948 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/s3.py
+-rw-r--r--   0        0        0    11836 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/storage.py
+-rw-r--r--   0        0        0     4586 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/table_op.py
+-rw-r--r--   0        0        0     2462 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/utils.py
+-rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 databudgie-2.8.3/setup.py
+-rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 databudgie-2.8.3/PKG-INFO
```

### Comparing `databudgie-2.8.2/CHANGELOG.md` & `databudgie-2.8.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/CONTRIBUTING.md` & `databudgie-2.8.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/LICENSE` & `databudgie-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/README.md` & `databudgie-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/pyproject.toml` & `databudgie-2.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databudgie"
-version = "2.8.2"
+version = "2.8.3"
 packages = [
     { include = "databudgie", from = "src" },
 ]
 
 authors = [
   "Andrew Sosa <andrewso@known.is>",
   "Dan Cardin <ddcardin@gmail.com>",
```

### Comparing `databudgie-2.8.2/src/databudgie/adapter/base.py` & `databudgie-2.8.3/src/databudgie/adapter/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,23 @@
         metadata.reflect(engine, schema=schema)
         table_ref = Table(table_name, metadata, autoload=True, autoload_with=engine, schema=schema)
 
         with engine.connect() as conn:
             conn.execute(table_ref.insert(), prepared_rows)
             conn.execute(text("commit"))
 
+    def execute_sql(self, sql: bytes, *, commit=False):
+        """Abstract the execution of SQL queries away from the calling code."""
+        text_sql = sql.decode("utf-8")
+        result = self.session.execute(sqlalchemy.text(text_sql))
+        if commit:
+            self.session.commit()
+
+        return result
+
     def export_schema_ddl(self, name: str):
         raise NotImplementedError()  # pragma: no cover
 
     def export_table_ddl(self, table_name: str, console: Console = default_console):
         raise NotImplementedError()  # pragma: no cover
 
     def truncate_table(self, table: str):
@@ -168,15 +177,16 @@
 
             if not table_op.raw_conf.follow_foreign_keys:
                 continue
 
             dependent_tables = self.collect_table_dependencies(table_op=table_op, console=console)
             for dependent_table in dependent_tables:
                 if dependent_table not in tables:
-                    table_location = join_paths(table_op.location(), "{table}")
+                    concrete_parent_location = table_op.location().format(table=table_op.full_name)
+                    table_location = join_paths(concrete_parent_location, "{table}")
                     conf = replace(table_op.raw_conf, name=dependent_table, location=table_location)
 
                     dependent_table_op = TableOp.from_name(dependent_table, conf)
                     tables.add(dependent_table)
                     dependent_table_ops.append(dependent_table_op)
 
         if reverse:
```

### Comparing `databudgie-2.8.2/src/databudgie/adapter/postgres.py` & `databudgie-2.8.3/src/databudgie/adapter/postgres.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,23 @@
             host=url.host,
             port=url.port,
             database=database or url.database,
         )
 
 
 class PostgresAdapter(Adapter):
+    def execute_sql(self, sql: bytes, *, commit=False):
+        """Abstract the execution of SQL queries away from the calling code.
+
+        Additionally performs pg_dump-specific SQL "cleaning" to remove statements
+        which could/would cause issues or otherwise bloat the resultant query.
+        """
+        cleaned_sql = clean_sql(sql)
+        return super().execute_sql(cleaned_sql, commit=commit)
+
     def export_query(self, query: str) -> QueryResult:
         engine: Engine = cast(Engine, self.session.get_bind())
 
         result = QueryResult()
         with result.binary_buffer() as buffer:
             with contextlib.closing(engine.raw_connection()) as conn:
                 with cast(cursor, conn.cursor()) as cursor_:
@@ -228,15 +237,15 @@
     def collect_sequence_value(self, sequence_name: str) -> int:
         return cast(int, self.session.execute(text(f"SELECT last_value from {sequence_name}")).scalar())  # noqa: S608
 
     def restore_sequence_value(self, sequence_name: str, value: int) -> int:
         return cast(int, self.session.execute(text(f"SELECT setval('{sequence_name}', {value})")).scalar())
 
 
-def pg_dump(url: URL, rest: str = "", no_comments=True) -> bytes:
+def pg_dump(url: URL, rest: str = "", no_comments=True, clean=True) -> bytes:
     parts = [f"pg_dump -h {url.host} -p {url.port} -U {url.username} -d {url.database} --no-password"]
 
     if no_comments:
         parts.append("--no-comments")
 
     parts.append(rest)
 
@@ -247,8 +256,21 @@
     try:
         result = subprocess.run(  # nosec
             command, capture_output=True, env={**os.environ, "PGPASSWORD": str(url.password or "")}, check=True
         )
     except subprocess.CalledProcessError as e:
         raise RuntimeError(e.stderr)
 
-    return result.stdout
+    output = result.stdout
+
+    return clean_sql(output)
+
+
+def clean_sql(sql: bytes) -> bytes:
+    return b"\n".join(
+        line
+        for line in sql.splitlines()
+        if not line.startswith(b"--")
+        and not line.startswith(b"SET")
+        and not line.startswith(b"SELECT pg_catalog")
+        and line
+    )
```

### Comparing `databudgie-2.8.2/src/databudgie/backup.py` & `databudgie-2.8.3/src/databudgie/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,17 +226,23 @@
     Arguments:
         config: The raw backup configuration.
         table_op: The table operation being acted up on.
         adapter: the selected behavior adapter
         storage: the storage backend to use for backing up the data.
         console: Console used for output
     """
+    path = table_op.location()
+
+    if table_op.raw_conf.skip_if_exists and storage.path_exists(path):
+        console.trace(f"Skipping {table_op.full_name} due to `skip_if_exists`")
+        return
+
     buffer = adapter.export_query(table_op.query())
 
     # path.join will handle optionally trailing slashes in the location
     compression = table_op.raw_conf.compression
 
     filename = storage.write_buffer(
-        table_op.location(), buffer, file_type=FileTypes.data, name=table_op.full_name, compression=compression
+        path, buffer, file_type=FileTypes.data, name=table_op.full_name, compression=compression
     )
 
     console.trace(f"Uploaded {table_op.full_name} to {filename}")
```

### Comparing `databudgie-2.8.2/src/databudgie/cli/base.py` & `databudgie-2.8.3/src/databudgie/cli/base.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/cli/commands.py` & `databudgie-2.8.3/src/databudgie/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import click
 from sqlalchemy.orm import Session
 
 from databudgie.cli.base import resolver
 from databudgie.cli.config import (
     CliConfig,
     collect_config,
-    loaders,
+    file_loaders,
     pretty_print,
 )
 from databudgie.config import (
     BackupConfig,
     ConfigError,
     RestoreConfig,
     RootConfig,
@@ -77,15 +77,15 @@
     default=None,
     help="Accepts raw config as a string, rather than searching a file for it.",
 )
 @click.option(
     "--raw-config-format",
     default="json",
     help="The assumed format of --raw-config. Defaults to `json`. Must be one of: `yml`, `yaml`, `json`, `toml`.",
-    type=click.Choice(loaders),
+    type=click.Choice(file_loaders),
 )
 @click.version_option()
 def cli(
     strict: bool,
     config: Iterable[str],
     verbose: int = 0,
     color: bool = True,
```

### Comparing `databudgie-2.8.2/src/databudgie/cli/config.py` & `databudgie-2.8.3/src/databudgie/cli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import os
 import sys
 from dataclasses import asdict, dataclass
 from os import isatty
 from pathlib import Path
 from typing import Iterable, MutableMapping
 
-from configly import Config, JsonLoader, TomlLoader, YamlLoader
+import click
+from configly import Config, loaders
 from rich.console import Console
 from rich.syntax import Syntax
 from ruamel.yaml import YAML
 
 from databudgie.config import Config as DatabudgieConfig
 from databudgie.config import ConfigStack, RootConfig
 
@@ -20,20 +21,19 @@
     "config.databudgie.yml",
     "databudgie.yml",
     "databudgie.yaml",
     "databudgie.json",
     "databudgie.toml",
 )
 
-loaders: dict[str, type[JsonLoader | TomlLoader | YamlLoader]] = {
-    "yaml": YamlLoader,
-    "yml": YamlLoader,
-    "json": JsonLoader,
-    "toml": TomlLoader,
-}
+file_loaders: dict[str, type] = {}
+for ext, loader_name in [("yaml", "YamlLoader"), ("yml", "YamlLoader"), ("json", "JsonLoader"), ("toml", "TomlLoader")]:
+    loader = getattr(loaders, loader_name)
+    if loader:
+        file_loaders[ext] = loader
 
 
 @dataclass
 class CliConfig(DatabudgieConfig):
     tables: list[str] | None = None
     exclude: list[str] | None = None
     ddl: bool | None = None
@@ -141,16 +141,20 @@
         if stop_when_found:
             break
 
     return result
 
 
 def collect_raw_config(*, format: str, content: str | None = None, file: str | None = None) -> dict:
-    loader_cls = loaders[format]
-    config: Config = Config.from_loader(loader_cls(), file=file, content=content)  # type: ignore
+    loader_cls = file_loaders.get(format)
+    if loader_cls is None:
+        formats = ", ".join(file_loaders.keys())
+        raise click.UsageError(f"File format must be one of: {formats}")
+
+    config: Config = Config.from_loader(loader_cls(), file=file, content=content)
     return config.to_dict()
 
 
 def pretty_print(config: DatabudgieConfig):
     """Pretty print a config model."""
     console = Console()
     buffer = io.StringIO()
```

### Comparing `databudgie-2.8.2/src/databudgie/compression.py` & `databudgie-2.8.3/src/databudgie/compression.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/config.py` & `databudgie-2.8.3/src/databudgie/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,15 @@
     compression: str | None = None
     exclude: list = field(default_factory=list)
     ddl: bool = True
     sequences: bool = True
     data: bool = True
     follow_foreign_keys: bool = False
     strict: bool = False
+    skip_if_exists: bool = False
 
     @classmethod
     def from_stack(cls, stack: ConfigStack, root_location: str | None = None):
         ddl = stack.get("ddl", True)
         if isinstance(ddl, dict):
             ddl = ddl["enabled"]
 
@@ -263,14 +264,15 @@
             compression=stack.get("compression"),
             exclude=stack.get("exclude"),
             sequences=bool(stack.get("sequences", True)),
             data=bool(stack.get("data", True)),
             ddl=bool(ddl),
             follow_foreign_keys=bool(stack.get("follow_foreign_keys", False)),
             strict=bool(stack.get("strict", False)),
+            skip_if_exists=bool(stack.get("skip_if_exists", False)),
         )
 
 
 @dataclass
 class BackupConfig(TableParentConfig[BackupTableConfig]):
     @classmethod
     def get_child_class(cls):
```

### Comparing `databudgie-2.8.2/src/databudgie/manifest/manager.py` & `databudgie-2.8.3/src/databudgie/manifest/manager.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/manifest/sqlalchemy.py` & `databudgie-2.8.3/src/databudgie/manifest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/match.py` & `databudgie-2.8.3/src/databudgie/match.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/output.py` & `databudgie-2.8.3/src/databudgie/output.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/restore.py` & `databudgie-2.8.3/src/databudgie/restore.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 from typing import Optional, Sequence, TYPE_CHECKING, Union
 
-import sqlalchemy
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import Session
 
 from databudgie.adapter import Adapter
 from databudgie.config import RestoreConfig
 from databudgie.output import Console, default_console, Progress
 from databudgie.storage import FileTypes, StorageBackend
@@ -126,53 +125,43 @@
     with Progress(console) as progress:
         total = len(schema_ops) + len(table_ops)
         task = progress.add_task("Restoring DDL", total=total)
 
         for schema_op in schema_ops:
             progress.update(task, description=f"Restoring schema DDL: {schema_op.name}")
 
-            restore_ddl(session, schema_op, ddl_path, storage=storage, console=console)
+            restore_ddl(adapter, schema_op, ddl_path, storage=storage, console=console)
 
         for table_op in table_ops:
             progress.update(task, description=f"Restoring DDL: {table_op.full_name}")
 
-            restore_ddl(session, table_op, ddl_path, storage=storage, console=console)
+            restore_ddl(adapter, table_op, ddl_path, storage=storage, console=console)
 
     console.info("Finished Restoring DDL")
 
 
 def restore_ddl(
-    session: Session,
+    adapter: Adapter,
     op: Union[TableOp, SchemaOp],
     ddl_path: str,
     storage: StorageBackend,
     console: Console = default_console,
 ):
     location = op.location()
     strategy: str = op.raw_conf.strategy
 
     path = join_paths(ddl_path, location)
     with storage.get_file_content(path, strategy, file_type=FileTypes.ddl) as file_object:
         if not file_object:
             console.warn(f"Found no DDL backups under {path} to restore")
             return
 
-        query = file_object.content.read().decode("utf-8")
+        query = file_object.content.read()
 
-    query = "\n".join(
-        line
-        for line in query.splitlines()
-        # XXX: These should be being omitted at the backup stage, it's not the restore process' responsibility!
-        if not line.startswith("--")
-        and not line.startswith("SET")
-        and not line.startswith("SELECT pg_catalog")
-        and line
-    )
-    session.execute(sqlalchemy.text(query))
-    session.commit()
+    adapter.execute_sql(query, commit=True)
 
 
 def restore_sequences(
     session: Session,
     table_ops: Sequence[TableOp],
     adapter: Adapter,
     storage: StorageBackend,
```

### Comparing `databudgie-2.8.2/src/databudgie/s3.py` & `databudgie-2.8.3/src/databudgie/s3.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/storage.py` & `databudgie-2.8.3/src/databudgie/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,19 @@
         npath = pathlib.PurePath(path)
 
         parent = npath.parent
         os.makedirs(parent, exist_ok=True)
         with open(path, "wb") as f:
             f.write(buffer.getbuffer())
 
-    def path_exists(self, path: str):
-        matching_objects = [dir_entry for dir_entry in os.scandir(path) if dir_entry.is_file()]
-        return len(matching_objects) >= 1
+    def path_exists(self, path: str) -> bool:
+        if not os.path.exists("path"):
+            return False
+
+        return any(dir_entry for dir_entry in os.scandir(path) if dir_entry.is_file())
 
     def get_file_content(
         self, path: str, selection_strategy: SelectionStrategy, file_type: FileTypes, compression: str | None = None
     ) -> FileObject | None:
         try:
             files = os.scandir(path)
         except FileNotFoundError:
@@ -95,15 +97,15 @@
         return cls(resource=resource)
 
     def write_buffer(self, path: str, buffer: io.BytesIO):
         s3_location = S3Location(path)
         s3_bucket: Bucket = self.resource.Bucket(s3_location.bucket)
         s3_bucket.put_object(Key=s3_location.key, Body=buffer)
 
-    def path_exists(self, path: str):
+    def path_exists(self, path: str) -> bool:
         s3_location = S3Location(path)
         s3_bucket: Bucket = self.resource.Bucket(s3_location.bucket)
         matching_objects = list(s3_bucket.objects.filter(Prefix=s3_location.key).all())
         return len(matching_objects) >= 1
 
     def get_file_content(
         self, path: str, selection_strategy: SelectionStrategy, file_type: FileTypes, compression: str | None = None
```

### Comparing `databudgie-2.8.2/src/databudgie/table_op.py` & `databudgie-2.8.3/src/databudgie/table_op.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/src/databudgie/utils.py` & `databudgie-2.8.3/src/databudgie/utils.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.2/setup.py` & `databudgie-2.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  's3': ['boto3']}
 
 entry_points = \
 {'console_scripts': ['databudgie = databudgie.__main__:run']}
 
 setup_kwargs = {
     'name': 'databudgie',
-    'version': '2.8.2',
+    'version': '2.8.3',
     'description': 'Ergonomic and flexible tool for database backup and restore',
     'long_description': '# Databudgie\n\n![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)\n[![Documentation\nStatus](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)\n\n![](docs/source/_static/databudgie.png)\n\nDatabudgie is a CLI & library for database performing targeted backup and\nrestore of database tables or arbitrary queries against database tables.\n\n# Usage\n\nA minimal config file might look like:\n\n```yaml\n# databudgie.yml or config.databudgie.yml\nbackup:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      query: "select * from {table} where store_id > 4"\n      location: s3://my-s3-bucket/databudgie/public.product\nrestore:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      location: s3://my-s3-bucket/databudgie/public.product\n```\n\nWith that config in place, backing up the defined tables (using the specified\nconfig) is as simple as `databudgie backup`; and restore `databudgie restore`.\n\n## Installation\n\n```bash\npip install databudgie\n```\n',
     'author': 'Andrew Sosa',
     'author_email': 'andrewso@known.is',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/databudgie',
```

### Comparing `databudgie-2.8.2/PKG-INFO` & `databudgie-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databudgie
-Version: 2.8.2
+Version: 2.8.3
 Summary: Ergonomic and flexible tool for database backup and restore
 Home-page: https://github.com/schireson/databudgie
 License: MIT
 Keywords: sqlalchemy,postgres,database,etl,s3
 Author: Andrew Sosa
 Author-email: andrewso@known.is
 Requires-Python: >=3.7,<4
```

