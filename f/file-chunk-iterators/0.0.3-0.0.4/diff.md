# Comparing `tmp/file_chunk_iterators-0.0.3.tar.gz` & `tmp/file_chunk_iterators-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_chunk_iterators-0.0.3.tar", last modified: Wed Jun 21 10:55:53 2023, max compression
+gzip compressed data, was "file_chunk_iterators-0.0.4.tar", last modified: Wed Jun 21 12:43:54 2023, max compression
```

## Comparing `file_chunk_iterators-0.0.3.tar` & `file_chunk_iterators-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    35149 2022-11-25 16:47:46.000000 file_chunk_iterators-0.0.3/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5772 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5309 2023-03-22 11:44:25.000000 file_chunk_iterators-0.0.3/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 file_chunk_iterators-0.0.3/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      727 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 file_chunk_iterators-0.0.3/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/src/file_chunk_iterators/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      114 2023-06-21 10:54:23.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    10072 2022-11-25 16:54:32.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators/file_chunk_iterators.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 10:55:53.191098 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5772 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      329 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-06-21 10:55:53.000000 file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 12:43:54.295938 file_chunk_iterators-0.0.4/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    35149 2022-11-25 16:47:46.000000 file_chunk_iterators-0.0.4/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5772 2023-06-21 12:43:54.295938 file_chunk_iterators-0.0.4/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5309 2023-03-22 11:44:25.000000 file_chunk_iterators-0.0.4/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 file_chunk_iterators-0.0.4/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      727 2023-06-21 12:43:54.295938 file_chunk_iterators-0.0.4/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 file_chunk_iterators-0.0.4/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 12:43:54.295938 file_chunk_iterators-0.0.4/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 12:43:54.295938 file_chunk_iterators-0.0.4/src/file_chunk_iterators/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      114 2023-06-21 10:54:23.000000 file_chunk_iterators-0.0.4/src/file_chunk_iterators/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    10077 2023-06-21 12:29:16.000000 file_chunk_iterators-0.0.4/src/file_chunk_iterators/file_chunk_iterators.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-06-21 12:43:54.295938 file_chunk_iterators-0.0.4/src/file_chunk_iterators.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     5772 2023-06-21 12:43:54.000000 file_chunk_iterators-0.0.4/src/file_chunk_iterators.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      329 2023-06-21 12:43:54.000000 file_chunk_iterators-0.0.4/src/file_chunk_iterators.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-06-21 12:43:54.000000 file_chunk_iterators-0.0.4/src/file_chunk_iterators.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-06-21 12:43:54.000000 file_chunk_iterators-0.0.4/src/file_chunk_iterators.egg-info/top_level.txt
```

### Comparing `file_chunk_iterators-0.0.3/LICENSE` & `file_chunk_iterators-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `file_chunk_iterators-0.0.3/PKG-INFO` & `file_chunk_iterators-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_chunk_iterators
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python classes to iterate through files in chunks
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `file_chunk_iterators-0.0.3/README.md` & `file_chunk_iterators-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `file_chunk_iterators-0.0.3/setup.cfg` & `file_chunk_iterators-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = file_chunk_iterators
-version = 0.0.3
+version = 0.0.4
 author = Marco Mariotti
 author_email = marco.mariotti@ub.edu
 description = Python classes to iterate through files in chunks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `file_chunk_iterators-0.0.3/src/file_chunk_iterators/file_chunk_iterators.py` & `file_chunk_iterators-0.0.4/src/file_chunk_iterators/file_chunk_iterators.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     """
 
     def __init__(self, fname, nlines=None, nchunks=None):
         self.fh=open(fname, 'r')
         self.totlines=buf_count_newlines_gen(fname)
         if not nchunks is None:
-            self.chunksize=totlines/nchunks
+            self.chunksize=self.totlines/nchunks
         elif not nlines is None:
             self.chunksize=nlines
         else:
             raise Exception("ERROR you must specify nlines or nchunks")
         self.chunkindex=0
         self.globalindex=0
         self.finished=False
```

### Comparing `file_chunk_iterators-0.0.3/src/file_chunk_iterators.egg-info/PKG-INFO` & `file_chunk_iterators-0.0.4/src/file_chunk_iterators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-chunk-iterators
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python classes to iterate through files in chunks
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

