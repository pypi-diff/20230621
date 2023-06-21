# Comparing `tmp/pinecone_text-0.5.0.tar.gz` & `tmp/pinecone_text-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_text-0.5.0.tar", max compression
+gzip compressed data, was "pinecone_text-0.5.1.tar", max compression
```

## Comparing `pinecone_text-0.5.0.tar` & `pinecone_text-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    12229 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     6217 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/README.md
--rw-r--r--   0        0        0       34 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/__init__.py
--rw-r--r--   0        0        0      439 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/dense/__init__.py
--rw-r--r--   0        0        0      764 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/dense/base_dense_ecoder.py
--rw-r--r--   0        0        0     1259 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/dense/sentence_transformer_encoder.py
--rw-r--r--   0        0        0       67 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/hybrid/__init__.py
--rw-r--r--   0        0        0      998 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/hybrid/hybrid_convex.py
--rw-r--r--   0        0        0     1716 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/__init__.py
--rw-r--r--   0        0        0      818 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/base_sparse_encoder.py
--rw-r--r--   0        0        0     9727 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/bm25_encoder.py
--rw-r--r--   0        0        0     1760 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/bm25_tokenizer.py
--rw-r--r--   0        0        0     3826 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pinecone_text/sparse/splade_encoder.py
--rw-r--r--   0        0        0      802 2023-06-21 17:45:05.705082 pinecone_text-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6969 1970-01-01 00:00:00.000000 pinecone_text-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    12229 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     6217 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/README.md
+-rw-r--r--   0        0        0       34 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/dense/__init__.py
+-rw-r--r--   0        0        0      764 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/dense/base_dense_ecoder.py
+-rw-r--r--   0        0        0     1259 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/dense/sentence_transformer_encoder.py
+-rw-r--r--   0        0        0       67 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/hybrid/__init__.py
+-rw-r--r--   0        0        0      998 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/hybrid/hybrid_convex.py
+-rw-r--r--   0        0        0     2050 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/sparse/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/sparse/base_sparse_encoder.py
+-rw-r--r--   0        0        0     9727 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/sparse/bm25_encoder.py
+-rw-r--r--   0        0        0     1760 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/sparse/bm25_tokenizer.py
+-rw-r--r--   0        0        0     3826 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pinecone_text/sparse/splade_encoder.py
+-rw-r--r--   0        0        0      802 2023-06-21 19:06:04.257975 pinecone_text-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6969 1970-01-01 00:00:00.000000 pinecone_text-0.5.1/PKG-INFO
```

### Comparing `pinecone_text-0.5.0/LICENSE.txt` & `pinecone_text-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/README.md` & `pinecone_text-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pinecone_text/dense/base_dense_ecoder.py` & `pinecone_text-0.5.1/pinecone_text/dense/base_dense_ecoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pinecone_text/dense/sentence_transformer_encoder.py` & `pinecone_text-0.5.1/pinecone_text/dense/sentence_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pinecone_text/hybrid/hybrid_convex.py` & `pinecone_text-0.5.1/pinecone_text/hybrid/hybrid_convex.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pinecone_text/sparse/__init__.py` & `pinecone_text-0.5.1/pinecone_text/sparse/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,13 +18,21 @@
 
 ## SPLADE
 SPLADE is a Transformer based encoder, that uses sophisticated expansion to encode documents and queries in a sparse representation.
 This allows a semantic search to be performed on the sparse vectors. The SPLADE encoder is based on the work done by the research team in Naver Labs Europe.
 For more information, see the [SPLADE paper](https://arxiv.org/abs/2109.10086). The SPLADE encoder is currently only available for inference only.
 """
 
+import logging
 from typing import Union, Dict, List
 
 SparseVector = Dict[str, Union[List[int], List[float]]]
 
 from pinecone_text.sparse.bm25_encoder import BM25Encoder
-from pinecone_text.sparse.splade_encoder import SpladeEncoder
+
+# Try to import the SpladeEncoder. If it fails, let the usage of the encoder fail.
+try:
+    from pinecone_text.sparse.splade_encoder import SpladeEncoder
+except (ImportError, ModuleNotFoundError):
+    logging.warning(
+        "Failed to import splade encoder. If you want to use splade, install the splade extra dependencies by running: `pip install pinecone-text[splade]`"
+    )
```

### Comparing `pinecone_text-0.5.0/pinecone_text/sparse/base_sparse_encoder.py` & `pinecone_text-0.5.1/pinecone_text/sparse/base_sparse_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pinecone_text/sparse/bm25_encoder.py` & `pinecone_text-0.5.1/pinecone_text/sparse/bm25_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pinecone_text/sparse/bm25_tokenizer.py` & `pinecone_text-0.5.1/pinecone_text/sparse/bm25_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pinecone_text/sparse/splade_encoder.py` & `pinecone_text-0.5.1/pinecone_text/sparse/splade_encoder.py`

 * *Files identical despite different names*

### Comparing `pinecone_text-0.5.0/pyproject.toml` & `pinecone_text-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-text"
-version = "0.5.0"
+version = "0.5.1"
 description = "Text utilities library by Pinecone.io"
 authors = ["Pinecone.io"]
 readme = "README.md"
 packages = [{include = "pinecone_text"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `pinecone_text-0.5.0/PKG-INFO` & `pinecone_text-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-text
-Version: 0.5.0
+Version: 0.5.1
 Summary: Text utilities library by Pinecone.io
 Author: Pinecone.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

