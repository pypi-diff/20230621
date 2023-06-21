# Comparing `tmp/denoising-diffusion-pytorch-1.8.1.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.1.tar", last modified: Tue Jun 20 20:51:00 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.2.tar", last modified: Wed Jun 21 14:03:43 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.1.tar` & `denoising-diffusion-pytorch-1.8.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36132 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 20:51:00.000000 denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 20:51:00.510675 denoising-diffusion-pytorch-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-20 20:50:50.000000 denoising-diffusion-pytorch-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36175 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.1/LICENSE` & `denoising-diffusion-pytorch-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/PKG-INFO` & `denoising-diffusion-pytorch-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.1
+Version: 1.8.2
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.1/README.md` & `denoising-diffusion-pytorch-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -908,16 +908,17 @@
 
         # prepare model, dataloader, optimizer with accelerator
 
         self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
 
         # FID-score computation
 
-        self.calculate_fid = calculate_fid
-        if calculate_fid:
+        self.calculate_fid = calculate_fid and self.accelerator.is_main_process
+
+        if self.calculate_fid:
             if not self.model.is_ddim_sampling:
                 self.accelerator.print(
                     "WARNING: Robust FID computation requires a lot of generated samples and can therefore be very time consuming."\
                     "Consider using DDIM sampling to save time."
                 )
             self.fid_scorer = FIDEvaluation(
                 batch_size=self.batch_size,
```

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.1
+Version: 1.8.2
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.1/setup.py` & `denoising-diffusion-pytorch-1.8.2/setup.py`

 * *Files identical despite different names*

