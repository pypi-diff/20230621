# Comparing `tmp/comicon-0.2.4.tar.gz` & `tmp/comicon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicon-0.2.4.tar", max compression
+gzip compressed data, was "comicon-0.3.0.tar", max compression
```

## Comparing `comicon-0.2.4.tar` & `comicon-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-0.2.4/LICENSE
--rw-r--r--   0        0        0     1493 2023-04-28 17:41:58.055636 comicon-0.2.4/README.md
--rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-0.2.4/comicon/__init__.py
--rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-0.2.4/comicon/api.py
--rw-r--r--   0        0        0     1034 2023-04-28 17:41:58.057636 comicon-0.2.4/comicon/base.py
--rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-0.2.4/comicon/cirtools.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/__init__.py
--rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/cbz.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/cir.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/epub.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.2.4/comicon/common/pdf.py
--rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-0.2.4/comicon/errors.py
--rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-0.2.4/comicon/inputs/__init__.py
--rw-r--r--   0        0        0     4605 2023-04-28 17:41:58.058636 comicon-0.2.4/comicon/inputs/cbz.py
--rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-0.2.4/comicon/inputs/cir.py
--rw-r--r--   0        0        0     5888 2023-04-28 17:41:58.058636 comicon-0.2.4/comicon/inputs/epub.py
--rw-r--r--   0        0        0     2810 2023-04-28 17:41:58.057636 comicon-0.2.4/comicon/inputs/pdf.py
--rw-r--r--   0        0        0     1873 2023-04-28 17:41:58.061636 comicon-0.2.4/comicon/outputs/__init__.py
--rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-0.2.4/comicon/outputs/cbz.py
--rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-0.2.4/comicon/outputs/cir.py
--rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-0.2.4/comicon/outputs/epub.py
--rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-0.2.4/comicon/outputs/pdf.py
--rw-r--r--   0        0        0      964 2023-06-20 22:19:39.233040 comicon-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 comicon-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1493 2023-04-28 17:41:58.055636 comicon-0.3.0/README.md
+-rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-0.3.0/comicon/__init__.py
+-rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-0.3.0/comicon/api.py
+-rw-r--r--   0        0        0     1034 2023-04-28 17:41:58.057636 comicon-0.3.0/comicon/base.py
+-rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-0.3.0/comicon/cirtools.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/cbz.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/cir.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/epub.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/pdf.py
+-rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-0.3.0/comicon/errors.py
+-rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-0.3.0/comicon/inputs/__init__.py
+-rw-r--r--   0        0        0     4605 2023-04-28 17:41:58.058636 comicon-0.3.0/comicon/inputs/cbz.py
+-rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-0.3.0/comicon/inputs/cir.py
+-rw-r--r--   0        0        0     5888 2023-04-28 17:41:58.058636 comicon-0.3.0/comicon/inputs/epub.py
+-rw-r--r--   0        0        0     2810 2023-04-28 17:41:58.057636 comicon-0.3.0/comicon/inputs/pdf.py
+-rw-r--r--   0        0        0     1873 2023-04-28 17:41:58.061636 comicon-0.3.0/comicon/outputs/__init__.py
+-rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-0.3.0/comicon/outputs/cbz.py
+-rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-0.3.0/comicon/outputs/cir.py
+-rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-0.3.0/comicon/outputs/epub.py
+-rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-0.3.0/comicon/outputs/pdf.py
+-rw-r--r--   0        0        0      964 2023-06-21 03:28:41.534008 comicon-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 comicon-0.3.0/PKG-INFO
```

### Comparing `comicon-0.2.4/LICENSE` & `comicon-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/README.md` & `comicon-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/api.py` & `comicon-0.3.0/comicon/api.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/base.py` & `comicon-0.3.0/comicon/base.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/cirtools.py` & `comicon-0.3.0/comicon/cirtools.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/errors.py` & `comicon-0.3.0/comicon/errors.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/inputs/__init__.py` & `comicon-0.3.0/comicon/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/inputs/cbz.py` & `comicon-0.3.0/comicon/inputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/inputs/cir.py` & `comicon-0.3.0/comicon/inputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/inputs/epub.py` & `comicon-0.3.0/comicon/inputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/inputs/pdf.py` & `comicon-0.3.0/comicon/inputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/outputs/__init__.py` & `comicon-0.3.0/comicon/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/outputs/cbz.py` & `comicon-0.3.0/comicon/outputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/outputs/cir.py` & `comicon-0.3.0/comicon/outputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/outputs/epub.py` & `comicon-0.3.0/comicon/outputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/comicon/outputs/pdf.py` & `comicon-0.3.0/comicon/outputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.4/pyproject.toml` & `comicon-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "comicon"
-version = "0.2.4"
+version = "0.3.0"
 description = "A simple comic conversion library between CBZ/EPUB/PDF"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 repository = "https://github.com/potatoeggy/comicon"
 documentation = "https://github.com/potatoeggy/comicon"
 keywords = ["converter", "comic", "cbz", "epub", "pdf"]
```

### Comparing `comicon-0.2.4/PKG-INFO` & `comicon-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicon
-Version: 0.2.4
+Version: 0.3.0
 Summary: A simple comic conversion library between CBZ/EPUB/PDF
 Home-page: https://github.com/potatoeggy/comicon
 License: AGPL-3.0-only
 Keywords: converter,comic,cbz,epub,pdf
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10
```

