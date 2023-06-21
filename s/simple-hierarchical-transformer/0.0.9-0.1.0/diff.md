# Comparing `tmp/simple-hierarchical-transformer-0.0.9.tar.gz` & `tmp/simple-hierarchical-transformer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.9.tar", last modified: Wed Apr 12 02:50:51 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.1.0.tar", last modified: Wed Jun 21 17:46:35 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.9.tar` & `simple-hierarchical-transformer-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:46:35.635044 simple-hierarchical-transformer-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 17:46:25.000000 simple-hierarchical-transformer-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 17:46:35.635044 simple-hierarchical-transformer-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-21 17:46:25.000000 simple-hierarchical-transformer-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:46:35.635044 simple-hierarchical-transformer-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-21 17:46:25.000000 simple-hierarchical-transformer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:46:35.631044 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 17:46:25.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-21 17:46:25.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24863 2023-06-21 17:46:25.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:46:35.635044 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 17:46:35.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-21 17:46:35.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:46:35.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 17:46:35.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 17:46:35.000000 simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.9/LICENSE` & `simple-hierarchical-transformer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.9/PKG-INFO` & `simple-hierarchical-transformer-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.9/README.md` & `simple-hierarchical-transformer-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 ## Simple Hierarchical Transformer
 
 Experiments around a simple idea for inducing multiple hierarchical predictive coding models within a GPT. It is so simple, it may not work. But then again, deep learning progress is built on the bedrocks of simple ideas. Worth a shot.
 
 So far, the idea has passed the litmus test from a research friend. Will bring it to completion in the next week or so. If it does not work out, I'll leave the negative experimental results as well as the repository around, and maybe some PhD student can build upon it.
 
-<a href="https://api.wandb.ai/links/lucidrains/w8vdkz75">Ongoing experiments</a>
-
 Update: I think it is working 🤞 
 
 ## Appreciation
 
 - <a href="https://stability.ai/">StabilityAI</a> for the sponsorship to carry out this independent research
 
 - <a href="https://huggingface.co/">🤗 Huggingface</a> for their accelerate library
@@ -32,15 +30,15 @@
     num_tokens = 20000,                # number of tokens
     dim = 512,                         # model dimensions
     depth = 6,                         # depth
     dim_head = 64,                     # dimension per attention head
     heads = 8,                         # attention heads
     seq_len = 2048,                    # sequence lengths
     hierarchies = (1, 2, 8),           # hierarchies - here we have 1x (like in a regular transformer), then 2x and 8x compressed hierarchical tokens that undergo their own transformer blocks. information is pooled into one hierarchy at each layer
-    window_sizes = (32, 64, None)      # local attention window sizes - the idea is that the higher hierarchies can pass distant information to the local one. None stands for full receptive field
+    window_sizes = (32, 64, None)      # local attention window sizes - the idea is that the higher hierarchies can pass distant information to the local one. None stands for full receptive field. Setting 0 would turn off attention at this hierarchy altogether (while token shift will still be in effect in each layer)
 )
 
 ids = torch.randint(0, 20000, (1, 2048))
 
 loss, _ = model(ids, return_loss = True)
 loss.backward()
 
@@ -64,31 +62,59 @@
     seq_len = 2048,
     hierarchies = 1,        # implied 1 if not set
     window_sizes = None     # implied None (full sequence length) if not set
 )
 
 ```
 
+Now something more complex. Experiments show that as you compress up the hierarchies, you need greater model dimensions for appropriate capacity.
+
+```python
+model = HierarchicalTransformer(
+    num_tokens = 256,
+    dim = (128, 256, 512, 1024),
+    depth = 8,
+    seq_len = 1024,
+    use_flash_attn = True,
+    ff_mult = (2, 2, 4, 4),
+    dim_head = (16, 32, 64, 64),
+    heads = (2, 4, 8, 8),
+    hierarchies = (1, 2, 4, 16),
+    hierarchical_stride = (1, 1, 1, 8),  # this would determine the stride when compressing, and when concatting the hierarchical tokens to the fine tokens, the past tokens will be repeated this amount of time. causality is not violated as using the trick from hourglass transformers where sequence is shifted by compression factor - 1. recommend sticking with 1 except for highly compressed hierarchies, as it becomes very uncompetitive with baseline and generations look off
+    window_sizes = (16, 32, 64, None)
+).cuda()
+
+# hierarchies
+# 1x - dim 128 - attention (2 heads, 16 dim, receptive field 16)
+# 2x - dim 256 - attention (4 heads, 32 dim, receptive field 32)
+# 4x - dim 512 - attention (8 heads, 64 dim, receptive field 64)
+# 8x - dim 1024 - attention (8 heads, 64 dim, receptive field of all)
+```
+
 ## Todo
 
 - [x] branch out to two parallel paths, one for hierarchical tokens, other for plain fine tokens.
 - [x] show that local attention in fine + hierarchical tokens can come close to full attention baseline
 - [x] simple dsconv seems enough to merge for 1 hierarchy
 - [x] auto-set window size to be half of max sequence length for fine and all hierarchies
 - [x] figure out effects of just pooling all fine + hierarchical tokens before cross entropy loss - not much of a difference
 - [x] complete ability to add any number of hierarchies, and designate which hierarchy will pool the information from the others for prediction
+- [x] fully customizable dimensions across hierarchies, as higher hierarchies require greater model dimensions
+- [x] add prophet losses for hierarchical branches
+- [x] allow for repeating hierarchy tokens for fine tokens in the future, as position may matter less as one goes up the hierarchy. but not a priority, get things working first - implemented as `hierarchical_stride`
+- [x] allow for some layers to only rely on token shift, no attention
+- [x] random projections + vq, as was done in universal speech model paper from brain - for hierarchical predictive coding
 
-- [ ] try a few types of attention across hierarchies. full self attention, directional, or even token shift and feedforward
-- [ ] fully customizable dimensions across hierarchies, as higher hierarchies require greater model dimensions
-- [ ] play around with an autoregressive loss on the hierarchy tokens, can try with random projections + vq, as was done in universal speech model paper from brain - also try prophet loss
-- [ ] allow for repeating hierarchy tokens for fine tokens in the future, as position may matter less as one goes up the hierarchy. but not a priority, get things working first
+- [ ] allow for specifying which hierarchy receives information from the others during merging, maybe design a specialized attention with masking, but need to account fo different model dimensions across hierarchies
 - [ ] build out simple local attention block, for use across all hierarchies
 - [ ] add flash attention to local attention library
 - [ ] figure out if attention can be shared across hierarchies
-
+- [ ] do a clean wandb report showing 2x compression without much loss for character level enwik8
+- [ ] try a self attention based compressor for hierarchies 4 or above
+- [ ] build a small autoencoder using the token embeddings as input, at the very beginning of the network, and then use intermediate feature maps for each parallel hierarchical network
 
 ## Citations
 
 Closest idea would be <a href="https://arxiv.org/abs/2110.13711">hourglass transformers</a>.
 
 And my renewed interest in hierarchical approaches came from reading <a href="https://www.nature.com/articles/s41562-022-01516-2">this</a>.
 
@@ -148,7 +174,16 @@
     year      = {2021},
     publisher = {Zenodo},
     version   = {0.01},
     doi       = {10.5281/zenodo.5196578},
     url       = {https://doi.org/10.5281/zenodo.5196578}
 }
 ```
+
+```bibtex
+@inproceedings{Chiu2022SelfsupervisedLW,
+    title   = {Self-supervised Learning with Random-projection Quantizer for Speech Recognition},
+    author  = {Chung-Cheng Chiu and James Qin and Yu Zhang and Jiahui Yu and Yonghui Wu},
+    booktitle = {International Conference on Machine Learning},
+    year    = {2022}
+}
+```
```

#### html2text {}

```diff
@@ -1,61 +1,85 @@
 ## Simple Hierarchical Transformer Experiments around a simple idea for
 inducing multiple hierarchical predictive coding models within a GPT. It is so
 simple, it may not work. But then again, deep learning progress is built on the
 bedrocks of simple ideas. Worth a shot. So far, the idea has passed the litmus
 test from a research friend. Will bring it to completion in the next week or
 so. If it does not work out, I'll leave the negative experimental results as
 well as the repository around, and maybe some PhD student can build upon it.
-Ongoing_experiments Update: I think it is working ð¤ ## Appreciation -
-StabilityAI for the sponsorship to carry out this independent research - ð¤
-Huggingface for their accelerate library ## Install ``` $ pip install simple-
-hierarchical-transformer ``` ## Usage Three hierarchies, all servicing
-predicting the next token ```python import torch from
-simple_hierarchical_transformer import HierarchicalTransformer model =
-HierarchicalTransformer( num_tokens = 20000, # number of tokens dim = 512, #
-model dimensions depth = 6, # depth dim_head = 64, # dimension per attention
-head heads = 8, # attention heads seq_len = 2048, # sequence lengths
-hierarchies = (1, 2, 8), # hierarchies - here we have 1x (like in a regular
-transformer), then 2x and 8x compressed hierarchical tokens that undergo their
-own transformer blocks. information is pooled into one hierarchy at each layer
-window_sizes = (32, 64, None) # local attention window sizes - the idea is that
-the higher hierarchies can pass distant information to the local one. None
-stands for full receptive field ) ids = torch.randint(0, 20000, (1, 2048))
-loss, _ = model(ids, return_loss = True) loss.backward() # after much training
-logits = model(ids) ``` By not specifying `hierarchies` and `window_sizes`, you
+Update: I think it is working ð¤ ## Appreciation - StabilityAI for the
+sponsorship to carry out this independent research - ð¤_Huggingface for their
+accelerate library ## Install ``` $ pip install simple-hierarchical-transformer
+``` ## Usage Three hierarchies, all servicing predicting the next token
+```python import torch from simple_hierarchical_transformer import
+HierarchicalTransformer model = HierarchicalTransformer( num_tokens = 20000, #
+number of tokens dim = 512, # model dimensions depth = 6, # depth dim_head =
+64, # dimension per attention head heads = 8, # attention heads seq_len = 2048,
+# sequence lengths hierarchies = (1, 2, 8), # hierarchies - here we have 1x
+(like in a regular transformer), then 2x and 8x compressed hierarchical tokens
+that undergo their own transformer blocks. information is pooled into one
+hierarchy at each layer window_sizes = (32, 64, None) # local attention window
+sizes - the idea is that the higher hierarchies can pass distant information to
+the local one. None stands for full receptive field. Setting 0 would turn off
+attention at this hierarchy altogether (while token shift will still be in
+effect in each layer) ) ids = torch.randint(0, 20000, (1, 2048)) loss, _ =
+model(ids, return_loss = True) loss.backward() # after much training logits =
+model(ids) ``` By not specifying `hierarchies` and `window_sizes`, you
 basically default to a regular autoregressive transformer with attention across
 full sequence length. ```python # non-hierarchical transformer model =
 HierarchicalTransformer( num_tokens = 20000, dim = 512, depth = 8, dim_head =
 64, heads = 8, seq_len = 2048, hierarchies = 1, # implied 1 if not set
-window_sizes = None # implied None (full sequence length) if not set ) ``` ##
-Todo - [x] branch out to two parallel paths, one for hierarchical tokens, other
-for plain fine tokens. - [x] show that local attention in fine + hierarchical
-tokens can come close to full attention baseline - [x] simple dsconv seems
-enough to merge for 1 hierarchy - [x] auto-set window size to be half of max
-sequence length for fine and all hierarchies - [x] figure out effects of just
-pooling all fine + hierarchical tokens before cross entropy loss - not much of
-a difference - [x] complete ability to add any number of hierarchies, and
-designate which hierarchy will pool the information from the others for
-prediction - [ ] try a few types of attention across hierarchies. full self
-attention, directional, or even token shift and feedforward - [ ] fully
-customizable dimensions across hierarchies, as higher hierarchies require
-greater model dimensions - [ ] play around with an autoregressive loss on the
-hierarchy tokens, can try with random projections + vq, as was done in
-universal speech model paper from brain - also try prophet loss - [ ] allow for
+window_sizes = None # implied None (full sequence length) if not set ) ``` Now
+something more complex. Experiments show that as you compress up the
+hierarchies, you need greater model dimensions for appropriate capacity.
+```python model = HierarchicalTransformer( num_tokens = 256, dim = (128, 256,
+512, 1024), depth = 8, seq_len = 1024, use_flash_attn = True, ff_mult = (2, 2,
+4, 4), dim_head = (16, 32, 64, 64), heads = (2, 4, 8, 8), hierarchies = (1, 2,
+4, 16), hierarchical_stride = (1, 1, 1, 8), # this would determine the stride
+when compressing, and when concatting the hierarchical tokens to the fine
+tokens, the past tokens will be repeated this amount of time. causality is not
+violated as using the trick from hourglass transformers where sequence is
+shifted by compression factor - 1. recommend sticking with 1 except for highly
+compressed hierarchies, as it becomes very uncompetitive with baseline and
+generations look off window_sizes = (16, 32, 64, None) ).cuda() # hierarchies #
+1x - dim 128 - attention (2 heads, 16 dim, receptive field 16) # 2x - dim 256 -
+attention (4 heads, 32 dim, receptive field 32) # 4x - dim 512 - attention (8
+heads, 64 dim, receptive field 64) # 8x - dim 1024 - attention (8 heads, 64
+dim, receptive field of all) ``` ## Todo - [x] branch out to two parallel
+paths, one for hierarchical tokens, other for plain fine tokens. - [x] show
+that local attention in fine + hierarchical tokens can come close to full
+attention baseline - [x] simple dsconv seems enough to merge for 1 hierarchy -
+[x] auto-set window size to be half of max sequence length for fine and all
+hierarchies - [x] figure out effects of just pooling all fine + hierarchical
+tokens before cross entropy loss - not much of a difference - [x] complete
+ability to add any number of hierarchies, and designate which hierarchy will
+pool the information from the others for prediction - [x] fully customizable
+dimensions across hierarchies, as higher hierarchies require greater model
+dimensions - [x] add prophet losses for hierarchical branches - [x] allow for
 repeating hierarchy tokens for fine tokens in the future, as position may
 matter less as one goes up the hierarchy. but not a priority, get things
-working first - [ ] build out simple local attention block, for use across all
-hierarchies - [ ] add flash attention to local attention library - [ ] figure
-out if attention can be shared across hierarchies ## Citations Closest idea
-would be hourglass_transformers. And my renewed interest in hierarchical
-approaches came from reading this. ```bibtex @article{Nawrot2021HierarchicalTA,
-title = {Hierarchical Transformers Are More Efficient Language Models}, author
-= {Piotr Nawrot and Szymon Tworkowski and Michal Tyrolski and Lukasz Kaiser and
-Yuhuai Wu and Christian Szegedy and Henryk Michalewski}, journal = {ArXiv},
-year = {2021}, volume = {abs/2110.13711} } ``` ```bibtex @inproceedings
+working first - implemented as `hierarchical_stride` - [x] allow for some
+layers to only rely on token shift, no attention - [x] random projections + vq,
+as was done in universal speech model paper from brain - for hierarchical
+predictive coding - [ ] allow for specifying which hierarchy receives
+information from the others during merging, maybe design a specialized
+attention with masking, but need to account fo different model dimensions
+across hierarchies - [ ] build out simple local attention block, for use across
+all hierarchies - [ ] add flash attention to local attention library - [ ]
+figure out if attention can be shared across hierarchies - [ ] do a clean wandb
+report showing 2x compression without much loss for character level enwik8 -
+[ ] try a self attention based compressor for hierarchies 4 or above - [ ]
+build a small autoencoder using the token embeddings as input, at the very
+beginning of the network, and then use intermediate feature maps for each
+parallel hierarchical network ## Citations Closest idea would be hourglass
+transformers. And my renewed interest in hierarchical approaches came from
+reading this. ```bibtex @article{Nawrot2021HierarchicalTA, title =
+{Hierarchical Transformers Are More Efficient Language Models}, author = {Piotr
+Nawrot and Szymon Tworkowski and Michal Tyrolski and Lukasz Kaiser and Yuhuai
+Wu and Christian Szegedy and Henryk Michalewski}, journal = {ArXiv}, year =
+{2021}, volume = {abs/2110.13711} } ``` ```bibtex @inproceedings
 {dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
 Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
 Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
 in Neural Information Processing Systems}, year = {2022} } ``` ```bibtex
 @article{Yan2020ProphetNetPF, title = {ProphetNet: Predicting Future N-gram for
 Sequence-to-Sequence Pre-training}, author = {Yu Yan and Weizhen Qi and Yeyun
 Gong and Dayiheng Liu and Nan Duan and Jiusheng Chen and Ruofei Zhang and Ming
@@ -66,8 +90,12 @@
 archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @inproceedings
 {Sun2022ALT, title = {A Length-Extrapolatable Transformer}, author = {Yutao Sun
 and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim
 and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex
 @software{peng_bo_2021_5196578, author = {PENG Bo}, title = {BlinkDL/RWKV-LM:
 0.01}, month = {aug}, year = {2021}, publisher = {Zenodo}, version = {0.01},
 doi = {10.5281/zenodo.5196578}, url = {https://doi.org/10.5281/zenodo.5196578}
+} ``` ```bibtex @inproceedings{Chiu2022SelfsupervisedLW, title = {Self-
+supervised Learning with Random-projection Quantizer for Speech Recognition},
+author = {Chung-Cheng Chiu and James Qin and Yu Zhang and Jiahui Yu and Yonghui
+Wu}, booktitle = {International Conference on Machine Learning}, year = {2022}
 } ```
```

### Comparing `simple-hierarchical-transformer-0.0.9/setup.py` & `simple-hierarchical-transformer-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.9',
+  version = '0.1.0',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
@@ -18,15 +18,15 @@
     'hierarchical'
   ],
   install_requires=[
     'accelerate',
     'einops>=0.4',
     'local-attention',
     'torch>=1.6',
-    'vector-quantize-pytorch'
+    'vector-quantize-pytorch>=1.6.23'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import math
 from functools import partial
+from itertools import zip_longest
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, repeat
 from einops.layers.torch import Rearrange
 
 from simple_hierarchical_transformer.attention import Attend
 
+from typing import Tuple
 from local_attention import LocalMHA
 
+from vector_quantize_pytorch import RandomProjectionQuantizer
+
 # constants
 
 mlist = nn.ModuleList
 
 Linear = partial(nn.Linear, bias = False)
 
 LocalMHA = partial(LocalMHA, causal = True, prenorm = True)
@@ -27,14 +31,17 @@
 
 def is_power_of_two(n):
     return math.log2(n).is_integer()
 
 def all_unique(arr):
     return len(set(arr)) == len(arr)
 
+def apply_fns(fns, tensors):
+    return [fn(tensor) for fn, tensor in zip(fns, tensors)]
+
 def cast_tuple(t, length = 1):
     return t if isinstance(t, tuple) else ((t,) * length)
 
 def default(*vals):
     for val in vals:
         if exists(val):
             return val
@@ -142,116 +149,148 @@
 
     if remainder == 0:
         return t, seq_len
 
     t = F.pad(t, (0, 0, 0, remainder), value = 0.)
     return t, seq_len
 
+def curtail_seq_to_multiple(t, mult):
+    seq_len = t.shape[-2]
+    prev_seq_len_mult = (seq_len // mult) * mult
+    remainder = seq_len - prev_seq_len_mult
+
+    if remainder == 0:
+        return t
+
+    t = t[..., :prev_seq_len_mult, :]
+    return t
+
+def hierarchical_cat(tokens, strides: Tuple[int, ...]):
+    assert len(tokens) == len(strides)
+
+    if all([s == 1 for s in strides]):
+        return torch.cat(tokens, dim = -1)
+
+    tokens = [repeat(t, 'b n d -> b (n s) d', s = s) for t, s in zip(tokens, strides)]
+    min_seq_len = min([t.shape[-2] for t in tokens])
+    tokens = [t[..., :min_seq_len, :] for t in tokens]
+    return torch.cat(tokens, dim = -1)
+
 class CausalConv(nn.Module):
     def __init__(
         self,
         dim_in,
         dim_out,
-        kernel_size
+        kernel_size,
+        stride = 1
     ):
         super().__init__()
         self.causal_padding = kernel_size - 1
-        self.conv = nn.Conv1d(dim_in, dim_out, kernel_size)
+        self.conv = nn.Conv1d(dim_in, dim_out, kernel_size, stride = stride)
 
     def forward(self, x):
         x = F.pad(x, (self.causal_padding, 0))
         return self.conv(x)
 
 class Compress(nn.Module):
     def __init__(
         self,
         *,
         dim,
-        num_tokens,
-        compress_factor = 2,
+        dim_out,
+        num_tokens = None,
+        stride = 1,
+        compress_factor = 1,
         expansion_factor = 4,
         dim_head = 64,
         heads = 8,
-        ignore_index = 0
+        ignore_index = 0,
+        should_recon = False,
+        prophet_num_predictions = None
     ):
         super().__init__()
         assert compress_factor > 0 and is_power_of_two(compress_factor)
 
+        self.stride = stride
         self.no_compress = compress_factor == 1
         self.compress_factor = compress_factor
 
+        self.should_recon = should_recon
+
         if self.no_compress:
-            self.compress_fn = nn.Identity()
+            self.compress_fn = Linear(dim, dim_out) if dim != dim_out else nn.Identity()
             return
 
         dim_inner = int(dim * expansion_factor)
 
         self.compress_fn = nn.Sequential(
             Rearrange('b n d -> b d n'),
-            CausalConv(dim, dim_inner, compress_factor),
+            CausalConv(dim, dim_inner, compress_factor, stride = stride),
             nn.SiLU(),
-            nn.Conv1d(dim_inner, dim, 1),
+            nn.Conv1d(dim_inner, dim_out, 1),
             Rearrange('b d n -> b n d')
         )
 
-        self.to_recon = Linear(dim, compress_factor * num_tokens)
+        if should_recon:
+            assert exists(num_tokens)
+            self.to_recon = Linear(dim_out, compress_factor * num_tokens)
+
         self.ignore_index = ignore_index
 
     def recon(self, h, ids):
+        assert self.should_recon
 
         if self.no_compress:
             return torch.zeros((), device = h.device).requires_grad_()
 
         c = self.compress_factor
         seq_len = ids.shape[-1]
 
         recon_logits = self.to_recon(h)
         recon_logits = rearrange(recon_logits, 'b n (c d) -> (b c) d n', c = c)
 
-        recon_ids = F.pad(ids, (c - 1, 0), value = 0)
+        recon_ids = F.pad(ids, (c - 1, 0), value = self.ignore_index)
         recon_ids = tuple(recon_ids[:, i:(seq_len + i)] for i in range(c))
         recon_ids = torch.stack(recon_ids, dim = 1)
         recon_ids = rearrange(recon_ids, 'b c n -> (b c) n')
 
+        if self.stride > 1:
+            recon_ids = recon_ids[..., ::self.stride]
+
         recon_loss = F.cross_entropy(recon_logits, recon_ids, ignore_index = self.ignore_index)
         return recon_loss
 
     def forward(self, x):
         return self.compress_fn(x)
 
 class HierarchicalMerge(nn.Module):
     def __init__(
         self,
-        dim,
-        num_hierarchies = 2
+        dims: Tuple[int, ...],
+        dim_out,
+        h_strides = 1
     ):
         super().__init__()
-        self.norms = mlist([RMSNorm(dim) for _ in range(num_hierarchies)])
+        dim = sum(dims)
 
-        # simple dsconv for now
+        strides = cast_tuple(h_strides, len(dims))
+        assert len(strides) == len(dims)
 
-        self.num_hierarchies = num_hierarchies
-        self.conv = nn.Conv1d(dim, dim, num_hierarchies, stride = num_hierarchies, groups = dim)
+        self.strides = strides
 
-    def forward(self, tokens):
-        """
-        einops notations:
-        b - batch
-        h - hierarchies
-        n - sequence length
-        d - dimension
-        """
-        nh = self.num_hierarchies
-
-        tokens = [norm(h) for norm, h in zip(self.norms, tokens)]
+        self.net = nn.Sequential(
+            RMSNorm(dim),
+            nn.Linear(dim, dim_out * 2),
+            nn.SiLU(),
+            nn.Linear(dim_out * 2, dim_out)
+        )
 
-        x = rearrange(tokens, 'h b n d -> b d (n h)')
-        x = self.conv(x)
-        x = rearrange(x, 'b d n -> b n d')
-        return x
+    def forward(self, tokens):
+        x = hierarchical_cat(tokens, self.strides)
+        return self.net(x)
 
 # classes
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.scale = dim ** 0.5
@@ -307,53 +346,69 @@
         q, k = apply_rotary_pos_emb_qk(rotary_emb, q, k)
 
         out = self.attend(q, k, v)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
-class HierarchicalAttention(nn.Module):
+class HierarchicalBlock(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
         window_size = None,
-        compress_factor = 1
+        compress_factor = 1,
+        stride = 1,
+        ff_mult = 4
     ):
         super().__init__()
+        self.stride = stride
+
         assert is_power_of_two(compress_factor)
         self.compress_factor = compress_factor
         self.no_compress = compress_factor == 1
 
-        attn_klass = Attention
+        assert not exists(window_size) or window_size >= 0
+        self.has_attn = window_size != 0
+
+        self.attn = None
 
-        if exists(window_size):
-            attn_klass = partial(LocalMHA, window_size = window_size)
+        if self.has_attn:
+            attn_klass = Attention
+            if exists(window_size):
+                attn_klass = partial(LocalMHA, window_size = window_size)
 
-        self.attn = attn_klass(dim = dim, dim_head = dim_head, heads = heads)
+            self.attn = attn_klass(dim = dim, dim_head = dim_head, heads = heads)
+
+        self.ff = FeedForward(dim = dim, mult = ff_mult)
 
     def forward(self, x):
         c = self.compress_factor
-        x, orig_seq_len = pad_seq_to_multiple(x, c)
+        axial_dim = c // self.stride
+
+        x, orig_seq_len = pad_seq_to_multiple(x, axial_dim)
 
         # hierarchical attention is performed with a simple axial attention
 
         # this, and using a convolution for compressing at the beginning
         # is one of the improvements on top of hourglass transformer
-        # the downside is that the savings are only O(c) instead of O(c ** 2)
-        # but this should provide better learning per-token
+        # the downside is that the savings are only O(c) instead of O(c ** 2) as in hourglass transformer
+        # you can get the O(c ** 2) saving by setting the hierarchical stride == c, but you'll see that performance is much worse, as some tokens will have a c - 1 token gap to the last hierarchical token
 
         if not self.no_compress:
-            x = rearrange(x, 'b (n c) d -> (b c) n d', c = c)
+            x = rearrange(x, 'b (n c) d -> (b c) n d', c = axial_dim)
+
+        if exists(self.attn):
+            x = self.attn(token_shift(x)) + x
 
-        x = self.attn(x)
+        x = self.ff(token_shift(x)) + x
 
         if not self.no_compress:
-            x = rearrange(x, '(b c) n d -> b (n c) d', c = c)
+            x = rearrange(x, '(b c) n d -> b (n c) d', c = axial_dim)
 
         return x[:, :orig_seq_len]
 
 class HierarchicalTransformer(nn.Module):
     def __init__(
         self,
         *,
@@ -361,106 +416,194 @@
         dim,
         depth,
         seq_len = 2048,
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
         hierarchies = 1,
-        predict_hierarchy = None,
         window_sizes = None,
+        hierarchical_stride = 1,
+        hierarchy_merge_all = False,  # whether to pass the pooled hierarchical information back to all hierarchies or just one doing the prediction
         ignore_index = 0,
+        use_flash_attn = False,
         recon_loss_weight = 0.1,
-        use_flash_attn = False
+        prophet_loss_weight = 0.,
+        prophet_loss_use_quantized = False, # for prophet, whether to use the next 1x token ids, or use the ids from random projection quantization
+        prophet_quantized_use_embed = False,
+        predict_hierarchy = None,
+        predict_use_all_hierarchy = False,
+        rq_num_codebooks = 4,
+        rq_codebook_dim = 256,
+        rq_codebook_size = 1024,
     ):
         super().__init__()
         self.seq_len = seq_len
 
-        self.token_emb = nn.Embedding(num_tokens, dim)
-        self.post_token_emb_norm = RMSNorm(dim)
-
-        hierarchies = tuple(sorted(cast_tuple(hierarchies)))
-
+        hierarchies = cast_tuple(hierarchies)
         assert all_unique(hierarchies), 'hierarchies compression factors must be all unique integers'
         assert all([*map(is_power_of_two, hierarchies)]), 'only powers of two allowed for hierarchies'
 
+        self.hierarchies = hierarchies
+
+        # just use a simple tuple list per hyperparameter to customize each hierarchy
+
         num_hierarchies = len(hierarchies)
-        predict_hierarchy = default(predict_hierarchy, min(hierarchies))
 
-        self.predict_hierarchy_index = hierarchies.index(predict_hierarchy)
+        dims = cast_tuple(dim, num_hierarchies)
+        assert len(dims) == num_hierarchies
 
         window_sizes = cast_tuple(window_sizes, num_hierarchies)
-        assert len(window_sizes) == len(hierarchies)
+        assert len(window_sizes) == num_hierarchies
+
+        dim_head = cast_tuple(dim_head, num_hierarchies)
+        assert len(dim_head) == num_hierarchies
+
+        heads = cast_tuple(heads, num_hierarchies)
+        assert len(heads) == num_hierarchies
+
+        ff_mult = cast_tuple(ff_mult, num_hierarchies)
+        assert len(ff_mult) == num_hierarchies
+
+        hierarchical_stride = cast_tuple(hierarchical_stride, num_hierarchies)
+
+        assert all([*map(is_power_of_two, hierarchical_stride)]), 'all hierarchical strides must be power of two'
+        assert all([s <= h for s, h in zip(hierarchical_stride, hierarchies)]), 'all strides must be less than the compression factor of the hierarchy'
+
+        self.h_strides = hierarchical_stride
+
+        assert len(hierarchical_stride) == num_hierarchies
+
+        # this determines to which hierarchy is everything pooled into for final prediction
+        # however, final next token prediction can also use all hierarchies with `predict_use_all_hierarchy`
+
+        predict_hierarchy = default(predict_hierarchy, min(hierarchies))
+        self.predict_hierarchy_index = hierarchies.index(predict_hierarchy)
+        hierarchy_predict_dim = dims[self.predict_hierarchy_index]
+
+        self.hierarchy_merge_all = hierarchy_merge_all
+        assert hierarchy_merge_all or self.h_strides[self.predict_hierarchy_index] == 1, 'the hierarchy level being used for final next token prediction must have compression stride of 1'
+
+        # training related loss weights
+
+        self.recon_loss_weight = recon_loss_weight
+        self.prophet_loss_weight = prophet_loss_weight
+
+        should_recon = recon_loss_weight > 0
+        should_prophet = prophet_loss_weight > 0
+
+        self.should_recon = should_recon
+        self.should_prophet = should_prophet
+
+        self.prophet_loss_use_quantized = prophet_loss_use_quantized
+        self.prophet_quantized_use_embed = prophet_quantized_use_embed
+
+        # token embedding
+
+        dim_token_emb = max(dims)
+        self.token_emb = nn.Embedding(num_tokens, dim_token_emb)
 
         # hierarchy compressions - 1x just uses the base token_emb weights
 
         self.compressors = mlist([])
 
-        for hierarchy in hierarchies:
+        for dim, hierarchy, stride in zip(dims, hierarchies, hierarchical_stride):
             self.compressors.append(Compress(
-                dim = dim,
+                dim = dim_token_emb,
+                dim_out = dim,
                 num_tokens = num_tokens,
                 compress_factor = hierarchy,
+                stride = stride,
+                should_recon = should_recon
             ))
 
+        # post token embedding norms
+
+        self.post_token_emb_norms = mlist([nn.LayerNorm(dim) for dim in dims])
+
         # layers
 
         self.layers = mlist([])
-        self.hierarchical_merges = mlist([])
 
-        local_attn = partial(LocalMHA, causal = True, prenorm = True)
+        self.dims = dims
+
+        self.hierarchical_merges = mlist([])
+        self.need_hierarchical_merge = num_hierarchies > 1
 
         for _ in range(depth):
             hierarchical_layer = mlist([])
 
             # add a transformer block for each layer in the hierarchy
 
-            for hierarchy, window_size in zip(hierarchies, window_sizes):
+            for hierarchy, h_stride, h_dim, h_window_size, h_dim_head, h_heads, h_ff_mult in zip(hierarchies, hierarchical_stride, dims, window_sizes, dim_head, heads, ff_mult):
 
                 # make sure the window size never exceeds the effective sequence length
 
                 effective_seq_len = seq_len // hierarchy
 
-                if exists(window_size) and window_size > effective_seq_len:
+                if exists(h_window_size) and h_window_size > effective_seq_len:
                     print(f'window size for hierarchy {hierarchy}x is greater than effective sequence length - setting window size to None (which would use normal full attention)')
-                    window_size = None
+                    h_window_size = None
 
                 # add attention and feedforward
 
-                hierarchical_layer.append(mlist([
-                    HierarchicalAttention(
-                        dim = dim,
-                        dim_head = dim_head,
-                        heads = heads,
-                        window_size = window_size,
-                        compress_factor = hierarchy
-                    ),
-                    FeedForward(dim = dim, mult = ff_mult)
-                ]))
+                hierarchical_layer.append(
+                    HierarchicalBlock(
+                        dim = h_dim,
+                        dim_head = h_dim_head,
+                        heads = h_heads,
+                        window_size = h_window_size,
+                        compress_factor = hierarchy,
+                        stride = h_stride,
+                        ff_mult = h_ff_mult
+                    )
+                )
 
             self.layers.append(hierarchical_layer)
 
             # for merging the information across hierarchies
             # for now, only one direction, from all hierarchies to the hierarchy that is being used to make predictions on, set by predict_hierarchy_index above
 
-            merge = HierarchicalMerge(dim = dim, num_hierarchies = num_hierarchies)
+            if not self.need_hierarchical_merge:
+                continue
+
+            merge = HierarchicalMerge(
+                dims = dims,
+                dim_out = hierarchy_predict_dim if not self.hierarchy_merge_all else sum(dims),
+                h_strides = hierarchical_stride
+            )
 
             self.hierarchical_merges.append(merge)
 
         # final post-transformer norms, for all hierarchies
 
-        self.norms = mlist([RMSNorm(dim) for _ in range(num_hierarchies)])
+        self.norms = mlist([nn.LayerNorm(dim) for dim in dims])
+
+        # random projection quantizer, for another approach to hierarchical predictive coding
+
+        if self.prophet_loss_use_quantized:
+            rpq_klass = partial(
+                RandomProjectionQuantizer,
+                num_codebooks = rq_num_codebooks,
+                codebook_dim = rq_codebook_dim,
+                codebook_size = rq_codebook_size
+            )
 
-        # to logit, for hierarchy set at predict_hierarchy_index
+            self.rand_proj_quantizers = mlist([rpq_klass(dim = dim) for dim in dims])
+            self.rq_num_codebooks = rq_num_codebooks
 
-        self.to_logits = Linear(dim, num_tokens)
+        # to logit, for hierarchy set at predict_hierarchy_index, or all hierarchies
+
+        self.predict_use_all_hierarchy = predict_use_all_hierarchy
+        logit_dim_in = sum(dims) if predict_use_all_hierarchy else hierarchy_predict_dim
+
+        self.to_logits = Linear(logit_dim_in, num_tokens)
 
         # training related loss parameters
 
         self.ignore_index = ignore_index
-        self.recon_loss_weight = recon_loss_weight
 
     @torch.no_grad()
     @eval_decorator
     def generate(
         self,
         prompt,
         seq_len,
@@ -485,15 +628,18 @@
     def device(self):
         return next(self.parameters()).device
     
     def forward(
         self,
         ids,
         return_loss = False,
-        ablate_hierarchical_merge = False
+        return_hierarchical_token_embeds = False,
+        return_hierarchical_embeds = False,
+        ablate_hierarchical_merge = False,
+        return_random_proj_quantize_ids = False
     ):
         """
         einops notation:
 
         b - batch
         n - sequence length
         c - compression factor
@@ -509,76 +655,134 @@
 
         assert ids.shape[-1] <= self.seq_len
 
         # get token embeddings, and pad to multiple of compression factor
 
         x = self.token_emb(ids)
 
-        # post embedding norm
-
-        x = self.post_token_emb_norm(x)
-
         # for every hierarchy, compress token embeddings appropriately to the hierarchical embeddings
 
         tokens = []
 
         for compress in self.compressors:
             tokens.append(compress(x))
 
-        # layers
+        # save hierarchical tokens right before norm for random projection quantization, if needed
+
+        post_compressed_tokens = tokens
 
-        for layer, merge in zip(self.layers, self.hierarchical_merges):
+        # post embedding norms
 
-            next_tokens = []
+        tokens = apply_fns(self.post_token_emb_norms, tokens)
 
-            for (attn, ff), h in zip(layer, tokens):
-                h = attn(h) + h
-                h = ff(token_shift(h)) + h
+        # if one wants all the compressed token embeds
+        # just to investigate the space
+
+        if return_hierarchical_token_embeds:
+            return tokens
+
+        # layers
 
-                next_tokens.append(h)
+        for layer, merge in zip_longest(self.layers, self.hierarchical_merges):
 
-            tokens = next_tokens
+            tokens = apply_fns(layer, tokens)
 
             # pool the information all hierarchies
             # and then update the tokens that will be used to make the final autoregressive prediction
 
-            if ablate_hierarchical_merge:
+            if not self.need_hierarchical_merge or ablate_hierarchical_merge:
                 continue
 
             pooled = merge(tokens)
-            predict_tokens = tokens[self.predict_hierarchy_index]
-            predict_tokens = predict_tokens + pooled
-            tokens[self.predict_hierarchy_index] = predict_tokens
 
-        # final norm and logits
+            if self.hierarchy_merge_all:
+                tokens = [(t + p[..., ::s, :]) for t, p, s in zip(tokens, pooled.split(self.dims, dim = -1), self.h_strides)]
+            else:
+                predict_tokens = tokens[self.predict_hierarchy_index]
+                predict_tokens = predict_tokens + pooled
+                tokens[self.predict_hierarchy_index] = predict_tokens
+
+        # if the researcher wants the randomly projected ids of either compressed tokens or embeddings of the hierarchies
+
+        if return_random_proj_quantize_ids:
+            assert self.prophet_loss_use_quantized
+
+            quantize_input = tokens if self.prophet_quantized_use_embed else post_compressed_tokens
+            hierarchical_ids = apply_fns(self.rand_proj_quantizers, quantize_input)
+            return hierarchical_ids
+
+        # final normalized embeddings
+
+        embeds = apply_fns(self.norms, tokens)
+
+        # if one wants all the normalized hierarchical embeds
 
-        tokens = [norm(t) for norm, t in zip(self.norms, tokens)]
+        if return_hierarchical_embeds:
+            return embeds
 
         # select the hierarchical embeddings that will be doing the predicting
 
-        predict_embed = tokens[self.predict_hierarchy_index]
+        if self.predict_use_all_hierarchy:
+            predict_embed = hierarchical_cat(embeds, self.h_strides)
+        else:
+            predict_embed = embeds[self.predict_hierarchy_index]
 
         # logits for predicting next token
 
         logits = self.to_logits(predict_embed)
 
         if not return_loss:
             return logits
 
+        ce_loss_fn = partial(F.cross_entropy, ignore_index = self.ignore_index)
+
         # autoregressive loss (predictive coding)
 
         logits = rearrange(logits, 'b n c -> b c n')
-        ce_loss = F.cross_entropy(logits, labels, ignore_index = self.ignore_index)
+        ce_loss = ce_loss_fn(logits, labels)
+
+        # reconstruction losses for hierarchy tokens
+
+        recon_losses = prophet_losses = torch.zeros((), device = self.device).requires_grad_()
+
+        if self.should_recon:
+            for compress, t in zip(self.compressors, embeds):
+                recon_loss = compress.recon(t, ids)
+                recon_losses = recon_losses + recon_loss
+
+        # prophet losses for hierarchy tokens
+
+        if self.should_prophet:
+            if self.prophet_loss_use_quantized:
+                # using random projected quantizer of the next hierarchical token
+
+                quantize_input = embed if self.prophet_quantized_use_embed else post_compressed_tokens
+
+                hierarchical_ids = apply_fns(self.rand_proj_quantizers, quantize_input)
+
+                for rand_proj_quantizer, hierarchy, stride, compress, embed, pred_ids in zip(self.rand_proj_quantizers, self.hierarchies, self.h_strides, self.compressors, embeds, hierarchical_ids):
+
+                    if hierarchy == 1:
+                        continue
+
+                    # vector-quantize-pytorch library can compute cross entropy loss on distance matrix
+
+                    prophet_loss = rand_proj_quantizer(
+                        embed[:, :-1],
+                        indices = pred_ids[:, 1:]
+                    )
 
-        # reconstruction losses for hierarchy tokens -> may remove if see no benefit, which seems to be leaning that way
+                    prophet_losses = prophet_losses + prophet_loss
 
-        recon_losses = 0
+            else:
+                # or predicting the next N 1x base token ids
+                # like prophetnet paper
 
-        for compress, t in zip(self.compressors, tokens):
-            recon_loss = compress.recon(t, ids)
-            recon_losses = recon_losses + recon_loss
+                for compress, t in zip(self.compressors, embeds):
+                    prophet_loss = compress.prophet(t, ids)
+                    prophet_losses = prophet_losses + prophet_loss
 
         # total loss
 
-        total_loss = ce_loss + recon_loss * self.recon_loss_weight
+        total_loss = ce_loss + recon_losses * self.recon_loss_weight + prophet_losses * self.prophet_loss_weight
 
-        return total_loss, (ce_loss, recon_loss)
+        return total_loss, (ce_loss, recon_losses, prophet_losses)
```

### Comparing `simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.1.0/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

