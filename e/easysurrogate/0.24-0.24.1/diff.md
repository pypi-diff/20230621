# Comparing `tmp/easysurrogate-0.24.tar.gz` & `tmp/easysurrogate-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easysurrogate-0.24.tar", last modified: Tue Jun 20 14:07:44 2023, max compression
+gzip compressed data, was "easysurrogate-0.24.1.tar", last modified: Wed Jun 21 08:38:00 2023, max compression
```

## Comparing `easysurrogate-0.24.tar` & `easysurrogate-0.24.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-20 14:07:44.356232 easysurrogate-0.24/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)    26526 2021-05-06 20:30:42.000000 easysurrogate-0.24/LICENSE
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       90 2023-06-20 14:07:44.356232 easysurrogate-0.24/PKG-INFO
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     4731 2023-06-19 14:14:19.000000 easysurrogate-0.24/README.md
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-20 14:07:44.352232 easysurrogate-0.24/easysurrogate/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       76 2021-11-30 12:39:19.000000 easysurrogate-0.24/easysurrogate/__init__.py
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-20 14:07:44.352232 easysurrogate-0.24/easysurrogate/analysis/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     5024 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/analysis/ANN_analysis.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)    10309 2021-11-30 12:39:19.000000 easysurrogate-0.24/easysurrogate/analysis/CCM_analysis.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     4490 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/analysis/DAS_analysis.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)    10468 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/analysis/GP_analysis.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     3862 2021-11-30 12:39:19.000000 easysurrogate-0.24/easysurrogate/analysis/KMN_analysis.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     6691 2023-06-19 14:14:19.000000 easysurrogate-0.24/easysurrogate/analysis/QSN_analysis.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)      263 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/analysis/__init__.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     6107 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/analysis/base.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)     9900 2023-06-19 14:14:19.000000 easysurrogate-0.24/easysurrogate/campaign.py
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-20 14:07:44.356232 easysurrogate-0.24/easysurrogate/methods/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     2011 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/CumSum_Layer.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)    11433 2023-06-20 12:02:55.000000 easysurrogate-0.24/easysurrogate/methods/DAS_Layer.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)     7390 2023-06-20 12:32:02.000000 easysurrogate-0.24/easysurrogate/methods/DAS_network.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)    30632 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/Feature_Engineering.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     6718 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/GP.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)    17542 2023-06-19 14:14:19.000000 easysurrogate-0.24/easysurrogate/methods/Layer.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)    31340 2023-06-20 12:34:43.000000 easysurrogate-0.24/easysurrogate/methods/NN.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     2065 2021-11-30 12:39:19.000000 easysurrogate-0.24/easysurrogate/methods/SimpleBin.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)      642 2023-06-19 14:14:19.000000 easysurrogate-0.24/easysurrogate/methods/__init__.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)    13536 2023-06-20 11:41:54.000000 easysurrogate-0.24/easysurrogate/methods/ann_surrogate.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     6648 2023-06-19 14:14:19.000000 easysurrogate-0.24/easysurrogate/methods/batch_normalization.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)    15029 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/ccm_surrogate.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     9614 2023-06-20 12:15:45.000000 easysurrogate-0.24/easysurrogate/methods/das_surrogate.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     4238 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/gaussian_process_regressor.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)    11134 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/gp_surrogate.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)     7287 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/kmn_surrogate.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)     7592 2023-06-19 14:14:19.000000 easysurrogate-0.24/easysurrogate/methods/qsn_surrogate.py
--rwxrwxr-x   0 wouter    (1000) wouter    (1000)    16515 2023-05-23 09:01:38.000000 easysurrogate-0.24/easysurrogate/methods/reduced_surrogate.py
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-20 14:07:44.352232 easysurrogate-0.24/easysurrogate.egg-info/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       90 2023-06-20 14:07:44.000000 easysurrogate-0.24/easysurrogate.egg-info/PKG-INFO
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1245 2023-06-20 14:07:44.000000 easysurrogate-0.24/easysurrogate.egg-info/SOURCES.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)        1 2023-06-20 14:07:44.000000 easysurrogate-0.24/easysurrogate.egg-info/dependency_links.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       60 2023-06-20 14:07:44.000000 easysurrogate-0.24/easysurrogate.egg-info/requires.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       14 2023-06-20 14:07:44.000000 easysurrogate-0.24/easysurrogate.egg-info/top_level.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       38 2023-06-20 14:07:44.356232 easysurrogate-0.24/setup.cfg
--rw-rw-r--   0 wouter    (1000) wouter    (1000)      429 2023-06-20 14:07:10.000000 easysurrogate-0.24/setup.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-21 08:38:00.611050 easysurrogate-0.24.1/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    26526 2021-05-06 20:30:42.000000 easysurrogate-0.24.1/LICENSE
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       92 2023-06-21 08:38:00.611050 easysurrogate-0.24.1/PKG-INFO
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     4731 2023-06-19 14:14:19.000000 easysurrogate-0.24.1/README.md
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-21 08:38:00.607050 easysurrogate-0.24.1/easysurrogate/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       76 2021-11-30 12:39:19.000000 easysurrogate-0.24.1/easysurrogate/__init__.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-21 08:38:00.607050 easysurrogate-0.24.1/easysurrogate/analysis/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     5024 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/analysis/ANN_analysis.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)    10309 2021-11-30 12:39:19.000000 easysurrogate-0.24.1/easysurrogate/analysis/CCM_analysis.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     4490 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/analysis/DAS_analysis.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    10468 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/analysis/GP_analysis.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     3862 2021-11-30 12:39:19.000000 easysurrogate-0.24.1/easysurrogate/analysis/KMN_analysis.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     6691 2023-06-19 14:14:19.000000 easysurrogate-0.24.1/easysurrogate/analysis/QSN_analysis.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      263 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/analysis/__init__.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     6107 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/analysis/base.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)     9900 2023-06-19 14:14:19.000000 easysurrogate-0.24.1/easysurrogate/campaign.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-21 08:38:00.611050 easysurrogate-0.24.1/easysurrogate/methods/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2011 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/methods/CumSum_Layer.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)    11433 2023-06-20 12:02:55.000000 easysurrogate-0.24.1/easysurrogate/methods/DAS_Layer.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)     7390 2023-06-20 12:32:02.000000 easysurrogate-0.24.1/easysurrogate/methods/DAS_network.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    30629 2023-06-21 08:34:43.000000 easysurrogate-0.24.1/easysurrogate/methods/Feature_Engineering.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     6718 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/methods/GP.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    17542 2023-06-19 14:14:19.000000 easysurrogate-0.24.1/easysurrogate/methods/Layer.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    31337 2023-06-21 08:35:29.000000 easysurrogate-0.24.1/easysurrogate/methods/NN.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2065 2021-11-30 12:39:19.000000 easysurrogate-0.24.1/easysurrogate/methods/SimpleBin.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      641 2023-06-20 15:21:12.000000 easysurrogate-0.24.1/easysurrogate/methods/__init__.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)    13536 2023-06-20 11:41:54.000000 easysurrogate-0.24.1/easysurrogate/methods/ann_surrogate.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     6648 2023-06-19 14:14:19.000000 easysurrogate-0.24.1/easysurrogate/methods/batch_normalization.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)    15026 2023-06-21 08:35:02.000000 easysurrogate-0.24.1/easysurrogate/methods/ccm_surrogate.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     9614 2023-06-20 12:15:45.000000 easysurrogate-0.24.1/easysurrogate/methods/das_surrogate.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     4238 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/methods/gaussian_process_regressor.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    11134 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/methods/gp_surrogate.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)     7287 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/methods/kmn_surrogate.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)     7592 2023-06-19 14:14:19.000000 easysurrogate-0.24.1/easysurrogate/methods/qsn_surrogate.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)    16515 2023-05-23 09:01:38.000000 easysurrogate-0.24.1/easysurrogate/methods/reduced_surrogate.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    14714 2023-06-20 21:22:33.000000 easysurrogate-0.24.1/easysurrogate/methods/resampling.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-06-21 08:38:00.607050 easysurrogate-0.24.1/easysurrogate.egg-info/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       92 2023-06-21 08:38:00.000000 easysurrogate-0.24.1/easysurrogate.egg-info/PKG-INFO
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1281 2023-06-21 08:38:00.000000 easysurrogate-0.24.1/easysurrogate.egg-info/SOURCES.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)        1 2023-06-21 08:38:00.000000 easysurrogate-0.24.1/easysurrogate.egg-info/dependency_links.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       60 2023-06-21 08:38:00.000000 easysurrogate-0.24.1/easysurrogate.egg-info/requires.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       14 2023-06-21 08:38:00.000000 easysurrogate-0.24.1/easysurrogate.egg-info/top_level.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       38 2023-06-21 08:38:00.611050 easysurrogate-0.24.1/setup.cfg
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      433 2023-06-21 08:36:49.000000 easysurrogate-0.24.1/setup.py
```

### Comparing `easysurrogate-0.24/LICENSE` & `easysurrogate-0.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/README.md` & `easysurrogate-0.24.1/README.md`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/analysis/ANN_analysis.py` & `easysurrogate-0.24.1/easysurrogate/analysis/ANN_analysis.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/analysis/CCM_analysis.py` & `easysurrogate-0.24.1/easysurrogate/analysis/CCM_analysis.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/analysis/DAS_analysis.py` & `easysurrogate-0.24.1/easysurrogate/analysis/DAS_analysis.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/analysis/GP_analysis.py` & `easysurrogate-0.24.1/easysurrogate/analysis/GP_analysis.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/analysis/KMN_analysis.py` & `easysurrogate-0.24.1/easysurrogate/analysis/KMN_analysis.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/analysis/QSN_analysis.py` & `easysurrogate-0.24.1/easysurrogate/analysis/QSN_analysis.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/analysis/base.py` & `easysurrogate-0.24.1/easysurrogate/analysis/base.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/campaign.py` & `easysurrogate-0.24.1/easysurrogate/campaign.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/CumSum_Layer.py` & `easysurrogate-0.24.1/easysurrogate/methods/CumSum_Layer.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/DAS_Layer.py` & `easysurrogate-0.24.1/easysurrogate/methods/DAS_Layer.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/DAS_network.py` & `easysurrogate-0.24.1/easysurrogate/methods/DAS_network.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/Feature_Engineering.py` & `easysurrogate-0.24.1/easysurrogate/methods/Feature_Engineering.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         # number of points in the computational grid
         self.n_points = feats[0].shape[1]
 
         # Depends on the way the test points are chosen
         # compute the size of the training set based on value of test_frac
         self.n_train = round(self.n_samples * (1.0 - test_frac))
         # number of testing points, as what is left after excluding training set
-        self.n_test = np.int(self.n_samples - self.n_train)
+        self.n_test = int(self.n_samples - self.n_train)
         # get indices of samples  to be used for training
         # 1) train_first True: choose first (1-test_frac) fraction of the data set points, if points arranged in time
         # 2) train_first False: choose (1-test_frac) fraction of data set at
         # random without replacement
         if train_first:
             # chose train fraction from first sims
             self.train_indices = np.arange(self.n_samples)[:self.n_train]
```

### Comparing `easysurrogate-0.24/easysurrogate/methods/GP.py` & `easysurrogate-0.24.1/easysurrogate/methods/GP.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/Layer.py` & `easysurrogate-0.24.1/easysurrogate/methods/Layer.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/NN.py` & `easysurrogate-0.24.1/easysurrogate/methods/NN.py`

 * *Files 0% similar despite different names*

```diff
@@ -685,15 +685,15 @@
                 if self.n_train > self.batch_size:
                     start = np.random.randint(0, self.n_train - self.batch_size, 1)
                 else:
                     start = 0
                 rand_idx = np.arange(start, start + self.batch_size)
 
             # compute learning rate
-            alpha = self.alpha * self.decay_rate**(np.int(i / self.decay_step))
+            alpha = self.alpha * self.decay_rate**(int(i / self.decay_step))
 
             # run the batch
             self.batch(
                 self.X[rand_idx],
                 self.y[rand_idx].T)
 
             # update the weights based on the computed loss gradient
```

### Comparing `easysurrogate-0.24/easysurrogate/methods/SimpleBin.py` & `easysurrogate-0.24.1/easysurrogate/methods/SimpleBin.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/__init__.py` & `easysurrogate-0.24.1/easysurrogate/methods/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#from .resampling import Resampler
+from .resampling import Resampler
 from .NN import ANN
 from .SimpleBin import SimpleBin
 from .Feature_Engineering import Feature_Engineering
 #from .RNN import RNN
 #from .Input_Layer import Input_Layer
 from .ccm_surrogate import CCM_Surrogate
 from .qsn_surrogate import QSN_Surrogate
```

### Comparing `easysurrogate-0.24/easysurrogate/methods/ann_surrogate.py` & `easysurrogate-0.24.1/easysurrogate/methods/ann_surrogate.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/batch_normalization.py` & `easysurrogate-0.24.1/easysurrogate/methods/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/ccm_surrogate.py` & `easysurrogate-0.24.1/easysurrogate/methods/ccm_surrogate.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         # Feature engineering object
         self.feat_eng = es.methods.Feature_Engineering()
 
         # number of training samples
         self.n_samples = feats[0].shape[0]
         # compute the size of the training set based on value of test_frac
-        self.n_train = np.int(self.n_samples * (1.0 - test_frac))
+        self.n_train = int(self.n_samples * (1.0 - test_frac))
         print('Using first', self.n_train, 'of', self.n_samples, 'samples to train QSN')
 
         # list of features
         X = [X_i[0:self.n_train] for X_i in feats]
         # the data
         y = [target[0:self.n_train]]
```

### Comparing `easysurrogate-0.24/easysurrogate/methods/das_surrogate.py` & `easysurrogate-0.24.1/easysurrogate/methods/das_surrogate.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/gaussian_process_regressor.py` & `easysurrogate-0.24.1/easysurrogate/methods/gaussian_process_regressor.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/gp_surrogate.py` & `easysurrogate-0.24.1/easysurrogate/methods/gp_surrogate.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/kmn_surrogate.py` & `easysurrogate-0.24.1/easysurrogate/methods/kmn_surrogate.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/qsn_surrogate.py` & `easysurrogate-0.24.1/easysurrogate/methods/qsn_surrogate.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate/methods/reduced_surrogate.py` & `easysurrogate-0.24.1/easysurrogate/methods/reduced_surrogate.py`

 * *Files identical despite different names*

### Comparing `easysurrogate-0.24/easysurrogate.egg-info/SOURCES.txt` & `easysurrogate-0.24.1/easysurrogate.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 easysurrogate/methods/batch_normalization.py
 easysurrogate/methods/ccm_surrogate.py
 easysurrogate/methods/das_surrogate.py
 easysurrogate/methods/gaussian_process_regressor.py
 easysurrogate/methods/gp_surrogate.py
 easysurrogate/methods/kmn_surrogate.py
 easysurrogate/methods/qsn_surrogate.py
-easysurrogate/methods/reduced_surrogate.py
+easysurrogate/methods/reduced_surrogate.py
+easysurrogate/methods/resampling.py
```

