# Comparing `tmp/pyliger-0.2.0b1.tar.gz` & `tmp/pyliger-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyliger-0.2.0b1.tar", last modified: Sat Apr  8 06:36:59 2023, max compression
+gzip compressed data, was "pyliger-0.2.0rc1.tar", last modified: Wed Jun 21 14:55:45 2023, max compression
```

## Comparing `pyliger-0.2.0b1.tar` & `pyliger-0.2.0rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    35149 2023-04-08 06:36:38.024846 pyliger-0.2.0b1/LICENSE
--rw-r--r--   0        0        0      578 2023-04-08 06:36:38.024846 pyliger-0.2.0b1/README.md
--rw-r--r--   0        0        0     1539 2023-04-08 06:36:38.036847 pyliger-0.2.0b1/pyproject.toml
--rw-r--r--   0        0        0      440 2023-04-08 06:36:38.036847 pyliger-0.2.0b1/src/pyliger/__init__.py
--rw-r--r--   0        0        0     4541 2023-04-08 06:36:38.036847 pyliger-0.2.0b1/src/pyliger/_utilities.py
--rw-r--r--   0        0        0     1812 2023-04-08 06:36:38.036847 pyliger-0.2.0b1/src/pyliger/clustering/__init__.py
--rw-r--r--   0        0        0     2877 2023-04-08 06:36:38.036847 pyliger-0.2.0b1/src/pyliger/clustering/_leiden.py
--rw-r--r--   0        0        0     2654 2023-04-08 06:36:38.036847 pyliger-0.2.0b1/src/pyliger/clustering/_louvain.py
--rw-r--r--   0        0        0     3782 2023-04-08 06:36:38.036847 pyliger-0.2.0b1/src/pyliger/clustering/_utilities.py
--rw-r--r--   0        0        0 16300140 2023-04-08 06:36:38.116847 pyliger-0.2.0b1/src/pyliger/datasets/PBMC_control.h5ad
--rw-r--r--   0        0        0 16633964 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad
--rw-r--r--   0        0        0     1568 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/factorization/__init__.py
--rw-r--r--   0        0        0     7688 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/factorization/_iNMF_ANLS.py
--rw-r--r--   0        0        0     6106 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/factorization/_iNMF_HALS.py
--rw-r--r--   0        0        0    26732 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/factorization/_online_iNMF.py
--rw-r--r--   0        0        0    13195 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/factorization/_utilities.py
--rw-r--r--   0        0        0       14 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/logging.py
--rw-r--r--   0        0        0     2037 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/plotting/__init__.py
--rw-r--r--   0        0        0     3796 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/plotting/_dataset_cluster.py
--rw-r--r--   0        0        0    11677 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/plotting/_gene.py
--rw-r--r--   0        0        0     6608 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/plotting/_gene_loadings.py
--rw-r--r--   0        0        0    53282 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/plotting/_go.py
--rw-r--r--   0        0        0     2648 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/plotting/_spatial.py
--rw-r--r--   0        0        0     1371 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/plotting/_utilities.py
--rw-r--r--   0        0        0      249 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/preprocessing/__init__.py
--rw-r--r--   0        0        0     3242 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/preprocessing/_cal_feature.py
--rw-r--r--   0        0        0     7223 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/preprocessing/_initialization.py
--rw-r--r--   0        0        0     3274 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/preprocessing/_normalization.py
--rw-r--r--   0        0        0     2388 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/preprocessing/_qc.py
--rw-r--r--   0        0        0     4360 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/preprocessing/_scale.py
--rw-r--r--   0        0        0     9430 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/preprocessing/_select_genes.py
--rw-r--r--   0        0        0     8207 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/pyliger.py
--rw-r--r--   0        0        0    16438 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/read_write.py
--rw-r--r--   0        0        0     1430 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/tools/__init__.py
--rw-r--r--   0        0        0     3724 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/tools/_go.py
--rw-r--r--   0        0        0    14330 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/tools/_marker.py
--rw-r--r--   0        0        0     1832 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/tools/_metrics.py
--rw-r--r--   0        0        0     7777 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/tools/_quantile_norm.py
--rw-r--r--   0        0        0     4678 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/tools/_umap.py
--rw-r--r--   0        0        0    11015 2023-04-08 06:36:38.200848 pyliger-0.2.0b1/src/pyliger/tools/_wilcoxon.py
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 pyliger-0.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-21 14:55:04.310149 pyliger-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0      578 2023-06-21 14:55:04.310149 pyliger-0.2.0rc1/README.md
+-rw-r--r--   0        0        0     1566 2023-06-21 14:55:04.330150 pyliger-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      440 2023-06-21 14:55:04.330150 pyliger-0.2.0rc1/src/pyliger/__init__.py
+-rw-r--r--   0        0        0     4541 2023-06-21 14:55:04.330150 pyliger-0.2.0rc1/src/pyliger/_utilities.py
+-rw-r--r--   0        0        0     1812 2023-06-21 14:55:04.330150 pyliger-0.2.0rc1/src/pyliger/clustering/__init__.py
+-rw-r--r--   0        0        0     2877 2023-06-21 14:55:04.330150 pyliger-0.2.0rc1/src/pyliger/clustering/_leiden.py
+-rw-r--r--   0        0        0     2654 2023-06-21 14:55:04.330150 pyliger-0.2.0rc1/src/pyliger/clustering/_louvain.py
+-rw-r--r--   0        0        0     3782 2023-06-21 14:55:04.330150 pyliger-0.2.0rc1/src/pyliger/clustering/_utilities.py
+-rw-r--r--   0        0        0 16300140 2023-06-21 14:55:04.422154 pyliger-0.2.0rc1/src/pyliger/datasets/PBMC_control.h5ad
+-rw-r--r--   0        0        0 16633964 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad
+-rw-r--r--   0        0        0     1568 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/factorization/__init__.py
+-rw-r--r--   0        0        0     7688 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/factorization/_iNMF_ANLS.py
+-rw-r--r--   0        0        0     6106 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/factorization/_iNMF_HALS.py
+-rw-r--r--   0        0        0    26732 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/factorization/_online_iNMF.py
+-rw-r--r--   0        0        0    13195 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/factorization/_utilities.py
+-rw-r--r--   0        0        0       14 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/logging.py
+-rw-r--r--   0        0        0     2037 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/plotting/__init__.py
+-rw-r--r--   0        0        0     3796 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/plotting/_dataset_cluster.py
+-rw-r--r--   0        0        0    11677 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/plotting/_gene.py
+-rw-r--r--   0        0        0     6608 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/plotting/_gene_loadings.py
+-rw-r--r--   0        0        0    53282 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/plotting/_go.py
+-rw-r--r--   0        0        0     2648 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/plotting/_spatial.py
+-rw-r--r--   0        0        0     1371 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/plotting/_utilities.py
+-rw-r--r--   0        0        0      249 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3242 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/preprocessing/_cal_feature.py
+-rw-r--r--   0        0        0     7223 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/preprocessing/_initialization.py
+-rw-r--r--   0        0        0     3274 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/preprocessing/_normalization.py
+-rw-r--r--   0        0        0     2388 2023-06-21 14:55:04.530158 pyliger-0.2.0rc1/src/pyliger/preprocessing/_qc.py
+-rw-r--r--   0        0        0     4360 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/preprocessing/_scale.py
+-rw-r--r--   0        0        0     9430 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/preprocessing/_select_genes.py
+-rw-r--r--   0        0        0     8207 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/pyliger.py
+-rw-r--r--   0        0        0    16438 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/read_write.py
+-rw-r--r--   0        0        0     1430 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/tools/__init__.py
+-rw-r--r--   0        0        0     3724 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/tools/_go.py
+-rw-r--r--   0        0        0    14330 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/tools/_marker.py
+-rw-r--r--   0        0        0     1832 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/tools/_metrics.py
+-rw-r--r--   0        0        0     7777 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/tools/_quantile_norm.py
+-rw-r--r--   0        0        0     4678 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/tools/_umap.py
+-rw-r--r--   0        0        0    11015 2023-06-21 14:55:04.534158 pyliger-0.2.0rc1/src/pyliger/tools/_wilcoxon.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 pyliger-0.2.0rc1/PKG-INFO
```

### Comparing `pyliger-0.2.0b1/LICENSE` & `pyliger-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/README.md` & `pyliger-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/pyproject.toml` & `pyliger-0.2.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -47,26 +47,27 @@
     "pandas",
     "plotnine",
     "python-igraph",
     "scikit-learn",
     "scipy",
     "seaborn",
     "umap-learn",
+    "setuptools>=68.0.0",
 ]
 description = "The Python version of LIGER package."
 keywords = [
     "LIGER",
 ]
 maintainers = [
     { name = "Andrew Robbins", email = "robbiand@med.umich.edu" },
 ]
 name = "pyliger"
 readme = "README.md"
 requires-python = "<3.12, >=3.8"
-version = "0.2.0b1"
+version = "0.2.0rc1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://welch-lab.github.io"
 repository = "https://github.com/welch-lab/pyliger"
```

### Comparing `pyliger-0.2.0b1/src/pyliger/_utilities.py` & `pyliger-0.2.0rc1/src/pyliger/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/clustering/__init__.py` & `pyliger-0.2.0rc1/src/pyliger/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/clustering/_leiden.py` & `pyliger-0.2.0rc1/src/pyliger/clustering/_leiden.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/clustering/_louvain.py` & `pyliger-0.2.0rc1/src/pyliger/clustering/_louvain.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/clustering/_utilities.py` & `pyliger-0.2.0rc1/src/pyliger/clustering/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/datasets/PBMC_control.h5ad` & `pyliger-0.2.0rc1/src/pyliger/datasets/PBMC_control.h5ad`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad` & `pyliger-0.2.0rc1/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/factorization/__init__.py` & `pyliger-0.2.0rc1/src/pyliger/factorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/factorization/_iNMF_ANLS.py` & `pyliger-0.2.0rc1/src/pyliger/factorization/_iNMF_ANLS.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/factorization/_iNMF_HALS.py` & `pyliger-0.2.0rc1/src/pyliger/factorization/_iNMF_HALS.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/factorization/_online_iNMF.py` & `pyliger-0.2.0rc1/src/pyliger/factorization/_online_iNMF.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/factorization/_utilities.py` & `pyliger-0.2.0rc1/src/pyliger/factorization/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/plotting/__init__.py` & `pyliger-0.2.0rc1/src/pyliger/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/plotting/_dataset_cluster.py` & `pyliger-0.2.0rc1/src/pyliger/plotting/_dataset_cluster.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/plotting/_gene.py` & `pyliger-0.2.0rc1/src/pyliger/plotting/_gene.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/plotting/_gene_loadings.py` & `pyliger-0.2.0rc1/src/pyliger/plotting/_gene_loadings.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/plotting/_go.py` & `pyliger-0.2.0rc1/src/pyliger/plotting/_go.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/plotting/_spatial.py` & `pyliger-0.2.0rc1/src/pyliger/plotting/_spatial.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/plotting/_utilities.py` & `pyliger-0.2.0rc1/src/pyliger/plotting/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/preprocessing/_cal_feature.py` & `pyliger-0.2.0rc1/src/pyliger/preprocessing/_cal_feature.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/preprocessing/_initialization.py` & `pyliger-0.2.0rc1/src/pyliger/preprocessing/_initialization.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/preprocessing/_normalization.py` & `pyliger-0.2.0rc1/src/pyliger/preprocessing/_normalization.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/preprocessing/_qc.py` & `pyliger-0.2.0rc1/src/pyliger/preprocessing/_qc.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/preprocessing/_scale.py` & `pyliger-0.2.0rc1/src/pyliger/preprocessing/_scale.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/preprocessing/_select_genes.py` & `pyliger-0.2.0rc1/src/pyliger/preprocessing/_select_genes.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/pyliger.py` & `pyliger-0.2.0rc1/src/pyliger/pyliger.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/read_write.py` & `pyliger-0.2.0rc1/src/pyliger/read_write.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/tools/__init__.py` & `pyliger-0.2.0rc1/src/pyliger/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/tools/_go.py` & `pyliger-0.2.0rc1/src/pyliger/tools/_go.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/tools/_marker.py` & `pyliger-0.2.0rc1/src/pyliger/tools/_marker.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/tools/_metrics.py` & `pyliger-0.2.0rc1/src/pyliger/tools/_metrics.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/tools/_quantile_norm.py` & `pyliger-0.2.0rc1/src/pyliger/tools/_quantile_norm.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/tools/_umap.py` & `pyliger-0.2.0rc1/src/pyliger/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/src/pyliger/tools/_wilcoxon.py` & `pyliger-0.2.0rc1/src/pyliger/tools/_wilcoxon.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.0b1/PKG-INFO` & `pyliger-0.2.0rc1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliger
-Version: 0.2.0b1
+Version: 0.2.0rc1
 Summary: The Python version of LIGER package.
 License: MIT
 Keywords: LIGER
 Author-email: Joshua Welch <welchjd@med.umich.edu>,Lu Lu <luluhz@umich.edu>
 Maintainer-email: Andrew Robbins <robbiand@med.umich.edu>
 Requires-Python: <3.12, >=3.8
 Classifier: Development Status :: 4 - Beta
```

