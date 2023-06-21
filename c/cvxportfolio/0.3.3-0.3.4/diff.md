# Comparing `tmp/cvxportfolio-0.3.3.tar.gz` & `tmp/cvxportfolio-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.3.3.tar", last modified: Mon Jun 19 17:48:13 2023, max compression
+gzip compressed data, was "cvxportfolio-0.3.4.tar", last modified: Wed Jun 21 02:55:07 2023, max compression
```

## Comparing `cvxportfolio-0.3.3.tar` & `cvxportfolio-0.3.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.788514 cvxportfolio-0.3.3/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.3/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.3/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-19 17:48:13.788174 cvxportfolio-0.3.3/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     5710 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.775309 cvxportfolio-0.3.3/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)      912 2023-06-19 17:48:06.000000 cvxportfolio-0.3.3/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     2053 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/benchmark.py
--rw-r--r--   0 enzo       (501) staff       (20)    11940 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    14023 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    20123 2023-06-10 04:38:54.000000 cvxportfolio-0.3.3/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    14756 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     9724 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    21189 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     6483 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)     9003 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    17823 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    39747 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.787300 cvxportfolio-0.3.3/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:06.000000 cvxportfolio-0.3.3/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1623 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)     9929 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     8359 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10308 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     6737 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     8877 2023-06-10 04:38:54.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    21842 2023-06-14 04:09:34.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     5754 2023-06-10 04:38:54.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9065 2023-05-27 05:39:35.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    26143 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.3/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo       (501) staff       (20)     1269 2023-06-18 05:48:46.000000 cvxportfolio-0.3.3/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:13.777056 cvxportfolio-0.3.3/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       59 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-06-19 17:48:13.000000 cvxportfolio-0.3.3/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-06-19 17:48:13.788594 cvxportfolio-0.3.3/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)      783 2023-06-19 17:48:06.000000 cvxportfolio-0.3.3/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.841200 cvxportfolio-0.3.4/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.4/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.4/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)     6080 2023-06-21 02:55:07.840826 cvxportfolio-0.3.4/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     5710 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.821729 cvxportfolio-0.3.4/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)      912 2023-06-21 02:54:26.000000 cvxportfolio-0.3.4/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2053 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/benchmark.py
+-rw-r--r--   0 enzo       (501) staff       (20)    11940 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14023 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20123 2023-06-10 04:38:54.000000 cvxportfolio-0.3.4/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14756 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9724 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21189 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6483 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9003 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    17823 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    39887 2023-06-21 02:54:26.000000 cvxportfolio-0.3.4/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.838670 cvxportfolio-0.3.4/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:06.000000 cvxportfolio-0.3.4/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1623 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     9929 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8359 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10308 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6737 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8877 2023-06-10 04:38:54.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21842 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5754 2023-06-10 04:38:54.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9065 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    26143 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     1269 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.824043 cvxportfolio-0.3.4/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)     6080 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       59 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-06-21 02:55:07.841290 cvxportfolio-0.3.4/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)      937 2023-06-21 02:54:26.000000 cvxportfolio-0.3.4/setup.py
```

### Comparing `cvxportfolio-0.3.3/LICENSE` & `cvxportfolio-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/README.md` & `cvxportfolio-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/__init__.py` & `cvxportfolio-0.3.4/cvxportfolio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 from .data import *
 from .simulator import *
 from .result import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
```

### Comparing `cvxportfolio-0.3.3/cvxportfolio/benchmark.py` & `cvxportfolio-0.3.4/cvxportfolio/benchmark.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/constraints.py` & `cvxportfolio-0.3.4/cvxportfolio/constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/costs.py` & `cvxportfolio-0.3.4/cvxportfolio/costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/data.py` & `cvxportfolio-0.3.4/cvxportfolio/data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/errors.py` & `cvxportfolio-0.3.4/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/estimator.py` & `cvxportfolio-0.3.4/cvxportfolio/estimator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/forecast.py` & `cvxportfolio-0.3.4/cvxportfolio/forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/policies.py` & `cvxportfolio-0.3.4/cvxportfolio/policies.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/result.py` & `cvxportfolio-0.3.4/cvxportfolio/result.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/returns.py` & `cvxportfolio-0.3.4/cvxportfolio/returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/risks.py` & `cvxportfolio-0.3.4/cvxportfolio/risks.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/simulator.py` & `cvxportfolio-0.3.4/cvxportfolio/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -681,14 +681,16 @@
     def _concatenated_backtests(self, policy, start_time, end_time, h):
         constituent_backtests_params = self.market_data.get_limited_backtests(start_time, end_time)
         # print(constituent_backtests_params)
         results = []
         orig_md = self.market_data
         orig_policy = policy
         for el in constituent_backtests_params:
+            logging.info(f"current universe: {el['universe']}")
+            logging.info(f"interval: {el['start_time']}, {el['end_time']}")
             self.market_data = orig_md._reduce_universe(el['universe'])
             # TODO improve
             if len(el['universe']) > len(h):
                 tmp = pd.Series(0, el['universe'])
                 tmp[h.index] = h
                 h = tmp
             else:
```

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/base.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/base.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.3.4/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.3.4/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_policies.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_risks.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-0.3.4/cvxportfolio/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.3.4/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio/utils.py` & `cvxportfolio-0.3.4/cvxportfolio/utils.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.3.4/cvxportfolio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.3/setup.py` & `cvxportfolio-0.3.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup
 
+with open('README.md') as f:
+    long_descr = ''.join(f.readlines())
+
 setup(
     name='cvxportfolio',
-    version='0.3.3',
+    version='0.3.4',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
@@ -16,8 +19,10 @@
     description='Portfolio optimization.',
     install_requires=["pandas",
                       "numpy",
                       "matplotlib",
                       "yfinance",
                       "cvxpy>=1.0.6",
                       "multiprocess"],
+    long_description=long_descr,
+    long_description_content_type='text/markdown',
 )
```

