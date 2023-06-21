# Comparing `tmp/mkdocs_typer-0.0.2.tar.gz` & `tmp/mkdocs_typer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs_typer-0.0.2.tar", last modified: Mon Jan 25 21:55:12 2021, max compression
+gzip compressed data, was "mkdocs_typer-0.0.3.tar", last modified: Wed Jun 21 16:33:36 2023, max compression
```

## Comparing `mkdocs_typer-0.0.2.tar` & `mkdocs_typer-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 21:55:12.198639 mkdocs_typer-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       85 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4851 2021-01-25 21:55:12.198639 mkdocs_typer-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3098 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 21:55:12.198639 mkdocs_typer-0.0.2/mkdocs_typer/
--rw-r--r--   0 runner    (1001) docker     (116)      299 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       94 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3665 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/_docs.py
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1544 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/_extension.py
--rw-r--r--   0 runner    (1001) docker     (116)      945 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/_loader.py
--rw-r--r--   0 runner    (1001) docker     (116)     1278 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/_processing.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/mkdocs_typer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 21:55:12.198639 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4851 2021-01-25 21:55:12.000000 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      533 2021-01-25 21:55:12.000000 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-25 21:55:12.000000 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-01-25 21:55:12.000000 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-25 21:54:54.000000 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       25 2021-01-25 21:55:12.000000 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-01-25 21:55:12.000000 mkdocs_typer-0.0.2/mkdocs_typer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       57 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      352 2021-01-25 21:55:12.202639 mkdocs_typer-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1555 2021-01-25 21:54:45.000000 mkdocs_typer-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:33:36.920944 mkdocs_typer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-21 16:33:36.920944 mkdocs_typer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:33:36.916944 mkdocs_typer-0.0.3/mkdocs_typer/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/mkdocs_typer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:33:36.920944 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-21 16:33:36.000000 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 16:33:36.000000 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:33:36.000000 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 16:33:36.000000 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:33:22.000000 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 16:33:36.000000 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 16:33:36.000000 mkdocs_typer-0.0.3/mkdocs_typer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-21 16:33:36.920944 mkdocs_typer-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:33:36.920944 mkdocs_typer-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-21 16:33:10.000000 mkdocs_typer-0.0.3/tests/test_extension.py
```

### Comparing `mkdocs_typer-0.0.2/LICENSE` & `mkdocs_typer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_typer-0.0.2/PKG-INFO` & `mkdocs_typer-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: mkdocs_typer
-Version: 0.0.2
+Version: 0.0.3
 Summary: An MkDocs extension to generate documentation for Typer command line applications
 Home-page: https://github.com/bruce-szalwinski/mkdocs-typer
 Author: Bruce Szalwinski
 Author-email: bruce.szalwinski@gmail.com
 License: Apache
 Description: # mkdocs-typer
         
-        ![Tests](https://github.com/bruce-szalwinski/mkdocs-typer/workflows/Tests/badge.svg?branch=master)
+        ![Tests](https://github.com/bruce-szalwinski/mkdocs-typer/workflows/Tests/badge.svg?branch=main)
         ![Python versions](https://img.shields.io/pypi/pyversions/mkdocs-typer.svg)
         [![Package version](https://badge.fury.io/py/mkdocs-typer.svg)](https://pypi.org/project/mkdocs-typer)
         
         An MkDocs extension to generate documentation for Typer command line applications.
         
         ## Installation
         
@@ -137,9 +137,10 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mkdocs_typer-0.0.2/README.md` & `mkdocs_typer-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # mkdocs-typer
 
-![Tests](https://github.com/bruce-szalwinski/mkdocs-typer/workflows/Tests/badge.svg?branch=master)
+![Tests](https://github.com/bruce-szalwinski/mkdocs-typer/workflows/Tests/badge.svg?branch=main)
 ![Python versions](https://img.shields.io/pypi/pyversions/mkdocs-typer.svg)
 [![Package version](https://badge.fury.io/py/mkdocs-typer.svg)](https://pypi.org/project/mkdocs-typer)
 
 An MkDocs extension to generate documentation for Typer command line applications.
 
 ## Installation
```

### Comparing `mkdocs_typer-0.0.2/mkdocs_typer/_docs.py` & `mkdocs_typer-0.0.3/mkdocs_typer/_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,49 +13,49 @@
     """Create the Markdown lines for a command and its sub-commands."""
     cmd = get_command(command)
     for line in _recursively_make_command_docs(prog_name, cmd, level=level):
         yield line.replace("\b", "")
 
 
 def _recursively_make_command_docs(
-    prog_name: str, command: click.Command, parent: typer.Context = None, level: int = 0
+    prog_name: Optional[str], command: click.Command, parent: typer.Context = None, level: int = 0
 ) -> Iterator[str]:
     """Create the raw Markdown lines for a command and its sub-commands."""
     ctx = typer.Context(command, parent=parent)
 
     yield from _make_title(prog_name, level)
     yield from _make_description(ctx)
     yield from _make_usage(ctx)
     yield from _make_options(ctx)
 
     subcommands = _get_sub_commands(ctx.command, ctx)
 
-    for command in sorted(subcommands, key=lambda cmd: cmd.name):
+    for command in sorted(subcommands, key=lambda cmd: cmd.name if cmd.name else ""):
         yield from _recursively_make_command_docs(command.name, command, parent=ctx, level=level + 1)
 
 
 def _get_sub_commands(command: click.Command, ctx: typer.Context) -> List[click.Command]:
     """Return subcommands of a Typer command."""
     subcommands = getattr(command, "commands", {})
     if subcommands:
-        return subcommands.values()
+        return list(subcommands.values())
     else:
         # MultiCommand not created by Typer.
         # See https://github.com/DataDog/mkdocs-click/blob/master/mkdocs_click/_docs.py#L45
 
         return []
 
 
-def _make_title(prog_name: str, level: int) -> Iterator[str]:
+def _make_title(prog_name: Optional[str], level: int) -> Iterator[str]:
     """Create the first markdown lines describing a command."""
     yield _make_header(prog_name, level)
     yield ""
 
 
-def _make_header(text: str, level: int) -> str:
+def _make_header(text: Optional[str], level: int) -> str:
     """Create a markdown header at a given level"""
     return f"{'#' * (level + 1)} {text}"
 
 
 def _make_description(ctx: click.Context) -> Iterator[str]:
     """Create markdown lines based on the command's own description."""
     help_string = ctx.command.help or ctx.command.short_help
```

### Comparing `mkdocs_typer-0.0.2/mkdocs_typer/_extension.py` & `mkdocs_typer-0.0.3/mkdocs_typer/_extension.py`

 * *Files identical despite different names*

### Comparing `mkdocs_typer-0.0.2/mkdocs_typer/_loader.py` & `mkdocs_typer-0.0.3/mkdocs_typer/_loader.py`

 * *Files identical despite different names*

### Comparing `mkdocs_typer-0.0.2/mkdocs_typer/_processing.py` & `mkdocs_typer-0.0.3/mkdocs_typer/_processing.py`

 * *Files identical despite different names*

### Comparing `mkdocs_typer-0.0.2/mkdocs_typer.egg-info/PKG-INFO` & `mkdocs_typer-0.0.3/mkdocs_typer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: mkdocs-typer
-Version: 0.0.2
+Version: 0.0.3
 Summary: An MkDocs extension to generate documentation for Typer command line applications
 Home-page: https://github.com/bruce-szalwinski/mkdocs-typer
 Author: Bruce Szalwinski
 Author-email: bruce.szalwinski@gmail.com
 License: Apache
 Description: # mkdocs-typer
         
-        ![Tests](https://github.com/bruce-szalwinski/mkdocs-typer/workflows/Tests/badge.svg?branch=master)
+        ![Tests](https://github.com/bruce-szalwinski/mkdocs-typer/workflows/Tests/badge.svg?branch=main)
         ![Python versions](https://img.shields.io/pypi/pyversions/mkdocs-typer.svg)
         [![Package version](https://badge.fury.io/py/mkdocs-typer.svg)](https://pypi.org/project/mkdocs-typer)
         
         An MkDocs extension to generate documentation for Typer command line applications.
         
         ## Installation
         
@@ -137,9 +137,10 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mkdocs_typer-0.0.2/mkdocs_typer.egg-info/SOURCES.txt` & `mkdocs_typer-0.0.3/mkdocs_typer.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 mkdocs_typer/py.typed
 mkdocs_typer.egg-info/PKG-INFO
 mkdocs_typer.egg-info/SOURCES.txt
 mkdocs_typer.egg-info/dependency_links.txt
 mkdocs_typer.egg-info/entry_points.txt
 mkdocs_typer.egg-info/not-zip-safe
 mkdocs_typer.egg-info/requires.txt
-mkdocs_typer.egg-info/top_level.txt
+mkdocs_typer.egg-info/top_level.txt
+tests/test_extension.py
```

### Comparing `mkdocs_typer-0.0.2/setup.py` & `mkdocs_typer-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,9 +38,10 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ]
 )
```

