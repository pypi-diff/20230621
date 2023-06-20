# Comparing `tmp/latex-document-reader-1.0.0.tar.gz` & `tmp/latex-document-reader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex-document-reader-1.0.0.tar", last modified: Tue Jun 20 19:56:17 2023, max compression
+gzip compressed data, was "latex-document-reader-1.0.1.tar", last modified: Tue Jun 20 22:07:34 2023, max compression
```

## Comparing `latex-document-reader-1.0.0.tar` & `latex-document-reader-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 19:56:17.211050 latex-document-reader-1.0.0/
--rw-rw-rw-   0        0        0     1084 2023-06-20 19:35:47.000000 latex-document-reader-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3079 2023-06-20 19:56:17.211050 latex-document-reader-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2289 2023-06-20 19:43:09.000000 latex-document-reader-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 19:56:17.201003 latex-document-reader-1.0.0/latex_document_reader/
--rw-rw-rw-   0        0        0      102 2023-06-20 19:45:17.000000 latex-document-reader-1.0.0/latex_document_reader/__init__.py
--rw-rw-rw-   0        0        0      927 2023-06-20 19:44:47.000000 latex-document-reader-1.0.0/latex_document_reader/latex_document_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-20 19:56:17.204049 latex-document-reader-1.0.0/latex_document_reader.egg-info/
--rw-rw-rw-   0        0        0     3079 2023-06-20 19:56:17.000000 latex-document-reader-1.0.0/latex_document_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-20 19:56:17.000000 latex-document-reader-1.0.0/latex_document_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 19:56:17.000000 latex-document-reader-1.0.0/latex_document_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-20 19:56:17.000000 latex-document-reader-1.0.0/latex_document_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 19:56:17.211050 latex-document-reader-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-06-20 19:46:55.000000 latex-document-reader-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 22:07:34.962637 latex-document-reader-1.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-06-20 19:35:47.000000 latex-document-reader-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3083 2023-06-20 22:07:34.962637 latex-document-reader-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2293 2023-06-20 20:00:06.000000 latex-document-reader-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 22:07:34.956673 latex-document-reader-1.0.1/latex_document_reader/
+-rw-rw-rw-   0        0        0      102 2023-06-20 19:45:17.000000 latex-document-reader-1.0.1/latex_document_reader/__init__.py
+-rw-rw-rw-   0        0        0     1512 2023-06-20 22:07:17.000000 latex-document-reader-1.0.1/latex_document_reader/latex_document_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-20 22:07:34.962637 latex-document-reader-1.0.1/latex_document_reader.egg-info/
+-rw-rw-rw-   0        0        0     3083 2023-06-20 22:07:34.000000 latex-document-reader-1.0.1/latex_document_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-20 22:07:34.000000 latex-document-reader-1.0.1/latex_document_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 22:07:34.000000 latex-document-reader-1.0.1/latex_document_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-20 22:07:34.000000 latex-document-reader-1.0.1/latex_document_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 22:07:34.962637 latex-document-reader-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-06-20 21:55:56.000000 latex-document-reader-1.0.1/setup.py
```

### Comparing `latex-document-reader-1.0.0/LICENSE` & `latex-document-reader-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latex-document-reader-1.0.0/PKG-INFO` & `latex-document-reader-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-document-reader
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for reading LaTeX documents and processing BibTeX files
 Home-page: https://github.com/ozanil/LaTeXDocumentReader.git
 Author: Anıl ÖZ
 Author-email: anil.oz@icloud.com
 Keywords: latex document reader bibtex
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LaTeX Document Reader
 
-[![PyPI version](https://badge.fury.io/py/LaTeXDocumentReader.svg)](https://badge.fury.io/py/LaTeXDocumentReader)
+[![PyPI version](https://badge.fury.io/py/LaTeX-Document-Reader.svg)](https://badge.fury.io/py/LaTeX-Document-Reader)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 A Python library for reading LaTeX documents and processing BibTeX files.
 
 ## Installation
 
 You can install the library using pip:
```

### Comparing `latex-document-reader-1.0.0/README.md` & `latex-document-reader-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # LaTeX Document Reader
 
-[![PyPI version](https://badge.fury.io/py/LaTeXDocumentReader.svg)](https://badge.fury.io/py/LaTeXDocumentReader)
+[![PyPI version](https://badge.fury.io/py/LaTeX-Document-Reader.svg)](https://badge.fury.io/py/LaTeX-Document-Reader)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 A Python library for reading LaTeX documents and processing BibTeX files.
 
 ## Installation
 
 You can install the library using pip:
```

### Comparing `latex-document-reader-1.0.0/latex_document_reader.egg-info/PKG-INFO` & `latex-document-reader-1.0.1/latex_document_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-document-reader
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for reading LaTeX documents and processing BibTeX files
 Home-page: https://github.com/ozanil/LaTeXDocumentReader.git
 Author: Anıl ÖZ
 Author-email: anil.oz@icloud.com
 Keywords: latex document reader bibtex
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LaTeX Document Reader
 
-[![PyPI version](https://badge.fury.io/py/LaTeXDocumentReader.svg)](https://badge.fury.io/py/LaTeXDocumentReader)
+[![PyPI version](https://badge.fury.io/py/LaTeX-Document-Reader.svg)](https://badge.fury.io/py/LaTeX-Document-Reader)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 A Python library for reading LaTeX documents and processing BibTeX files.
 
 ## Installation
 
 You can install the library using pip:
```

### Comparing `latex-document-reader-1.0.0/setup.py` & `latex-document-reader-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='latex-document-reader',
-    version='1.0.0',
+    version='1.0.1',
     author='Anıl ÖZ',
     author_email='anil.oz@icloud.com',
     description='A Python library for reading LaTeX documents and processing BibTeX files',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ozanil/LaTeXDocumentReader.git',
     packages=setuptools.find_packages(),
```

