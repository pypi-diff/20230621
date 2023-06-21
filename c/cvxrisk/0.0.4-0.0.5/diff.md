# Comparing `tmp/cvxrisk-0.0.4.tar.gz` & `tmp/cvxrisk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxrisk-0.0.4.tar", max compression
+gzip compressed data, was "cvxrisk-0.0.5.tar", max compression
```

## Comparing `cvxrisk-0.0.4.tar` & `cvxrisk-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11375 2023-06-20 16:02:07.344632 cvxrisk-0.0.4/LICENSE
--rw-r--r--   0        0        0     4710 2023-06-20 16:02:07.344632 cvxrisk-0.0.4/README.md
--rw-r--r--   0        0        0       97 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/__init__.py
--rw-r--r--   0        0        0       83 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/cvar/__init__.py
--rw-r--r--   0        0        0     1596 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/cvar/cvar.py
--rw-r--r--   0        0        0       92 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/factor/__init__.py
--rw-r--r--   0        0        0     1995 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/factor/factor.py
--rw-r--r--   0        0        0      137 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/__init__.py
--rw-r--r--   0        0        0      252 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/cholesky.py
--rw-r--r--   0        0        0     1301 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/pca.py
--rw-r--r--   0        0        0      512 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/linalg/valid.py
--rw-r--r--   0        0        0      492 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/model.py
--rw-r--r--   0        0        0       91 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/random/__init__.py
--rw-r--r--   0        0        0      159 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/random/rand_cov.py
--rw-r--r--   0        0        0       97 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/sample/__init__.py
--rw-r--r--   0        0        0     1725 2023-06-20 16:02:07.368631 cvxrisk-0.0.4/cvx/risk/sample/sample.py
--rw-r--r--   0        0        0      581 2023-06-20 16:02:32.720575 cvxrisk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 cvxrisk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-21 06:49:02.832458 cvxrisk-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4696 2023-06-21 06:49:02.832458 cvxrisk-0.0.5/README.md
+-rw-r--r--   0        0        0       97 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/cvar/__init__.py
+-rw-r--r--   0        0        0     1329 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/cvar/cvar.py
+-rw-r--r--   0        0        0       92 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/factor/__init__.py
+-rw-r--r--   0        0        0     2010 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/factor/factor.py
+-rw-r--r--   0        0        0      137 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/linalg/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/linalg/cholesky.py
+-rw-r--r--   0        0        0     1301 2023-06-21 06:49:02.856459 cvxrisk-0.0.5/cvx/risk/linalg/pca.py
+-rw-r--r--   0        0        0      512 2023-06-21 06:49:02.860458 cvxrisk-0.0.5/cvx/risk/linalg/valid.py
+-rw-r--r--   0        0        0     1899 2023-06-21 06:49:02.860458 cvxrisk-0.0.5/cvx/risk/model.py
+-rw-r--r--   0        0        0       91 2023-06-21 06:49:02.860458 cvxrisk-0.0.5/cvx/risk/random/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-21 06:49:02.860458 cvxrisk-0.0.5/cvx/risk/random/rand_cov.py
+-rw-r--r--   0        0        0       97 2023-06-21 06:49:02.860458 cvxrisk-0.0.5/cvx/risk/sample/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-21 06:49:02.860458 cvxrisk-0.0.5/cvx/risk/sample/sample.py
+-rw-r--r--   0        0        0      581 2023-06-21 06:49:29.644734 cvxrisk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 cvxrisk-0.0.5/PKG-INFO
```

### Comparing `cvxrisk-0.0.4/LICENSE` & `cvxrisk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.4/README.md` & `cvxrisk-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 Using this class, we can formulate a function computing a standard minimum risk portfolio as
 
 ```python
 import cvxpy as cp
 
 from cvx.risk import RiskModel
 
+
 def minimum_risk(w: cp.Variable, risk_model: RiskModel) -> cp.Problem:
     """Constructs a minimum variance portfolio.
 
     Args:
         w: cp.Variable representing the portfolio weights.
         risk_model: A risk model.
 
     Returns:
         A convex optimization problem.
     """
     return cp.Problem(
-        cp.Minimize(risk_model.estimate_risk(w)),
+        cp.Minimize(risk_model.estimate(w)),
         [cp.sum(w) == 1, w >= 0]
     )
 ```
 
 The risk model is injected into the function.
 The function is not aware of the precise risk model used.
-All risk models are required to implement the `estimate_risk` method.
+All risk models are required to implement the `estimate` method.
 
 ## A first example
 
 A first example is a risk model based on the sample covariance matrix.
 We construct the risk model as follows
 
 ```python
@@ -43,15 +44,15 @@
 
 from cvx.risk.sample import SampleCovariance
 
 riskmodel = SampleCovariance(num=2)
 w = cp.Variable(2)
 problem = minimum_risk(w, riskmodel)
 
-riskmodel.update_data(cov=np.array([[1.0, 0.5], [0.5, 2.0]]))
+riskmodel.update(cov=np.array([[1.0, 0.5], [0.5, 2.0]]))
 problem.solve()
 print(w.value)
 ```
 
 The risk model and the actual optimization problem are decoupled.
 This is good practice and keeps the code clean and maintainable.
```

### Comparing `cvxrisk-0.0.4/cvx/risk/cvar/cvar.py` & `cvxrisk-0.0.5/cvx/risk/sample/sample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,42 @@
 # -*- coding: utf-8 -*-
+"""Risk models based on the sample covariance matrix
+"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 import cvxpy as cvx
 import numpy as np
 
+from cvx.risk.linalg import cholesky
+from cvx.risk.model import Bounds
 from cvx.risk.model import RiskModel
 
 
 @dataclass
-class CVar(RiskModel):
-    """Conditional value at risk model"""
+class SampleCovariance(RiskModel):
+    """Risk model based on the Cholesky decomposition of the sample cov matrix"""
 
-    alpha: float = 0.95
-    n: int = 0
-    m: int = 0
+    num: int = 0
 
     def __post_init__(self):
-        self.k = int(self.n * (1 - self.alpha))
-        self.R = cvx.Parameter(
-            shape=(self.n, self.m), name="returns", value=np.zeros((self.n, self.m))
+        self.parameter["chol"] = cvx.Parameter(
+            shape=(self.num, self.num),
+            name="cholesky of covariance",
+            value=np.zeros((self.num, self.num)),
         )
-        self.lower = cvx.Parameter(
-            shape=self.m,
-            name="lower bound",
-            value=np.zeros(self.m),
-        )
-        self.upper = cvx.Parameter(
-            shape=self.m,
-            name="upper bound",
-            value=np.ones(self.m),
-        )
-
-    # R: np.ndarray = None
+        self.bounds = Bounds(m=self.num)
 
-    def estimate_risk(self, weights, **kwargs):
+    def estimate(self, weights, **kwargs):
         """Estimate the risk by computing the Cholesky decomposition of self.cov"""
-        # R is a matrix of returns, n is the number of rows in R
-        # n = self.R.shape[0]
-        # k is the number of returns in the left tail
-        # k = int(n * (1 - self.alpha))
-        # average value of the k elements in the left tail
-        return -cvx.sum_smallest(self.R @ weights, k=self.k) / self.k
-
-    def update_data(self, **kwargs):
-        ret = kwargs["returns"]
-        m = ret.shape[1]
+        return cvx.norm2(self.parameter["chol"] @ weights)
 
-        self.R.value[:, :m] = kwargs["returns"]
+    def update(self, **kwargs):
+        cov = kwargs["cov"]
+        n = cov.shape[0]
 
-        self.lower.value = np.zeros(self.m)
-        self.lower.value[:m] = kwargs["lower"]
+        self.parameter["chol"].value[:n, :n] = cholesky(cov)
+        self.bounds.update(**kwargs)
 
-        self.upper.value = np.zeros(self.m)
-        self.upper.value[:m] = kwargs["upper"]
+    def constraints(self, weights):
+        return self.bounds.constraints(weights)
```

### Comparing `cvxrisk-0.0.4/cvx/risk/linalg/pca.py` & `cvxrisk-0.0.5/cvx/risk/linalg/pca.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.4/cvx/risk/linalg/valid.py` & `cvxrisk-0.0.5/cvx/risk/linalg/valid.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.4/cvx/risk/sample/sample.py` & `cvxrisk-0.0.5/cvx/risk/cvar/cvar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,45 @@
 # -*- coding: utf-8 -*-
-"""Risk models based on the sample covariance matrix
-"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 import cvxpy as cvx
 import numpy as np
 
-from cvx.risk.linalg import cholesky
+from cvx.risk.model import Bounds
 from cvx.risk.model import RiskModel
-from cvx.risk.random import rand_cov
 
 
 @dataclass
-class SampleCovariance(RiskModel):
-    """Risk model based on the Cholesky decomposition of the sample cov matrix"""
+class CVar(RiskModel):
+    """Conditional value at risk model"""
 
-    num: int = 0
+    alpha: float = 0.95
+    n: int = 0
+    m: int = 0
 
     def __post_init__(self):
-        self._chol = cvx.Parameter(
-            shape=(self.num, self.num),
-            name="cholesky of covariance",
-            value=np.zeros((self.num, self.num)),
-        )
-        self.lower = cvx.Parameter(
-            shape=self.num,
-            name="lower bound",
-            value=np.zeros(self.num),
-        )
-        self.upper = cvx.Parameter(
-            shape=self.num,
-            name="upper bound",
-            value=np.ones(self.num),
+        self.k = int(self.n * (1 - self.alpha))
+        self.parameter["R"] = cvx.Parameter(
+            shape=(self.n, self.m), name="returns", value=np.zeros((self.n, self.m))
         )
+        self.bounds = Bounds(m=self.m)
 
-    def estimate_risk(self, weights, **kwargs):
+    def estimate(self, weights, **kwargs):
         """Estimate the risk by computing the Cholesky decomposition of self.cov"""
-        return cvx.norm2(self._chol @ weights)
-
-    def update_data(self, **kwargs):
-        cov = kwargs["cov"]
-        n = cov.shape[0]
-
-        self._chol.value[:n, :n] = cholesky(cov)
-        self.lower.value = np.zeros(self.num)
-        self.lower.value[:n] = kwargs["lower"]
-
-        self.upper.value = np.zeros(self.num)
-        self.upper.value[:n] = kwargs["upper"]
-
-
-if __name__ == "__main__":
-    s = SampleCovariance(num=5)
-    cov = rand_cov(4)
-    s.update_data(cov=cov, lower=np.zeros(4), upper=np.ones(4))
+        # R is a matrix of returns, n is the number of rows in R
+        # n = self.R.shape[0]
+        # k is the number of returns in the left tail
+        # k = int(n * (1 - self.alpha))
+        # average value of the k elements in the left tail
+        return -cvx.sum_smallest(self.parameter["R"] @ weights, k=self.k) / self.k
+
+    def update(self, **kwargs):
+        ret = kwargs["returns"]
+        m = ret.shape[1]
 
-    print(s.lower.value)
-    print(s.upper.value)
+        self.parameter["R"].value[:, :m] = kwargs["returns"]
+        self.bounds.update(**kwargs)
 
-    # z = np.zeros((5,5))
-    # z[:4,:4] = cholesky(cov)
-    # print(z
+    def constraints(self, weights):
+        return self.bounds.constraints(weights)
```

### Comparing `cvxrisk-0.0.4/pyproject.toml` & `cvxrisk-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxrisk"
-version = "v0.0.4"
+version = "v0.0.5"
 description = "Simple riskengine for cvxpy"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cvxrisk"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxrisk-0.0.4/PKG-INFO` & `cvxrisk-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxrisk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple riskengine for cvxpy
 Home-page: https://github.com/cvxgrp/cvxrisk
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,33 +26,34 @@
 Using this class, we can formulate a function computing a standard minimum risk portfolio as
 
 ```python
 import cvxpy as cp
 
 from cvx.risk import RiskModel
 
+
 def minimum_risk(w: cp.Variable, risk_model: RiskModel) -> cp.Problem:
     """Constructs a minimum variance portfolio.
 
     Args:
         w: cp.Variable representing the portfolio weights.
         risk_model: A risk model.
 
     Returns:
         A convex optimization problem.
     """
     return cp.Problem(
-        cp.Minimize(risk_model.estimate_risk(w)),
+        cp.Minimize(risk_model.estimate(w)),
         [cp.sum(w) == 1, w >= 0]
     )
 ```
 
 The risk model is injected into the function.
 The function is not aware of the precise risk model used.
-All risk models are required to implement the `estimate_risk` method.
+All risk models are required to implement the `estimate` method.
 
 ## A first example
 
 A first example is a risk model based on the sample covariance matrix.
 We construct the risk model as follows
 
 ```python
@@ -61,15 +62,15 @@
 
 from cvx.risk.sample import SampleCovariance
 
 riskmodel = SampleCovariance(num=2)
 w = cp.Variable(2)
 problem = minimum_risk(w, riskmodel)
 
-riskmodel.update_data(cov=np.array([[1.0, 0.5], [0.5, 2.0]]))
+riskmodel.update(cov=np.array([[1.0, 0.5], [0.5, 2.0]]))
 problem.solve()
 print(w.value)
 ```
 
 The risk model and the actual optimization problem are decoupled.
 This is good practice and keeps the code clean and maintainable.
```

