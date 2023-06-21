# Comparing `tmp/audiolm-pytorch-1.2.6.tar.gz` & `tmp/audiolm-pytorch-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.2.6.tar", last modified: Tue Jun 20 22:59:54 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.2.7.tar", last modified: Wed Jun 21 13:38:24 2023, max compression
```

## Comparing `audiolm-pytorch-1.2.6.tar` & `audiolm-pytorch-1.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    68030 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68033 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/setup.py
```

### Comparing `audiolm-pytorch-1.2.6/LICENSE` & `audiolm-pytorch-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/PKG-INFO` & `audiolm-pytorch-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.6
+Version: 1.2.7
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.6/README.md` & `audiolm-pytorch-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/attend.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/audiolm_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1371,15 +1371,15 @@
                 text_embeds = self.transformer.embed_text(text, output_device = device)
 
         if self.unique_consecutive:
             semantic_token_ids = batch_unique_consecutive(semantic_token_ids, pad_value=self.pad_id)
 
         # initialize
 
-        init_coarse_time_step = coarse_token_ids.shape[-1]
+        init_coarse_time_step = 0
         sampled_coarse_token_ids = coarse_token_ids.clone()
 
         for time_step in tqdm(range(init_coarse_time_step, max_time_steps), desc = 'generating coarse'):
             for ind in range(self.num_coarse_quantizers):
                 just_finished_quantizer_step = (ind == 0 and time_step > 0)
 
                 _, coarse_logits = self.transformer.forward_with_cond_scale(
@@ -1616,15 +1616,15 @@
             fine_token_ids = token_ids[..., self.num_coarse_quantizers:]
             fine_token_ids = rearrange(fine_token_ids, 'b ... -> b (...)')
         else:
             fine_token_ids = torch.empty((batch, 0), device = device, dtype = torch.long)
 
         # calculate number of sampling steps
 
-        init_fine_time_step = fine_token_ids.shape[-1]
+        init_fine_time_step = fine_token_ids.shape[-1] // self.num_fine_quantizers
         max_time_steps = coarse_token_ids.shape[1] // self.num_coarse_quantizers
 
         sampled_fine_token_ids = fine_token_ids.clone()
 
         for time_step in tqdm(range(init_fine_time_step, max_time_steps), desc = 'generating fine'):
             for ind in range(self.num_fine_quantizers):
                 just_finished_quantizer_step = (ind == 0 and time_step > 0)
```

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/data.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.2.7/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.6
+Version: 1.2.7
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.6/setup.py` & `audiolm-pytorch-1.2.7/setup.py`

 * *Files identical despite different names*

