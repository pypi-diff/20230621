# Comparing `tmp/pyoptmat-1.3.1.tar.gz` & `tmp/pyoptmat-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptmat-1.3.1.tar", last modified: Tue Jun  6 18:09:45 2023, max compression
+gzip compressed data, was "pyoptmat-1.3.2.tar", last modified: Wed Jun 21 17:07:13 2023, max compression
```

## Comparing `pyoptmat-1.3.1.tar` & `pyoptmat-1.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/pyoptmat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/chunktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/damage.py
--rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)    46061 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/flowrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    35630 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/hardening.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/neuralode.py
--rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/pyoptmat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_adjoint_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    35434 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_batch_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_chunktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_flowrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_hardening.py
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_model_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:13.228311 pyoptmat-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-21 17:07:13.228311 pyoptmat-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:13.228311 pyoptmat-1.3.2/pyoptmat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/chunktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46061 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/flowrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35630 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/hardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/neuralode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25328 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/pyoptmat/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:13.228311 pyoptmat-1.3.2/pyoptmat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-21 17:07:13.000000 pyoptmat-1.3.2/pyoptmat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-21 17:07:13.000000 pyoptmat-1.3.2/pyoptmat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:07:13.000000 pyoptmat-1.3.2/pyoptmat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 17:07:13.000000 pyoptmat-1.3.2/pyoptmat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 17:07:13.000000 pyoptmat-1.3.2/pyoptmat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:07:13.000000 pyoptmat-1.3.2/pyoptmat.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 17:07:13.228311 pyoptmat-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:07:13.228311 pyoptmat-1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_adjoint_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35434 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_batch_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_chunktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_flowrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_hardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_model_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-21 17:07:09.000000 pyoptmat-1.3.2/test/test_utility.py
```

### Comparing `pyoptmat-1.3.1/LICENSE` & `pyoptmat-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/PKG-INFO` & `pyoptmat-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptmat
-Version: 1.3.1
+Version: 1.3.2
 Summary: Statistical inference for material models
 Home-page: https://github.com/Argonne-National-Laboratory/pyoptmat
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
 License: UNKNOWN
 Keywords: materials inference modeling
 Platform: UNKNOWN
```

### Comparing `pyoptmat-1.3.1/README.md` & `pyoptmat-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/chunktime.py` & `pyoptmat-1.3.2/pyoptmat/chunktime.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,34 @@
         Form the factorization...
 
         Args:
             diag (torch.tensor): diagonal blocks of shape (nblk, sbat, sblk, sblk)
         """
         self.lu, self.pivots, _ = torch.linalg.lu_factor_ex(self.A)
 
+    def forward(self, v):
+        """
+        Run the solve using the linear algebra type interface
+        with the number of blocks and block size squeezed
+
+        Args:
+            v (torch.tensor): tensor of shape (sbat, sblk*nblk)
+        """
+        return (
+            self.matvec(
+                v.reshape((self.sbat, self.nblk, self.sblk))
+                .transpose(0, 1)
+                .unsqueeze(-1)
+                .contiguous()
+            )
+            .squeeze(-1)
+            .transpose(0, 1)
+            .flatten(start_dim=1)
+        )
+
 
 def thomas_solve(lu, pivots, B, v):
     """Simple function implementing a Thomas solve
 
     Solves in place of v
 
     Args:
@@ -173,72 +193,53 @@
     factorization
 
     Args:
         A (torch.tensor): tensor of shape (nblk,sbat,sblk,sblk) with the main diagonal
         B (torch.tensor): tensor of shape (nblk-1,sbat,sblk,sblk) with the off diagonal
     """
 
-    def forward(self, v):
+    def matvec(self, v):
         """
         Complete the backsolve for a given right hand side
 
         Args:
-            v (torch.tensor): tensor of shape (sbat, sblk*nblk)
+            v (torch.tensor): tensor of shape (nblk, sbat, sblk, 1)
         """
-        v = v.reshape((self.sbat, self.nblk, self.sblk)).transpose(0, 1).unsqueeze(-1)
-        v = thomas_solve(self.lu, self.pivots, self.B, v)
-
-        return v.squeeze(-1).transpose(0, 1).flatten(start_dim=1)
+        return thomas_solve(self.lu, self.pivots, self.B, v)
 
 
 class BidiagonalPCRFactorization(LUFactorization):
     """
     Manages the data needed to solve our bidiagonal system via parallel cyclic reduction
 
     Args:
         A (torch.tensor): tensor of shape (nblk,sbat,sblk,sblk) with the main diagonal
         B (torch.tensor): tensor of shape (nblk-1,sbat,sblk,sblk) with the off diagonal
     """
 
-    def forward(self, v):
+    def matvec(self, v):
         """
         Complete the backsolve for a given right hand side
 
         Args:
-            v (torch.tensor): tensor of shape (sbat, sblk*nblk)
+            v (torch.tensor): tensor of shape (nblk, sbat, sblk, 1)
         """
-        # Reshape and add dimensions
-        # This puts the input into "blocked form"
-        # contiguous is necessary because my _cyclic_shift function assumes initially
-        # contiguous memory
-        v = (
-            v.reshape((self.sbat, self.nblk, self.sblk))
-            .transpose(0, 1)
-            .unsqueeze(-1)
-            .contiguous()
-        )
-
         # We could do this in place if it wasn't for the pad
         self.B = pad(self.B, (0, 0, 0, 0, 0, 0, 1, 0))
 
         # Now figure out how many powers of 2 we need to complete our matrix
         for s, e in zip(*self._pow2(self.nblk)):
             self.B[s + 1 : e], v[s + 1 : e] = self._solve_block(
                 self.lu[s:e], self.pivots[s:e], self.B[s:e], v[s:e]
             )
 
         # To retain consistent sizes
         self.B = self.B[1:]
 
-        return (
-            torch.linalg.lu_solve(self.lu, self.pivots, v)
-            .squeeze(-1)
-            .transpose(0, 1)
-            .flatten(start_dim=1)
-        )
+        return torch.linalg.lu_solve(self.lu, self.pivots, v)
 
     def _solve_block(self, lu, pivots, B, v):
         """Solve a subsection of the matrix via PCR
 
         Args:
             lu (torch.tensor): (ncurr,sbat,sblk,sblk)
             pivots (torch.tensor): (ncurr,sbat,sblk)
@@ -337,32 +338,21 @@
 
     def __init__(self, *args, min_size=0, **kwargs):
         super().__init__(*args, **kwargs)
 
         # I use < below...
         self.min_size = min_size + 1
 
-    def forward(self, v):
+    def matvec(self, v):
         """
         Complete the backsolve for a given right hand side
 
         Args:
-            v (torch.tensor): tensor of shape (sbat, sblk*nblk)
+            v (torch.tensor): tensor of shape (nblk, sbat, sblk, 1)
         """
-        # Reshape and add dimensions
-        # This puts the input into "blocked form"
-        # contiguous is necessary because my _cyclic_shift function assumes initially
-        # contiguous memory
-        v = (
-            v.reshape((self.sbat, self.nblk, self.sblk))
-            .transpose(0, 1)
-            .unsqueeze(-1)
-            .contiguous()
-        )
-
         # We could do this in place if it wasn't for the pad
         self.B = pad(self.B, (0, 0, 0, 0, 0, 0, 1, 0))
 
         # Get the PCR blocks to actually use
         start, end, last = self._pcr_blocks()
 
         # Do PCR
@@ -377,21 +367,24 @@
         # We still need to solve the first block even if last is 0
 
         # The actual LU solve for the solution
         v[:last] = torch.linalg.lu_solve(self.lu[:last], self.pivots[:last], v[:last])
 
         # Now take over for Thomas
         for i in range(last, self.nblk):
+            # The .clone() here should not be necessary, but for whatever
+            # reason torch autograd give the usual "in place" complaint
+            # without it...
             v[i] = torch.linalg.lu_solve(
                 self.lu[i],
                 self.pivots[i],
                 v[i] - torch.bmm(self.B[i - 1], v[i - 1].clone()),
             )
 
-        return v.squeeze(-1).transpose(0, 1).flatten(start_dim=1)
+        return v
 
     def _pcr_blocks(self):
         """Figure out the PCR blocks we are actually going to use"""
         # Figure out which blocks we're going to use
         start, end = self._pow2(self.nblk)
         # These are sorted...
         blk_size = [e - s for e, s in zip(end, start)]
```

### Comparing `pyoptmat-1.3.1/pyoptmat/damage.py` & `pyoptmat-1.3.2/pyoptmat/damage.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/experiments.py` & `pyoptmat-1.3.2/pyoptmat/experiments.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/flowrules.py` & `pyoptmat-1.3.2/pyoptmat/flowrules.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/hardening.py` & `pyoptmat-1.3.2/pyoptmat/hardening.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/models.py` & `pyoptmat-1.3.2/pyoptmat/models.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/neuralode.py` & `pyoptmat-1.3.2/pyoptmat/neuralode.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/ode.py` & `pyoptmat-1.3.2/pyoptmat/ode.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     system and set of ODEs, but we highly recommend determining an
     optimal block size for your system and not leaving it set to the
     default value of 1.
 """
 import torch
 
 from pyoptmat import chunktime
+from pyoptmat.utility import mbmm
 
 
 class BackwardEulerScheme:
     """
     Integration with the backward Euler method
     """
 
@@ -87,48 +88,51 @@
         # This has I-J blocks on the main block diagonal and -I on the -1 block diagonal
         I = torch.eye(prob_size, device=dt.device).expand(ntime, batch_size, -1, -1)
 
         return R, chunktime.BidiagonalForwardOperator(
             I - yJ[1:] * dt.unsqueeze(-1).unsqueeze(-1), -I[1:], inverse_operator=solver
         )
 
-    def update_adjoint(self, dt, J, a_prev, grads):
+    def update_adjoint(
+        self, dt, J, a_prev, grads, solver=chunktime.BidiagonalThomasFactorization
+    ):
         """
         Update the adjoint for a block of time
 
         Args:
             dt (torch.tensor):      block of time steps
             J (torch.tensor):       block of Jacobians
             a_prev (torch.tensor):  previous adjoint
             grads (torch.tensor):   block of gradient values
 
         Returns:
             adjoint_block (torch.tensor): block of updated adjoint values
         """
+        # Setup and useful sizes
         ntime = J.shape[0] - 1
         prob_size = J.shape[2]
         batch_size = J.shape[1]
 
         adjoint_block = torch.zeros(J.shape[:-1], dtype=J.dtype, device=J.device)
-        adjoint_block[0] = a_prev
 
-        # Invert J all at once
+        # Basic operators
         I = torch.eye(prob_size, device=dt.device).expand(ntime, batch_size, -1, -1)
-        lu, pivot, _ = torch.linalg.lu_factor_ex(
-            I + J[:-1].transpose(-1, -2) * dt.unsqueeze(-1).unsqueeze(-1)
-        )
+        dJ = J[:-1].transpose(-1, -2) * dt.unsqueeze(-1).unsqueeze(-1)
 
-        # This has to be done sequentially...
-        for i in range(ntime):
-            adjoint_block[i + 1] = torch.linalg.lu_solve(
-                lu[i], pivot[i], adjoint_block[i].unsqueeze(-1)
-            ).squeeze(-1)
-            adjoint_block[i + 1] += grads[i + 1]
+        # The operator is pretty trivial
+        op = solver(I + dJ, -I[:-1])
+        rhs = grads[1:].unsqueeze(-1) + mbmm(
+            dJ,
+            grads[1:].unsqueeze(-1)
+            - a_prev.unsqueeze(0).expand(ntime, batch_size, -1).unsqueeze(-1),
+        )
 
-        return adjoint_block
+        # Actually do the batch solve
+        adjoint_block[1:] = op.matvec(rhs).squeeze(-1)
+        return adjoint_block + a_prev
 
     def accumulate(self, prev, time, y, a, grad, grad_fn):
         """
         Calculate the accumulated value given the results at each time step
 
         Args:
             prev (tuple of tensors): previous results
@@ -194,40 +198,50 @@
 
         return R, chunktime.BidiagonalForwardOperator(
             I,
             -I[1:] - yJ[1:-1] * dt[1:].unsqueeze(-1).unsqueeze(-1),
             inverse_operator=solver,
         )
 
-    def update_adjoint(self, dt, J, a_prev, grads):
+    def update_adjoint(
+        self, dt, J, a_prev, grads, solver=chunktime.BidiagonalThomasFactorization
+    ):
         """
         Update the adjoint for a block of time
 
         Args:
             dt (torch.tensor):      block of time steps
             J (torch.tensor):       block of Jacobians
             a_prev (torch.tensor):  previous adjoint
             grads (torch.tensor):   block of gradient values
 
         Returns:
             adjoint_block (torch.tensor): block of updated adjoint values
         """
+        # Setup and useful sizes
         ntime = J.shape[0] - 1
+        prob_size = J.shape[2]
+        batch_size = J.shape[1]
 
         adjoint_block = torch.zeros(J.shape[:-1], dtype=J.dtype, device=J.device)
-        adjoint_block[0] = a_prev
 
-        # This has to be done sequentially...
-        for i in range(ntime):
-            adjoint_block[i + 1] = adjoint_block[i] - torch.bmm(
-                J[i + 1].transpose(-1, -2), adjoint_block[i].unsqueeze(-1)
-            ).squeeze(-1) * dt[i].unsqueeze(-1)
-            adjoint_block[i + 1] += grads[i + 1]
+        # Basic operators
+        I = torch.eye(prob_size, device=dt.device).expand(ntime, batch_size, -1, -1)
+        dJ = J[1:].transpose(-1, -2) * dt.unsqueeze(-1).unsqueeze(-1)
+
+        # The operator is pretty trivial
+        op = solver(I, (dJ - I)[1:])
+        rhs = grads[1:].unsqueeze(-1) + mbmm(
+            dJ,
+            -a_prev.unsqueeze(0).expand(ntime, batch_size, -1).unsqueeze(-1),
+        )
 
-        return adjoint_block
+        # Actually do the batch solve
+        adjoint_block[1:] = op.matvec(rhs).squeeze(-1)
+        return adjoint_block + a_prev
 
     def accumulate(self, prev, time, y, a, grad, grad_fn):
         """
         Calculate the accumulated value given the results at each time step
 
         Args:
             prev (tuple of tensors): previous results
@@ -428,14 +442,15 @@
             )
 
             full_adjoint = self.scheme.update_adjoint(
                 self.t[k - 1 : k + self.n].diff(dim=0),
                 J,
                 prev_adjoint,
                 output_grad[k - 1 : k + self.n],
+                solver=self.direct_solver,
             )
 
             # Ugh, best way I can think to do this is to combine everything...
             grad_result = self.scheme.accumulate(
                 grad_result,
                 self.t[k - 1 : k + self.n],
                 self.result[k - 1 : k + self.n],
```

### Comparing `pyoptmat-1.3.1/pyoptmat/optimize.py` & `pyoptmat-1.3.2/pyoptmat/optimize.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/scaling.py` & `pyoptmat-1.3.2/pyoptmat/scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/solvers.py` & `pyoptmat-1.3.2/pyoptmat/solvers.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/temperature.py` & `pyoptmat-1.3.2/pyoptmat/temperature.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat/utility.py` & `pyoptmat-1.3.2/pyoptmat/utility.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/pyoptmat.egg-info/PKG-INFO` & `pyoptmat-1.3.2/pyoptmat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptmat
-Version: 1.3.1
+Version: 1.3.2
 Summary: Statistical inference for material models
 Home-page: https://github.com/Argonne-National-Laboratory/pyoptmat
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
 License: UNKNOWN
 Keywords: materials inference modeling
 Platform: UNKNOWN
```

### Comparing `pyoptmat-1.3.1/pyoptmat.egg-info/SOURCES.txt` & `pyoptmat-1.3.2/pyoptmat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/setup.py` & `pyoptmat-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(os.path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
   long_description = f.read()
 
 setup (
     # Name of the project
     name = 'pyoptmat',
     # Version
-    version = '1.3.1',
+    version = '1.3.2',
     # One line-description
     description = "Statistical inference for material models",
     # README
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     # Project webpage
     url='https://github.com/Argonne-National-Laboratory/pyoptmat',
```

### Comparing `pyoptmat-1.3.1/test/test_adjoint_gradients.py` & `pyoptmat-1.3.2/test/test_adjoint_gradients.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_batch_gradient.py` & `pyoptmat-1.3.2/test/test_batch_gradient.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_chunktime.py` & `pyoptmat-1.3.2/test/test_chunktime.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_damage.py` & `pyoptmat-1.3.2/test/test_damage.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_flowrules.py` & `pyoptmat-1.3.2/test/test_flowrules.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_hardening.py` & `pyoptmat-1.3.2/test/test_hardening.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_model_gradient.py` & `pyoptmat-1.3.2/test/test_model_gradient.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_models.py` & `pyoptmat-1.3.2/test/test_models.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_ode.py` & `pyoptmat-1.3.2/test/test_ode.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_scaling.py` & `pyoptmat-1.3.2/test/test_scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_solvers.py` & `pyoptmat-1.3.2/test/test_solvers.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_temperature_scaling.py` & `pyoptmat-1.3.2/test/test_temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.1/test/test_utility.py` & `pyoptmat-1.3.2/test/test_utility.py`

 * *Files identical despite different names*

