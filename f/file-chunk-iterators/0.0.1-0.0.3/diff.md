# Comparing `tmp/file_chunk_iterators-0.0.1.tar.gz` & `tmp/file_chunk_iterators-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_chunk_iterators-0.0.1.tar", last modified: Wed Mar 22 11:40:58 2023, max compression
+gzip compressed data, was "file_chunk_iterators-0.0.3.tar", last modified: Wed Jun 21 10:55:53 2023, max compression
```

## Comparing `file_chunk_iterators-0.0.1.tar` & `file_chunk_iterators-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 11:40:58.339454 file_chunk_iterators-0.0.1/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    35149 2022-11-25 16:47:46.000000 file_chunk_iterators-0.0.1/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5711 2023-03-22 11:40:58.339454 file_chunk_iterators-0.0.1/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5248 2022-11-25 16:57:52.000000 file_chunk_iterators-0.0.1/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 file_chunk_iterators-0.0.1/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      727 2023-03-22 11:40:58.339454 file_chunk_iterators-0.0.1/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 file_chunk_iterators-0.0.1/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 11:40:58.339454 file_chunk_iterators-0.0.1/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 11:40:58.339454 file_chunk_iterators-0.0.1/src/file_chunk_iterators/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       90 2023-03-22 11:35:37.000000 file_chunk_iterators-0.0.1/src/file_chunk_iterators/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    10072 2022-11-25 16:54:32.000000 file_chunk_iterators-0.0.1/src/file_chunk_iterators/file_chunk_iterators.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-22 11:40:58.339454 file_chunk_iterators-0.0.1/src/file_chunk_iterators.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5711 2023-03-22 11:40:58.000000 file_chunk_iterators-0.0.1/src/file_chunk_iterators.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      329 2023-03-22 11:40:58.000000 file_chunk_iterators-0.0.1/src/file_chunk_iterators.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-03-22 11:40:58.000000 file_chunk_iterators-0.0.1/src/file_chunk_iterators.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-03-22 11:40:58.000000 file_chunk_iterators-0.0.1/src/file_chunk_iterators.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    35149 2022-11-25 16:47:46.000000 file_chunk_iterators-0.0.3/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5772 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5309 2023-03-22 11:44:25.000000 file_chunk_iterators-0.0.3/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 file_chunk_iterators-0.0.3/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      727 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 file_chunk_iterators-0.0.3/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/src/file_chunk_iterators/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      114 2023-06-21 10:54:23.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    10072 2022-11-25 16:54:32.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators/file_chunk_iterators.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5772 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      329 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/top_level.txt
```

### Comparing `file_chunk_iterators-0.0.1/LICENSE` & `file_chunk_iterators-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `file_chunk_iterators-0.0.1/PKG-INFO` & `file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: file_chunk_iterators
-Version: 0.0.1
+Name: file-chunk-iterators
+Version: 0.0.3
 Summary: Python classes to iterate through files in chunks
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,20 @@
 License-File: LICENSE
 
 # file_chunk_iterators
 
 Python classes to iterate through files in chunks
 
 
+## Installation
+
+pip install file_chunk_iterators
+
+
+## Usage
 We provide two functions:
 
 1. iterate_file_in_chunks
    Iterator to iterate over chunks of a file.
    The iterator is initialized to specify how many lines/chunks to make.
    It is then used as iterator several times: each time, it will iterate over the lines of one chunk only.
```

### Comparing `file_chunk_iterators-0.0.1/README.md` & `file_chunk_iterators-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # file_chunk_iterators
 
 Python classes to iterate through files in chunks
 
 
+## Installation
+
+pip install file_chunk_iterators
+
+
+## Usage
 We provide two functions:
 
 1. iterate_file_in_chunks
    Iterator to iterate over chunks of a file.
    The iterator is initialized to specify how many lines/chunks to make.
    It is then used as iterator several times: each time, it will iterate over the lines of one chunk only.
```

### Comparing `file_chunk_iterators-0.0.1/setup.cfg` & `file_chunk_iterators-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = file_chunk_iterators
-version = 0.0.1
+version = 0.0.3
 author = Marco Mariotti
 author_email = marco.mariotti@ub.edu
 description = Python classes to iterate through files in chunks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `file_chunk_iterators-0.0.1/src/file_chunk_iterators/file_chunk_iterators.py` & `file_chunk_iterators-0.0.3/src/file_chunk_iterators/file_chunk_iterators.py`

 * *Files identical despite different names*

### Comparing `file_chunk_iterators-0.0.1/src/file_chunk_iterators.egg-info/PKG-INFO` & `file_chunk_iterators-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: file-chunk-iterators
-Version: 0.0.1
+Name: file_chunk_iterators
+Version: 0.0.3
 Summary: Python classes to iterate through files in chunks
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,20 @@
 License-File: LICENSE
 
 # file_chunk_iterators
 
 Python classes to iterate through files in chunks
 
 
+## Installation
+
+pip install file_chunk_iterators
+
+
+## Usage
 We provide two functions:
 
 1. iterate_file_in_chunks
    Iterator to iterate over chunks of a file.
    The iterator is initialized to specify how many lines/chunks to make.
    It is then used as iterator several times: each time, it will iterate over the lines of one chunk only.
```

