# Comparing `tmp/stanscofi-1.0.3.tar.gz` & `tmp/stanscofi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stanscofi-1.0.3.tar", last modified: Thu Jun 15 15:37:43 2023, max compression
+gzip compressed data, was "stanscofi-1.0.4.tar", last modified: Wed Jun 21 16:53:37 2023, max compression
```

## Comparing `stanscofi-1.0.3.tar` & `stanscofi-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.465273 stanscofi-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 15:37:43.461273 stanscofi-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-15 15:37:33.000000 stanscofi-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 15:37:33.000000 stanscofi-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:37:43.465273 stanscofi-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 15:37:33.000000 stanscofi-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.461273 stanscofi-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.461273 stanscofi-1.0.3/src/stanscofi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/training_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.461273 stanscofi-1.0.3/src/stanscofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-21 16:53:37.316577 stanscofi-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-21 16:53:27.000000 stanscofi-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 16:53:27.000000 stanscofi-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:53:37.316577 stanscofi-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-21 16:53:27.000000 stanscofi-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/src/stanscofi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/training_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/src/stanscofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/top_level.txt
```

### Comparing `stanscofi-1.0.3/PKG-INFO` & `stanscofi-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -16,15 +16,15 @@
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
 [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
 
-## Statement of need
+## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
 Medium-term outcomes to this package will significantly alleviate the economic burden of drug discovery pipelines, and will help find treatments in a more sustainable manner, especially for rare or tropical neglected diseases.
```

### Comparing `stanscofi-1.0.3/README.md` & `stanscofi-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
 [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
 
-## Statement of need
+## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
 Medium-term outcomes to this package will significantly alleviate the economic burden of drug discovery pipelines, and will help find treatments in a more sustainable manner, especially for rare or tropical neglected diseases.
```

### Comparing `stanscofi-1.0.3/setup.py` & `stanscofi-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "stanscofi"
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 
 setup(name=NAME,
     version=VERSION,
     author="Clémence Réda",
     author_email="recess-project@proton.me",
     url="https://github.com/RECeSS-EU-Project/stanscofi",
     license_files = ('LICENSE'),
```

### Comparing `stanscofi-1.0.3/src/stanscofi/datasets.py` & `stanscofi-1.0.4/src/stanscofi/datasets.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.3/src/stanscofi/models.py` & `stanscofi-1.0.4/src/stanscofi/models.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.3/src/stanscofi/preprocessing.py` & `stanscofi-1.0.4/src/stanscofi/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.3/src/stanscofi/training_testing.py` & `stanscofi-1.0.4/src/stanscofi/training_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     assert njobs in range(nsplits)
     cv_generator = StratifiedKFold(n_splits=nsplits, shuffle=True, random_state=random_state)
     Nitems, Nusers = len(np.unique(train_dataset.ratings[:,0])), len(np.unique(train_dataset.ratings[:,1]))
     grid = np.indices((Nitems,Nusers))
     full_list = np.zeros((Nitems*Nusers, 3))
     full_list[:,0] = grid[0].flatten()
     full_list[:,1] = grid[1].flatten()
-    full_list[:,2] = [train_dataset.ratings_mat[i,j] for i,j in full_list[:,:2].astype(int).tolist()]
+    full_list[:,2] = [train_dataset.ratings_mat[j,i] for i,j in full_list[:,:2].astype(int).tolist()]
     full_list = full_list.astype(int)
     cv_folds = cv_generator.split(full_list[:,:2], np.ravel(full_list[:,2]))
     best_estimator, best_metric = {}, -float("inf")
     def single_run(ncv, tfolds, sfolds, full_list):
         if (verbose):
             print("Crossvalidation step #%d/%d" % (ncv+1,nsplits))
         model = template(params)
```

### Comparing `stanscofi-1.0.3/src/stanscofi/utils.py` & `stanscofi-1.0.4/src/stanscofi/utils.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.3/src/stanscofi/validation.py` & `stanscofi-1.0.4/src/stanscofi/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     plots_args : dict
         dictionary of arguments to feed to the plot_metrics function
     '''
     assert scores.shape[1]==3
     assert predictions.shape[1]==3
     assert predictions.shape[0]==scores.shape[0]
     assert beta>0
-    y_true_all = np.array([test_dataset.ratings_mat[i,j] for i,j in scores[:,:2].astype(int).tolist()])
+    y_true_all = np.array([test_dataset.ratings_mat[j,i] for i,j in scores[:,:2].astype(int).tolist()])
     y_pred_all = predictions[:,2].flatten()
     if (not ignore_zeroes):
         scores_ = deepcopy(scores)
         predictions_ = deepcopy(predictions)
         y_true = (y_true_all>0).astype(int) 
         y_pred = (y_pred_all>0).astype(int)
     else:
```

### Comparing `stanscofi-1.0.3/src/stanscofi.egg-info/PKG-INFO` & `stanscofi-1.0.4/src/stanscofi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -16,15 +16,15 @@
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
 [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
 
-## Statement of need
+## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
 Medium-term outcomes to this package will significantly alleviate the economic burden of drug discovery pipelines, and will help find treatments in a more sustainable manner, especially for rare or tropical neglected diseases.
```

