# Comparing `tmp/getpaper-0.0.6.tar.gz` & `tmp/getpaper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.0.6.tar", last modified: Wed Jun 21 13:47:05 2023, max compression
+gzip compressed data, was "getpaper-0.0.8.tar", last modified: Wed Jun 21 14:09:13 2023, max compression
```

## Comparing `getpaper-0.0.6.tar` & `getpaper-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 13:47:05.744694 getpaper-0.0.6/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.6/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2280 2023-06-21 13:47:05.744694 getpaper-0.0.6/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1665 2023-06-21 13:18:25.000000 getpaper-0.0.6/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 13:47:05.740694 getpaper-0.0.6/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.6/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     4033 2023-06-21 12:30:05.000000 getpaper-0.0.6/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4415 2023-06-21 12:58:00.000000 getpaper-0.0.6/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5452 2023-06-21 12:24:40.000000 getpaper-0.0.6/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1068 2023-06-21 10:50:13.000000 getpaper-0.0.6/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 13:47:05.744694 getpaper-0.0.6/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2280 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 13:47:05.000000 getpaper-0.0.6/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 13:47:05.744694 getpaper-0.0.6/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1535 2023-06-21 13:45:20.000000 getpaper-0.0.6/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 14:09:13.526532 getpaper-0.0.8/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.8/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 14:09:13.526532 getpaper-0.0.8/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1976 2023-06-21 14:08:28.000000 getpaper-0.0.8/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 14:09:13.522532 getpaper-0.0.8/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.8/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     4033 2023-06-21 12:30:05.000000 getpaper-0.0.8/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4434 2023-06-21 13:55:47.000000 getpaper-0.0.8/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5437 2023-06-21 13:54:57.000000 getpaper-0.0.8/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1068 2023-06-21 10:50:13.000000 getpaper-0.0.8/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 14:09:13.522532 getpaper-0.0.8/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 14:09:13.000000 getpaper-0.0.8/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 14:09:13.000000 getpaper-0.0.8/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 14:09:13.000000 getpaper-0.0.8/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-21 14:09:13.000000 getpaper-0.0.8/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 14:09:13.000000 getpaper-0.0.8/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 14:09:13.000000 getpaper-0.0.8/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 14:09:13.526532 getpaper-0.0.8/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-21 14:08:53.000000 getpaper-0.0.8/setup.py
```

### Comparing `getpaper-0.0.6/LICENSE` & `getpaper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.6/PKG-INFO` & `getpaper-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.6
+Version: 0.0.8
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -50,14 +50,18 @@
 getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
+```bash
+python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
+```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.0.6/README.md` & `getpaper-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
+```bash
+python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
+```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.0.6/getpaper/download.py` & `getpaper-0.0.8/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.6/getpaper/index.py` & `getpaper-0.0.8/getpaper/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from langchain.embeddings import OpenAIEmbeddings, LlamaCppEmbeddings, VertexAIEmbeddings
 from langchain.embeddings.base import Embeddings
 from langchain.schema import Document
 from langchain.text_splitter import TextSplitter
 from langchain.vectorstores import Chroma
 from pycomfort.files import *
 
-from getpaper.parse import papers_to_documents
-from getpaper.splitter import RecursiveSplitterWithSource
+from parse import papers_to_documents
+from splitter import RecursiveSplitterWithSource
 
 
 def load_environment_keys(debug: bool = True):
     e = dotenv.find_dotenv()
     if debug:
         print(f"environment found at {e}")
     has_env: bool = load_dotenv(e, verbose=True, override=True)
@@ -104,7 +104,10 @@
 @click.option('--chunk_size', type=click.INT, default=6000, help='size of the chunk for splitting')
 @click.option('--embeddings', type=click.Choice(["openai", "lambda", "vertexai"]), default="openai",
               help='size of the chunk for splitting')
 def index_papers_command(papers: str, folder: str, collection: str, chunk_size: int, embeddings: str) -> Path:
     index = Path(folder)
     papers_folder = Path(papers)
     return index_papers(papers_folder, index, collection, chunk_size, embeddings)
+
+if __name__ == '__main__':
+    app()
```

### Comparing `getpaper-0.0.6/getpaper/parse.py` & `getpaper-0.0.8/getpaper/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 from typing import Optional, List
 
 import click
-import requests
 from click import Context
 from langchain.document_loaders import UnstructuredPDFLoader
 from langchain.schema import Document
 from pycomfort.files import traverse
 
+
 def parse_paper(paper: Path, folder: Optional[Path] = None,
                 mode: str = "single", strategy: str = "auto",
                 pdf_infer_table_structure: bool = True,
                 include_page_breaks: bool = False
                 ):
     """
     Parses the paper using Unstructured paper parser
```

### Comparing `getpaper-0.0.6/getpaper/splitter.py` & `getpaper-0.0.8/getpaper/splitter.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.6/getpaper.egg-info/PKG-INFO` & `getpaper-0.0.8/getpaper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.6
+Version: 0.0.8
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -50,14 +50,18 @@
 getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
+For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
+```bash
+python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
+```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.0.6/setup.py` & `getpaper-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.8'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
@@ -33,11 +33,12 @@
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     entry_points={
      "console_scripts": [
          "download=getpaper.download:app",
-         "parse=getpaper.parse:app"
+         "parse=getpaper.parse:app",
+         "index=getpaper.index:app"
      ]
     }
 )
```

