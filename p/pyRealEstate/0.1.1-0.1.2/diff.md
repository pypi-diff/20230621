# Comparing `tmp/pyRealEstate-0.1.1.tar.gz` & `tmp/pyRealEstate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.1.1.tar", last modified: Tue Jun 20 23:52:10 2023, max compression
+gzip compressed data, was "pyRealEstate-0.1.2.tar", last modified: Wed Jun 21 00:34:24 2023, max compression
```

## Comparing `pyRealEstate-0.1.1.tar` & `pyRealEstate-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/Pre_Processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/Time_Trending.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/Pre_Processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/Time_Trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/setup.cfg
```

### Comparing `pyRealEstate-0.1.1/LICENSE` & `pyRealEstate-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.1/PKG-INFO` & `pyRealEstate-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.1.1
+Version: 0.1.2
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.1.1/README.md` & `pyRealEstate-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pyRealEstate
 
-pyRealEstate is a library designed for data scientists working in the real estate industry. pyRealEstate is still currently under development but is aimed at providing functions to assist in the development and evaluation of AVM's. Below are some instructions on how to get started with pyRealEstate and some helpful links to descriptions and examples of all of PyRealEstates functionality 
+pyRealEstate is a library designed for data scientists working in the real estate industry. pyRealEstate is still currently under development but is aimed at providing functions to assist in the development and evaluation of AVM's. Below are some instructions on how to get started with pyRealEstate and some helpful links to descriptions and examples of all of PyRealEstates functionality. 
 
 ## Installation
 
-the pyRealEstate package is available on [PyPi](https://pypi.org/project/pyRealEstate). Simply run: 
+The pyRealEstate package is available on [PyPi](https://pypi.org/project/pyRealEstate). Simply run: 
 ```
 pip install pyRealEstate
 ```
-## AVM Evalutation Metrics
-pyRealEstate can provide metrics on the evaluation of your AVM (Automated Valuation Model) such as the weighted mean sale ratio, COD (Coefficient Of Disspersion), and PRD ( Price Related Differential) please visit the wiki for detailed documentation [pyRealEstate Evaluation](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/AVM-Evaluation-Metrics)
+## AVM Evaluation Metrics
+pyRealEstate can provide metrics on the evaluation of your AVM (Automated Valuation Model) such as the weighted mean sale ratio, COD (Coefficient Of Disspersion), and PRD (Price Related Differential) please visit the wiki for detailed documentation [pyRealEstate Evaluation](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/AVM-Evaluation-Metrics).
 
 ## Data Pre Processing
-In addition to the evaluation metrics for the models pyRealEstate also offers a multitude of functions to help with the pre processing of data. Please visit the wiki for detailed documentation [pyRealEstate Pre Processing](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/Pre-Processing)
+In addition to the evaluation metrics for the models, pyRealEstate also offers a multitude of functions to help with the pre processing of data. Please visit the wiki for detailed documentation [pyRealEstate Pre Processing](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/Pre-Processing).
 
 ## Time Trending for AVM's
-In creating Automated Valuation Models (AVM's) for real estate it is key to capture time trends in the market. There are typically two major approaches one is to model the time trend and then to adjust the sales based on the time adjustment rate. The other option is to include time directly in the model. If one wishes to take the first approach this pyRealEstate is to assist in the finding of the time adjustment rates. Please visit the wiki for detailed documentation [pyRealEstate Time Trending](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/Time-Trending)
+In creating Automated Valuation Models (AVM's) for real estate, it is key to capture time trends in the market. There are typically two major approaches; one is to model the time trend and then to adjust the sales based on the time adjustment rate. The other option is to include time directly in the model. If one wishes to take the first approach this pyRealEstate is to assist in the finding of the time adjustment rates. Please visit the wiki for detailed documentation [pyRealEstate Time Trending](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/Time-Trending).
```

### Comparing `pyRealEstate-0.1.1/pyRealEstate/Pre_Processing.py` & `pyRealEstate-0.1.2/pyRealEstate/Pre_Processing.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.1/pyRealEstate/RealEstateMetrics.py` & `pyRealEstate-0.1.2/pyRealEstate/RealEstateMetrics.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.1/pyRealEstate/Time_Trending.py` & `pyRealEstate-0.1.2/pyRealEstate/Time_Trending.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,19 +73,19 @@
 
   def __init__( self , attrs = None):
     self.attrs = attrs
 
   def fit( self ,SPPSF_ , Time_ , model_Type = 'Random Forest', Return_Gaussian_Smoothing = False , Smoothing_Sigma= 2  , return_model =False , model_params = {'random_state' : 42 , 'min_child_samples': 20 } ):
     #Creates df for SPPSF and Months
     
-    if( (model_Type == 'Random Forest') &  ('min_child_samples' in tst) ):
+    if( (model_Type == 'Random Forest') &  ('min_child_samples' in model_params) ):
       model_params['min_samples_leaf'] = model_params['min_child_samples']
       del model_params['min_child_samples']
     
-    if( (model_Type == 'LGBM') &  ('min_samples_leaf' in tst) ):
+    if( (model_Type == 'LGBM') &  ('min_samples_leaf' in model_params) ):
       model_params['min_child_samples'] = model_params['min_samples_leaf']
       del model_params['min_samples_leaf']
 
     Time_ = Time_.rename(columns = {Time_.columns.tolist()[0] : "Months" }).copy()
 
     Time_ML_Model = None 
     if(model_Type == 'Random Forest'):
```

### Comparing `pyRealEstate-0.1.1/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.1.2/pyRealEstate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.1.1
+Version: 0.1.2
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.1.1/pypi_description.md` & `pyRealEstate-0.1.2/pypi_description.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.1/setup.cfg` & `pyRealEstate-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.1.1
+version = 0.1.2
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
```

