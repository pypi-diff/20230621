# Comparing `tmp/Tacoma lib-1.0.0.tar.gz` & `tmp/Tacoma lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tacoma lib-1.0.0.tar", last modified: Tue Jul 12 10:53:17 2022, max compression
+gzip compressed data, was "Tacoma lib-1.0.1.tar", last modified: Tue Jun 20 23:50:33 2023, max compression
```

## Comparing `Tacoma lib-1.0.0.tar` & `Tacoma lib-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 jaime      (501) staff       (20)        0 2022-07-12 10:53:17.933933 Tacoma lib-1.0.0/
--rw-r--r--   0 jaime      (501) staff       (20)     1106 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/LICENSE
--rw-r--r--   0 jaime      (501) staff       (20)     2000 2022-07-12 10:53:17.933537 Tacoma lib-1.0.0/PKG-INFO
--rw-r--r--   0 jaime      (501) staff       (20)     1674 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/README.md
-drwxr-xr-x   0 jaime      (501) staff       (20)        0 2022-07-12 10:53:17.932060 Tacoma lib-1.0.0/Tacoma_lib.egg-info/
--rw-r--r--   0 jaime      (501) staff       (20)     2000 2022-07-12 10:53:17.000000 Tacoma lib-1.0.0/Tacoma_lib.egg-info/PKG-INFO
--rw-r--r--   0 jaime      (501) staff       (20)      285 2022-07-12 10:53:17.000000 Tacoma lib-1.0.0/Tacoma_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jaime      (501) staff       (20)        1 2022-07-12 10:53:17.000000 Tacoma lib-1.0.0/Tacoma_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jaime      (501) staff       (20)       79 2022-07-12 10:53:17.000000 Tacoma lib-1.0.0/Tacoma_lib.egg-info/requires.txt
--rw-r--r--   0 jaime      (501) staff       (20)        7 2022-07-12 10:53:17.000000 Tacoma lib-1.0.0/Tacoma_lib.egg-info/top_level.txt
--rw-r--r--   0 jaime      (501) staff       (20)       38 2022-07-12 10:53:17.934021 Tacoma lib-1.0.0/setup.cfg
--rw-r--r--   0 jaime      (501) staff       (20)     1022 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/setup.py
-drwxr-xr-x   0 jaime      (501) staff       (20)        0 2022-07-12 10:53:17.933186 Tacoma lib-1.0.0/tacoma/
--rw-r--r--   0 jaime      (501) staff       (20)        0 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/tacoma/__init__.py
--rw-r--r--   0 jaime      (501) staff       (20)     1847 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/tacoma/interpolator.py
--rw-r--r--   0 jaime      (501) staff       (20)     3855 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/tacoma/metrics.py
--rw-r--r--   0 jaime      (501) staff       (20)     5875 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/tacoma/rom.py
--rw-r--r--   0 jaime      (501) staff       (20)     6255 2022-07-12 10:52:43.000000 Tacoma lib-1.0.0/tacoma/utils.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-06-20 23:50:33.935823 Tacoma lib-1.0.1/
+-rw-r--r--   0 jaime      (501) staff       (20)     1106 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/LICENSE
+-rw-r--r--   0 jaime      (501) staff       (20)     1944 2023-06-20 23:50:33.935539 Tacoma lib-1.0.1/PKG-INFO
+-rw-r--r--   0 jaime      (501) staff       (20)     1674 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/README.md
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-06-20 23:50:33.931153 Tacoma lib-1.0.1/Tacoma_lib.egg-info/
+-rw-r--r--   0 jaime      (501) staff       (20)     1944 2023-06-20 23:50:33.000000 Tacoma lib-1.0.1/Tacoma_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jaime      (501) staff       (20)      421 2023-06-20 23:50:33.000000 Tacoma lib-1.0.1/Tacoma_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-06-20 23:50:33.000000 Tacoma lib-1.0.1/Tacoma_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jaime      (501) staff       (20)       79 2023-06-20 23:50:33.000000 Tacoma lib-1.0.1/Tacoma_lib.egg-info/requires.txt
+-rw-r--r--   0 jaime      (501) staff       (20)        7 2023-06-20 23:50:33.000000 Tacoma lib-1.0.1/Tacoma_lib.egg-info/top_level.txt
+-rw-r--r--   0 jaime      (501) staff       (20)       38 2023-06-20 23:50:33.935900 Tacoma lib-1.0.1/setup.cfg
+-rw-r--r--   0 jaime      (501) staff       (20)     1022 2023-06-20 23:14:32.000000 Tacoma lib-1.0.1/setup.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-06-20 23:50:33.932890 Tacoma lib-1.0.1/tacoma/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tacoma/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3810 2023-06-20 23:38:39.000000 Tacoma lib-1.0.1/tacoma/interpolator.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3855 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tacoma/metrics.py
+-rw-r--r--   0 jaime      (501) staff       (20)     5633 2023-06-20 23:43:19.000000 Tacoma lib-1.0.1/tacoma/rom.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6255 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tacoma/utils.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-06-20 23:50:33.935171 Tacoma lib-1.0.1/tests/
+-rw-r--r--   0 jaime      (501) staff       (20)      697 2023-06-20 23:35:18.000000 Tacoma lib-1.0.1/tests/test_backmapping.py
+-rw-r--r--   0 jaime      (501) staff       (20)      535 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tests/test_metrics.py
+-rw-r--r--   0 jaime      (501) staff       (20)      415 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tests/test_regressor.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1231 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tests/test_rom.py
+-rw-r--r--   0 jaime      (501) staff       (20)      500 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tests/test_util.py
+-rw-r--r--   0 jaime      (501) staff       (20)      495 2022-07-12 10:52:43.000000 Tacoma lib-1.0.1/tests/test_util_scripts.py
```

### Comparing `Tacoma lib-1.0.0/LICENSE` & `Tacoma lib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Tacoma lib-1.0.0/PKG-INFO` & `Tacoma lib-1.0.1/Tacoma_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: Tacoma lib
-Version: 1.0.0
+Name: Tacoma-lib
+Version: 1.0.1
 Summary: TACOMA lib
-Home-page: UNKNOWN
 Author: Jaime Bowen Varela, Rodrigo Castellanos, Alejandro Gorgues
 Author-email: jbowvar@inta.es, rcasgar@inta.es, gorguesva@inta.es
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TACOMA lib 
 A python library for applying Machine Learning in CFD. This library is on active deveplopment and expect the API to change overtime.
 At the moment, most of the classes and functions are centered on Reduce Order Modelling techniques (ROMs).
 
@@ -35,9 +32,7 @@
 ## Examples
 The examples are contained in [here](https://github.com/jaimebw/tacoma_lib/tree/main/examples). The examples show some implemetations of the Tacoma lib for ROMs:
 * [An example on how to use ROMs with Sklearn](https://github.com/TACOMA-INTA/tacoma-lib/blob/main/examples/rom_regression_example.py)
 * [An example on how to do hyperoptimization with Sklearn and Optuna](https://github.com/TACOMA-INTA/tacoma-lib/blob/main/examples/rom_sklearn_optuna_example.py)
 * [An example on how to use ROMs with PyTorch](https://github.com/TACOMA-INTA/tacoma-lib/blob/main/examples/rom_pytorch_example.py)
 
 More examples to be added in the future
-
-
```

### Comparing `Tacoma lib-1.0.0/README.md` & `Tacoma lib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Tacoma lib-1.0.0/Tacoma_lib.egg-info/PKG-INFO` & `Tacoma lib-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: Tacoma-lib
-Version: 1.0.0
+Name: Tacoma lib
+Version: 1.0.1
 Summary: TACOMA lib
-Home-page: UNKNOWN
 Author: Jaime Bowen Varela, Rodrigo Castellanos, Alejandro Gorgues
 Author-email: jbowvar@inta.es, rcasgar@inta.es, gorguesva@inta.es
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TACOMA lib 
 A python library for applying Machine Learning in CFD. This library is on active deveplopment and expect the API to change overtime.
 At the moment, most of the classes and functions are centered on Reduce Order Modelling techniques (ROMs).
 
@@ -35,9 +32,7 @@
 ## Examples
 The examples are contained in [here](https://github.com/jaimebw/tacoma_lib/tree/main/examples). The examples show some implemetations of the Tacoma lib for ROMs:
 * [An example on how to use ROMs with Sklearn](https://github.com/TACOMA-INTA/tacoma-lib/blob/main/examples/rom_regression_example.py)
 * [An example on how to do hyperoptimization with Sklearn and Optuna](https://github.com/TACOMA-INTA/tacoma-lib/blob/main/examples/rom_sklearn_optuna_example.py)
 * [An example on how to use ROMs with PyTorch](https://github.com/TACOMA-INTA/tacoma-lib/blob/main/examples/rom_pytorch_example.py)
 
 More examples to be added in the future
-
-
```

### Comparing `Tacoma lib-1.0.0/setup.py` & `Tacoma lib-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 with open(path.join(HERE, 'requirements.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 
 
 setup(
     name="Tacoma lib",
-    version="1.0.0",
+    version="1.0.1",
     description="TACOMA lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jaime Bowen Varela, Rodrigo Castellanos, Alejandro Gorgues',
     author_email="jbowvar@inta.es, rcasgar@inta.es, gorguesva@inta.es", 
     packages=["tacoma"],
     include_package_data=True,
```

### Comparing `Tacoma lib-1.0.0/tacoma/metrics.py` & `Tacoma lib-1.0.1/tacoma/metrics.py`

 * *Files identical despite different names*

### Comparing `Tacoma lib-1.0.0/tacoma/rom.py` & `Tacoma lib-1.0.1/tacoma/rom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 import numpy as np
-import pandas as pd
-import pickle
-from pathlib import Path
-import pickle
 from sklearn.manifold import Isomap 
-from sklearn.neighbors import kneighbors_graph
-from sklearn.neighbors import NearestNeighbors
-from sklearn.neighbors import KNeighborsRegressor
-from sklearn import metrics
-
+import joblib
 class PODRegressor:
     """POD Regression ROM. is a numerical method that enables a reduction in the complexity of computer intensive simulations such as computational fluid dynamics.
     It is based on the usage of Singular Value Descomposition to obtain the spatial and temporal modes 
     """
     def __init__(self,n_PODmodes = None,regression_model=None,**kwargs):
         self.__init_regression_model__(regression_model)
         self.n_PODmodes = n_PODmodes 
@@ -142,17 +134,18 @@
         X_test: testing features
         y_test: testing labels
 
         """
         self.y_iso_train = self.embedding.fit_transform(y_train)
         self.regression_model.fit(X_train,self.y_iso_train)
         self.y_iso_pred = self.regression_model.predict(X_test)
-        self.backmapping_model.fit(y_train,self.y_iso_train,self.y_iso_pred)               
-        self.y_pred = self.backmapping_model.predict()
+        self.backmapping_model.fit(y_train,self.y_iso_train)
+        self.y_pred = self.backmapping_model.predict(self.y_iso_pred) 
 
     def get_params(self):
         """
         Returns the global parameters of the model. 
         The first element is the regression model parameters. The second model is the Isomap embedding parameters
         """
         return self.regression_model.get_params(), self.embedding.get_params()
     
+
```

### Comparing `Tacoma lib-1.0.0/tacoma/utils.py` & `Tacoma lib-1.0.1/tacoma/utils.py`

 * *Files identical despite different names*

