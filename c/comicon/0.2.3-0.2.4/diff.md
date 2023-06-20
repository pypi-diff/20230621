# Comparing `tmp/comicon-0.2.3.tar.gz` & `tmp/comicon-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicon-0.2.3.tar", max compression
+gzip compressed data, was "comicon-0.2.4.tar", max compression
```

## Comparing `comicon-0.2.3.tar` & `comicon-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34520 2023-01-19 01:21:43.343731 comicon-0.2.3/LICENSE
--rw-r--r--   0        0        0     1493 2023-01-24 02:59:24.432940 comicon-0.2.3/README.md
--rw-r--r--   0        0        0      348 2023-01-19 03:38:16.600950 comicon-0.2.3/comicon/__init__.py
--rw-r--r--   0        0        0      585 2023-01-19 03:20:26.070654 comicon-0.2.3/comicon/api.py
--rw-r--r--   0        0        0     1034 2023-02-14 03:05:01.345420 comicon-0.2.3/comicon/base.py
--rw-r--r--   0        0        0     3548 2023-04-09 23:32:40.814526 comicon-0.2.3/comicon/cirtools.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:14.098947 comicon-0.2.3/comicon/common/__init__.py
--rw-r--r--   0        0        0      410 2023-04-09 23:34:20.162767 comicon-0.2.3/comicon/common/cbz.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:23.310865 comicon-0.2.3/comicon/common/cir.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:16.479925 comicon-0.2.3/comicon/common/epub.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:27.834825 comicon-0.2.3/comicon/common/pdf.py
--rw-r--r--   0        0        0      810 2023-01-19 14:44:56.400117 comicon-0.2.3/comicon/errors.py
--rw-r--r--   0        0        0     1890 2023-03-10 05:20:48.406102 comicon-0.2.3/comicon/inputs/__init__.py
--rw-r--r--   0        0        0     4605 2023-04-27 21:51:31.834322 comicon-0.2.3/comicon/inputs/cbz.py
--rw-r--r--   0        0        0      631 2023-01-18 18:36:38.546802 comicon-0.2.3/comicon/inputs/cir.py
--rw-r--r--   0        0        0     5888 2023-02-11 18:50:43.896715 comicon-0.2.3/comicon/inputs/epub.py
--rw-r--r--   0        0        0     2810 2023-01-19 03:30:58.621800 comicon-0.2.3/comicon/inputs/pdf.py
--rw-r--r--   0        0        0     1873 2023-03-10 05:20:48.406102 comicon-0.2.3/comicon/outputs/__init__.py
--rw-r--r--   0        0        0     1845 2023-01-19 03:01:28.528083 comicon-0.2.3/comicon/outputs/cbz.py
--rw-r--r--   0        0        0      657 2023-01-18 19:12:20.005904 comicon-0.2.3/comicon/outputs/cir.py
--rw-r--r--   0        0        0     3117 2023-01-19 03:30:47.666814 comicon-0.2.3/comicon/outputs/epub.py
--rw-r--r--   0        0        0     1891 2023-02-11 18:47:57.091972 comicon-0.2.3/comicon/outputs/pdf.py
--rw-r--r--   0        0        0      964 2023-04-27 21:52:58.311564 comicon-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 comicon-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1493 2023-04-28 17:41:58.055636 comicon-0.2.4/README.md
+-rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-0.2.4/comicon/__init__.py
+-rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-0.2.4/comicon/api.py
+-rw-r--r--   0        0        0     1034 2023-04-28 17:41:58.057636 comicon-0.2.4/comicon/base.py
+-rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-0.2.4/comicon/cirtools.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/cbz.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/cir.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/epub.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/pdf.py
+-rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-0.2.4/comicon/errors.py
+-rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-0.2.4/comicon/inputs/__init__.py
+-rw-r--r--   0        0        0     4605 2023-04-28 17:41:58.058636 comicon-0.2.4/comicon/inputs/cbz.py
+-rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-0.2.4/comicon/inputs/cir.py
+-rw-r--r--   0        0        0     5888 2023-04-28 17:41:58.058636 comicon-0.2.4/comicon/inputs/epub.py
+-rw-r--r--   0        0        0     2810 2023-04-28 17:41:58.057636 comicon-0.2.4/comicon/inputs/pdf.py
+-rw-r--r--   0        0        0     1873 2023-04-28 17:41:58.061636 comicon-0.2.4/comicon/outputs/__init__.py
+-rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-0.2.4/comicon/outputs/cbz.py
+-rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-0.2.4/comicon/outputs/cir.py
+-rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-0.2.4/comicon/outputs/epub.py
+-rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-0.2.4/comicon/outputs/pdf.py
+-rw-r--r--   0        0        0      964 2023-06-20 22:19:39.233040 comicon-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 comicon-0.2.4/PKG-INFO
```

### Comparing `comicon-0.2.3/LICENSE` & `comicon-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/README.md` & `comicon-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/api.py` & `comicon-0.2.4/comicon/api.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/base.py` & `comicon-0.2.4/comicon/base.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/cirtools.py` & `comicon-0.2.4/comicon/cirtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,26 @@
     - `{number}.{ext}`: ordered image files representing one comic page (min. 1)
 - `cover.{ext}`: a file containing the cover of the comic. Extensions allowed include
 jpg, jpeg, png, and gif.
 
 All folders as well as the cover image must be declared in `comicon.json`. Only image
 files are allowed in the chapter folders, but any file is allowed in the root of
 the CIR folder.
+
+Extra files or folders in the CIR root will be ignored.
 """
 
 import json
 from pathlib import Path
 
 from .base import Comic
 from .errors import (
     BadImageError,
     EmptyChapterError,
     NoChaptersError,
-    UndeclaredChapterError,
     UnusedChapterError,
 )
 
 IR_DATA_FILE = "comicon.json"
 ALLOWED_COVER_EXTENSIONS = [".jpg", ".jpeg", ".png", ".gif"]
 
 
@@ -72,19 +73,14 @@
     chapter_folder_set = {f.name for f in chapter_folders}
     if diff := chapter_slugs - chapter_folder_set:
         raise UnusedChapterError(
             f"Chapters were declared in {data_file} but "
             f"were not found in the filesystem: {diff}"
         )
 
-    if diff := chapter_folder_set - chapter_slugs:
-        raise UndeclaredChapterError(
-            f"Found following chapters that were not declared in {data_file}: {diff}"
-        )
-
     # check that all chapter folders contain at least one image
     for chapter_folder in chapter_folders:
         images = sorted(f for f in chapter_folder.iterdir() if f.is_file())
         if not images:
             raise EmptyChapterError(f"{chapter_folder} is empty")
         for image in images:
             if image.suffix.lower() not in ALLOWED_COVER_EXTENSIONS:
```

### Comparing `comicon-0.2.3/comicon/inputs/__init__.py` & `comicon-0.2.4/comicon/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/inputs/cbz.py` & `comicon-0.2.4/comicon/inputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/inputs/cir.py` & `comicon-0.2.4/comicon/inputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/inputs/epub.py` & `comicon-0.2.4/comicon/inputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/inputs/pdf.py` & `comicon-0.2.4/comicon/inputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/outputs/__init__.py` & `comicon-0.2.4/comicon/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/outputs/cbz.py` & `comicon-0.2.4/comicon/outputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/outputs/cir.py` & `comicon-0.2.4/comicon/outputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/outputs/epub.py` & `comicon-0.2.4/comicon/outputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/comicon/outputs/pdf.py` & `comicon-0.2.4/comicon/outputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.3/pyproject.toml` & `comicon-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "comicon"
-version = "0.2.3"
+version = "0.2.4"
 description = "A simple comic conversion library between CBZ/EPUB/PDF"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 repository = "https://github.com/potatoeggy/comicon"
 documentation = "https://github.com/potatoeggy/comicon"
 keywords = ["converter", "comic", "cbz", "epub", "pdf"]
```

### Comparing `comicon-0.2.3/PKG-INFO` & `comicon-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicon
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple comic conversion library between CBZ/EPUB/PDF
 Home-page: https://github.com/potatoeggy/comicon
 License: AGPL-3.0-only
 Keywords: converter,comic,cbz,epub,pdf
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10
```

