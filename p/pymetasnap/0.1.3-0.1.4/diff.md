# Comparing `tmp/pymetasnap-0.1.3.tar.gz` & `tmp/pymetasnap-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.1.3.tar", max compression
+gzip compressed data, was "pymetasnap-0.1.4.tar", max compression
```

## Comparing `pymetasnap-0.1.3.tar` & `pymetasnap-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/LICENSE
--rw-r--r--   0        0        0     2927 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/__init__.py
--rw-r--r--   0        0        0     2403 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/core.py
--rw-r--r--   0        0        0     1286 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/main.py
--rw-r--r--   0        0        0     2550 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/render.py
--rw-r--r--   0        0        0     1916 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/utils.py
--rw-r--r--   0        0        0      823 2023-06-14 14:41:25.956433 pymetasnap-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/__init__.py
+-rw-r--r--   0        0        0      684 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/checks.py
+-rw-r--r--   0        0        0     3118 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/core.py
+-rw-r--r--   0        0        0     1276 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/main.py
+-rw-r--r--   0        0        0     2550 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/render.py
+-rw-r--r--   0        0        0     1916 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/utils.py
+-rw-r--r--   0        0        0      845 2023-06-21 19:37:29.981801 pymetasnap-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.1.4/PKG-INFO
```

### Comparing `pymetasnap-0.1.3/LICENSE` & `pymetasnap-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.3/README.md` & `pymetasnap-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.3/extractor/main.py` & `pymetasnap-0.1.4/extractor/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from enum import Enum
 from pathlib import Path
 
 import typer
 from typing_extensions import Annotated
 
-from extractor.core import generate_data
-from extractor.utils import get_version_from_pyproject
+from extractor.core import extract_data, save_data
 
 app = typer.Typer()
 
 
 class RequirementsFormat(str, Enum):
     pip_list = "pip_list"
     pip_freeze = "pip_freeze"
 
 
-@app.command(name="version")
-def version():
-    return print(get_version_from_pyproject())
+# @app.command(name="version")
+# def version():
+#     return print(get_version_from_pyproject())
 
 
 @app.command(name="extract")
-def main(
+def extract(
     source_path: Annotated[
         Path,
         typer.Option(
             exists=True,
             file_okay=True,
             dir_okay=False,
             writable=False,
@@ -47,12 +46,13 @@
         ),
     ] = "",
     format: Annotated[
         RequirementsFormat,
         typer.Option(prompt=True, help="Incoming requirements format."),
     ] = RequirementsFormat.pip_freeze,
 ):
-    generate_data(source_path, output, format)
+    data = extract_data(source_path, format)
+    save_data(data, output)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pymetasnap-0.1.3/extractor/render.py` & `pymetasnap-0.1.4/extractor/render.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.3/extractor/utils.py` & `pymetasnap-0.1.4/extractor/utils.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.3/pyproject.toml` & `pymetasnap-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.1.3"
+version = "0.1.4"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
@@ -24,11 +24,12 @@
 
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^23.3.0", allow-prereleases = true}
 pytest = "^7.3.1"
 pylint = "^2.17.4"
 pre-commit = "^3.3.2"
+jupyterlab = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pymetasnap-0.1.3/PKG-INFO` & `pymetasnap-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

