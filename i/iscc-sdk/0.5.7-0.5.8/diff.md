# Comparing `tmp/iscc_sdk-0.5.7.tar.gz` & `tmp/iscc_sdk-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscc_sdk-0.5.7.tar", max compression
+gzip compressed data, was "iscc_sdk-0.5.8.tar", max compression
```

## Comparing `iscc_sdk-0.5.7.tar` & `iscc_sdk-0.5.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      895 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/__init__.py
--rw-r--r--   0        0        0     4346 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/audio.py
--rw-r--r--   0        0        0     5183 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/cli.py
--rw-r--r--   0        0        0       99 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/compat.py
--rw-r--r--   0        0        0      897 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/docx_.py
--rw-r--r--   0        0        0     1491 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/epub.py
--rw-r--r--   0        0        0      166 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/exceptions.py
--rw-r--r--   0        0        0     8091 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/image.py
--rw-r--r--   0        0        0      683 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/install.py
--rw-r--r--   0        0        0     1274 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/ipfs.py
--rw-r--r--   0        0        0     7218 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/main.py
--rw-r--r--   0        0        0     9258 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/mediatype.py
--rw-r--r--   0        0        0     1898 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/metadata.py
--rw-r--r--   0        0        0     1905 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/monkeys.py
--rw-r--r--   0        0        0     3021 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/mp7.py
--rw-r--r--   0        0        0     2886 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/options.py
--rw-r--r--   0        0        0     2502 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/pdf.py
--rw-r--r--   0        0        0     5761 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/text.py
--rw-r--r--   0        0        0      684 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/thumbnail.py
--rw-r--r--   0        0        0    21133 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/tools.py
--rw-r--r--   0        0        0      602 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/utils.py
--rw-r--r--   0        0        0     6067 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/video.py
--rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.7/LICENSE
--rw-r--r--   0        0        0     3343 2023-06-21 15:10:58.024147 iscc_sdk-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3562 2023-06-21 15:10:58.024147 iscc_sdk-0.5.7/README.md
--rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 iscc_sdk-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      895 2023-06-21 19:32:14.804988 iscc_sdk-0.5.8/iscc_sdk/__init__.py
+-rw-r--r--   0        0        0     4346 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/audio.py
+-rw-r--r--   0        0        0     5272 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/cli.py
+-rw-r--r--   0        0        0       99 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/compat.py
+-rw-r--r--   0        0        0      897 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/docx_.py
+-rw-r--r--   0        0        0     1491 2023-06-21 19:32:14.796759 iscc_sdk-0.5.8/iscc_sdk/epub.py
+-rw-r--r--   0        0        0      166 2023-06-21 19:32:14.797758 iscc_sdk-0.5.8/iscc_sdk/exceptions.py
+-rw-r--r--   0        0        0     8091 2023-06-21 19:32:14.797758 iscc_sdk-0.5.8/iscc_sdk/image.py
+-rw-r--r--   0        0        0      683 2023-06-21 19:32:14.798760 iscc_sdk-0.5.8/iscc_sdk/install.py
+-rw-r--r--   0        0        0     1274 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/ipfs.py
+-rw-r--r--   0        0        0     7218 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/main.py
+-rw-r--r--   0        0        0     9258 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/mediatype.py
+-rw-r--r--   0        0        0     1898 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/metadata.py
+-rw-r--r--   0        0        0     1905 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/monkeys.py
+-rw-r--r--   0        0        0     3021 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/mp7.py
+-rw-r--r--   0        0        0     2886 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/options.py
+-rw-r--r--   0        0        0     2502 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/pdf.py
+-rw-r--r--   0        0        0     5761 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/text.py
+-rw-r--r--   0        0        0      684 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/thumbnail.py
+-rw-r--r--   0        0        0    21133 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/tools.py
+-rw-r--r--   0        0        0      602 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/utils.py
+-rw-r--r--   0        0        0     6067 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/video.py
+-rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.8/LICENSE
+-rw-r--r--   0        0        0     3343 2023-06-21 19:32:14.735278 iscc_sdk-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3562 2023-06-21 19:32:14.735278 iscc_sdk-0.5.8/README.md
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 iscc_sdk-0.5.8/PKG-INFO
```

### Comparing `iscc_sdk-0.5.7/iscc_sdk/__init__.py` & `iscc_sdk-0.5.8/iscc_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ISCC - Software Development Kit."""
 import os
 from platformdirs import PlatformDirs
 
-__version__ = "0.5.7"
+__version__ = "0.5.8"
 APP_NAME = "iscc-sdk"
 APP_AUTHOR = "iscc"
 dirs = PlatformDirs(appname=APP_NAME, appauthor=APP_AUTHOR)
 os.makedirs(dirs.user_data_dir, exist_ok=True)
 os.environ["LOGURU_AUTOINIT"] = "False"
```

### Comparing `iscc_sdk-0.5.7/iscc_sdk/audio.py` & `iscc_sdk-0.5.8/iscc_sdk/audio.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/cli.py` & `iscc_sdk-0.5.8/iscc_sdk/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from typing import Iterator, Optional, Tuple
 from loguru import logger as log
 import typer
 from pathlib import Path
+import iscc_core as ic
 import iscc_sdk as idk
 from rich.console import Console
 from rich.progress import (
     Progress,
     BarColumn,
     TextColumn,
     TransferSpeedColumn,
@@ -15,32 +16,35 @@
     DownloadColumn,
 )
 
 console = Console()
 app = typer.Typer(add_completion=False, no_args_is_help=True)
 
 
-def log_formatter(record: dict) -> str:  # pragma: no cover
+def _log_formatter(record: dict) -> str:  # pragma: no cover
     """Log message formatter"""
     color_map = {
         "TRACE": "blue",
         "DEBUG": "cyan",
         "INFO": "bold",
         "SUCCESS": "bold green",
         "WARNING": "yellow",
         "ERROR": "bold red",
         "CRITICAL": "bold white on red",
     }
     lvl_color = color_map.get(record["level"].name, "cyan")
     return (
-        "[not bold green]{time:YYYY/MM/DD HH:mm:ss}[/not bold green] | {module:<12} | {level}"
+        "[not bold green]{time:YYYY/MM/DD HH:mm:ss}[/not bold green] | {module:<12} | {line:<3} | {level.icon}"
         + f"  - [{lvl_color}]{{message}}[/{lvl_color}]"
     )
 
 
+log.add(console.print, level="DEBUG", format=_log_formatter, colorize=True)
+
+
 def iter_unprocessed(path, root_path=None):
     # type: (str|Path, Optional[str|Path]) -> Iterator[Tuple[Path, int]]
     """
     Walk directory tree recursively with deterministic ordering and yield tuples of file metadata.
 
     Metadata = (relpath, size)
 
@@ -65,15 +69,15 @@
         for dir_entry in dirs:
             yield from iter_unprocessed(Path(dir_entry.path), root_path=root_path)
 
         # Process files in the current directory
         for file_entry in files:
             file_path = Path(file_entry)
             # Ignore result files
-            if file_path.name.endswith(".iscc.json"):
+            if file_path.name.endswith(".iscc.json") or file_path.name.endswith(".iscc.mp7sig"):
                 continue
             # Ignore files that have results
             if Path(file_path.as_posix() + ".iscc.json").exists():
                 continue
             file_size = file_entry.stat().st_size
             yield file_path, file_size
 
@@ -85,26 +89,26 @@
     except Exception as e:
         return fp, e
 
 
 @app.command()
 def create(file: Path):
     """Create ISCC-CODE for single FILE."""
+    log.remove()
     if file.is_file() and file.exists():
         result = idk.code_iscc(file.as_posix())
         typer.echo(result.json(indent=2))
     else:
         typer.echo(f"Invalid file path {file}")
         raise typer.Exit(code=1)
 
 
 @app.command()
 def batch(folder: Path, workers: int = os.cpu_count()):  # pragma: no cover
     """Create ISCC-CODEs for files in FOLDER (parallel & recursive)."""
-    log.add(console.print, level="TRACE", format=log_formatter, colorize=True)
     if not folder.is_dir() or not folder.exists():
         typer.echo(f"Invalid folder {folder}")
         raise typer.Exit(1)
 
     file_paths = []
     file_sizes = []
     for path, size in iter_unprocessed(folder):
@@ -130,26 +134,29 @@
         task_id = progress.add_task("Processing", dirname=folder.name, total=total_size)
         with ProcessPoolExecutor(max_workers=workers) as executor:
             futures = [executor.submit(process_file, fp) for fp in file_paths]
             for future in as_completed(futures):
                 fp, iscc_meta = future.result()
                 if isinstance(iscc_meta, idk.IsccMeta):
                     out_path = Path(fp.as_posix() + ".iscc.json")
-                    with out_path.open(mode="wt") as outf:
+                    with out_path.open(mode="wt", encoding="utf-8") as outf:
                         outf.write(iscc_meta.json(indent=2))
                     log.info(f"Finished {fp.name}")
                 else:
-                    log.warning(f"Failed {fp.name}: {iscc_meta}")
+                    log.error(f"Failed {fp.name}: {iscc_meta}")
                 progress.update(task_id, advance=file_sizes_dict[fp], refresh=True)
 
 
 @app.command()
+def install():
+    """Install content processing tools."""
+    idk.install()
+
+
+@app.command()
 def selftest():
     """Run conformance tests."""
-    log.add(console.print, format=log_formatter, colorize=True)
-    from iscc_core.conformance import conformance_selftest
-
-    conformance_selftest()
+    ic.conformance_selftest()
 
 
 if __name__ == "__main__":  # pragma: no cover
     app()
```

### Comparing `iscc_sdk-0.5.7/iscc_sdk/docx_.py` & `iscc_sdk-0.5.8/iscc_sdk/docx_.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/epub.py` & `iscc_sdk-0.5.8/iscc_sdk/epub.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/image.py` & `iscc_sdk-0.5.8/iscc_sdk/image.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/install.py` & `iscc_sdk-0.5.8/iscc_sdk/install.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/ipfs.py` & `iscc_sdk-0.5.8/iscc_sdk/ipfs.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/main.py` & `iscc_sdk-0.5.8/iscc_sdk/main.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/mediatype.py` & `iscc_sdk-0.5.8/iscc_sdk/mediatype.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/metadata.py` & `iscc_sdk-0.5.8/iscc_sdk/metadata.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/monkeys.py` & `iscc_sdk-0.5.8/iscc_sdk/monkeys.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/mp7.py` & `iscc_sdk-0.5.8/iscc_sdk/mp7.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/options.py` & `iscc_sdk-0.5.8/iscc_sdk/options.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/pdf.py` & `iscc_sdk-0.5.8/iscc_sdk/pdf.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/text.py` & `iscc_sdk-0.5.8/iscc_sdk/text.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/thumbnail.py` & `iscc_sdk-0.5.8/iscc_sdk/thumbnail.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/tools.py` & `iscc_sdk-0.5.8/iscc_sdk/tools.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/utils.py` & `iscc_sdk-0.5.8/iscc_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/iscc_sdk/video.py` & `iscc_sdk-0.5.8/iscc_sdk/video.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/LICENSE` & `iscc_sdk-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/pyproject.toml` & `iscc_sdk-0.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iscc-sdk"
-version = "0.5.7"
+version = "0.5.8"
 description = "SDK for creating ISCCs (International Standard Content Codes)"
 authors = ["Titusz <tp@py7.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://sdk.iscc.codes"
 repository = "https://github.com/iscc/iscc-sdk"
 keywords=["iscc", "identifier", "media", "content", "hash", "blockchain", "similarity"]
```

### Comparing `iscc_sdk-0.5.7/README.md` & `iscc_sdk-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.7/PKG-INFO` & `iscc_sdk-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iscc-sdk
-Version: 0.5.7
+Version: 0.5.8
 Summary: SDK for creating ISCCs (International Standard Content Codes)
 Home-page: https://sdk.iscc.codes
 License: Apache-2.0
 Keywords: iscc,identifier,media,content,hash,blockchain,similarity
 Author: Titusz
 Author-email: tp@py7.de
 Requires-Python: >=3.8,<4.0
```

