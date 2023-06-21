# Comparing `tmp/mec_jun2023-1.0.tar.gz` & `tmp/mec_jun2023-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mec_jun2023-1.0.tar", last modified: Wed Jun 21 09:42:17 2023, max compression
+gzip compressed data, was "mec_jun2023-1.0.1.tar", last modified: Wed Jun 21 12:01:05 2023, max compression
```

## Comparing `mec_jun2023-1.0.tar` & `mec_jun2023-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 09:42:17.407675 mec_jun2023-1.0/
--rw-r--r--   0 antoine    (501) staff       (20)    35138 2023-06-21 09:21:00.000000 mec_jun2023-1.0/LICENSE
--rw-r--r--   0 antoine    (501) staff       (20)      233 2023-06-21 09:42:17.407566 mec_jun2023-1.0/PKG-INFO
-drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 09:42:17.407407 mec_jun2023-1.0/mec_jun2023.egg-info/
--rw-r--r--   0 antoine    (501) staff       (20)      233 2023-06-21 09:42:17.000000 mec_jun2023-1.0/mec_jun2023.egg-info/PKG-INFO
--rw-r--r--   0 antoine    (501) staff       (20)      168 2023-06-21 09:42:17.000000 mec_jun2023-1.0/mec_jun2023.egg-info/SOURCES.txt
--rw-r--r--   0 antoine    (501) staff       (20)        1 2023-06-21 09:42:17.000000 mec_jun2023-1.0/mec_jun2023.egg-info/dependency_links.txt
--rw-r--r--   0 antoine    (501) staff       (20)        9 2023-06-21 09:42:17.000000 mec_jun2023-1.0/mec_jun2023.egg-info/top_level.txt
--rw-r--r--   0 antoine    (501) staff       (20)     7015 2023-06-21 09:26:44.000000 mec_jun2023-1.0/pymec_lp.py
--rw-r--r--   0 antoine    (501) staff       (20)       38 2023-06-21 09:42:17.407709 mec_jun2023-1.0/setup.cfg
--rw-r--r--   0 antoine    (501) staff       (20)      302 2023-06-21 09:41:59.000000 mec_jun2023-1.0/setup.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:01:05.786771 mec_jun2023-1.0.1/
+-rw-r--r--   0 antoine    (501) staff       (20)    35138 2023-06-21 09:21:00.000000 mec_jun2023-1.0.1/LICENSE
+-rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:01:05.786652 mec_jun2023-1.0.1/PKG-INFO
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-06-21 12:01:05.786450 mec_jun2023-1.0.1/mec_jun2023.egg-info/
+-rw-r--r--   0 antoine    (501) staff       (20)      188 2023-06-21 12:01:05.000000 mec_jun2023-1.0.1/mec_jun2023.egg-info/PKG-INFO
+-rw-r--r--   0 antoine    (501) staff       (20)      168 2023-06-21 12:01:05.000000 mec_jun2023-1.0.1/mec_jun2023.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        1 2023-06-21 12:01:05.000000 mec_jun2023-1.0.1/mec_jun2023.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        9 2023-06-21 12:01:05.000000 mec_jun2023-1.0.1/mec_jun2023.egg-info/top_level.txt
+-rw-r--r--   0 antoine    (501) staff       (20)     7664 2023-06-21 12:00:09.000000 mec_jun2023-1.0.1/pymec_lp.py
+-rw-r--r--   0 antoine    (501) staff       (20)       38 2023-06-21 12:01:05.786821 mec_jun2023-1.0.1/setup.cfg
+-rw-r--r--   0 antoine    (501) staff       (20)      340 2023-06-21 12:00:29.000000 mec_jun2023-1.0.1/setup.py
```

### Comparing `mec_jun2023-1.0/LICENSE` & `mec_jun2023-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mec_jun2023-1.0/pymec_lp.py` & `mec_jun2023-1.0.1/pymec_lp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,20 @@
 import pandas as pd
 import numpy as np
 import scipy.sparse as spr
-import gurobipy as grb
+#import gurobipy as grb
 import sympy
 from sympy.solvers import solve
 from sympy import *
 import matplotlib.pyplot as plt
 
-def round_expr(expr, num_digits):
-    return expr.xreplace({n : round(n, num_digits) for n in expr.atoms(Number)})
-    
-    
-def plot_path_so_far(the_path):
-    x1, x2 = np.meshgrid(np.linspace(-0.2, 1.4, 400), np.linspace(-0.2, 1.4, 400))
-    feasible_region = (2 * x1 + x2 <= 2) & (x1 + 2 * x2 <= 2) & (x1 >= 0) & (x2 >= 0)
-    fig, ax = plt.subplots(figsize=(5, 5))
-    plt.contourf(x1, x2, np.where(feasible_region, x1+x2, np.nan), 50, alpha = 0.5, cmap='gray_r', levels=30)
-    plt.text(0.4, 0.4, 'Feasible solutions', color = 'white', ha='center', va='center')
-    ax.plot(x1[0, :], 2 - 2*x1[0, :], label='z1 = 0')
-    ax.plot(2 - 2*x2[:, 0], x2[:, 0], label='z2 = 0')
-    ax.plot([a for (a,_) in the_path], [b for (_,b) in the_path], 'r--', label='Algorithm path')
-    ax.scatter([a for (a,_) in the_path], [b for (_,b) in the_path], color='red')
-    for i, bfs in enumerate(the_path):
-        plt.text(bfs[0], bfs[1], 'BFS'+str(i), color = 'red', ha='left', va='bottom')
-    ax.set_xlim(-0.2, 1.4), ax.set_ylim(-0.2, 1.4)
-    ax.set_xlabel('x1'), ax.set_ylabel('x2')
-    ax.spines[['left', 'bottom']].set_position('zero')
-    ax.spines[['right', 'top']].set_color('none')
-    ax.legend()
-    plt.show()
-
 
-# LP1: Intro to linear programming
+#############################
+# LP1: Intro to linear programming #
+#############################
 
 def load_stigler_data(verbose=False):
     import pandas as pd
     thepath = 'https://raw.githubusercontent.com/math-econ-code/mec_optim_2021-01/master/data_mec_optim/lp_stigler-diet/'
     filename = 'StiglerData1939.txt'
     thedata = pd.read_csv(thepath + filename, sep='\t')
     thedata = thedata.dropna(how = 'all')
@@ -49,16 +28,41 @@
     return({'N_i_j':thedata.iloc[:-1, 4:].fillna(0).transpose().values,
            'd_i':np.array(allowance),
            'c_j':np.ones(len(commodities)),
             'nbi':len(allowance),
             'nbj':len(commodities),
             'names_j':commodities})
 
+def print_optimal_diet(q_j):
+    print('***Optimal solution***')
+    total,thelist = 0.0, []
+    for j,commodity in enumerate(commodities):
+        if q_j[j] > 0:
+            total += q_j[j] * 365
+            thelist.append([commodity,q_j[j]])
+    thelist.append(['Total cost (optimal):', total])
+    print(tabulate(thelist))
+
+
+#########################
+# LP2: The simplex algorithm #
+#########################
+
+def round_expr(expr, num_digits):
+    ---
+    description of the function
+    arg:
+       expr: meaning
+       num_digits: meaning
+    return:
+       expr.xreplace: meaning & type
+    ---
+    return expr.xreplace({n : round(n, num_digits) for n in expr.atoms(Number)})
+
 
-# LP2: The simplex algorithm
 
 class Tableau():
     def __init__(self, names_basic, names_nonbasic, A_i_j, b_i, c_j): # z = d - A @ x
         self.nonbasic = list(symbols(names_nonbasic))
         self.base = { Symbol('obj') : c_j @ self.nonbasic }
         self.base.update( { list(symbols(names_basic))[i]: b_i[i]  - (A_i_j @ self.nonbasic)[i] for i in range(len(b_i))} )
 
@@ -92,29 +96,28 @@
             if the_expr_list: # if one can invert the previous expression
                 the_expr = the_expr_list[0] # express entering variable as a function of the other ones:
                 val_entering_var = the_expr.subs([ (variable,0) for variable in [var]+self.nonbasic])
                 if (val_entering_var >= 0) & (val_entering_var < runmin) :
                   runmin,departing_var = val_entering_var, var
         return departing_var # if no variable is found, None returned
         
-    def pivot(self,entering_var,departing_var, verbose = 0):
-        expr_entering = solve(self.base[departing_var] - departing_var,entering_var)[0]
+    def pivot(self, entering_var, departing_var, verbose = 0):
+        expr_entering = solve(self.base[departing_var] - departing_var, entering_var)[0]
         for var in self.base:
             self.base[var] = self.base[var].subs([(entering_var, expr_entering)])
         self.base[entering_var] = expr_entering
         del self.base[departing_var]
         self.nonbasic.remove(entering_var)
         self.nonbasic.append(departing_var)
         if verbose > 0:
             print('Entering = ' + str( entering_var)+'; departing = '+ str( departing_var))
         if verbose > 1:
             print(str( entering_var)+' = '+str(round_expr(expr_entering,2)))
         return expr_entering
-        
-        
+
     def simplex_loop(dual_tableau,primal_tableau,primals):
         entering_var = dual_tableau.determine_entering()
         if entering_var is None:
             print('Optimal solution found.\n=======================')
             primal_tableau.print_solution('Basic primal variables:')
             dual_tableau.print_solution('Basic dual variables:')
         else:
@@ -122,25 +125,47 @@
             if departing_var is None:
                 print('Unbounded solution.')
             else:
                 expr_entering_var = dual_tableau.pivot(entering_var,departing_var, verbose= 1)
                 _ = primal_tableau.pivot(primals[departing_var],primals[entering_var])
                 return False # not finished
         return True # finished
+
+def plot_path_so_far(the_path):
+    x1, x2 = np.meshgrid(np.linspace(-0.2, 1.4, 400), np.linspace(-0.2, 1.4, 400))
+    feasible_region = (2 * x1 + x2 <= 2) & (x1 + 2 * x2 <= 2) & (x1 >= 0) & (x2 >= 0)
+    fig, ax = plt.subplots(figsize=(5, 5))
+    plt.contourf(x1, x2, np.where(feasible_region, x1+x2, np.nan), 50, alpha = 0.5, cmap='gray_r', levels=30)
+    plt.text(0.4, 0.4, 'Feasible solutions', color = 'white', ha='center', va='center')
+    ax.plot(x1[0, :], 2 - 2*x1[0, :], label='z1 = 0')
+    ax.plot(2 - 2*x2[:, 0], x2[:, 0], label='z2 = 0')
+    ax.plot([a for (a,_) in the_path], [b for (_,b) in the_path], 'r--', label='Algorithm path')
+    ax.scatter([a for (a,_) in the_path], [b for (_,b) in the_path], color='red')
+    for i, bfs in enumerate(the_path):
+        plt.text(bfs[0], bfs[1], 'BFS'+str(i), color = 'red', ha='left', va='bottom')
+    ax.set_xlim(-0.2, 1.4), ax.set_ylim(-0.2, 1.4)
+    ax.set_xlabel('x1'), ax.set_ylabel('x2')
+    ax.spines[['left', 'bottom']].set_position('zero')
+    ax.spines[['right', 'top']].set_color('none')
+    ax.legend()
+    plt.show()
         
-        
+
+#########################
+# LP3: Interior Point Methods #
+#########################
+
 class InteriorPoint():
     def __init__(self,A,b,c,current_point=None):
         self.A = A
         self.b = b
         self.c = c
         self.current_point = current_point
         self.α = 1 - (1/8)/(1/5 + np.sqrt(len(c))) # shrinkage coeff α given by Freund & Vera
 
-    
     def update(self, verbose=0):
         x, y, s, θ = self.current_point
         Δy = np.linalg.solve(self.A @ np.diag(1/s) @ np.diag(x) @ self.A.T, θ * self.A @ (1/s) - self.b)
         Δs = self.A.T @ Δy
         Δx = - x - np.diag(1/s) @ np.diag(x) @ Δs + θ * (1/s)
         self.current_point = [x+Δx, y+Δy, s+Δs, self.α*θ]
         return self.current_point
```

