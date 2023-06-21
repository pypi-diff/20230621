# Comparing `tmp/zeus-ml-0.3.0.tar.gz` & `tmp/zeus-ml-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus-ml-0.3.0.tar", last modified: Mon Dec  5 20:55:48 2022, max compression
+gzip compressed data, was "zeus-ml-0.4.0.tar", last modified: Wed Jun 21 01:27:37 2023, max compression
```

## Comparing `zeus-ml-0.3.0.tar` & `zeus-ml-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 20:55:48.905149 zeus-ml-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      842 2022-12-05 20:55:48.905149 zeus-ml-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 20:55:48.905149 zeus-ml-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 20:55:48.889148 zeus-ml-0.3.0/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 20:55:48.893148 zeus-ml-0.3.0/zeus/policy/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/policy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/policy/mab.py
--rw-r--r--   0 runner    (1001) docker     (123)    23443 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/policy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 20:55:48.893148 zeus-ml-0.3.0/zeus/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/profile/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 20:55:48.897148 zeus-ml-0.3.0/zeus/run/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50454 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/run/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/run/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    36484 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 20:55:48.901149 zeus-ml-0.3.0/zeus/util/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/util/lr_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2022-12-05 20:55:09.000000 zeus-ml-0.3.0/zeus/util/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 20:55:48.905149 zeus-ml-0.3.0/zeus_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2022-12-05 20:55:48.000000 zeus-ml-0.3.0/zeus_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-05 20:55:48.000000 zeus-ml-0.3.0/zeus_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 20:55:48.000000 zeus-ml-0.3.0/zeus_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-05 20:55:48.000000 zeus-ml-0.3.0/zeus_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-05 20:55:48.000000 zeus-ml-0.3.0/zeus_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/run/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/run/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/lr_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/top_level.txt
```

### Comparing `zeus-ml-0.3.0/LICENSE` & `zeus-ml-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.3.0/PKG-INFO` & `zeus-ml-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.3.0
+Version: 0.4.0
 Summary: An Energy Optimization Framework for DNN Training
 Home-page: https://github.com/SymbioticLab/Zeus
 Author: Jae-Won Chung
 Author-email: jwnchung@umich.edu
 License: Apache-2.0
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,mlsys
@@ -13,13 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zeus: An Energy Optimization Framework for DNN Training
```

### Comparing `zeus-ml-0.3.0/README.md` & `zeus-ml-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,46 +3,47 @@
   <source media="(prefers-color-scheme: dark)" srcset="docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="docs/assets/img/logo_light.svg">
   <img alt="Zeus logo" width="55%" src="docs/assets/img/logo_dark.svg">
 </picture>
 <h1>An Energy Optimization Framework for DNN Training</h1>
 </div>
 
-[![arXiv](https://custom-icon-badges.herokuapp.com/badge/ID-2208.06102-b31b1b.svg?logo=arxiv-white&logoWidth=35)](https://arxiv.org/abs/2208.06102)
-[![Docker Hub](https://img.shields.io/badge/Docker-SymbioticLab%2FZeus-blue.svg?logo=docker&logoColor=white)](https://hub.docker.com/r/symbioticlab/zeus)
+[![NSDI23 paper](https://custom-icon-badges.herokuapp.com/badge/NSDI'23-paper-b31b1b.svg)](https://www.usenix.org/conference/nsdi23/presentation/you)
+[![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
+[![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/611f69?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Homepage build](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml/badge.svg)](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/SymbioticLab/Zeus?logo=law)](/LICENSE)
 
 Zeus automatically optimizes the **energy and time** of training a DNN to a target validation metric by finding the optimal **batch size** and **GPU power limit**.
 
-Please refer to our [NSDI’23 publication](https://arxiv.org/abs/2208.06102) for details.
+Please refer to our NSDI’23 [paper](https://www.usenix.org/conference/nsdi23/presentation/you) and [slides](https://www.usenix.org/system/files/nsdi23_slides_chung.pdf) for details.
 Checkout [Overview](https://ml.energy/zeus/overview/) for a summary.
 
 Zeus is part of [The ML.ENERGY Initiative](https://ml.energy).
 
 ## Repository Organization
 
 ```
 .
 ├── zeus/                # ⚡ Zeus Python package
 │   ├── run/             #    - Tools for running Zeus on real training jobs
 │   ├── policy/          #    - Optimization policies and extension interfaces
-│   ├── profile/         #    - Tools for profiling energy and time
-│   ├── simulate.py      #    - Tools for trace-driven simulation
 │   ├── util/            #    - Utility functions and classes
+│   ├── simulate.py      #    - Tools for trace-driven simulation
+│   ├── monitor.py       #    - `ZeusMonitor`: Measure GPU time and energy of any code block
 │   ├── analyze.py       #    - Analysis functions for power logs
-│   ├── monitor.py       #    - Class for profiling energy inside training scripts
 │   └── job.py           #    - Class for job specification
 │
 ├── zeus_monitor/        # 🔌 GPU power monitor
 │   ├── zemo/            #    -  A header-only library for querying NVML
 │   └── main.cpp         #    -  Source code of the power monitor
 │
 ├── examples/            # 🛠️ Examples of integrating Zeus
 │   ├── capriccio/       #    - Integrating with Huggingface and Capriccio
+│   ├── imagenet/        #    - Integrating with torchvision and ImageNet
 │   ├── cifar100/        #    - Integrating with torchvision and CIFAR100
 │   └── trace_driven/    #    - Using the Zeus trace-driven simulator
 │
 ├── capriccio/           # 🌊 A drifting sentiment analysis dataset
 │
 └── trace/               # 🗃️ Train and power traces for various GPUs and DNNs
 ```
@@ -80,14 +81,19 @@
 
 ## Extending Zeus
 
 You can easily implement custom policies for batch size and power limit optimization and plug it into Zeus.
 
 Refer to [Extending Zeus](https://ml.energy/zeus/extend/) for details.
 
+## Carbon-Aware Zeus
+
+The use of GPUs for training DNNs results in high carbon emissions and energy consumption. Building on top of Zeus, we introduce *Chase* -- a carbon-aware solution. *Chase* dynamically controls the energy consumption of GPUs; adapts to shifts in carbon intensity during DNN training, reducing carbon footprint with minimal compromises on training performance. To proactively adapt to shifting carbon intensity, a lightweight machine learning algorithm is used to forecast the carbon intensity of the upcoming time frame. For more details on Chase, please refer to our [paper](https://www.usenix.org/conference/nsdi23/presentation/you) and the [chase branch](https://github.com/SymbioticLab/Zeus/tree/chase). 
+
+
 ## Citation
 
 Please consider citing our NSDI’23 paper if you find Zeus to be related to your research project.
 
 ```bibtex
 @inproceedings{zeus-nsdi23,
     title     = {Zeus: Understanding and Optimizing {GPU} Energy Consumption of {DNN} Training},
```

### Comparing `zeus-ml-0.3.0/setup.py` & `zeus-ml-0.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages
 
+extras_require={
+    "lint": ["ruff", "black==22.6.0"],
+    "test": ["pytest==7.3.2", "pytest-mock==3.10.0", "pytest-xdist==3.3.1"],
+}
+extras_require["dev"] = extras_require["lint"] + extras_require["test"]
+
 setup(
     name="zeus-ml",
-    version="0.3.0",
+    version="0.4.0",
     description="An Energy Optimization Framework for DNN Training",
     long_description="# Zeus: An Energy Optimization Framework for DNN Training\n",
     long_description_content_type="text/markdown",
     url="https://github.com/SymbioticLab/Zeus",
     author="Jae-Won Chung",
     author_email="jwnchung@umich.edu",
     license="Apache-2.0",
@@ -34,18 +40,15 @@
     ],
     keywords=["deep-learning", "power", "energy", "mlsys"],
     project_urls={
         "Documentation": "https://ml.energy/zeus",
     },
     packages=find_packages("."),
     install_requires=[
-        "torch",
         "numpy",
         "pandas==1.4.2",
         "scikit-learn",
         "pynvml",
     ],
     python_requires=">=3.8",
-    extras_require={
-        "dev": ["pylint==2.14.5", "black==22.6.0", "pydocstyle==6.1.1"],
-    }
+    extras_require=extras_require,
 )
```

### Comparing `zeus-ml-0.3.0/zeus/__init__.py` & `zeus-ml-0.4.0/zeus/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Zeus is an energy optimization framework for DNN training.
+"""Zeus is an energy optimization framework for DNN training.
 
 Modules:
 
 - [`analyze`][zeus.analyze]: Functions for analyzing log files.
-- [`profile`][zeus.profile]: Tools for profiling energy and time.
+- [`profile`][zeus.profile]: Tools for profiling energy and time. Will be deprecated.
+- [`profiling`][zeus.profiling]: Tools for profiling energy for an arbitrary profilng window inside training scripts
 - [`job`][zeus.job]: Job specification.
 - [`run`][zeus.run]: Machinery for actually running Zeus.
 - [`simulate`][zeus.simulate]: Machinery for trace-driven Zeus.
 - [`policy`][zeus.policy]: Collection of optimization policies.
 - [`monitor`][zeus.monitor]: Class for profiling energy inside training scripts.
 - [`util`][zeus.util]: Utility functions and classes.
 """
```

### Comparing `zeus-ml-0.3.0/zeus/analyze.py` & `zeus-ml-0.4.0/zeus/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     bs: int
     pl: int
     energy: float
     reached: bool
     time: float
 
 
+# ruff: noqa: PLR2004
 def energy(
     logfile: Path | str,
     start: float | None = None,
     end: float | None = None,
 ) -> float:
     """Compute the energy consumption from the Zeus monitor power log file.
```

### Comparing `zeus-ml-0.3.0/zeus/job.py` & `zeus-ml-0.4.0/zeus/job.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.3.0/zeus/policy/__init__.py` & `zeus-ml-0.4.0/zeus/policy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Optimization policies for Zeus.
+"""Optimization policies for Zeus.
 
 [`PowerLimitOptimizer`][zeus.policy.interface.PowerLimitOptimizer] and
 [`BatchSizeOptimizer`][zeus.policy.interface.BatchSizeOptimizer] are
 abstract classes. Users can implement custom policies by extending the
 abstract classes and implementing required method.
 Currently, [`Simulator`][zeus.simulate.Simulator] supports custom policies
 for both classes, while [`ZeusMaster`][zeus.run.ZeusMaster] only supports
```

### Comparing `zeus-ml-0.3.0/zeus/policy/interface.py` & `zeus-ml-0.4.0/zeus/policy/interface.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.3.0/zeus/policy/mab.py` & `zeus-ml-0.4.0/zeus/policy/mab.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         reset: bool,
     ) -> None:
         """Fit the bandit on the given list of observations.
 
         Args:
             decisions: A list of arms chosen.
             rewards: A list of rewards that resulted from choosing the arms in `decisions`.
+            reset: Whether to reset all arms.
         """
         decisions_arr = np.array(decisions)
         rewards_arr = np.array(rewards)
 
         # Fit all arms.
         for arm in self.arms:
             self.fit_arm(arm, rewards_arr[decisions_arr == arm], reset)
@@ -165,10 +166,13 @@
             A mapping from every arm to their sampled expected reward.
         """
         expectations = {}
         for arm in self.arms:
             mean = self.arm_param_mean[arm]
             prec = self.arm_param_prec[arm]
             if prec == self.prior_prec:
-                warnings.warn(f"predict_expectations called when arm '{arm}' is cold.")
+                warnings.warn(
+                    f"predict_expectations called when arm '{arm}' is cold.",
+                    stacklevel=1,
+                )
             expectations[arm] = self.rng.normal(mean, np.sqrt(np.reciprocal(prec)))
         return expectations
```

### Comparing `zeus-ml-0.3.0/zeus/policy/optimizer.py` & `zeus-ml-0.4.0/zeus/policy/optimizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,38 +8,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Implementations for various optimization policies.
+"""Implementations of various optimization policies.
 
 [`JITPowerLimitOptimizer`][zeus.policy.optimizer.JITPowerLimitOptimizer] and
 [`PruningGTSBatchSizeOptimizer`][zeus.policy.optimizer.PruningGTSBatchSizeOptimizer]
 are the implementations used in Zeus's publication.
 """
 
 from __future__ import annotations
 
-import unittest
 from collections import defaultdict
 from typing import Generator
 
 import numpy as np
 
 from zeus.job import Job
 from zeus.policy.interface import BatchSizeOptimizer, PowerLimitOptimizer
 from zeus.policy.mab import GaussianTS
 
 
 class GTSBatchSizeOptimizer(BatchSizeOptimizer):
     """One Gaussian Thompson Sampling MAB for each job."""
 
+    # ruff: noqa: D417
     def __init__(
         self,
         learn_reward_precision: bool,
         reward_precision: float = 0.0,
         prior_mean: float = 0.0,
         prior_precision: float = 0.0,
         num_exploration: int = 1,
@@ -134,18 +133,17 @@
             arm_rewards = np.array(self.history[job][batch_size])
             variance = np.var(arm_rewards)
             # When there is only one observation for the arm, the variance is zero.
             # NOTE: We might still want to have a pre-determined reward precision here
             #       because sampling from an infinite precision Gaussian distribution
             #       always returns the mean (the observation), and it will hamper
             #       exploration in the early stage.
-            if variance == 0.0:
-                precision = np.inf
-            else:
-                precision = np.reciprocal(variance)
+            precision = (
+                np.inf if variance == 0.0 else np.reciprocal(variance)
+            )  # ruff: noqa: PLR2004
             mab = self.mabs[job]
             mab.arm_reward_prec[batch_size] = precision
             mab.fit_arm(batch_size, arm_rewards, reset=True)
             self.mabs[job] = mab
             if self.verbose:
                 arm_rewards_repr = ", ".join([f"{r:.2f}" for r in arm_rewards])
                 self._log(
@@ -264,116 +262,14 @@
             cost: The energy-time cost of running the job with this batch size.
             reached: Whether the job reached the target metric.
         """
         none = self.gen.send((batch_size, cost, reached))
         assert none is None, "Call order may have been wrong."
 
 
-class TestPruningExploreManager(unittest.TestCase):
-    """Unit test class for pruning exploration."""
-
-    batch_sizes: list[int] = [8, 16, 32, 64, 128, 256]
-
-    def run_exploration(
-        self,
-        manager: PruningExploreManager,
-        exploration: list[tuple[int, float, bool]],
-        result: list[int],
-    ) -> None:
-        """Drive the pruning explore manager and check results."""
-        for bs, cost, reached in exploration:
-            self.assertEqual(manager.next_batch_size(), bs)
-            manager.report_batch_size_result(bs, cost, reached)
-        with self.assertRaises(StopIteration) as raised:
-            manager.next_batch_size()
-        self.assertEqual(raised.exception.value, result)
-
-    def test_normal(self):
-        """Test a typical case."""
-        manager = PruningExploreManager(self.batch_sizes, 128)
-        exploration = [
-            (128, 10.0, True),
-            (64, 9.0, True),
-            (32, 8.0, True),
-            (16, 12.0, True),
-            (8, 21.0, False),
-            (256, 15.0, True),
-            (32, 8.0, True),
-            (16, 12.0, False),
-            (64, 9.0, True),
-            (128, 10.0, True),
-            (256, 17.0, False),
-        ]
-        result = [32, 64, 128]
-        self.run_exploration(manager, exploration, result)
-
-    def test_default_is_largest(self):
-        """Test the case when the default batch size is the largest one."""
-        manager = PruningExploreManager(self.batch_sizes, 256)
-        exploration = [
-            (256, 7.0, True),
-            (128, 8.0, True),
-            (64, 9.0, True),
-            (32, 13.0, True),
-            (16, 22.0, False),
-            (256, 8.0, True),
-            (128, 8.5, True),
-            (64, 9.0, True),
-            (32, 12.0, True),
-        ]
-        result = [32, 64, 128, 256]
-        self.run_exploration(manager, exploration, result)
-
-    def test_default_is_smallest(self):
-        """Test the case when the default batch size is the smallest one."""
-        manager = PruningExploreManager(self.batch_sizes, 8)
-        exploration = [
-            (8, 10.0, True),
-            (16, 17.0, True),
-            (32, 20.0, True),
-            (64, 25.0, False),
-            (8, 10.0, True),
-            (16, 21.0, False),
-        ]
-        result = [8]
-        self.run_exploration(manager, exploration, result)
-
-    def test_all_converge(self):
-        """Test the case when every batch size converges."""
-        manager = PruningExploreManager(self.batch_sizes, 64)
-        exploration = [
-            (64, 10.0, True),
-            (32, 8.0, True),
-            (16, 12.0, True),
-            (8, 15.0, True),
-            (128, 12.0, True),
-            (256, 13.0, True),
-            (32, 7.0, True),
-            (16, 10.0, True),
-            (8, 15.0, True),
-            (64, 10.0, True),
-            (128, 12.0, True),
-            (256, 13.0, True),
-        ]
-        result = self.batch_sizes
-        self.run_exploration(manager, exploration, result)
-
-    def test_every_bs_is_bs(self):
-        """Test the case when every batch size other than the default fail to converge."""
-        manager = PruningExploreManager(self.batch_sizes, 64)
-        exploration = [
-            (64, 10.0, True),
-            (32, 22.0, False),
-            (128, 25.0, False),
-            (64, 9.0, True),
-        ]
-        result = [64]
-        self.run_exploration(manager, exploration, result)
-
-
 class PruningGTSBatchSizeOptimizer(BatchSizeOptimizer):
     """One Gaussian Thompson Sampling MAB for each job with double pruning exploration."""
 
     def __init__(
         self,
         prior_mean: float = 0.0,
         prior_precision: float = 0.0,
@@ -587,11 +483,7 @@
     def observe(self, job: Job, batch_size: int, power_limit: int, cost: float) -> None:
         """Learn from the cost of using the given knobs for the job."""
         self.observe_count[job][batch_size] += 1
         prev_best_cost = self.best_cost[job].get(batch_size)
         if prev_best_cost is None or prev_best_cost > cost:
             self.best_pl[job][batch_size] = power_limit
             self.best_cost[job][batch_size] = cost
-
-
-if __name__ == "__main__":
-    unittest.main()
```

### Comparing `zeus-ml-0.3.0/zeus/profile/__init__.py` & `zeus-ml-0.4.0/zeus/util/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Tools for profiling.
+"""Utility functions and classes."""
 
-Currently only PyTorch is integrated with Zeus.
-"""
+from zeus.util.check import get_env
+from zeus.util.logging import FileAndConsole
+from zeus.util.lr_scaler import LinearScaler, SquareRootScaler
+from zeus.util.metric import zeus_cost, ZeusCostThresholdExceededError
```

### Comparing `zeus-ml-0.3.0/zeus/run/__init__.py` & `zeus-ml-0.4.0/zeus/run/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.3.0/zeus/run/dataloader.py` & `zeus-ml-0.4.0/zeus/run/dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,46 +15,37 @@
 """Defines the ZeusDataLoader class."""
 
 from __future__ import annotations
 
 import atexit
 import json
 import os
-import signal
-import subprocess
-import time
 import logging
 from functools import cached_property
 from pathlib import Path
-from typing import Generator, Literal
+from typing import Generator, Literal, ClassVar
 import numpy as np
 
 import pynvml
 import torch
 import torch.distributed as dist
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 
-from zeus import analyze
+from zeus.monitor import ZeusMonitor, Measurement
 from zeus.util.check import get_env
-from zeus.util.metric import ZeusCostThresholdExceededException, zeus_cost
+from zeus.util.metric import ZeusCostThresholdExceededError, zeus_cost
+from zeus.util.logging import get_logger
+
 
 # JIT profiling states
 NOT_PROFILING = "NOT_PROFILING"
 WARMING_UP = "WARMING_UP"
 PROFILING = "PROFILING"
 
-# Config logging
-LOG = logging.Logger(__name__)
-LOG.setLevel(logging.INFO)
-LOG_HANDLER = logging.StreamHandler()
-LOG_FORMATTER = logging.Formatter("%(asctime)s %(message)s")
-LOG_HANDLER.setFormatter(LOG_FORMATTER)
-LOG.addHandler(LOG_HANDLER)
-
 
 class ZeusDataLoader(DataLoader):
     r"""Profiles and optimizes GPU power limit.
 
     `ZeusDataLoader` is integrated into the DNN training script, and transparently
     profiles power and time consumption to determine the optimal GPU power limit.
 
@@ -162,75 +153,78 @@
       - `ZEUS_JOB_ID`        : String to prefix in logs. (Default:` "zeus"`)
       - `ZEUS_COST_THRESH`   : Stop training when the energy-time cost will exceed
                                this threshold.  (Default:` "inf"`)
       - `ZEUS_ETA_KNOB`      : $\eta$ knob to tradeoff between energy and time.
                                Larger values reduce more energy and sacrifice time.
                                (Default:` "0.5"`)
       - `ZEUS_MONITOR_PATH`  : Path to the Zeus power monitor binary.
-                               (Default:` "/workspace/zeus/zeus_monitor/zeus_monitor"`)
+                               (Default:` "zeus_monitor"`)
       - `ZEUS_PROFILE_PARAMS`: Warmup and measure iterations for each power limit,
                                separated by a comma. (Default:` "10,40"`)
       - `ZEUS_USE_OPTIMAL_PL`: Whether to actually use the optimal power limit found.
                                Setting this to false is the Observer Mode described
                                in Section 5. (Default:` "True"`)
     """
 
-    # Global power monitor instances.
-    monitors: list[subprocess.Popen] = []
-
     # The power limit currently set for the GPU.
-    current_gpu_pl: int = 0
+    current_gpu_pl: ClassVar[int] = 0
 
     # Train batch size to be accessed by the eval dataloader.
-    train_batch_size: int = 0
+    train_batch_size: ClassVar[int] = 0
 
     # Length of the eval dataloader. `epochs` in the train dataloader needs this.
-    eval_num_samples: int = 0
+    eval_num_samples: ClassVar[int] = 0
 
     # Train-time power profiling result. Maps power limit to avg_power & throughput.
-    train_power_result: dict[int, float] = {}
-    train_tput_result: dict[int, float] = {}
+    train_power_result: ClassVar[dict[int, float]] = {}
+    train_tput_result: ClassVar[dict[int, float]] = {}
 
     # Eval-time power profiling result. Maps power limit to avg_power & throughput.
-    eval_power_result: dict[int, float] = {}
-    eval_tput_result: dict[int, float] = {}
+    eval_power_result: ClassVar[dict[int, float]] = {}
+    eval_tput_result: ClassVar[dict[int, float]] = {}
 
     # Cost-optimal power limit. Set by the train dataloader after the last power limit
     # was explored.
-    optimal_pl: int = 0
+    optimal_pl: ClassVar[int] = 0
 
     # Train epoch measurements for time/energy accounting.
-    train_epoch_time: list[float] = []
+    train_epoch_time: ClassVar[list[float]] = []
     # The master process will record ALL GPUs' energy consumption during training.
     # GPU_i's energy records is `train_epoch_energy[i]`.
-    train_epoch_energy: np.ndarray = np.empty(0)
+    train_epoch_energy: ClassVar[np.ndarray] = np.empty(0)
 
     # Eval-time latency profiling result. Maps power limit to epoch latency.
-    eval_epoch_time: list[float] = []
+    eval_epoch_time: ClassVar[list[float]] = []
     # The master process will record ALL GPUs' energy consumption during evaluation.
     # GPU_i's energy records is `eval_epoch_energy[i]`.
-    eval_epoch_energy: np.ndarray = np.empty(0)
+    eval_epoch_energy: ClassVar[np.ndarray] = np.empty(0)
 
+    # Zeus monitor instance
+    zeus_monitor: ClassVar[ZeusMonitor | None] = None
+
+    # ruff: noqa: PLR0912, PLR0915
     def __init__(
         self,
         *args,
         batch_size: int,
         max_epochs: int = -1,
         distributed: Literal["dp"] | None = None,
         **kwargs,
     ) -> None:
         """Initialize the dataloader.
 
         Args:
             batch_size: Batch size to use for training.
             max_epochs: Maximum number of epochs to train. **Specify this parameter only
-                to the train data loader.**
+                to the train data loader.** (Default: `-1`)
             distributed: Distributed strategy to use for training. If training with single GPU,
                 this value should be `None`; if training using data parallel with multi-GPU on
-                a single node, this value should be `"dp"`.
+                a single node, this value should be `"dp"`. (Default: `None`)
+            *args: Arguments to pass to `torch.utils.data.DataLoader`.
+            **kwargs: Keyword arguments to pass to `torch.utils.data.DataLoader`.
 
         Raises:
             ValueError: `max_epochs` is specified when initializing the evaluation dataloader.
             RuntimeError: `torch.distributed` package is not available.
             RuntimeError: The default process group is not initialized. Make sure to call
                 `torch.distributed.init_process_group` to initialize the default process
                 group before doing a multiprocessing distributed training.
@@ -249,14 +243,15 @@
                 Please consider increasing batch size.
         """
         # Save attributes.
         self.batch_size = batch_size
         self.split = "train" if max_epochs != -1 else "eval"
         self.max_epochs = max_epochs
         self.log_prefix = f"[ZeusDataLoader({self.split})]"
+        self.logger = get_logger(self.log_prefix)
 
         # Initialize the DataLoader.
         super().__init__(*args, batch_size=batch_size, **kwargs)
 
         # World size and rank for distributed training.
         # Set default value for single-GPU.
         self.world_size = 1
@@ -291,19 +286,16 @@
                 raise ValueError(
                     "`DistributedSampler` is inconsistent with the default process group."
                     f" The default process group has `world_size={dist.get_world_size()}`,"
                     f" `rank={dist.get_rank()}`."
                 )
             self.world_size = dist.get_world_size()
             self.rank = dist.get_rank()
-        else:
-            if self.distributed is not None:
-                raise TypeError(
-                    '`distributed` currently only accepts `"dp"` or `None`.'
-                )
+        elif self.distributed is not None:
+            raise ValueError('`distributed` currently only accepts `"dp"` or `None`.')
 
         if self._is_train:
             self._log(
                 f"Distributed data parallel: {'ON' if self.world_size > 1 else 'OFF'}"
             )
 
         if self._is_train:
@@ -323,28 +315,24 @@
         self.logdir = get_env("ZEUS_LOG_DIR", str, default="zeus_log")
         self.job_id = get_env("ZEUS_JOB_ID", str, default="zeus")
         self.cost_thresh = get_env("ZEUS_COST_THRESH", float, default=float("inf"))
         self.eta_knob = get_env("ZEUS_ETA_KNOB", float, default=0.5)
         self.monitor_path = get_env(
             "ZEUS_MONITOR_PATH",
             str,
-            default="/workspace/zeus/zeus_monitor/zeus_monitor",
+            default="zeus_monitor",
         )
         self.warmup_iter, self.profile_iter = map(
             int, get_env("ZEUS_PROFILE_PARAMS", str, default="10,40").split(",")
         )
         self.use_optimal_pl = get_env("ZEUS_USE_OPTIMAL_PL", bool, default=True)
 
         # Create ZEUS_LOG_DIR if it does not exist.
         os.makedirs(self.logdir, exist_ok=True)
 
-        # Check whether the monitor path is good.
-        if not os.access(self.monitor_path, os.X_OK):
-            raise RuntimeError(f"'{self.monitor_path}' is not executable")
-
         # Whether the target metric was reached.
         self.target_metric_reached = False
 
         # Construct relevant paths.
         self.train_json = (
             f"{self.logdir}/{self.job_id}+bs{self.train_batch_size}.train.json"
         )
@@ -388,31 +376,34 @@
                 )
             self._log(
                 f"Scaling done! New profile window takes {self.warmup_iter + self.profile_iter}"
                 f" iterations ({self.warmup_iter} for warmup + {self.profile_iter} for profile)."
             )
 
         # Power profiling windows
+        # We're interested in the average power and throughput here.
         #
         # +----- warmup_start (change power limit)
-        # |        +----- prof_start (record timestamp)
-        # |        |                      +----- prof_end (compute and save results)
+        # |        +----- prof_start (`_prof_window_push`)
+        # |        |                      +----- prof_end (`_prof_window_pop`)
         # | warmup |        profile       |
         # v  iter  v          iter        v
         # ================================= =====================
         # |      power limit = 250W       | | power limit = 225W  ...
         # ================================= =====================
         #
         # =======================================================
         # |                         Epoch 1                       ...
         # =======================================================
+        # ^
+        # |
+        # +------- Time/energy accounting for the entire training job (`_prof_window_push`)
         #
         # Initialize variables for profiling
         self.warmup_start_sample = 0
-        self.prof_start_time = 0.0
         self.prof_start_sample = 0
         self.prof_state = NOT_PROFILING
         self.prof_pl_index = 0
 
         # Initialize data structure for storing the energy accounting
         # based on the number of GPUs.
         if self._is_train:
@@ -428,14 +419,15 @@
 
         # Initialize NVML and get GPU handle or each GPU at the master process.
         self.gpu_handles = []
         pynvml.nvmlInit()
         for index in range(self.world_size):
             handle = pynvml.nvmlDeviceGetHandleByIndex(index)
             # Set persistent mode.
+            # TODO(JW): Check SYS_ADMIN permissions and error with an explanation.
             pynvml.nvmlDeviceSetPersistenceMode(handle, pynvml.NVML_FEATURE_ENABLED)
             self.gpu_handles.append(handle)
         # Query NVML for the possible power limit range. Unit is mW.
         min_pl, self.max_pl = pynvml.nvmlDeviceGetPowerManagementLimitConstraints(
             self.gpu_handles[0]
         )
         self.power_limits = list(range(self.max_pl, min_pl - 25_000, -25_000))
@@ -443,34 +435,31 @@
             self._log(f"Power limit range: {self.power_limits}")
 
         # Check whether profiling is ON or OFF. If OFF, load the power limit
         # from power_json, and set power limit for all GPUs at the master process.
         if self._is_train and self.rank == 0:
             should_profile = self._should_profile
             self._log(f"Power profiling: {'ON' if should_profile else 'OFF'}")
+            # Initialize profiling service
+            ZeusDataLoader.zeus_monitor = ZeusMonitor(
+                list(range(self.world_size)),
+                self.monitor_path,
+            )
+
             # If we need to do profiling, no need to touch the power limit.
             # If profiling is already done, load profile information from power_json.
             # Only then do we have the optimal PL available.
             # We only load in the train dataloader since it populates classvars.
             if not should_profile:
                 self._load_power_results()
                 self._set_gpu_steady_power_limit()
 
-        # Make sure NVML is shutdown and the monitor is killed when the training script exits.
+        # Make sure NVML is shutdown when the training script exits.
         if self._is_train:
-
-            def exit_hook():
-                pynvml.nvmlShutdown()
-                # Master process kills all the monitors.
-                if self.rank == 0:
-                    for index, monitor in enumerate(self.monitors):
-                        monitor.kill()
-                        self._log(f"[GPU_{index}] Stopped Zeus monitor.")
-
-            atexit.register(exit_hook)
+            atexit.register(pynvml.nvmlShutdown)
 
     def epochs(self) -> Generator[int, None, None]:
         """Yield the current epoch number from 0 until when training should stop.
 
         Training should stop when
 
         - the cost reached the cost threshold, or
@@ -613,15 +602,15 @@
                     # the purpose of multiprocessing management.
                     # When doing data parallel training on multiple processes, ONLY the master
                     # process will predict `next_cost` and do the threshold checking. However,
                     # once the predicted cost exceeds the threshold, we want to terminate ALL
                     # the processes. Currently this is achieved by throwing an exception at the
                     # master process. The lauching script will terminate all the processes that
                     # are still alive.
-                    raise ZeusCostThresholdExceededException(
+                    raise ZeusCostThresholdExceededError(
                         time_consumed,
                         energy_consumed,
                         cost,
                         next_cost,
                         self.cost_thresh,
                     )
 
@@ -636,14 +625,15 @@
 
         Args:
             metric: The validation metric of the current epoch.
             higher_is_better: For example, this should be `True` for accuracy
                 and `False` for error.
         """
         assert self._is_train, "Use report_metric on the train dataloader."
+        # ruff: noqa: PLR5501
         if higher_is_better:
             if metric >= self.target_metric:
                 self.target_metric_reached = True
         else:
             if metric <= self.target_metric:
                 self.target_metric_reached = True
 
@@ -727,64 +717,46 @@
             master_only: Whether only logged by master process. Usually set to True for the
                 global logging and False for the GPU-specific logging . If set to False,
                 a prefix indicates which GPU this log comes from will be included as well.
                 (Default: `True`)
         """
         if master_only:
             if self.rank == 0:
-                LOG.log(level, "%s %s", self.log_prefix, message)
+                self.logger.log(level, "%s", message)
         else:
             gpu_log_prefix = f"[GPU_{self.rank}]"
-            LOG.log(level, "%s %s %s", self.log_prefix, gpu_log_prefix, message)
+            self.logger.log(level, "%s %s", gpu_log_prefix, message)
 
     @cached_property
     def _is_train(self) -> bool:
         """Return whether this dataloader is for training."""
         return self.split == "train"
 
-    def _power_log_path(self, rank: int) -> str:
-        """Build the path for the power monitor log file at the GPU with rank."""
-        return f"{self.logdir}/bs{self.train_batch_size}+e{self.epoch_num}+gpu{rank}.power.log"
-
-    def _start_monitor(self) -> None:
-        """Start the power monitor subprocess."""
-        # Sanity checks.
-        assert not ZeusDataLoader.monitors
-        # Only the master process starts the monitors.
-        assert self.rank == 0
+    @property
+    def _monitor_log_prefix(self) -> str:
+        """Build the prefix for the power monitor log file."""
+        return f"bs{self.train_batch_size}+e{self.epoch_num}"
 
-        # Start monitors. Master process starts and records all monitors.
-        for index in range(self.world_size):
-            monitor = subprocess.Popen(
-                [
-                    self.monitor_path,
-                    self._power_log_path(index),
-                    "0",
-                    "100",
-                    str(index),
-                ],
-            )
-            self._log(f"[GPU_{index}] Zeus monitor started.")
-            ZeusDataLoader.monitors.append(monitor)
+    @property
+    def _monitor(self) -> ZeusMonitor:
+        """Return the `ZeusMonitor` instance."""
+        assert (
+            ZeusDataLoader.zeus_monitor is not None
+        ), "ZeusDataLoader.zeus_monitor was not instantiated"
+        return ZeusDataLoader.zeus_monitor
 
-    def _kill_monitor(self) -> None:
-        """Kill the power monitor subprocess."""
-        # Sanity checks.
-        assert ZeusDataLoader.monitors
-        # Only the master process kills the monitors.
+    def _begin_measurement(self, name: str) -> None:
+        """A wrapper function that starts a measurement window."""
         assert self.rank == 0
+        self._monitor.begin_window(name, sync_cuda=True)
 
-        # Kill monitors.
-        for monitor in ZeusDataLoader.monitors:
-            monitor.send_signal(signal.SIGINT)
-        for monitor in ZeusDataLoader.monitors:
-            monitor.wait(timeout=1.0)
-
-        # Cleanup the monitor list
-        ZeusDataLoader.monitors = []
+    def _end_measurement(self, name: str) -> Measurement:
+        """A wrapper function that ends a measurement window and returns measurements."""
+        assert self.rank == 0
+        return self._monitor.end_window(name, sync_cuda=True)
 
     def _start_warmup(self) -> None:
         """Let the GPU run for some time with the poewr limit to profile."""
         # Sanity checks.
         assert self._should_profile, f"start_warmup: {self._should_profile=}"
         assert self._is_train, f"start_warmup: {self._is_train=}"
         assert self._power_limits_left, f"start_warmup: {self._power_limits_left=}"
@@ -821,16 +793,18 @@
         # Sanity check that this profile window ends before the end of the current epoch.
         assert self.sample_num + self.profile_iter < self.num_samples, (
             "start_prof: "
             f"end_of_this_profile_window {self.sample_num + self.profile_iter} "
             f"< end_of_this_epoch {self.num_samples}"
         )
 
-        # Start profile timer.
-        self.prof_start_time = time.monotonic()
+        if self.rank == 0:
+            # Push profiling window for the current power limit value.
+            # This window will profile for `self.profile_iter` iterations.
+            self._begin_measurement("__ZeusDataLoader_power_limit")
 
         # Set the sample number when we started profiling.
         self.prof_start_sample = self.sample_num
 
         # Set profiling state.
         self.prof_state = PROFILING
 
@@ -857,45 +831,29 @@
 
         # Set profiling state.
         self.prof_state = NOT_PROFILING
 
         # Call cudaSynchronize to make sure this is the iteration boundary.
         torch.cuda.synchronize()
 
-        # Freeze time.
-        now = time.monotonic()
-
         # Advance to the next power limit. Affects self.power_limits_left.
         self.prof_pl_index += 1
 
         if self.rank == 0:
+            # Pop profiling window for the current power limit and fetch profiling results.
+            profiling_result = self._end_measurement("__ZeusDataLoader_power_limit")
+            time_consumed, energy_consumed = (
+                profiling_result.time,
+                profiling_result.energy,
+            )
             # Summing up the average power on all GPUs.
-            sum_avg_power = 0
-            for index in range(self.world_size):
-                # Compute and save average power.
-                # The monitor is still running, so we just integrate from the beginning
-                # of this profiling window (of course exclude warmup) up to now.
-                # The power log file only records for the current epoch,
-                # so we compute an offset.
-                try:
-                    avg_power = analyze.avg_power(
-                        self._power_log_path(index),
-                        start=self.prof_start_time - self.epoch_start_time,
-                    )
-                except ValueError:
-                    self._log(
-                        "ValueError from analyze.avg_power, please consider increasing self.profile_iter.",
-                        logging.ERROR,
-                    )
-                    raise
-                sum_avg_power += avg_power
+            sum_avg_power = sum(energy_consumed.values()) / time_consumed
             self.train_power_result[self.current_gpu_pl] = sum_avg_power
 
             # Compute and save throughput. We use the time at the master process.
-            time_consumed = now - self.prof_start_time
             samples_processed = self.sample_num - self.prof_start_sample
             throughput = samples_processed / time_consumed
             self.train_tput_result[self.current_gpu_pl] = throughput
 
             self._log(f"Profile done with power limit {self.current_gpu_pl//1000}W")
 
             # If we're done with all power limits, compute the optimal power limit
@@ -972,43 +930,41 @@
         )
         with open(self.train_json, "w") as f:
             json.dump(train_result, f)
         with open(self.train_json, "r") as f:
             self._log("Training done.")
             self._log(f"Saved {self.train_json}: {f.read()}")
 
-    # pylint: disable=attribute-defined-outside-init
     def __iter__(self):
         """Signal the beginning of an epoch."""
         # Sanity check that there is no incomplete profile window at the beginning of epoch,
         # because we start profiling only if the entire profiling window can fit in the rest of
         # the training epoch.
         assert self.prof_state == NOT_PROFILING, f"__iter__: {self.prof_state=}"
 
         # Update counters.
         self.epoch_num += 1
         self.sample_num = 0
         self._log(f"Epoch {self.epoch_num} begin.")
 
-        # Start epoch timer.
-        self.epoch_start_time = time.monotonic()
-
         # Cache the dataloader iterator.
         self.iter = super().__iter__()
 
-        # The power limit of the GPU is only changed by the train dataloader.
-        if self._is_train and self.rank == 0:
-            # The train loader always starts the monitor, and the eval loader kills it.
-            self._start_monitor()
-            # If we're not profiling, use the steady state power limit.
-            # If we are profiling, the power limit will be set in __next__ with warmup.
-            # Power limit result is already loaded in when initializing the train dataloader,
-            # so we just set the power limit directly.
-            if not self._should_profile:
-                self._set_gpu_steady_power_limit()
+        if self.rank == 0:
+            # Push profiling window for the current epoch.
+            # Note that both train and eval dataloaders will push one profiling window *separately*.
+            self._begin_measurement("__ZeusDataLoader_epoch")
+            # The power limit of the GPU is only changed by the train dataloader.
+            if self._is_train:  # ruff: noqa: SIM102
+                # If we're not profiling, use the steady state power limit.
+                # If we are profiling, the power limit will be set in __next__ with warmup.
+                # Power limit result is already loaded in when initializing the train dataloader,
+                # so we just set the power limit directly.
+                if not self._should_profile:
+                    self._set_gpu_steady_power_limit()
 
         return self
 
     def __next__(self):
         """Signal the beginning of an iteration."""
         # Update counters.
         self.sample_num += 1
@@ -1020,82 +976,73 @@
             # End of this epoch.
             # Sanity check that there is no incomplete profile window at the end of epoch.
             assert self.prof_state == NOT_PROFILING, f"__next__: {self.prof_state=}"
 
             # Make sure all GPU operations are done so that now is the *actual* end of this epoch.
             torch.cuda.synchronize()
 
-            # The eval dataloader kills the monitor.
-            if not self._is_train and self.rank == 0:
-                self._kill_monitor()
-
             # Compute epoch time and energy consumption.
             # We're interested in the actual time/energy consumption here.
             #
-            #   <----------------- monitor lifetime ------------------>
-            #
-            #   =======================================================
-            #   |                Train                    ||   Eval   |
-            #   =======================================================
-            #   ^                                         ^^          ^
-            #   |                                        / |          |
-            #   epoch_start_time          time.monotonic() |          |
-            #   for train loader          for train loader |          |
-            #                                              |          |
-            #                               epoch_start_time   time.monotonic()
-            #                                for eval loader   for eval loader
+            #   ================================================================
+            #   |                      Train                       ||   Eval   |
+            #   ================================================================
+            #   ^                                                  ^^          ^
+            #   |                                                 / |          |
+            #   _prof_window_push()              _prof_window_pop() |          |
+            #   for train loader                   for train loader |          |
+            #                                                       |          |
+            #                                     _prof_window_push()   _prof_window_pop()
+            #                                         for eval loader      for eval loader
             #
             if self.rank == 0:
                 # Sanity check that `epoch_num` is within valid range
                 assert self.epoch_num >= 1, f"__next__: {self.epoch_num=}"
-                # Compute the time/energy consumption for this epoch.
-                time_consumption = time.monotonic() - self.epoch_start_time
+                # Pop profiling window for the current epoch and fetch profiling result.
+                profiling_result = self._end_measurement("__ZeusDataLoader_epoch")
+                time_consumed, energy_consumed = (
+                    profiling_result.time,
+                    profiling_result.energy,
+                )
+                sum_energy_consumed = sum(energy_consumed.values())
                 if self._is_train:
-                    self.train_epoch_time.append(time_consumption)
+                    self.train_epoch_time.append(time_consumed)
                     # Record the energy consumption for each GPU.
                     for index in range(self.world_size):
-                        # The monitor is still running, and we integrate over the entire log.
-                        energy_consumption = analyze.energy(self._power_log_path(index))
                         self.train_epoch_energy[index][
                             self.epoch_num - 1
-                        ] = energy_consumption
+                        ] = energy_consumed[index]
                 else:
-                    # We just killed the monitor. Integrate the last time_consumption seconds.
-                    self.eval_epoch_time.append(time_consumption)
-                    sum_energy_consumption = 0
+                    # Integrate the last time_consumed seconds.
+                    self.eval_epoch_time.append(time_consumed)
                     # Record the energy consumption for each GPU.
                     for index in range(self.world_size):
-                        # We set the `start` to exclude the logs during train time.
-                        energy_consumption = analyze.energy(
-                            self._power_log_path(index), start=-time_consumption
-                        )
                         self.eval_epoch_energy[index][
                             self.epoch_num - 1
-                        ] = energy_consumption
-                        sum_energy_consumption += energy_consumption
+                        ] = energy_consumed[index]
                     # For the eval dataloader, we want to record the throughput and power
                     # for the current power limit. Since the train dataloader sets the power limit
                     # to the optimal power limit right after profiling is done, this will naturally
                     # record the tput/power of the optimal PL. From the following epochs where we
                     # don't profile anything, we directly use these values to compute the time and
                     # energy consumed.
                     if self._should_profile:
                         self.eval_tput_result[self.current_gpu_pl] = (
-                            self.num_samples / time_consumption
+                            self.num_samples / time_consumed
                         )
                         self.eval_power_result[self.current_gpu_pl] = (
-                            sum_energy_consumption / time_consumption
+                            sum_energy_consumed / time_consumed
                         )
                         # The optimal PL being known means that all power limits have been explored.
                         # Let us end profiling by writing profile information to `power_json`.
                         if self.optimal_pl != 0:
                             self._save_power_results()
                 self._log(
                     f"{self.split} epoch {self.epoch_num} done: "
-                    f"time={time_consumption:.2f} energy={energy_consumption:.2f}"
+                    f"time={time_consumed:.2f} energy={sum_energy_consumed:.2f}"
                 )
 
             # Re-raise StopIteration.
             raise
 
         # We're in the middle of an epoch. The train loader has power limits left to profile.
         if self._is_train and self._should_profile and self._power_limits_left:
```

### Comparing `zeus-ml-0.3.0/zeus/run/master.py` & `zeus-ml-0.4.0/zeus/run/master.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             A list of [`HistoryEntry`][zeus.analyze.HistoryEntry] objects for each job run.
         """
         # Sanity checks
         if job.default_bs is None:
             raise ValueError("You must provide a default batch size for the job.")
         if job.command is None:
             raise ValueError("You must provide a command format string for the job.")
-        if eta_knob < 0.0 or eta_knob > 1.0:
+        if eta_knob < 0.0 or eta_knob > 1.0:  # ruff: noqa: PLR2004
             raise ValueError("eta_knob must be in [0.0, 1.0].")
 
         print(f"[Zeus Master] {job} x {num_recurrence}")
         print(f"[Zeus Master] Batch sizes: {batch_sizes}")
 
         # Copy all internal state so that simulation does not modify any
         # internal state and is deterministic w.r.t. the random seed.
```

### Comparing `zeus-ml-0.3.0/zeus/simulate.py` & `zeus-ml-0.4.0/zeus/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from zeus.analyze import HistoryEntry
 from zeus.job import Job
 from zeus.policy import BatchSizeOptimizer, PowerLimitOptimizer
 from zeus.util import zeus_cost
 
 
+# ruff: noqa: PLR0912, PLR0915
 class Simulator:
     """Simulates job execution optimized by Zeus."""
 
     def __init__(
         self,
         summary_train: str | pd.DataFrame,
         summary_power: str | pd.DataFrame,
```

### Comparing `zeus-ml-0.3.0/zeus/util/logging.py` & `zeus-ml-0.4.0/zeus/util/logging.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,29 +11,44 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utilities for logging."""
 
 import sys
+import logging
 from pathlib import Path
 
 
 class FileAndConsole:
     """Like tee, but for Python prints."""
 
     def __init__(self, filepath: Path) -> None:
         """Initialize the object."""
-        self.file = open(filepath, "w")
+        self.file = open(filepath, "w")  # ruff: noqa: SIM115
         self.stdout = sys.stdout
 
     def write(self, message):
         """Write message."""
         self.file.write(message)
         self.stdout.write(message)
         self.file.flush()
         self.stdout.flush()
 
     def flush(self):
         """Flush both log file and stdout."""
         self.file.flush()
         self.stdout.flush()
+
+
+def get_logger(name: str, level: int = logging.INFO) -> logging.Logger:
+    """Get a logger with the given name with some formatting configs."""
+    logger = logging.getLogger(name)
+    logger.propagate = False
+    logger.setLevel(level)
+    formatter = logging.Formatter(
+        "[%(asctime)s] [%(name)s](%(filename)s:%(lineno)d) %(message)s"
+    )
+    handler = logging.StreamHandler(sys.stdout)
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+    return logger
```

### Comparing `zeus-ml-0.3.0/zeus/util/lr_scaler.py` & `zeus-ml-0.4.0/zeus/util/lr_scaler.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.3.0/zeus/util/metric.py` & `zeus-ml-0.4.0/zeus/util/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     Returns:
         The cost of the DL training job.
     """
     return eta_knob * energy + (1 - eta_knob) * max_power * time
 
 
-class ZeusCostThresholdExceededException(Exception):
+class ZeusCostThresholdExceededError(Exception):
     """Raised when the predicted cost of the next epoch exceeds the cost threshold.
 
     This exception is used for terminating all the processes when doing data
     parallel training with multiple processes, because ONLY the master
     process will predict `next_cost` and do the threshold checking. However,
     once the predicted cost exceeds the threshold, we want to terminate ALL
     the processes. Currently this is achieved by throwing an exception at the
```

### Comparing `zeus-ml-0.3.0/zeus_ml.egg-info/PKG-INFO` & `zeus-ml-0.4.0/zeus_ml.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.3.0
+Version: 0.4.0
 Summary: An Energy Optimization Framework for DNN Training
 Home-page: https://github.com/SymbioticLab/Zeus
 Author: Jae-Won Chung
 Author-email: jwnchung@umich.edu
 License: Apache-2.0
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,mlsys
@@ -13,13 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zeus: An Energy Optimization Framework for DNN Training
```

