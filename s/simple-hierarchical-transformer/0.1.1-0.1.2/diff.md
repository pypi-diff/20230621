# Comparing `tmp/simple-hierarchical-transformer-0.1.1.tar.gz` & `tmp/simple-hierarchical-transformer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.1.1.tar", last modified: Wed Jun 21 18:33:22 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.1.2.tar", last modified: Wed Jun 21 18:40:10 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.1.1.tar` & `simple-hierarchical-transformer-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:33:22.375683 simple-hierarchical-transformer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 18:33:03.000000 simple-hierarchical-transformer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 18:33:22.375683 simple-hierarchical-transformer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-21 18:33:03.000000 simple-hierarchical-transformer-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:33:22.375683 simple-hierarchical-transformer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-21 18:33:03.000000 simple-hierarchical-transformer-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:33:22.371683 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 18:33:03.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-21 18:33:03.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    26494 2023-06-21 18:33:03.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:33:22.375683 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 18:33:22.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-21 18:33:22.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:33:22.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 18:33:22.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 18:33:22.000000 simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:40:10.724887 simple-hierarchical-transformer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 18:40:01.000000 simple-hierarchical-transformer-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 18:40:10.724887 simple-hierarchical-transformer-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-21 18:40:01.000000 simple-hierarchical-transformer-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:40:10.724887 simple-hierarchical-transformer-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-21 18:40:01.000000 simple-hierarchical-transformer-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:40:10.724887 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 18:40:01.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-21 18:40:01.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26494 2023-06-21 18:40:01.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:40:10.724887 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 18:40:10.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-21 18:40:10.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:40:10.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 18:40:10.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 18:40:10.000000 simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.1.1/LICENSE` & `simple-hierarchical-transformer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.1.1/PKG-INFO` & `simple-hierarchical-transformer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.1.1/README.md` & `simple-hierarchical-transformer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.1.1/setup.py` & `simple-hierarchical-transformer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.1.1',
+  version = '0.1.2',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
```

### Comparing `simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -726,27 +726,27 @@
             if self.hierarchy_merge_all:
                 tokens = [(t + p[..., ::s, :]) for t, p, s in zip(tokens, pooled.split(self.dims, dim = -1), self.h_strides)]
             else:
                 predict_tokens = tokens[self.predict_hierarchy_index]
                 predict_tokens = predict_tokens + pooled
                 tokens[self.predict_hierarchy_index] = predict_tokens
 
+        # final normalized embeddings
+
+        embeds = apply_fns(self.norms, tokens)
+
         # if the researcher wants the randomly projected ids of either compressed tokens or embeddings of the hierarchies
 
         if return_random_proj_quantize_ids:
             assert self.prophet_loss_use_quantized
 
-            quantize_input = tokens if self.prophet_quantized_use_embed else post_compressed_tokens
+            quantize_input = embeds if self.prophet_quantized_use_embed else post_compressed_tokens
             hierarchical_ids = apply_fns(self.rand_proj_quantizers, quantize_input)
             return hierarchical_ids
 
-        # final normalized embeddings
-
-        embeds = apply_fns(self.norms, tokens)
-
         # if one wants all the normalized hierarchical embeds
 
         if return_hierarchical_embeds:
             return embeds
 
         # select the hierarchical embeddings that will be doing the predicting
```

### Comparing `simple-hierarchical-transformer-0.1.1/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.1.2/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

