# Comparing `tmp/audiolm-pytorch-1.2.5.tar.gz` & `tmp/audiolm-pytorch-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.2.5.tar", last modified: Tue Jun 20 19:06:11 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.2.6.tar", last modified: Tue Jun 20 22:59:54 2023, max compression
```

## Comparing `audiolm-pytorch-1.2.5.tar` & `audiolm-pytorch-1.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:06:10.994884 audiolm-pytorch-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 19:06:10.994884 audiolm-pytorch-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:06:10.994884 audiolm-pytorch-1.2.5/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    67366 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:06:10.994884 audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 19:06:10.000000 audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 19:06:10.000000 audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:06:10.000000 audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 19:06:10.000000 audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 19:06:10.000000 audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:06:10.994884 audiolm-pytorch-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-20 19:06:00.000000 audiolm-pytorch-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68030 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 22:59:54.000000 audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:59:54.248891 audiolm-pytorch-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-20 22:59:42.000000 audiolm-pytorch-1.2.6/setup.py
```

### Comparing `audiolm-pytorch-1.2.5/LICENSE` & `audiolm-pytorch-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/PKG-INFO` & `audiolm-pytorch-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.5
+Version: 1.2.6
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.5/README.md` & `audiolm-pytorch-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/attend.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/audiolm_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1326,14 +1326,15 @@
     @torch.no_grad()
     @beartype
     def generate(
         self,
         *,
         semantic_token_ids,
         prime_wave: Optional[Tensor] = None,
+        prime_coarse_token_ids: Optional[Tensor] = None,
         text: Optional[List[str]] = None,
         text_embeds = None,
         max_time_steps = 512,
         cond_scale = 3.,
         filter_thres = 0.9,
         temperature = 1.,
         reconstruct_wave = False,
@@ -1342,15 +1343,19 @@
         batch, device = semantic_token_ids.shape[0], self.device
 
         semantic_token_ids = semantic_token_ids.to(device)
 
         # initialize coarse token ids
         # if a prime audio wave was supplied, then start off with appropriate acoustic tokens
 
-        if exists(prime_wave):
+        assert not (exists(prime_wave) and exists(prime_coarse_token_ids)), 'you can either pass in the prime as a raw wave (codec required) or as preprocessed acoustic token ids'
+
+        if exists(prime_coarse_token_ids):
+            coarse_token_ids = prime_coarse_token_ids
+        elif exists(prime_wave):
             assert exists(self.codec)
             with torch.no_grad():
                 self.codec.eval()
                 _, indices, _ = self.codec(prime_wave, return_encoded = True)
                 coarse_token_ids = indices[..., :self.num_coarse_quantizers]
                 coarse_token_ids = rearrange(coarse_token_ids, 'b ... -> b (...)')
         else:
@@ -1566,14 +1571,15 @@
     @torch.no_grad()
     @beartype
     def generate(
         self,
         *,
         coarse_token_ids,
         prime_wave: Optional[Tensor] = None,
+        prime_fine_token_ids: Optional[Tensor] = None,
         text: Optional[List[str]] = None,
         text_embeds = None,
         cond_scale = 3.,
         filter_thres = 0.9,
         temperature = 1.,
         reconstruct_wave = False,
         mask_out_generated_fine_tokens = False,
@@ -1593,15 +1599,19 @@
         if not exists(text_embeds) and exists(text):
             with torch.no_grad():
                 text_embeds = self.transformer.embed_text(text, output_device = device)
 
         # initialize fine token ids
         # if a prime wave was supplied, start off with fine acoustic tokens
 
-        if exists(prime_wave):
+        assert not (exists(prime_wave) and exists(prime_fine_token_ids)), 'you can either pass in the prime as a raw wave (codec required) or as preprocessed acoustic token ids'
+
+        if exists(prime_fine_token_ids):
+            fine_token_ids = prime_fine_token_ids
+        elif exists(prime_wave):
             assert exists(self.codec)
             with torch.no_grad():
                 self.codec.eval()
                 _, token_ids, _ = self.codec(prime_wave, return_encoded = True)
 
             fine_token_ids = token_ids[..., self.num_coarse_quantizers:]
             fine_token_ids = rearrange(fine_token_ids, 'b ... -> b (...)')
```

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/data.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.2.6/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.5
+Version: 1.2.6
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.5/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.2.6/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.5/setup.py` & `audiolm-pytorch-1.2.6/setup.py`

 * *Files identical despite different names*

