# Comparing `tmp/mizue-0.3.3.tar.gz` & `tmp/mizue-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.3.3.tar", last modified: Wed Jun 21 18:18:22 2023, max compression
+gzip compressed data, was "mizue-0.3.4.tar", last modified: Wed Jun 21 18:24:38 2023, max compression
```

## Comparing `mizue-0.3.3.tar` & `mizue-0.3.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 18:18:05.000000 mizue-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-21 18:18:22.543189 mizue-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-21 18:18:05.000000 mizue-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/file/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/file/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/network/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/network/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/network/downloader/data/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/download_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/download_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/downloader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/progress_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/printer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/mizue/printer/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/border_character_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/border_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/cell_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/row_border_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/terminal_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/mizue/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/colorful_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/progress_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/mizue/util/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:18:22.543189 mizue-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 18:18:20.000000 mizue-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.354353 mizue-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 18:24:19.000000 mizue-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-21 18:24:38.354353 mizue-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-21 18:24:19.000000 mizue-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.354353 mizue-0.3.4/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/colorful_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.354353 mizue-0.3.4/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:24:38.354353 mizue-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 18:24:36.000000 mizue-0.3.4/setup.py
```

### Comparing `mizue-0.3.3/LICENSE` & `mizue-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/PKG-INFO` & `mizue-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 
 A simple package containing various command-line utilities.
 
 ## Table of Contents
 - [Caution](#caution)
 - [Installation](#installation)
 - [Utilities](#contents)
+  - [Grid](#grid)
   - [Printer](#printer)
   - [Progress](#progress)
 
 
 ## Caution
 
 **This package does not have any tests. It is not recommended to use it in production.
@@ -29,14 +30,15 @@
 ## Installation
 
 ```bash
   pip install mizue
 ```
 
 ## Utilities (Work in Progress)
+- [Grid](#grid)
 - [Printer](#printer)
 - [Progress](#progress)
 - More utilities coming soon...
 
 
 ### Grid
 
@@ -56,26 +58,29 @@
 grid_data = list(map(lambda f: [f, FileUtils.get_readable_file_size(os.stat(f).st_size)], filelist))
 grid = Grid(columns, grid_data)
 grid.print()
 ```
 
 `ColumnSettings` allows the following attributes to be set:
 - `title`: The title of the column
-- `alignment`: The alignment of the column
+- `alignment`: The alignment of the column. Can be one of the following: 
+  - ``Alignment.LEFT`` 
+  - ``Alignment.CENTER`` 
+  - ``Alignment.RIGHT``
 - `width`: The width of the column
-- `renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the column
+- `renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the column.
 
 `Grid` allows the following attributes to be set:
 - `border_color`: The color of the border in hex format
 - `border_style`: The style of the border. Can be one of the following: 
   - ``BorderStyle.SINGLE`` 
   - ``BorderStyle.DOUBLE`` 
   - ``BorderStyle.BASIC`` 
   - ``BorderStyle.NONE``
-- `cell_renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the cell
+- `cell_renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the cell.
 
 ### Printer
 
 This class contains various static methods for printing text in different colors.
 
 ```python
 from mizue.printer import Printer
```

### Comparing `mizue-0.3.3/README.md` & `mizue-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 A simple package containing various command-line utilities.
 
 ## Table of Contents
 - [Caution](#caution)
 - [Installation](#installation)
 - [Utilities](#contents)
+  - [Grid](#grid)
   - [Printer](#printer)
   - [Progress](#progress)
 
 
 ## Caution
 
 **This package does not have any tests. It is not recommended to use it in production.
@@ -17,14 +18,15 @@
 ## Installation
 
 ```bash
   pip install mizue
 ```
 
 ## Utilities (Work in Progress)
+- [Grid](#grid)
 - [Printer](#printer)
 - [Progress](#progress)
 - More utilities coming soon...
 
 
 ### Grid
 
@@ -44,26 +46,29 @@
 grid_data = list(map(lambda f: [f, FileUtils.get_readable_file_size(os.stat(f).st_size)], filelist))
 grid = Grid(columns, grid_data)
 grid.print()
 ```
 
 `ColumnSettings` allows the following attributes to be set:
 - `title`: The title of the column
-- `alignment`: The alignment of the column
+- `alignment`: The alignment of the column. Can be one of the following: 
+  - ``Alignment.LEFT`` 
+  - ``Alignment.CENTER`` 
+  - ``Alignment.RIGHT``
 - `width`: The width of the column
-- `renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the column
+- `renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the column.
 
 `Grid` allows the following attributes to be set:
 - `border_color`: The color of the border in hex format
 - `border_style`: The style of the border. Can be one of the following: 
   - ``BorderStyle.SINGLE`` 
   - ``BorderStyle.DOUBLE`` 
   - ``BorderStyle.BASIC`` 
   - ``BorderStyle.NONE``
-- `cell_renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the cell
+- `cell_renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the cell.
 
 ### Printer
 
 This class contains various static methods for printing text in different colors.
 
 ```python
 from mizue.printer import Printer
```

### Comparing `mizue-0.3.3/mizue/file/fileutils.py` & `mizue-0.3.4/mizue/file/fileutils.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/network/downloader/data/colors.json` & `mizue-0.3.4/mizue/network/downloader/data/colors.json`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/network/downloader/download_event.py` & `mizue-0.3.4/mizue/network/downloader/download_event.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/network/downloader/downloader.py` & `mizue-0.3.4/mizue/network/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/network/downloader/downloader_tool.py` & `mizue-0.3.4/mizue/network/downloader/downloader_tool.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/printer/grid/border_character_codes.py` & `mizue-0.3.4/mizue/printer/grid/border_character_codes.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/printer/grid/column.py` & `mizue-0.3.4/mizue/printer/grid/column.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/printer/grid/grid.py` & `mizue-0.3.4/mizue/printer/grid/grid.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/printer/printer.py` & `mizue-0.3.4/mizue/printer/printer.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/progress/colorful_progress.py` & `mizue-0.3.4/mizue/progress/colorful_progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/progress/progress.py` & `mizue-0.3.4/mizue/progress/progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/progress/progress_renderer_args.py` & `mizue-0.3.4/mizue/progress/progress_renderer_args.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/progress/spinner.py` & `mizue-0.3.4/mizue/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/util/event_listener.py` & `mizue-0.3.4/mizue/util/event_listener.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/util/signal_handler.py` & `mizue-0.3.4/mizue/util/signal_handler.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue/util/utility.py` & `mizue-0.3.4/mizue/util/utility.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/mizue.egg-info/PKG-INFO` & `mizue-0.3.4/mizue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 
 A simple package containing various command-line utilities.
 
 ## Table of Contents
 - [Caution](#caution)
 - [Installation](#installation)
 - [Utilities](#contents)
+  - [Grid](#grid)
   - [Printer](#printer)
   - [Progress](#progress)
 
 
 ## Caution
 
 **This package does not have any tests. It is not recommended to use it in production.
@@ -29,14 +30,15 @@
 ## Installation
 
 ```bash
   pip install mizue
 ```
 
 ## Utilities (Work in Progress)
+- [Grid](#grid)
 - [Printer](#printer)
 - [Progress](#progress)
 - More utilities coming soon...
 
 
 ### Grid
 
@@ -56,26 +58,29 @@
 grid_data = list(map(lambda f: [f, FileUtils.get_readable_file_size(os.stat(f).st_size)], filelist))
 grid = Grid(columns, grid_data)
 grid.print()
 ```
 
 `ColumnSettings` allows the following attributes to be set:
 - `title`: The title of the column
-- `alignment`: The alignment of the column
+- `alignment`: The alignment of the column. Can be one of the following: 
+  - ``Alignment.LEFT`` 
+  - ``Alignment.CENTER`` 
+  - ``Alignment.RIGHT``
 - `width`: The width of the column
-- `renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the column
+- `renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the column.
 
 `Grid` allows the following attributes to be set:
 - `border_color`: The color of the border in hex format
 - `border_style`: The style of the border. Can be one of the following: 
   - ``BorderStyle.SINGLE`` 
   - ``BorderStyle.DOUBLE`` 
   - ``BorderStyle.BASIC`` 
   - ``BorderStyle.NONE``
-- `cell_renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the cell
+- `cell_renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the cell.
 
 ### Printer
 
 This class contains various static methods for printing text in different colors.
 
 ```python
 from mizue.printer import Printer
```

### Comparing `mizue-0.3.3/mizue.egg-info/SOURCES.txt` & `mizue-0.3.4/mizue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizue-0.3.3/setup.py` & `mizue-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="mizue",
-    version="0.3.3",
+    version="0.3.4",
     description="A Python package for various utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hoshilily",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

