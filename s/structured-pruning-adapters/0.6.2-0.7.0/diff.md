# Comparing `tmp/structured-pruning-adapters-0.6.2.tar.gz` & `tmp/structured-pruning-adapters-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structured-pruning-adapters-0.6.2.tar", last modified: Fri Jun 16 08:57:21 2023, max compression
+gzip compressed data, was "structured-pruning-adapters-0.7.0.tar", last modified: Wed Jun 21 13:28:17 2023, max compression
```

## Comparing `structured-pruning-adapters-0.6.2.tar` & `structured-pruning-adapters-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.414612 structured-pruning-adapters-0.6.2/sp_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/splopa.py
--rw-r--r--   0 runner    (1001) docker     (123)    30918 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/splora.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/torch_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.414612 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_lin_as_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_splopa.py
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_splora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_torchpruning.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_utils.py
+drwxr-xr-x   0 au478108 (794351465) UNI\Domain Users (357318537)        0 2023-06-21 13:28:17.193543 structured-pruning-adapters-0.7.0/
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)    11357 2022-06-15 08:39:30.000000 structured-pruning-adapters-0.7.0/LICENSE
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     7752 2023-06-21 13:28:17.193279 structured-pruning-adapters-0.7.0/PKG-INFO
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     6515 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/README.md
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)       38 2023-06-21 13:28:17.193644 structured-pruning-adapters-0.7.0/setup.cfg
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     2565 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/setup.py
+drwxr-xr-x   0 au478108 (794351465) UNI\Domain Users (357318537)        0 2023-06-21 13:28:17.191247 structured-pruning-adapters-0.7.0/sp_adapters/
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      599 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/__init__.py
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      116 2022-06-15 13:38:30.000000 structured-pruning-adapters-0.7.0/sp_adapters/base.py
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     1445 2022-11-17 10:31:11.000000 structured-pruning-adapters-0.7.0/sp_adapters/lora.py
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     7089 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/splopa.py
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)    31521 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/splora.py
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     9919 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/sppara.py
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)    13244 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/torch_pruning.py
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     2076 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/utils.py
+drwxr-xr-x   0 au478108 (794351465) UNI\Domain Users (357318537)        0 2023-06-21 13:28:17.192829 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     7752 2023-06-21 13:28:16.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      460 2023-06-21 13:28:17.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)        1 2023-06-21 13:28:16.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      119 2023-06-21 13:28:16.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/requires.txt
+-rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)       12 2023-06-21 13:28:17.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/top_level.txt
```

### Comparing `structured-pruning-adapters-0.6.2/LICENSE` & `structured-pruning-adapters-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.2/PKG-INFO` & `structured-pruning-adapters-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.6.2
+Version: 0.7.0
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
@@ -131,14 +131,22 @@
 <div align="center">
 <img src="figures/SPLoRA.png" width="400">
 </div>
 Adds a low-rank bottle-neck projection in projection in parallel with the main weights projection.
 
 <br/>
 
+### Structured Pruning Parllel Residual Adapter (SPPaRA) for _Channel Pruning_ of CNNs
+```python3
+from sp_adapters import SPPaRA
+```
+Adds a pointwise convolution as adapter to convolutional layers. First proposed in ["Efficient parametrization of multi-domain deep neural networks" by Rebuffi et al.](https://arxiv.org/pdf/1803.10082.pdf),
+
+<br/>
+
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_ (experimental)
 ```python3
 from sp_adapters import SPLoPA
 ```
 
 <div align="center">
 <img src="figures/SPLoPA.png" width="600">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.7.0 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -63,14 +63,19 @@
 dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
 dtype=torch.bool), ) ``` ### Demo See also [notebooks/demo.ipynb](notebooks/
 demo.ipynb) for a hands-on demo. ### Structured Pruning Low-Rank Adapter
 (SPLoRA) for _Channel Pruning_ ```python3 from sp_adapters import SPLoRA ```
                              [figures/SPLoRA.png]
 Adds a low-rank bottle-neck projection in projection in parallel with the main
 weights projection.
+### Structured Pruning Parllel Residual Adapter (SPPaRA) for _Channel Pruning_
+of CNNs ```python3 from sp_adapters import SPPaRA ``` Adds a pointwise
+convolution as adapter to convolutional layers. First proposed in ["Efficient
+parametrization of multi-domain deep neural networks" by Rebuffi et al.](https:
+//arxiv.org/pdf/1803.10082.pdf),
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
 (experimental) ```python3 from sp_adapters import SPLoPA ```
                              [figures/SPLoPA.png]
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [
 [paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank
 prototypes for block-sparse adaptation. ## Citation If you enjoy this work,
 please consider citing it ```bibtex @article{hedegaard2022structured, title=
```

### Comparing `structured-pruning-adapters-0.6.2/README.md` & `structured-pruning-adapters-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,22 @@
 <div align="center">
 <img src="figures/SPLoRA.png" width="400">
 </div>
 Adds a low-rank bottle-neck projection in projection in parallel with the main weights projection.
 
 <br/>
 
+### Structured Pruning Parllel Residual Adapter (SPPaRA) for _Channel Pruning_ of CNNs
+```python3
+from sp_adapters import SPPaRA
+```
+Adds a pointwise convolution as adapter to convolutional layers. First proposed in ["Efficient parametrization of multi-domain deep neural networks" by Rebuffi et al.](https://arxiv.org/pdf/1803.10082.pdf),
+
+<br/>
+
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_ (experimental)
 ```python3
 from sp_adapters import SPLoPA
 ```
 
 <div align="center">
 <img src="figures/SPLoPA.png" width="600">
```

#### html2text {}

```diff
@@ -46,14 +46,19 @@
 dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
 dtype=torch.bool), ) ``` ### Demo See also [notebooks/demo.ipynb](notebooks/
 demo.ipynb) for a hands-on demo. ### Structured Pruning Low-Rank Adapter
 (SPLoRA) for _Channel Pruning_ ```python3 from sp_adapters import SPLoRA ```
                              [figures/SPLoRA.png]
 Adds a low-rank bottle-neck projection in projection in parallel with the main
 weights projection.
+### Structured Pruning Parllel Residual Adapter (SPPaRA) for _Channel Pruning_
+of CNNs ```python3 from sp_adapters import SPPaRA ``` Adds a pointwise
+convolution as adapter to convolutional layers. First proposed in ["Efficient
+parametrization of multi-domain deep neural networks" by Rebuffi et al.](https:
+//arxiv.org/pdf/1803.10082.pdf),
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
 (experimental) ```python3 from sp_adapters import SPLoPA ```
                              [figures/SPLoPA.png]
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [
 [paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank
 prototypes for block-sparse adaptation. ## Citation If you enjoy this work,
 please consider citing it ```bibtex @article{hedegaard2022structured, title=
```

### Comparing `structured-pruning-adapters-0.6.2/setup.py` & `structured-pruning-adapters-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.2/sp_adapters/lora.py` & `structured-pruning-adapters-0.7.0/sp_adapters/lora.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.2/sp_adapters/splopa.py` & `structured-pruning-adapters-0.7.0/sp_adapters/splopa.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.2/sp_adapters/splora.py` & `structured-pruning-adapters-0.7.0/sp_adapters/splora.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,29 @@
 
         self.adapter = LowRankMatrix(
             1, in_features, out_features, rank, init_range=init_range
         )
         self.reset_parameters()
 
     def forward(self, input):
+        if self.training:
+            # Low memory impl - gradient size significantly smaller
+            if self.weight.requires_grad:
+                self.weight.requires_grad = False
+                logger.warning("Forcing `weight.requires_grad = False`")
+            return nn.functional.linear(
+                input, self.weight, self.bias
+            ) + nn.functional.linear(
+                nn.functional.linear(
+                    input,
+                    self.adapter.rows.squeeze(0),
+                ),
+                self.adapter.cols.squeeze(0),
+            )
+        # Low FLOPs impl
         return nn.functional.linear(input, self.adapted_weight, self.bias)
 
     @property
     def adapted_weight(self) -> nn.Parameter:
         if self.weight.requires_grad:
             self.weight.requires_grad = False
             logger.warning("Forcing `weight.requires_grad = False`")
```

### Comparing `structured-pruning-adapters-0.6.2/sp_adapters/torch_pruning.py` & `structured-pruning-adapters-0.7.0/sp_adapters/torch_pruning.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.2/sp_adapters/utils.py` & `structured-pruning-adapters-0.7.0/sp_adapters/utils.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/PKG-INFO` & `structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.6.2
+Version: 0.7.0
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
@@ -131,14 +131,22 @@
 <div align="center">
 <img src="figures/SPLoRA.png" width="400">
 </div>
 Adds a low-rank bottle-neck projection in projection in parallel with the main weights projection.
 
 <br/>
 
+### Structured Pruning Parllel Residual Adapter (SPPaRA) for _Channel Pruning_ of CNNs
+```python3
+from sp_adapters import SPPaRA
+```
+Adds a pointwise convolution as adapter to convolutional layers. First proposed in ["Efficient parametrization of multi-domain deep neural networks" by Rebuffi et al.](https://arxiv.org/pdf/1803.10082.pdf),
+
+<br/>
+
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_ (experimental)
 ```python3
 from sp_adapters import SPLoPA
 ```
 
 <div align="center">
 <img src="figures/SPLoPA.png" width="600">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.7.0 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -63,14 +63,19 @@
 dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
 dtype=torch.bool), ) ``` ### Demo See also [notebooks/demo.ipynb](notebooks/
 demo.ipynb) for a hands-on demo. ### Structured Pruning Low-Rank Adapter
 (SPLoRA) for _Channel Pruning_ ```python3 from sp_adapters import SPLoRA ```
                              [figures/SPLoRA.png]
 Adds a low-rank bottle-neck projection in projection in parallel with the main
 weights projection.
+### Structured Pruning Parllel Residual Adapter (SPPaRA) for _Channel Pruning_
+of CNNs ```python3 from sp_adapters import SPPaRA ``` Adds a pointwise
+convolution as adapter to convolutional layers. First proposed in ["Efficient
+parametrization of multi-domain deep neural networks" by Rebuffi et al.](https:
+//arxiv.org/pdf/1803.10082.pdf),
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
 (experimental) ```python3 from sp_adapters import SPLoPA ```
                              [figures/SPLoPA.png]
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [
 [paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank
 prototypes for block-sparse adaptation. ## Citation If you enjoy this work,
 please consider citing it ```bibtex @article{hedegaard2022structured, title=
```

