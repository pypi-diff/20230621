# Comparing `tmp/JaxSSO-0.0.5.tar.gz` & `tmp/JaxSSO-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JaxSSO-0.0.5.tar", last modified: Tue Apr  4 14:34:59 2023, max compression
+gzip compressed data, was "JaxSSO-0.0.6.tar", last modified: Wed Jun 21 14:05:02 2023, max compression
```

## Comparing `JaxSSO-0.0.5.tar` & `JaxSSO-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 14:34:59.688914 JaxSSO-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-04-04 14:34:59.664903 JaxSSO-0.0.5/JaxSSO/
--rw-rw-rw-   0        0        0    11838 2023-02-19 15:37:12.000000 JaxSSO-0.0.5/JaxSSO/BeamCol.py
--rw-rw-rw-   0        0        0    16130 2023-04-04 14:17:50.000000 JaxSSO-0.0.5/JaxSSO/Model_Sens.py
--rw-rw-rw-   0        0        0      645 2022-10-19 17:46:55.000000 JaxSSO-0.0.5/JaxSSO/Node.py
--rw-rw-rw-   0        0        0    12593 2023-04-04 14:23:31.000000 JaxSSO-0.0.5/JaxSSO/Optimization.py
--rw-rw-rw-   0        0        0       82 2022-11-22 19:43:25.000000 JaxSSO-0.0.5/JaxSSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 14:34:59.686902 JaxSSO-0.0.5/JaxSSO.egg-info/
--rw-rw-rw-   0        0        0     6876 2023-04-04 14:34:59.000000 JaxSSO-0.0.5/JaxSSO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-04 14:34:59.000000 JaxSSO-0.0.5/JaxSSO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 14:34:59.000000 JaxSSO-0.0.5/JaxSSO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-04 14:34:59.000000 JaxSSO-0.0.5/JaxSSO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-04 14:34:59.000000 JaxSSO-0.0.5/JaxSSO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6876 2023-04-04 14:34:59.688914 JaxSSO-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5506 2022-12-21 21:17:44.000000 JaxSSO-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 14:34:59.688914 JaxSSO-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-04-04 14:28:05.000000 JaxSSO-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:05:02.440747 JaxSSO-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:05:02.391703 JaxSSO-0.0.6/JaxSSO/
+-rw-rw-rw-   0        0        0     7959 2023-05-05 21:13:08.000000 JaxSSO-0.0.6/JaxSSO/BeamCol.py
+-rw-rw-rw-   0        0        0    14160 2023-05-09 02:29:25.000000 JaxSSO-0.0.6/JaxSSO/Model.py
+-rw-rw-rw-   0        0        0      644 2023-05-03 21:33:47.000000 JaxSSO-0.0.6/JaxSSO/Node.py
+-rw-rw-rw-   0        0        0    13011 2023-05-03 14:24:39.000000 JaxSSO-0.0.6/JaxSSO/Optimization.py
+-rw-rw-rw-   0        0        0     3586 2023-05-09 02:29:16.000000 JaxSSO-0.0.6/JaxSSO/SSO_Model.py
+-rw-rw-rw-   0        0        0      141 2023-05-05 15:02:50.000000 JaxSSO-0.0.6/JaxSSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:05:02.434191 JaxSSO-0.0.6/JaxSSO.egg-info/
+-rw-rw-rw-   0        0        0     6916 2023-06-21 14:05:02.000000 JaxSSO-0.0.6/JaxSSO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-21 14:05:02.000000 JaxSSO-0.0.6/JaxSSO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 14:05:02.000000 JaxSSO-0.0.6/JaxSSO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-21 14:05:02.000000 JaxSSO-0.0.6/JaxSSO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-21 14:05:02.000000 JaxSSO-0.0.6/JaxSSO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6916 2023-06-21 14:05:02.439743 JaxSSO-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5538 2023-04-04 14:47:29.000000 JaxSSO-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 14:05:02.440747 JaxSSO-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1245 2023-06-21 14:04:31.000000 JaxSSO-0.0.6/setup.py
```

### Comparing `JaxSSO-0.0.5/JaxSSO/Node.py` & `JaxSSO-0.0.6/JaxSSO/Node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 References
 ---------
 1. PyNite: An open-source FEA solver for python; https://github.com/JWock82/PyNite
 2. Bathe, K. J. (2006). Finite element procedures. Klaus-Jurgen Bathe.
 """      
+
+
 class Node():
     """
     Create a JaxSSO node.
 
     Input
     -----
     nodeTag: int 
@@ -18,8 +20,9 @@
     """
     
     def __init__(self, nodeTag, X, Y, Z):
         self.nodeTag = nodeTag      # Index of this node
         self.X = X            # Global X coordinate
         self.Y = Y            # Global Y coordinate
         self.Z = Z            # Global Z coordinate
-        
+    
+
```

### Comparing `JaxSSO-0.0.5/JaxSSO/Optimization.py` & `JaxSSO-0.0.6/JaxSSO/Optimization.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,418 +1,418 @@
-"""
-A optimization module for JAX-SSO.
-Available optimizers:
-    1. Vanilla gradient descent for unconstrained problems
-    2. SLSQP for constrained problems from Nlopt (Install Nlopt: pip install nlopt) [https://nlopt.readthedocs.io/en/latest/NLopt_Python_Reference]
-"""
-
-
-import numpy as np
-import nlopt
-
-class Optimization():
-    """
-    A class for optimization
-    """
-
-    def __init__(self,n_x,method='GD'):
-        """
-        Initialize an Optimization() object.
-        
-        Parameters:
-            method: str
-                'GD': vanilla gradient descent, default
-                'SLSQP': sequential least-squares quadratic programming:
-                    Reference:Dieter Kraft, "A software package for sequential quadratic programming", Technical Report DFVLR-FB 88-28, Institut für Dynamik der Flugsysteme, Oberpfaffenhofen, July 1988.
-               
-            n_x: int
-                number of parameters to optimize        
-        """
-        
-        self.method = method      # Optimizer
-        self.n_x = n_x   # Number of parameters
-
-        self.if_eq_c = False # if there is equality constraint
-        self.if_ineq_c = False #if there is inequality constraint
-        self.if_bounds = False #if there are bounds for parameters
-        self.if_maxiter = False # if there is stop criteria: Number of maximum function evaluation
-        self.if_ftol_rel = False # if there is stop criteria: Relative tolerance
-        self.if_ftol_abs = False # if there is stop criteria: Absolute tolerance
-        self.GD_norm = False #if the gradients are normalized
-
-    def set_objective(self,fun):
-        """
-        The objective function to minimize, and its gradient
-
-        Parameters:
-        -----
-        fun: callable 
-            fun(x, *args) -> tuple, (fun_value,grad_fun)
-                fun_value: float
-                    the objective value
-        
-                grad_fun: ndarry of shape (n_x,)
-                    the gradient of the objective
-
-        """   
-        self.fun = fun #the objective function
-
-    def set_maxiter(self,maxiter):
-        """
-        Set the maximum number of iterations
-
-        Parameters:
-        -----
-        maxiter: int 
-        """
-        self.if_maxiter = True
-        self.maxiter = maxiter #set maxiter
-
-    def set_step_size(self,ln_rate):
-        """
-        Set the step size for gradient descent
-
-        Parameters:
-        -----
-        ln_rate: float
-        """
-        
-        if self.method == 'GD':
-            self.ln_rate = ln_rate
-
-    def set_GD_normalized(self,normalized=False):
-        """
-        If set to 'True', the gradient will be normalized by the max(abs) of the gradient.
-
-        Parameters:
-        -----
-        ln_rate: float
-        """
-        
-        if normalized:
-            self.GD_norm = True
-        else:
-            self.GD_norm = False
-    
-    def set_ftol_rel(self,ftol_rel):
-        """
-        Stop criteria: relative function value
-
-        Parameters:
-        -----
-        ftol_rel: float
-        """
-        self.if_ftol_rel = True
-        self.ftol_rel = ftol_rel
-
-    def set_ftol_abs(self,ftol_abs):
-        """
-        Stop criteria: relative function value
-
-        Parameters:
-        -----
-        ftol_abs: float
-        """
-        self.if_ftol_abs = True
-        self.ftol_abs = ftol_abs
-
-    def set_bounds(self,x_lb,x_ub):
-        """
-        Setting bounds for parameters
-
-        Parameters:
-        -----
-        x_lb: ndarray
-            lower bounds
-        
-        x_ub: ndarray
-            upper bounds
-        """
-        if self.method == 'GD':
-            raise TypeError(" Gradient descent cannot deal with bounds, change \'method\'")
-        else:
-            self.if_bounds = True
-            self.lb = x_lb
-            self.ub = x_ub
-
-
-    def set_inequality_constraints(self,fc,grad_fc,d_fc,tol=0):
-        """
-        Setting inequality constraints
-
-        Parameters:
-        -----
-        fc: callable 
-            fc(x, *args) -> float/ndarray of shape (d_fc,); function for constraints; fc(x) <= 0
-
-        grad_fc: callable 
-            grad_fc(x, *args) -> ndarray of shape (d_fc,n_x); gradients of constraints
-        
-        d_fc: int
-            shape of the return of fc(x, *args); dimension of the constraints
-
-        tol:float/ndarray of shape (d_fc,)
-            tolerence for constraints; default is zero
-
-        """
-        if self.method == 'GD':
-            raise TypeError(" Gradient descent cannot deal with constraints, change \'method\'")
-        
-        else:
-            self.if_ineq_c = True
-            self.ineq_fc = fc
-            self.ineq_grad_fc = grad_fc
-            self.d_ineq_c = d_fc
-            if self.d_ineq_c > 1:
-                if np.size(tol) == 1:
-                    self.ineq_tol = tol * np.ones(self.d_ineq_c) 
-                else:
-                    self.ineq_tol = tol
-            elif self.d_ineq_c == 1:
-                self.ineq_tol = tol
-
-    def set_equality_constraints(self,fc,grad_fc,d_fc,tol=0):
-        """
-        Setting equality constraints
-
-        Parameters:
-        -----
-        fc: callable 
-            fc(x, *args) -> float/ndarray of shape (d_fc,); function for constraints; fc(x) = 0
-
-        grad_fc: callable 
-            grad_fc(x, *args) -> ndarray of shape (d_fc,n_x); gradients of constraints
-        
-        d_fc: int
-            shape of the return of fc(x, *args); dimension of the constraints
-
-        tol:float/ndarray of shape (d_fc,)
-            tolerence for constraints; default is zero
-
-        """
-        if method == 'GD':
-            raise TypeError(" Gradient descent cannot deal with constraints, change \'method\'")
-        else:
-            self.if_eq_c = True 
-            self.eq_fc = fc
-            self.eq_grad_fc = grad_fc
-            self.d_eq_c = d_fc
-            if self.d_eq_c > 1:
-                if np.size(tol) == 1:
-                    self.eq_tol = tol * np.ones(self.d_eq_c) 
-                else:
-                    self.eq_tol = tol
-            elif self.d_eq_c == 1:
-                self.eq_tol = tol
-
-    def Nlopt_objective(self):
-        '''
-        The objective function for Nlopt package.
-        
-        --------------------
-        Form required by Nlopt
-        --------------------
-        def f(x, grad):
-            if grad.size > 0:
-               ...set grad to gradient, in-place...
-               return ...value of f(x)...
-        --------------------
-        '''
-
-        def f(x,grad):
-            res_1,res_2 = self.fun(x)
-            if grad.size>0:
-                grad[:] = res_2
-
-            return res_1
-
-
-        return f
-
-    def Nlopt_eq_constraints(self):
-        '''
-        The equality constraints for Nlopt package. Single-valued.
-        
-        --------------------
-        Form required by Nlopt
-        --------------------
-        def f(x, grad):
-            if grad.size > 0:
-               ...set grad to gradient, in-place...
-               return ...value of f(x)...
-        --------------------
-        '''
-
-        #function for Nlopt
-        def f(x,grad):
-            if grad.size>0:
-                grad[:] = self.eq_grad_fc(x)
-            return self.eq_fc(x)
-
-        return f
-
-    def Nlopt_eq_mconstraints(self):
-        '''
-        The equality constraints for Nlopt package. Vector-valued.
-        
-        --------------------
-        Form required by Nlopt
-        --------------------
-        def f(x, grad):
-            if grad.size > 0:
-               ...set grad to gradient, in-place...
-               return ...value of f(x)...
-        --------------------
-        '''
-
-        #function for Nlopt
-        def c(result,x,grad):
-            if grad.size>0:
-                grad[:] = self.eq_grad_fc(x)
-                result[:] = self.eq_fc(x)
-            
-
-        return c
-
-    def Nlopt_in_constraints(self):
-        '''
-        The inequality constraints for Nlopt package.Single value.
-        
-        --------------------
-        Form required by Nlopt
-        --------------------
-        def f(x, grad):
-            if grad.size > 0:
-               ...set grad to gradient, in-place...
-               return ...value of f(x)...
-        --------------------
-        '''
-
-        #function for Nlopt
-        def f(x,grad):
-            if grad.size>0:
-                grad[:] = self.ineq_grad_fc(x)
-            return self.ineq_fc(x)
-
-        return f
-
-    def Nlopt_in_mconstraints(self):
-        '''
-        The inequality constraints for Nlopt package. Vector-valued.
-        
-        --------------------
-        Form required by Nlopt
-        --------------------
-        def f(x, grad):
-            if grad.size > 0:
-               ...set grad to gradient, in-place...
-               return ...value of f(x)...
-        --------------------
-        '''
-
-        #function for Nlopt
-        def c(result,x,grad):
-            if grad.size>0:
-                grad[:] = self.ineq_grad_fc(x)
-                result[:] = self.ineq_fc(x)
-            
-
-        return c
-
-    #Conduct optimization
-    def optimize(self,x_ini,log=True):
-        '''
-        Conduct optimization, given initial guess.
-        
-        Parameters:
-        -----
-        x_ini: ndarray
-            initial guess of optimization parameters, shape of (n_x,)
-
-        log: bool
-            print log at each functional call
-
-        Return:
-        -----
-        x_fin: ndarray
-            optimized parameters
-        --------------------
-        '''
-
-        #Vanilla gradient descent with/without normalized gradients
-        if self.method == 'GD':
-            i = 0 #initial iteration number
-            current_x = x_ini #initial parameters
-            f_store = [] # store the functional value
-            while i < self.maxiter:
-                obj,grad_obj = self.fun(current_x) #functional value and its gradient
-                f_store.append (obj) #store the functional value
-                normalized_grad = grad_obj #original gradient
-                if self.GD_norm == True:
-                    normalized_grad = normalized_grad/np.max(np.abs(normalized_grad)) #normalize the gradients
-                if i>=1:
-                    if self.if_ftol_rel==True:
-                        if abs((f_store[i-1] - f_store[i])/f_store[i-1]) <= self.ftol_rel:
-                            print('Stopping criteria \'ftol_rel\' met, end of optimization')
-                            
-                            break
-                    if self.if_ftol_abs==True:
-                        if abs(f_store[i-1] - f_store[i]) <= self.ftol_abs:
-                            print('Stopping criteria \'ftol_abs\' met, end of optimization')
-                            break
-
-                
-                current_x = current_x - self.ln_rate * normalized_grad #update parameters
-                if log ==True:
-                    print('Step {}, objective = {}'.format(i,f_store[i]))
-                i += 1 #update iteration number
-
-            x_fin = current_x #store the final value
-            
-            if i==self.maxiter:
-                print('Stopping criteria \'maxiter\' met, end of optimization')
-
-        #SLSQP, a SQP method
-        elif self.method == 'SLSQP':
-            opt = nlopt.opt(nlopt.LD_SLSQP,self.n_x) # opt objects
-
-            #The objective function
-
-            opt.set_min_objective(self.Nlopt_objective()) #objective function
-            
-            #bounds
-            if self.if_bounds == True:
-                opt.set_lower_bounds(self.lb)
-                opt.set_upper_bounds(self.ub)
-
-            #equality constraints
-            if self.if_eq_c == True:
-                if self.d_eq_c == 0:
-                    opt.add_equality_constraint(self.Nlopt_eq_constraints(),self.eq_tol)
-                else:
-                    opt.add_equality_mconstraint(self.Nlopt_eq_mconstraints(),self.eq_tol)
-
-            #inequality constraints
-            if self.if_ineq_c == True:
-                if self.d_ineq_c == 0:
-                    opt.add_inequality_constraint(self.Nlopt_in_constraints(),self.ineq_tol)
-                else:
-                    opt.add_inequality_mconstraint(self.Nlopt_in_mconstraints(),self.ineq_tol)
-
-            #stopping criteria
-            if self.if_maxiter:
-                opt.set_maxeval(self.maxiter)
-            if self.if_ftol_abs:
-                opt.set_ftol_abs(self.set_ftol_abs) 
-            if self.if_ftol_rel:
-                opt.set_ftol_rel(self.set_ftol_rel)
-
-            #perform optimization
-            x_fin = opt.optimize(x_ini)
-
-        return x_fin
-
-                
-
-
-
-
+"""
+A optimization module for JAX-SSO.
+Available optimizers:
+    1. Vanilla gradient descent for unconstrained problems
+    2. SLSQP for constrained problems from Nlopt (Install Nlopt: pip install nlopt) [https://nlopt.readthedocs.io/en/latest/NLopt_Python_Reference]
+"""
+
+
+import numpy as np
+import nlopt
+
+class Optimization():
+    """
+    A class for optimization
+    """
+
+    def __init__(self,n_x,method='GD'):
+        """
+        Initialize an Optimization() object.
+        
+        Parameters:
+            method: str
+                'GD': vanilla gradient descent, default
+                'SLSQP': sequential least-squares quadratic programming:
+                    Reference:Dieter Kraft, "A software package for sequential quadratic programming", Technical Report DFVLR-FB 88-28, Institut für Dynamik der Flugsysteme, Oberpfaffenhofen, July 1988.
+               
+            n_x: int
+                number of parameters to optimize        
+        """
+        
+        self.method = method      # Optimizer
+        self.n_x = n_x   # Number of parameters
+
+        self.if_eq_c = False # if there is equality constraint
+        self.if_ineq_c = False #if there is inequality constraint
+        self.if_bounds = False #if there are bounds for parameters
+        self.if_maxiter = False # if there is stop criteria: Number of maximum function evaluation
+        self.if_ftol_rel = False # if there is stop criteria: Relative tolerance
+        self.if_ftol_abs = False # if there is stop criteria: Absolute tolerance
+        self.GD_norm = False #if the gradients are normalized
+
+    def set_objective(self,fun):
+        """
+        The objective function to minimize, and its gradient
+
+        Parameters:
+        -----
+        fun: callable 
+            fun(x, *args) -> tuple, (fun_value,grad_fun)
+                fun_value: float
+                    the objective value
+        
+                grad_fun: ndarry of shape (n_x,)
+                    the gradient of the objective
+
+        """   
+        self.fun = fun #the objective function
+
+    def set_maxiter(self,maxiter):
+        """
+        Set the maximum number of iterations
+
+        Parameters:
+        -----
+        maxiter: int 
+        """
+        self.if_maxiter = True
+        self.maxiter = maxiter #set maxiter
+
+    def set_step_size(self,ln_rate):
+        """
+        Set the step size for gradient descent
+
+        Parameters:
+        -----
+        ln_rate: float
+        """
+        
+        if self.method == 'GD':
+            self.ln_rate = ln_rate
+
+    def set_GD_normalized(self,normalized=False):
+        """
+        If set to 'True', the gradient will be normalized by the max(abs) of the gradient.
+
+        Parameters:
+        -----
+        ln_rate: float
+        """
+        
+        if normalized:
+            self.GD_norm = True
+        else:
+            self.GD_norm = False
+    
+    def set_ftol_rel(self,ftol_rel):
+        """
+        Stop criteria: relative function value
+
+        Parameters:
+        -----
+        ftol_rel: float
+        """
+        self.if_ftol_rel = True
+        self.ftol_rel = ftol_rel
+
+    def set_ftol_abs(self,ftol_abs):
+        """
+        Stop criteria: relative function value
+
+        Parameters:
+        -----
+        ftol_abs: float
+        """
+        self.if_ftol_abs = True
+        self.ftol_abs = ftol_abs
+
+    def set_bounds(self,x_lb,x_ub):
+        """
+        Setting bounds for parameters
+
+        Parameters:
+        -----
+        x_lb: ndarray
+            lower bounds
+        
+        x_ub: ndarray
+            upper bounds
+        """
+        if self.method == 'GD':
+            raise TypeError(" Gradient descent cannot deal with bounds, change \'method\'")
+        else:
+            self.if_bounds = True
+            self.lb = x_lb
+            self.ub = x_ub
+
+
+    def set_inequality_constraints(self,fc,grad_fc,d_fc,tol=0):
+        """
+        Setting inequality constraints
+
+        Parameters:
+        -----
+        fc: callable 
+            fc(x, *args) -> float/ndarray of shape (d_fc,); function for constraints; fc(x) <= 0
+
+        grad_fc: callable 
+            grad_fc(x, *args) -> ndarray of shape (d_fc,n_x); gradients of constraints
+        
+        d_fc: int
+            shape of the return of fc(x, *args); dimension of the constraints
+
+        tol:float/ndarray of shape (d_fc,)
+            tolerence for constraints; default is zero
+
+        """
+        if self.method == 'GD':
+            raise TypeError(" Gradient descent cannot deal with constraints, change \'method\'")
+        
+        else:
+            self.if_ineq_c = True
+            self.ineq_fc = fc
+            self.ineq_grad_fc = grad_fc
+            self.d_ineq_c = d_fc
+            if self.d_ineq_c > 1:
+                if np.size(tol) == 1:
+                    self.ineq_tol = tol * np.ones(self.d_ineq_c) 
+                else:
+                    self.ineq_tol = tol
+            elif self.d_ineq_c == 1:
+                self.ineq_tol = tol
+
+    def set_equality_constraints(self,fc,grad_fc,d_fc,tol=0):
+        """
+        Setting equality constraints
+
+        Parameters:
+        -----
+        fc: callable 
+            fc(x, *args) -> float/ndarray of shape (d_fc,); function for constraints; fc(x) = 0
+
+        grad_fc: callable 
+            grad_fc(x, *args) -> ndarray of shape (d_fc,n_x); gradients of constraints
+        
+        d_fc: int
+            shape of the return of fc(x, *args); dimension of the constraints
+
+        tol:float/ndarray of shape (d_fc,)
+            tolerence for constraints; default is zero
+
+        """
+        if method == 'GD':
+            raise TypeError(" Gradient descent cannot deal with constraints, change \'method\'")
+        else:
+            self.if_eq_c = True 
+            self.eq_fc = fc
+            self.eq_grad_fc = grad_fc
+            self.d_eq_c = d_fc
+            if self.d_eq_c > 1:
+                if np.size(tol) == 1:
+                    self.eq_tol = tol * np.ones(self.d_eq_c) 
+                else:
+                    self.eq_tol = tol
+            elif self.d_eq_c == 1:
+                self.eq_tol = tol
+
+    def Nlopt_objective(self):
+        '''
+        The objective function for Nlopt package.
+        
+        --------------------
+        Form required by Nlopt
+        --------------------
+        def f(x, grad):
+            if grad.size > 0:
+               ...set grad to gradient, in-place...
+               return ...value of f(x)...
+        --------------------
+        '''
+
+        def f(x,grad):
+            res_1,res_2 = self.fun(x)
+            if grad.size>0:
+                grad[:] = res_2
+
+            return res_1
+
+
+        return f
+
+    def Nlopt_eq_constraints(self):
+        '''
+        The equality constraints for Nlopt package. Single-valued.
+        
+        --------------------
+        Form required by Nlopt
+        --------------------
+        def f(x, grad):
+            if grad.size > 0:
+               ...set grad to gradient, in-place...
+               return ...value of f(x)...
+        --------------------
+        '''
+
+        #function for Nlopt
+        def f(x,grad):
+            if grad.size>0:
+                grad[:] = self.eq_grad_fc(x)
+            return self.eq_fc(x)
+
+        return f
+
+    def Nlopt_eq_mconstraints(self):
+        '''
+        The equality constraints for Nlopt package. Vector-valued.
+        
+        --------------------
+        Form required by Nlopt
+        --------------------
+        def f(x, grad):
+            if grad.size > 0:
+               ...set grad to gradient, in-place...
+               return ...value of f(x)...
+        --------------------
+        '''
+
+        #function for Nlopt
+        def c(result,x,grad):
+            if grad.size>0:
+                grad[:] = self.eq_grad_fc(x)
+                result[:] = self.eq_fc(x)
+            
+
+        return c
+
+    def Nlopt_in_constraints(self):
+        '''
+        The inequality constraints for Nlopt package.Single value.
+        
+        --------------------
+        Form required by Nlopt
+        --------------------
+        def f(x, grad):
+            if grad.size > 0:
+               ...set grad to gradient, in-place...
+               return ...value of f(x)...
+        --------------------
+        '''
+
+        #function for Nlopt
+        def f(x,grad):
+            if grad.size>0:
+                grad[:] = self.ineq_grad_fc(x)
+            return self.ineq_fc(x)
+
+        return f
+
+    def Nlopt_in_mconstraints(self):
+        '''
+        The inequality constraints for Nlopt package. Vector-valued.
+        
+        --------------------
+        Form required by Nlopt
+        --------------------
+        def f(x, grad):
+            if grad.size > 0:
+               ...set grad to gradient, in-place...
+               return ...value of f(x)...
+        --------------------
+        '''
+
+        #function for Nlopt
+        def c(result,x,grad):
+            if grad.size>0:
+                grad[:] = self.ineq_grad_fc(x)
+                result[:] = self.ineq_fc(x)
+            
+
+        return c
+
+    #Conduct optimization
+    def optimize(self,x_ini,log=True):
+        '''
+        Conduct optimization, given initial guess.
+        
+        Parameters:
+        -----
+        x_ini: ndarray
+            initial guess of optimization parameters, shape of (n_x,)
+
+        log: bool
+            print log at each functional call
+
+        Return:
+        -----
+        x_fin: ndarray
+            optimized parameters
+        --------------------
+        '''
+
+        #Vanilla gradient descent with/without normalized gradients
+        if self.method == 'GD':
+            i = 0 #initial iteration number
+            current_x = x_ini #initial parameters
+            f_store = [] # store the functional value
+            while i < self.maxiter:
+                obj,grad_obj = self.fun(current_x) #functional value and its gradient
+                f_store.append (obj) #store the functional value
+                normalized_grad = grad_obj #original gradient
+                if self.GD_norm == True:
+                    normalized_grad = normalized_grad/np.max(np.abs(normalized_grad)) #normalize the gradients
+                if i>=1:
+                    if self.if_ftol_rel==True:
+                        if abs((f_store[i-1] - f_store[i])/f_store[i-1]) <= self.ftol_rel:
+                            print('Stopping criteria \'ftol_rel\' met, end of optimization')
+                            
+                            break
+                    if self.if_ftol_abs==True:
+                        if abs(f_store[i-1] - f_store[i]) <= self.ftol_abs:
+                            print('Stopping criteria \'ftol_abs\' met, end of optimization')
+                            break
+
+                
+                current_x = current_x - self.ln_rate * normalized_grad #update parameters
+                if log ==True:
+                    print('Step {}, objective = {}'.format(i,f_store[i]))
+                i += 1 #update iteration number
+
+            x_fin = current_x #store the final value
+            
+            if i==self.maxiter:
+                print('Stopping criteria \'maxiter\' met, end of optimization')
+
+        #SLSQP, a SQP method
+        elif self.method == 'SLSQP':
+            opt = nlopt.opt(nlopt.LD_SLSQP,self.n_x) # opt objects
+
+            #The objective function
+
+            opt.set_min_objective(self.Nlopt_objective()) #objective function
+            
+            #bounds
+            if self.if_bounds == True:
+                opt.set_lower_bounds(self.lb)
+                opt.set_upper_bounds(self.ub)
+
+            #equality constraints
+            if self.if_eq_c == True:
+                if self.d_eq_c == 0:
+                    opt.add_equality_constraint(self.Nlopt_eq_constraints(),self.eq_tol)
+                else:
+                    opt.add_equality_mconstraint(self.Nlopt_eq_mconstraints(),self.eq_tol)
+
+            #inequality constraints
+            if self.if_ineq_c == True:
+                if self.d_ineq_c == 0:
+                    opt.add_inequality_constraint(self.Nlopt_in_constraints(),self.ineq_tol)
+                else:
+                    opt.add_inequality_mconstraint(self.Nlopt_in_mconstraints(),self.ineq_tol)
+
+            #stopping criteria
+            if self.if_maxiter:
+                opt.set_maxeval(self.maxiter)
+            if self.if_ftol_abs:
+                opt.set_ftol_abs(self.set_ftol_abs) 
+            if self.if_ftol_rel:
+                opt.set_ftol_rel(self.set_ftol_rel)
+
+            #perform optimization
+            x_fin = opt.optimize(x_ini)
+
+        return x_fin
+
+                
+
+
+
+
```

### Comparing `JaxSSO-0.0.5/JaxSSO.egg-info/PKG-INFO` & `JaxSSO-0.0.6/JaxSSO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxSSO
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework for structural shape optimization based on automatic differentiation (AD) and the adjoint method, enabled by JAX
 Home-page: https://github.com/GaoyuanWu/JaxSSO
 Author: Gaoyuan Wu
 Author-email: gaoyuanw@princeton.edu
 License: UNKNOWN
 Description: # JaxSSO
         A framework for structural shape optimization based on automatic differentiation (AD) and the adjoint method, enabled by [JAX](https://github.com/google/jax).
@@ -55,14 +55,15 @@
         
         ### Dependencies
         JaxSSO is written in Python and requires:
         * [numpy](https://numpy.org/doc/stable/index.html) >= 1.22.0.
         * [JAX](https://jax.readthedocs.io/en/latest/index.html): "JAX is [Autograd](https://github.com/hips/autograd) and [XLA](https://www.tensorflow.org/xla), brought together for high-performance machine learning research." Please refer to [this link](https://github.com/google/jax#installation) for the installation of JAX.
         * [Nlopt](https://nlopt.readthedocs.io/en/latest/): Nlopt is a library for nonlinear optimization. It has Python interface, which is implemented herein. Refer to [this link](https://nlopt.readthedocs.io/en/latest/NLopt_Installation/) for the installation of Nlopt. Alternatively, you can use `pip install nlopt`, please refer to [
         nlopt-python](https://pypi.org/project/nlopt/).
+        * [scipy](https://scipy.org/).
         
         
         ### Quickstart
         The project provides you with interactive examples with Google Colab for quick start:
         * [2D-arch](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Arch_2D.ipynb): form-finding of a 2d-arch
         * [3D-arch](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Arch_3D.ipynb): form-finding of a 3d-arch
         * [Mannheim Multihalle](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Mannheim_Multihalle.ipynb): form-finding of Mannheim Multihalle
```

### Comparing `JaxSSO-0.0.5/PKG-INFO` & `JaxSSO-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxSSO
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework for structural shape optimization based on automatic differentiation (AD) and the adjoint method, enabled by JAX
 Home-page: https://github.com/GaoyuanWu/JaxSSO
 Author: Gaoyuan Wu
 Author-email: gaoyuanw@princeton.edu
 License: UNKNOWN
 Description: # JaxSSO
         A framework for structural shape optimization based on automatic differentiation (AD) and the adjoint method, enabled by [JAX](https://github.com/google/jax).
@@ -55,14 +55,15 @@
         
         ### Dependencies
         JaxSSO is written in Python and requires:
         * [numpy](https://numpy.org/doc/stable/index.html) >= 1.22.0.
         * [JAX](https://jax.readthedocs.io/en/latest/index.html): "JAX is [Autograd](https://github.com/hips/autograd) and [XLA](https://www.tensorflow.org/xla), brought together for high-performance machine learning research." Please refer to [this link](https://github.com/google/jax#installation) for the installation of JAX.
         * [Nlopt](https://nlopt.readthedocs.io/en/latest/): Nlopt is a library for nonlinear optimization. It has Python interface, which is implemented herein. Refer to [this link](https://nlopt.readthedocs.io/en/latest/NLopt_Installation/) for the installation of Nlopt. Alternatively, you can use `pip install nlopt`, please refer to [
         nlopt-python](https://pypi.org/project/nlopt/).
+        * [scipy](https://scipy.org/).
         
         
         ### Quickstart
         The project provides you with interactive examples with Google Colab for quick start:
         * [2D-arch](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Arch_2D.ipynb): form-finding of a 2d-arch
         * [3D-arch](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Arch_3D.ipynb): form-finding of a 3d-arch
         * [Mannheim Multihalle](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Mannheim_Multihalle.ipynb): form-finding of Mannheim Multihalle
```

### Comparing `JaxSSO-0.0.5/README.md` & `JaxSSO-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 ### Dependencies
 JaxSSO is written in Python and requires:
 * [numpy](https://numpy.org/doc/stable/index.html) >= 1.22.0.
 * [JAX](https://jax.readthedocs.io/en/latest/index.html): "JAX is [Autograd](https://github.com/hips/autograd) and [XLA](https://www.tensorflow.org/xla), brought together for high-performance machine learning research." Please refer to [this link](https://github.com/google/jax#installation) for the installation of JAX.
 * [Nlopt](https://nlopt.readthedocs.io/en/latest/): Nlopt is a library for nonlinear optimization. It has Python interface, which is implemented herein. Refer to [this link](https://nlopt.readthedocs.io/en/latest/NLopt_Installation/) for the installation of Nlopt. Alternatively, you can use `pip install nlopt`, please refer to [
 nlopt-python](https://pypi.org/project/nlopt/).
+* [scipy](https://scipy.org/).
 
 
 ### Quickstart
 The project provides you with interactive examples with Google Colab for quick start:
 * [2D-arch](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Arch_2D.ipynb): form-finding of a 2d-arch
 * [3D-arch](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Arch_3D.ipynb): form-finding of a 3d-arch
 * [Mannheim Multihalle](https://github.com/GaoyuanWu/JaxSSO/blob/main/Examples/Mannheim_Multihalle.ipynb): form-finding of Mannheim Multihalle
```

### Comparing `JaxSSO-0.0.5/setup.py` & `JaxSSO-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="JaxSSO",
-    version="0.0.5",
+    version="0.0.6",
     author="Gaoyuan Wu",
     author_email="gaoyuanw@princeton.edu",
     description="A framework for structural shape optimization based on automatic differentiation (AD) and the adjoint method, enabled by JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GaoyuanWu/JaxSSO",
     packages=setuptools.find_packages(include=['JaxSSO']),
```

