# Comparing `tmp/mizue-0.3.2.tar.gz` & `tmp/mizue-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.3.2.tar", last modified: Tue Jun 20 16:25:04 2023, max compression
+gzip compressed data, was "mizue-0.3.3.tar", last modified: Wed Jun 21 18:18:22 2023, max compression
```

## Comparing `mizue-0.3.2.tar` & `mizue-0.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 16:24:48.000000 mizue-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-20 16:25:04.775235 mizue-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-20 16:24:48.000000 mizue-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/file/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/file/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/network/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/network/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/network/downloader/data/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/downloader/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/downloader/download_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/downloader/download_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/downloader/downloader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/network/downloader/progress_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/printer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/printer/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/border_character_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/border_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/cell_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/grid/row_border_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/printer/terminal_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/progress/colorful_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/progress/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/progress/progress_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue/util/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/util/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/util/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/util/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-20 16:24:48.000000 mizue-0.3.2/mizue/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:25:04.775235 mizue-0.3.2/mizue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-20 16:25:04.000000 mizue-0.3.2/mizue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 16:25:04.000000 mizue-0.3.2/mizue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:25:04.000000 mizue-0.3.2/mizue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 16:25:04.000000 mizue-0.3.2/mizue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 16:25:04.000000 mizue-0.3.2/mizue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:25:04.775235 mizue-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 16:25:03.000000 mizue-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 18:18:05.000000 mizue-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-21 18:18:22.543189 mizue-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-21 18:18:05.000000 mizue-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/colorful_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.543189 mizue-0.3.3/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-21 18:18:05.000000 mizue-0.3.3/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:18:22.539189 mizue-0.3.3/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:18:22.000000 mizue-0.3.3/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:18:22.543189 mizue-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 18:18:20.000000 mizue-0.3.3/setup.py
```

### Comparing `mizue-0.3.2/LICENSE` & `mizue-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/PKG-INFO` & `mizue-0.3.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: mizue
-Version: 0.3.2
-Summary: A Python package for various utilities
-Author: Hoshilily
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 A simple package containing various command-line utilities.
 
 ## Table of Contents
 - [Caution](#caution)
 - [Installation](#installation)
 - [Utilities](#contents)
   - [Printer](#printer)
@@ -33,14 +21,50 @@
 ```
 
 ## Utilities (Work in Progress)
 - [Printer](#printer)
 - [Progress](#progress)
 - More utilities coming soon...
 
+
+### Grid
+
+This class can be used to print a table/grid in the terminal.
+
+```python
+from mizue.printer.grid import Grid, ColumnSettings, Alignment
+from mizue.file import FileUtils
+import os
+
+column2 = ColumnSettings(title='File', alignment=Alignment.RIGHT)
+column3 = ColumnSettings(title='Size', alignment=Alignment.CENTER, width=50)
+columns = [column2, column3]
+
+
+filelist = FileUtils.list_files(".", recursive=True, fullpath=True)
+grid_data = list(map(lambda f: [f, FileUtils.get_readable_file_size(os.stat(f).st_size)], filelist))
+grid = Grid(columns, grid_data)
+grid.print()
+```
+
+`ColumnSettings` allows the following attributes to be set:
+- `title`: The title of the column
+- `alignment`: The alignment of the column
+- `width`: The width of the column
+- `renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the column
+
+`Grid` allows the following attributes to be set:
+- `border_color`: The color of the border in hex format
+- `border_style`: The style of the border. Can be one of the following: 
+  - ``BorderStyle.SINGLE`` 
+  - ``BorderStyle.DOUBLE`` 
+  - ``BorderStyle.BASIC`` 
+  - ``BorderStyle.NONE``
+- `cell_renderer`: A function that takes in an object of type ``CellRendererArgs`` and returns a string to be displayed in the cell
+
 ### Printer
 
 This class contains various static methods for printing text in different colors.
 
 ```python
 from mizue.printer import Printer
 
@@ -116,8 +140,8 @@
 progress.start()
 
 for i in range(1200):
   progress.update_value(i)
   sleep(0.1)
 
 progress.stop()
-```
+```
```

### Comparing `mizue-0.3.2/mizue/file/fileutils.py` & `mizue-0.3.3/mizue/file/fileutils.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/network/downloader/data/colors.json` & `mizue-0.3.3/mizue/network/downloader/data/colors.json`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/network/downloader/download_event.py` & `mizue-0.3.3/mizue/network/downloader/download_event.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/network/downloader/downloader.py` & `mizue-0.3.3/mizue/network/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/network/downloader/downloader_tool.py` & `mizue-0.3.3/mizue/network/downloader/downloader_tool.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/printer/grid/border_character_codes.py` & `mizue-0.3.3/mizue/printer/grid/border_character_codes.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/printer/grid/column.py` & `mizue-0.3.3/mizue/printer/grid/column.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/printer/grid/grid.py` & `mizue-0.3.3/mizue/printer/grid/grid.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/printer/printer.py` & `mizue-0.3.3/mizue/printer/printer.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/progress/colorful_progress.py` & `mizue-0.3.3/mizue/progress/colorful_progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/progress/progress.py` & `mizue-0.3.3/mizue/progress/progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/progress/progress_renderer_args.py` & `mizue-0.3.3/mizue/progress/progress_renderer_args.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/progress/spinner.py` & `mizue-0.3.3/mizue/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/util/event_listener.py` & `mizue-0.3.3/mizue/util/event_listener.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/util/signal_handler.py` & `mizue-0.3.3/mizue/util/signal_handler.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue/util/utility.py` & `mizue-0.3.3/mizue/util/utility.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/mizue.egg-info/SOURCES.txt` & `mizue-0.3.3/mizue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizue-0.3.2/setup.py` & `mizue-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="mizue",
-    version="0.3.2",
+    version="0.3.3",
     description="A Python package for various utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hoshilily",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

