# Comparing `tmp/symbex-0.5.tar.gz` & `tmp/symbex-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.5.tar", last modified: Tue Jun 20 11:51:30 2023, max compression
+gzip compressed data, was "symbex-0.6.tar", last modified: Tue Jun 20 22:40:25 2023, max compression
```

## Comparing `symbex-0.5.tar` & `symbex-0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 11:51:15.000000 symbex-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-20 11:51:30.299520 symbex-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-20 11:51:15.000000 symbex-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 11:51:30.299520 symbex-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-20 11:51:15.000000 symbex-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:15.000000 symbex-0.5/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 11:51:15.000000 symbex-0.5/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-20 11:51:15.000000 symbex-0.5/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-06-20 11:51:15.000000 symbex-0.5/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 11:51:30.000000 symbex-0.5/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:51:30.299520 symbex-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-20 11:51:15.000000 symbex-0.5/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-20 11:51:15.000000 symbex-0.5/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-20 11:51:15.000000 symbex-0.5/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.602926 symbex-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 22:40:05.000000 symbex-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-20 22:40:25.602926 symbex-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-06-20 22:40:05.000000 symbex-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:40:25.602926 symbex-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-20 22:40:05.000000 symbex-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.598926 symbex-0.6/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:05.000000 symbex-0.6/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 22:40:05.000000 symbex-0.6/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-20 22:40:05.000000 symbex-0.6/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-06-20 22:40:05.000000 symbex-0.6/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.602926 symbex-0.6/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.602926 symbex-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-20 22:40:05.000000 symbex-0.6/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-20 22:40:05.000000 symbex-0.6/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-20 22:40:05.000000 symbex-0.6/tests/test_symbols.py
```

### Comparing `symbex-0.5/LICENSE` & `symbex-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.5/PKG-INFO` & `symbex-0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.5
+Version: 0.6
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -18,14 +18,16 @@
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
 Find the Python code for specified symbols
 
+Read [symbex: search Python code for functions and classes, then pipe them into a LLM](https://simonwillison.net/2023/Jun/18/symbex/) for background on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install symbex
 ```
 ## Usage
@@ -81,14 +83,16 @@
 In addition to searching for symbols, you can apply filters to the results.
 
 The following filters are available:
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
+- `--documented` - functions/classes that have a docstring
+- `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
 
@@ -135,65 +139,100 @@
 ```
 ### Just the signatures
 
 The `-s/--signatures` option will list just the signatures of the functions and classes, for example:
 ```bash
 symbex -s -d symbex
 ```
-
 <!-- [[[cog
 import cog
 from click.testing import CliRunner
 import pathlib
 from symbex.cli import cli
 
 path = pathlib.Path("symbex").resolve()
 runner = CliRunner()
 result = runner.invoke(cli, ["-s", "-d", str(path)])
 # Need a consistent sort order
 chunks = result.stdout.strip().split("\n\n")
 chunks.sort()
 cog.out(
-    "```\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
-```
-# File: symbex/cli.py Line: 80
-def cli(symbols, files, directories, signatures, count, silent, async_, function, class_, typed, untyped, partially_typed, fully_typed)
+```python
+# File: symbex/cli.py Line: 95
+def cli(symbols, files, directories, signatures, docstrings, count, silent, async_, function, class_, documented, undocumented, typed, untyped, partially_typed, fully_typed)
 
-# File: symbex/lib.py Line: 11
+# File: symbex/lib.py Line: 105
+def function_definition(function_node: AST)
+
+# File: symbex/lib.py Line: 12
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 159
+# File: symbex/lib.py Line: 173
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 193
+# File: symbex/lib.py Line: 207
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 211
+# File: symbex/lib.py Line: 225
 def read_file(path)
 
-# File: symbex/lib.py Line: 237
+# File: symbex/lib.py Line: 251
 class TypeSummary
 
-# File: symbex/lib.py Line: 242
+# File: symbex/lib.py Line: 256
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 35
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool) -> Tuple[(str, int)]
+# File: symbex/lib.py Line: 302
+def quoted_string(s)
 
-# File: symbex/lib.py Line: 66
-def match(name: str, symbols: Iterable[str]) -> bool
+# File: symbex/lib.py Line: 36
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 91
-def function_definition(function_node: AST)
+# File: symbex/lib.py Line: 70
+def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
+
+# File: symbex/lib.py Line: 80
+def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
+To include docstrings in those signatures, use `--docstrings`:
+```bash
+symbex --docstrings --documented -f symbex/lib.py
+```
+
+<!-- [[[cog
+runner = CliRunner()
+result = runner.invoke(cli, ["--docstrings", "--documented", "-f", str(path / "lib.py")])
+# Need a consistent sort order
+chunks = result.stdout.strip().split("\n\n")
+chunks.sort()
+cog.out(
+    "```python\n{}\n```\n".format("\n\n".join(chunks))
+)
+]]] -->
+```python
+# File: symbex/lib.py Line: 12
+def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
+    "Returns ast Nodes matching symbols"
+
+# File: symbex/lib.py Line: 36
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
+    "Returns the code for a given node"
+
+# File: symbex/lib.py Line: 80
+def match(name: str, symbols: Iterable[str]) -> bool
+    "Returns True if name matches any of the symbols, resolving wildcards"
+```
+<!-- [[[end]]] -->
+
 ## Counting symbols
 
 If you just want to count the number of functions and classes that match your filters, use the `--count` option. Here's how to count your classes:
 
 ```bash
 symbex --class --count
 ```
@@ -270,19 +309,22 @@
       symbex --async --count
 
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   -s, --signatures           Show just function and class signatures
+  --docstrings               Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
   --async                    Filter async functions
   --function                 Filter functions
   --class                    Filter classes
+  --documented               Filter functions with docstrings
+  --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --help                     Show this message and exit.
 
 ```
```

### Comparing `symbex-0.5/README.md` & `symbex-0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
 Find the Python code for specified symbols
 
+Read [symbex: search Python code for functions and classes, then pipe them into a LLM](https://simonwillison.net/2023/Jun/18/symbex/) for background on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install symbex
 ```
 ## Usage
@@ -66,14 +68,16 @@
 In addition to searching for symbols, you can apply filters to the results.
 
 The following filters are available:
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
+- `--documented` - functions/classes that have a docstring
+- `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
 
@@ -120,65 +124,100 @@
 ```
 ### Just the signatures
 
 The `-s/--signatures` option will list just the signatures of the functions and classes, for example:
 ```bash
 symbex -s -d symbex
 ```
-
 <!-- [[[cog
 import cog
 from click.testing import CliRunner
 import pathlib
 from symbex.cli import cli
 
 path = pathlib.Path("symbex").resolve()
 runner = CliRunner()
 result = runner.invoke(cli, ["-s", "-d", str(path)])
 # Need a consistent sort order
 chunks = result.stdout.strip().split("\n\n")
 chunks.sort()
 cog.out(
-    "```\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
-```
-# File: symbex/cli.py Line: 80
-def cli(symbols, files, directories, signatures, count, silent, async_, function, class_, typed, untyped, partially_typed, fully_typed)
+```python
+# File: symbex/cli.py Line: 95
+def cli(symbols, files, directories, signatures, docstrings, count, silent, async_, function, class_, documented, undocumented, typed, untyped, partially_typed, fully_typed)
 
-# File: symbex/lib.py Line: 11
+# File: symbex/lib.py Line: 105
+def function_definition(function_node: AST)
+
+# File: symbex/lib.py Line: 12
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 159
+# File: symbex/lib.py Line: 173
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 193
+# File: symbex/lib.py Line: 207
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 211
+# File: symbex/lib.py Line: 225
 def read_file(path)
 
-# File: symbex/lib.py Line: 237
+# File: symbex/lib.py Line: 251
 class TypeSummary
 
-# File: symbex/lib.py Line: 242
+# File: symbex/lib.py Line: 256
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 35
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool) -> Tuple[(str, int)]
+# File: symbex/lib.py Line: 302
+def quoted_string(s)
 
-# File: symbex/lib.py Line: 66
-def match(name: str, symbols: Iterable[str]) -> bool
+# File: symbex/lib.py Line: 36
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 91
-def function_definition(function_node: AST)
+# File: symbex/lib.py Line: 70
+def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
+
+# File: symbex/lib.py Line: 80
+def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
+To include docstrings in those signatures, use `--docstrings`:
+```bash
+symbex --docstrings --documented -f symbex/lib.py
+```
+
+<!-- [[[cog
+runner = CliRunner()
+result = runner.invoke(cli, ["--docstrings", "--documented", "-f", str(path / "lib.py")])
+# Need a consistent sort order
+chunks = result.stdout.strip().split("\n\n")
+chunks.sort()
+cog.out(
+    "```python\n{}\n```\n".format("\n\n".join(chunks))
+)
+]]] -->
+```python
+# File: symbex/lib.py Line: 12
+def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
+    "Returns ast Nodes matching symbols"
+
+# File: symbex/lib.py Line: 36
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
+    "Returns the code for a given node"
+
+# File: symbex/lib.py Line: 80
+def match(name: str, symbols: Iterable[str]) -> bool
+    "Returns True if name matches any of the symbols, resolving wildcards"
+```
+<!-- [[[end]]] -->
+
 ## Counting symbols
 
 If you just want to count the number of functions and classes that match your filters, use the `--count` option. Here's how to count your classes:
 
 ```bash
 symbex --class --count
 ```
@@ -255,19 +294,22 @@
       symbex --async --count
 
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   -s, --signatures           Show just function and class signatures
+  --docstrings               Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
   --async                    Filter async functions
   --function                 Filter functions
   --class                    Filter classes
+  --documented               Filter functions with docstrings
+  --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --help                     Show this message and exit.
 
 ```
```

### Comparing `symbex-0.5/setup.py` & `symbex-0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.5"
+VERSION = "0.6"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-0.5/symbex/cli.py` & `symbex-0.6/symbex/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 @click.option(
     "-s",
     "--signatures",
     is_flag=True,
     help="Show just function and class signatures",
 )
 @click.option(
+    "--docstrings",
+    is_flag=True,
+    help="Show function and class signatures plus docstrings",
+)
+@click.option(
     "--count",
     is_flag=True,
     help="Show count of matching symbols",
 )
 @click.option(
     "--silent",
     is_flag=True,
@@ -54,14 +59,24 @@
 @click.option(
     "class_",
     "--class",
     is_flag=True,
     help="Filter classes",
 )
 @click.option(
+    "--documented",
+    is_flag=True,
+    help="Filter functions with docstrings",
+)
+@click.option(
+    "--undocumented",
+    is_flag=True,
+    help="Filter functions without docstrings",
+)
+@click.option(
     "--typed",
     is_flag=True,
     help="Filter functions with type annotations",
 )
 @click.option(
     "--untyped",
     is_flag=True,
@@ -78,19 +93,22 @@
     help="Filter functions with full type annotations",
 )
 def cli(
     symbols,
     files,
     directories,
     signatures,
+    docstrings,
     count,
     silent,
     async_,
     function,
     class_,
+    documented,
+    undocumented,
     typed,
     untyped,
     partially_typed,
     fully_typed,
 ):
     """
     Find symbols in Python code and print the code for them.
@@ -133,24 +151,26 @@
         # View signatures for all async functions with type definitions
         symbex --async --typed -s
 
     \b
         # Count the number of --async functions in the project
         symbex --async --count
     """
-    if count:
+    if count or docstrings:
         signatures = True
     # Show --help if no filter options are provided:
     if not any(
         [
             symbols,
             signatures,
             async_,
             function,
             class_,
+            documented,
+            undocumented,
             typed,
             untyped,
             partially_typed,
             fully_typed,
         ]
     ):
         ctx = click.get_current_context()
@@ -160,14 +180,16 @@
     if (
         any(
             [
                 signatures,
                 async_,
                 function,
                 class_,
+                documented,
+                undocumented,
                 typed,
                 untyped,
                 partially_typed,
                 fully_typed,
             ]
         )
         and not symbols
@@ -184,26 +206,42 @@
                     yield path
 
     # Filter symbols by type
     def filter(node: ast.AST) -> bool:
         return True
 
     # If any --filters were supplied, handle them:
-    if any([async_, function, class_, typed, untyped, partially_typed, fully_typed]):
+    if any(
+        [
+            async_,
+            function,
+            class_,
+            documented,
+            undocumented,
+            typed,
+            untyped,
+            partially_typed,
+            fully_typed,
+        ]
+    ):
 
         def filter(node: ast.AST) -> bool:
             # Filters must ALL match
             if async_ and not isinstance(node, ast.AsyncFunctionDef):
                 return False
             if function and not isinstance(
                 node, (ast.FunctionDef, ast.AsyncFunctionDef)
             ):
                 return False
             if class_ and not isinstance(node, ast.ClassDef):
                 return False
+            if documented and not ast.get_docstring(node):
+                return False
+            if undocumented and ast.get_docstring(node):
+                return False
             summary = type_summary(node)
             # if no summary, type filters all fail
             if not summary and (typed or untyped or partially_typed or fully_typed):
                 return False
             # Apply type filters
             if typed and not summary.partially:
                 return False
@@ -234,15 +272,17 @@
                 continue
             # If file is within pwd, print relative path
             if pwd in file.resolve().parents:
                 path = file.resolve().relative_to(pwd)
             else:
                 # else print absolute path
                 path = file.resolve()
-            snippet, line_no = code_for_node(code, node, class_name, signatures)
+            snippet, line_no = code_for_node(
+                code, node, class_name, signatures, docstrings
+            )
             bits = ["# File:", path]
             if class_name:
                 bits.extend(["Class:", class_name])
             bits.extend(["Line:", line_no])
             print(*bits)
             print(snippet)
             print()
```

### Comparing `symbex-0.5/symbex/lib.py` & `symbex-0.6/symbex/lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import fnmatch
 import ast
 from ast import literal_eval, parse, AST, AsyncFunctionDef, FunctionDef, ClassDef
 import codecs
 from dataclasses import dataclass
 from itertools import zip_longest
 import re
+import textwrap
 from typing import Iterable, List, Optional, Tuple
 
 
 def find_symbol_nodes(
     code: str, filename: str, symbols: Iterable[str]
 ) -> List[Tuple[AST, Optional[str]]]:
     "Returns ast Nodes matching symbols"
@@ -29,28 +30,31 @@
                     if match(qualified_name, symbols):
                         matches.append((child, name))
 
     return matches
 
 
 def code_for_node(
-    code: str, node: AST, class_name: str, signatures: bool
+    code: str, node: AST, class_name: str, signatures: bool, docstrings: bool
 ) -> Tuple[str, int]:
     "Returns the code for a given node"
     lines = code.split("\n")
     start = None
     end = None
     if signatures:
         if isinstance(node, (FunctionDef, AsyncFunctionDef)):
             definition, lineno = function_definition(node), node.lineno
             if class_name:
                 definition = "    " + definition
+            definition = add_docstring(definition, node, docstrings, bool(class_name))
             return definition, lineno
         elif isinstance(node, ClassDef):
-            return class_definition(node), node.lineno
+            definition, lineno = class_definition(node), node.lineno
+            definition = add_docstring(definition, node, docstrings, bool(class_name))
+            return definition, lineno
         else:
             # Not a function or class, fall back on just the line
             start = node.lineno - 1
             end = node.lineno
     else:
         # If the node has decorator_list, include those too
         if getattr(node, "decorator_list", None):
@@ -59,14 +63,24 @@
             start = node.lineno - 1
         end = node.end_lineno
     output = "\n".join(lines[start:end])
     # If it's in a class, indent it 4 spaces
     return output, start + 1
 
 
+def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str:
+    if not docstrings:
+        return definition
+    docstring = ast.get_docstring(node)
+    if not docstring:
+        return definition
+    docstring = quoted_string(docstring)
+    return f"{definition}\n{textwrap.indent(docstring, '        ' if is_method else '    ')}"
+
+
 def match(name: str, symbols: Iterable[str]) -> bool:
     "Returns True if name matches any of the symbols, resolving wildcards"
     if name is None:
         return False
     for search in symbols:
         if "*" not in search:
             # Exact matches only
@@ -279,7 +293,18 @@
             # Doesn't matter if we have a return type
             fully = True
 
     return TypeSummary(
         fully=fully,
         partially=partially,
     )
+
+
+def quoted_string(s):
+    if "\n" in s:
+        # Escape triple double quotes
+        s = s.replace('"""', '\\"\\"\\"')
+        return f'"""{s}"""'
+    else:
+        # Escape double quotes
+        s = s.replace('"', '\\"')
+        return f'"{s}"'
```

### Comparing `symbex-0.5/symbex.egg-info/PKG-INFO` & `symbex-0.6/symbex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.5
+Version: 0.6
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -18,14 +18,16 @@
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
 Find the Python code for specified symbols
 
+Read [symbex: search Python code for functions and classes, then pipe them into a LLM](https://simonwillison.net/2023/Jun/18/symbex/) for background on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install symbex
 ```
 ## Usage
@@ -81,14 +83,16 @@
 In addition to searching for symbols, you can apply filters to the results.
 
 The following filters are available:
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
+- `--documented` - functions/classes that have a docstring
+- `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
 
@@ -135,65 +139,100 @@
 ```
 ### Just the signatures
 
 The `-s/--signatures` option will list just the signatures of the functions and classes, for example:
 ```bash
 symbex -s -d symbex
 ```
-
 <!-- [[[cog
 import cog
 from click.testing import CliRunner
 import pathlib
 from symbex.cli import cli
 
 path = pathlib.Path("symbex").resolve()
 runner = CliRunner()
 result = runner.invoke(cli, ["-s", "-d", str(path)])
 # Need a consistent sort order
 chunks = result.stdout.strip().split("\n\n")
 chunks.sort()
 cog.out(
-    "```\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format("\n\n".join(chunks))
 )
 ]]] -->
-```
-# File: symbex/cli.py Line: 80
-def cli(symbols, files, directories, signatures, count, silent, async_, function, class_, typed, untyped, partially_typed, fully_typed)
+```python
+# File: symbex/cli.py Line: 95
+def cli(symbols, files, directories, signatures, docstrings, count, silent, async_, function, class_, documented, undocumented, typed, untyped, partially_typed, fully_typed)
 
-# File: symbex/lib.py Line: 11
+# File: symbex/lib.py Line: 105
+def function_definition(function_node: AST)
+
+# File: symbex/lib.py Line: 12
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 159
+# File: symbex/lib.py Line: 173
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 193
+# File: symbex/lib.py Line: 207
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 211
+# File: symbex/lib.py Line: 225
 def read_file(path)
 
-# File: symbex/lib.py Line: 237
+# File: symbex/lib.py Line: 251
 class TypeSummary
 
-# File: symbex/lib.py Line: 242
+# File: symbex/lib.py Line: 256
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 35
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool) -> Tuple[(str, int)]
+# File: symbex/lib.py Line: 302
+def quoted_string(s)
 
-# File: symbex/lib.py Line: 66
-def match(name: str, symbols: Iterable[str]) -> bool
+# File: symbex/lib.py Line: 36
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 91
-def function_definition(function_node: AST)
+# File: symbex/lib.py Line: 70
+def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
+
+# File: symbex/lib.py Line: 80
+def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
+To include docstrings in those signatures, use `--docstrings`:
+```bash
+symbex --docstrings --documented -f symbex/lib.py
+```
+
+<!-- [[[cog
+runner = CliRunner()
+result = runner.invoke(cli, ["--docstrings", "--documented", "-f", str(path / "lib.py")])
+# Need a consistent sort order
+chunks = result.stdout.strip().split("\n\n")
+chunks.sort()
+cog.out(
+    "```python\n{}\n```\n".format("\n\n".join(chunks))
+)
+]]] -->
+```python
+# File: symbex/lib.py Line: 12
+def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
+    "Returns ast Nodes matching symbols"
+
+# File: symbex/lib.py Line: 36
+def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
+    "Returns the code for a given node"
+
+# File: symbex/lib.py Line: 80
+def match(name: str, symbols: Iterable[str]) -> bool
+    "Returns True if name matches any of the symbols, resolving wildcards"
+```
+<!-- [[[end]]] -->
+
 ## Counting symbols
 
 If you just want to count the number of functions and classes that match your filters, use the `--count` option. Here's how to count your classes:
 
 ```bash
 symbex --class --count
 ```
@@ -270,19 +309,22 @@
       symbex --async --count
 
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   -s, --signatures           Show just function and class signatures
+  --docstrings               Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
   --async                    Filter async functions
   --function                 Filter functions
   --class                    Filter classes
+  --documented               Filter functions with docstrings
+  --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --help                     Show this message and exit.
 
 ```
```

### Comparing `symbex-0.5/tests/test_filters.py` & `symbex-0.6/tests/test_filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -133,14 +133,46 @@
             ["--fully-typed", "*.*"],
             ["def method_types", "def __init__", "def method_fully_typed"],
         ),
         (
             ["--partially-typed", "*.*"],
             ["def method_partially_typed"],
         ),
+        # Documented and undocumented
+        (
+            ["--documented"],
+            [
+                "def func_no_args",
+                "def func_positional_args",
+            ],
+        ),
+        (
+            ["--undocumented", "func_arbitrary_*"],
+            [
+                "def func_arbitrary_positional_args",
+                "def func_arbitrary_keyword_args",
+                "def func_arbitrary_args",
+            ],
+        ),
+        (
+            ["--documented", "*.*"],
+            [
+                "def method_fully_typed",
+                "def method_partially_typed",
+            ],
+        ),
+        (
+            ["--undocumented", "*.method_*"],
+            [
+                "def method_types",
+                "def method_positional_only_args",
+                "def method_keyword_only_args",
+                "def method_untyped",
+            ],
+        ),
     ),
 )
 def test_filters(args, expected):
     runner = CliRunner()
     full_args = args + [
         "-s",
         "-f",
```

### Comparing `symbex-0.5/tests/test_symbex.py` & `symbex-0.6/tests/test_symbex.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 import pytest
 import textwrap
 from click.testing import CliRunner
 
 from symbex.cli import cli
-from symbex.lib import read_file
+from symbex.lib import read_file, quoted_string
 
 
 def test_no_args_shows_help():
     runner = CliRunner()
     result = runner.invoke(cli, catch_exceptions=False)
     assert result.exit_code == 0
     assert "Usage: cli [OPTIONS]" in result.stdout
@@ -194,7 +194,33 @@
     text = read_file(path)
     assert text == (
         "# coding: iso-8859-5\n"
         "# (Unlikely to be the default encoding for most testers.)\n"
         "# БЖџрстуфхцчшщъыьэюя <- Cyrillic characters\n"
         'u = "Ўт№Ф"\n'
     )
+
+
+def test_quoted_string():
+    # Single line, no quotes
+    assert quoted_string("Hello, World!") == '"Hello, World!"'
+
+    # Single line, with quotes
+    assert quoted_string('Hello, "World"!') == '"Hello, \\"World\\"!"'
+
+    # Multiline, no quotes
+    multiline_str = "Hello,\nWorld!"
+    expected_result = '"""Hello,\nWorld!"""'
+    assert quoted_string(multiline_str) == expected_result
+
+    # Multiline, with triple quotes
+    multiline_str = '''Hello,
+"World",
+Here are some triple quotes: """ '''
+    expected_multiline_result = (
+        '"""Hello,\n"World",\nHere are some triple quotes: \\"\\"\\" """'
+    )
+    quoted_multiline_result = quoted_string(multiline_str)
+    assert quoted_multiline_result == expected_multiline_result
+
+    # Empty string
+    assert quoted_string("") == '""'
```

### Comparing `symbex-0.5/tests/test_symbols.py` & `symbex-0.6/tests/test_symbols.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Tests for "symbex -s", using content of example_code.py
 import pathlib
 import pytest
+import re
 from click.testing import CliRunner
 
 from symbex.cli import cli
 
 
 @pytest.fixture
 def symbols_text():
@@ -63,11 +64,48 @@
         "-s",
         "-f",
         str(pathlib.Path(__file__).parent / "example_symbols.py"),
     ]
     result = runner.invoke(cli, args, catch_exceptions=False)
     assert result.exit_code == 0
     assert result.stdout == (
-        "# File: tests/example_symbols.py Class: ClassWithMethods Line: 88\n"
+        "# File: tests/example_symbols.py Class: ClassWithMethods Line: 91\n"
         "    async def async_method(a, b, c)\n"
         "\n"
     )
+
+
+def test_docstrings():
+    runner = CliRunner()
+    args = [
+        "*.*",
+        "*",
+        "--documented",
+        "--docstrings",
+        "-f",
+        str(pathlib.Path(__file__).parent / "example_symbols.py"),
+    ]
+    result = runner.invoke(cli, args, catch_exceptions=False)
+    assert result.exit_code == 0
+    expected = """
+# File: tests/example_symbols.py Line: X
+def func_no_args()
+    "This has a single line docstring"
+
+# File: tests/example_symbols.py Line: X
+def func_positional_args(a, b, c)
+    \"\"\"This has a
+    multi-line docstring\"\"\"
+
+# File: tests/example_symbols.py Class: ClassForTypedTests Line: X
+    def method_fully_typed(self, a: int, b: str) -> bool
+        "Single line"
+
+# File: tests/example_symbols.py Class: ClassForTypedTests Line: X
+    def method_partially_typed(self, a: int, b) -> bool
+        \"\"\"Multiple
+        lines\"\"\"
+    """.strip()
+    actual = result.stdout.strip()
+    # Replace 'Line \d' with 'Line X' before comparison using re
+    actual = re.sub(r"Line: \d+", "Line: X", actual)
+    assert actual == expected
```

