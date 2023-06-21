# Comparing `tmp/pinecone_text-0.4.2.tar.gz` & `tmp/pinecone_text-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_text-0.4.2.tar", max compression
+gzip compressed data, was "pinecone_text-0.5.0.tar", max compression
```

## Comparing `pinecone_text-0.4.2.tar` & `pinecone_text-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    12229 2023-04-11 11:35:10.504735 pinecone_text-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     6095 2023-04-11 11:35:10.504735 pinecone_text-0.4.2/README.md
--rw-r--r--   0        0        0       34 2023-04-11 11:35:10.504735 pinecone_text-0.4.2/pinecone_text/__init__.py
--rw-r--r--   0        0        0      439 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/dense/__init__.py
--rw-r--r--   0        0        0      764 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/dense/base_dense_ecoder.py
--rw-r--r--   0        0        0     1259 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/dense/sentence_transformer_encoder.py
--rw-r--r--   0        0        0       67 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/hybrid/__init__.py
--rw-r--r--   0        0        0      998 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/hybrid/hybrid_convex.py
--rw-r--r--   0        0        0     1716 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/__init__.py
--rw-r--r--   0        0        0      818 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/base_sparse_encoder.py
--rw-r--r--   0        0        0     9727 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/bm25_encoder.py
--rw-r--r--   0        0        0     1760 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/bm25_tokenizer.py
--rw-r--r--   0        0        0     3073 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pinecone_text/sparse/splade_encoder.py
--rw-r--r--   0        0        0      624 2023-04-11 11:35:10.508735 pinecone_text-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6785 1970-01-01 00:00:00.000000 pinecone_text-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    12229 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     6217 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/README.md
+-rw-r--r--   0        0        0       34 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/dense/__init__.py
+-rw-r--r--   0        0        0      764 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/dense/base_dense_ecoder.py
+-rw-r--r--   0        0        0     1259 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/dense/sentence_transformer_encoder.py
+-rw-r--r--   0        0        0       67 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/hybrid/__init__.py
+-rw-r--r--   0        0        0      998 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/hybrid/hybrid_convex.py
+-rw-r--r--   0        0        0     1716 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/base_sparse_encoder.py
+-rw-r--r--   0        0        0     9727 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/bm25_encoder.py
+-rw-r--r--   0        0        0     1760 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/bm25_tokenizer.py
+-rw-r--r--   0        0        0     3826 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/splade_encoder.py
+-rw-r--r--   0        0        0      802 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6969 1970-01-01 00:00:00.000000 pinecone_text-0.5.0/PKG-INFO
```

### Comparing `pinecone_text-0.4.2/LICENSE.txt` & `pinecone_text-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/README.md` & `pinecone_text-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,20 @@
 > **_⚠️ Warning_**
 >
 > This is a **public preview** ("Beta") version.   
 > For any issues or requests, please reach out to our [support](support@pinecone.io) team.
 ## Installation
 To install the Pinecone Text Client, use the following command:
 ```bash
-pip install -U pinecone-text
+pip install pinecone-text
+```
+
+If you wish to use SpladeEncoder, you will need to install the `splade` extra:
+```bash
+pip install pincone-text[splade]
 ```
 
 ## Sparse Encoding
 
 To convert your own text corpus to sparse vectors, you can either use [BM25](https://www.pinecone.io/learn/semantic-search/#bm25) or [SPLADE](https://www.pinecone.io/learn/splade/).
 
 ### BM25
```

### Comparing `pinecone_text-0.4.2/pinecone_text/dense/base_dense_ecoder.py` & `pinecone_text-0.5.0/pinecone_text/dense/base_dense_ecoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/pinecone_text/dense/sentence_transformer_encoder.py` & `pinecone_text-0.5.0/pinecone_text/dense/sentence_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/pinecone_text/hybrid/hybrid_convex.py` & `pinecone_text-0.5.0/pinecone_text/hybrid/hybrid_convex.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/pinecone_text/sparse/__init__.py` & `pinecone_text-0.5.0/pinecone_text/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/pinecone_text/sparse/base_sparse_encoder.py` & `pinecone_text-0.5.0/pinecone_text/sparse/base_sparse_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/pinecone_text/sparse/bm25_encoder.py` & `pinecone_text-0.5.0/pinecone_text/sparse/bm25_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/pinecone_text/sparse/bm25_tokenizer.py` & `pinecone_text-0.5.0/pinecone_text/sparse/bm25_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.4.2/pyproject.toml` & `pinecone_text-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [tool.poetry]
 name = "pinecone-text"
-version = "0.4.2"
+version = "0.5.0"
 description = "Text utilities library by Pinecone.io"
 authors = ["Pinecone.io"]
 readme = "README.md"
 packages = [{include = "pinecone_text"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-torch = "^1.13.1"
-transformers = "^4.26.1"
-sentence-transformers = "^2.0.0"
+torch = { version = ">=1.13.1", optional = true }
+transformers = { version = ">=4.26.1", optional = true }
+sentence-transformers = { version = ">=2.0.0", optional = true }
 wget = "^3.2"
 mmh3 = "^3.1.0"
 nltk = "^3.6.5"
 
+[tool.poetry.extras]
+splade = ["torch", "transformers", "sentence-transformers"]
+
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mypy = "^1.0.1"
 black = "^23.1.0"
```

### Comparing `pinecone_text-0.4.2/PKG-INFO` & `pinecone_text-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pinecone-text
-Version: 0.4.2
+Version: 0.5.0
 Summary: Text utilities library by Pinecone.io
 Author: Pinecone.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: splade
 Requires-Dist: mmh3 (>=3.1.0,<4.0.0)
 Requires-Dist: nltk (>=3.6.5,<4.0.0)
-Requires-Dist: sentence-transformers (>=2.0.0,<3.0.0)
-Requires-Dist: torch (>=1.13.1,<2.0.0)
-Requires-Dist: transformers (>=4.26.1,<5.0.0)
+Requires-Dist: sentence-transformers (>=2.0.0) ; extra == "splade"
+Requires-Dist: torch (>=1.13.1) ; extra == "splade"
+Requires-Dist: transformers (>=4.26.1) ; extra == "splade"
 Requires-Dist: wget (>=3.2,<4.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <img src="https://avatars.githubusercontent.com/u/54333248?s=200&v=4">
     <br>
     Pinecone Text Client
@@ -29,15 +30,20 @@
 > **_⚠️ Warning_**
 >
 > This is a **public preview** ("Beta") version.   
 > For any issues or requests, please reach out to our [support](support@pinecone.io) team.
 ## Installation
 To install the Pinecone Text Client, use the following command:
 ```bash
-pip install -U pinecone-text
+pip install pinecone-text
+```
+
+If you wish to use SpladeEncoder, you will need to install the `splade` extra:
+```bash
+pip install pincone-text[splade]
 ```
 
 ## Sparse Encoding
 
 To convert your own text corpus to sparse vectors, you can either use [BM25](https://www.pinecone.io/learn/semantic-search/#bm25) or [SPLADE](https://www.pinecone.io/learn/splade/).
 
 ### BM25
```

