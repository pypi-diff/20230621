# Comparing `tmp/rl4co-0.0.2.tar.gz` & `tmp/rl4co-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.0.2.tar", last modified: Wed Jun 14 21:17:58 2023, max compression
+gzip compressed data, was "rl4co-0.0.3.dev0.tar", last modified: Wed Jun 21 18:07:12 2023, max compression
```

## Comparing `rl4co-0.0.2.tar` & `rl4co-0.0.3.dev0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:58.991207 rl4co-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 21:17:47.000000 rl4co-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-06-14 21:17:58.991207 rl4co-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-14 21:17:47.000000 rl4co-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-14 21:17:47.000000 rl4co-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:58.987207 rl4co-0.0.2/rl4co/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 21:17:47.000000 rl4co-0.0.2/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:58.987207 rl4co-0.0.2/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-06-14 21:17:58.000000 rl4co-0.0.2/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-14 21:17:58.000000 rl4co-0.0.2/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:17:58.000000 rl4co-0.0.2/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-14 21:17:58.000000 rl4co-0.0.2/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 21:17:58.000000 rl4co-0.0.2/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:17:58.991207 rl4co-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:58.991207 rl4co-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-14 21:17:47.000000 rl4co-0.0.2/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-14 21:17:47.000000 rl4co-0.0.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-14 21:17:47.000000 rl4co-0.0.2/tests/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:12.862406 rl4co-0.0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-21 18:07:03.000000 rl4co-0.0.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-06-21 18:07:12.862406 rl4co-0.0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-21 18:07:03.000000 rl4co-0.0.3.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-21 18:07:03.000000 rl4co-0.0.3.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:12.862406 rl4co-0.0.3.dev0/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 18:07:03.000000 rl4co-0.0.3.dev0/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:12.862406 rl4co-0.0.3.dev0/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-06-21 18:07:12.000000 rl4co-0.0.3.dev0/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-21 18:07:12.000000 rl4co-0.0.3.dev0/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:07:12.000000 rl4co-0.0.3.dev0/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 18:07:12.000000 rl4co-0.0.3.dev0/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:07:12.000000 rl4co-0.0.3.dev0/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:07:12.862406 rl4co-0.0.3.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:12.862406 rl4co-0.0.3.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-21 18:07:03.000000 rl4co-0.0.3.dev0/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-21 18:07:03.000000 rl4co-0.0.3.dev0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 18:07:03.000000 rl4co-0.0.3.dev0/tests/test_ops.py
```

### Comparing `rl4co-0.0.2/LICENSE` & `rl4co-0.0.3.dev0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Federico Berto, Chuanbo Hua, Junyoung Park
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rl4co-0.0.2/PKG-INFO` & `rl4co-0.0.3.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.2
+Version: 0.0.3.dev0
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,40 +187,42 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright 2023 Federico Berto, Chuanbo Hua, Junyoung Park
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/kaist-silab/rl4co
+Project-URL: Bug Tracker, https://github.com/kaist-silab/rl4co/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: graph
 Provides-Extra: testing
+Provides-Extra: linting
 License-File: LICENSE
 
 <div align="center">
 
 # RL4CO
     
 An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering. 
@@ -270,16 +272,14 @@
 
 > Note: `conda` is also a good candidate for hassle-free installation of PyTorch: check out the [PyTorch website](https://pytorch.org/get-started/locally/) for more details.
 
 </details>
 
 
 
-
-
 To get started, we recommend checking out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 
 ## Usage
 
 
 Train model with default configuration (AM on TSP environment):
 ```bash
@@ -362,9 +362,15 @@
 ### Testing
 
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
-We will enable automated tests when we make the repo public.
 
+## Contributing
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO! 
+
+### Contributors
+<a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
+</a>
```

### Comparing `rl4co-0.0.2/README.md` & `rl4co-0.0.3.dev0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -49,16 +49,14 @@
 
 > Note: `conda` is also a good candidate for hassle-free installation of PyTorch: check out the [PyTorch website](https://pytorch.org/get-started/locally/) for more details.
 
 </details>
 
 
 
-
-
 To get started, we recommend checking out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 
 ## Usage
 
 
 Train model with default configuration (AM on TSP environment):
 ```bash
@@ -141,9 +139,15 @@
 ### Testing
 
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
-We will enable automated tests when we make the repo public.
 
+## Contributing
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO! 
+
+### Contributors
+<a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
+</a>
```

#### html2text {}

```diff
@@ -46,8 +46,12 @@
 trainer = L.Trainer( max_epochs=3, # only few epochs accelerator="gpu", # use
 GPU if available, else you can use others as "cpu" logger=None, # can replace
 with WandbLogger, TensorBoardLogger, etc. precision="16-mixed", # Lightning
 will handle faster training with mixed precision gradient_clip_val=1.0, # clip
 gradients to avoid exploding gradients reload_dataloaders_every_n_epochs=1, #
 necessary for sampling new data ) # Fit the model trainer.fit(lit_module) ```
 ### Testing Run tests with `pytest` from the root directory: ```bash pytest
-tests ``` We will enable automated tests when we make the repo public.
+tests ``` ## Contributing Have a suggestion, request, or found a bug? Feel free
+to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a
+pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome
+contributions to RL4CO! ### Contributors [https://contrib.rocks/
+image?repo=kaist-silab/rl4co]
```

### Comparing `rl4co-0.0.2/rl4co.egg-info/PKG-INFO` & `rl4co-0.0.3.dev0/rl4co.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.2
+Version: 0.0.3.dev0
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,40 +187,42 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright 2023 Federico Berto, Chuanbo Hua, Junyoung Park
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/kaist-silab/rl4co
+Project-URL: Bug Tracker, https://github.com/kaist-silab/rl4co/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: graph
 Provides-Extra: testing
+Provides-Extra: linting
 License-File: LICENSE
 
 <div align="center">
 
 # RL4CO
     
 An extensive Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our goal is to provide a unified framework for RL-based CO algorithms, and to facilitate reproducible research in this field, decoupling the science from the engineering. 
@@ -270,16 +272,14 @@
 
 > Note: `conda` is also a good candidate for hassle-free installation of PyTorch: check out the [PyTorch website](https://pytorch.org/get-started/locally/) for more details.
 
 </details>
 
 
 
-
-
 To get started, we recommend checking out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 
 ## Usage
 
 
 Train model with default configuration (AM on TSP environment):
 ```bash
@@ -362,9 +362,15 @@
 ### Testing
 
 Run tests with `pytest` from the root directory:
 
 ```bash
 pytest tests
 ```
-We will enable automated tests when we make the repo public.
 
+## Contributing
+Have a suggestion, request, or found a bug? Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/rl4co/pulls). We welcome contributions to RL4CO! 
+
+### Contributors
+<a href="https://github.com/kaist-silab/rl4co/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=kaist-silab/rl4co" />
+</a>
```

### Comparing `rl4co-0.0.2/tests/test_envs.py` & `rl4co-0.0.3.dev0/tests/test_envs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import torch
+
 from rl4co.envs import ATSPEnv, CVRPEnv, DPPEnv, MTSPEnv, PDPEnv, SDVRPEnv, TSPEnv
 
 
 def policy(td):
     """Helper function to select a random action from available actions"""
     action = torch.multinomial(td["action_mask"].float(), 1).squeeze(-1)
     td.set("action", action)
```

### Comparing `rl4co-0.0.2/tests/test_models.py` & `rl4co-0.0.3.dev0/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 
 sys.path.append(".")
 import pytest
+
 from rl4co.models import (
     POMO,
     AttentionModel,
     HeterogeneousAttentionModel,
+    MDAMPolicy,
     PointerNetwork,
     SymNCO,
     SymNCOPolicy,
-    MDAMPolicy,
 )
 from rl4co.utils.test_utils import generate_env_data
 
 
 @pytest.mark.parametrize("size", [20])
 @pytest.mark.parametrize(
     "env_name", ["tsp", "cvrp", "mtsp", "op", "dpp", "pctsp"]
```

### Comparing `rl4co-0.0.2/tests/test_ops.py` & `rl4co-0.0.3.dev0/tests/test_ops.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 import torch
-from rl4co.utils.ops import batchify, unbatchify
+
 from tensordict import TensorDict
 
+from rl4co.utils.ops import batchify, unbatchify
+
 
 @pytest.mark.parametrize(
     "a",
     [
         torch.randn(10, 20, 2),
         TensorDict(
             {"a": torch.randn(10, 20, 2), "b": torch.randn(10, 20, 2)}, batch_size=10
```

