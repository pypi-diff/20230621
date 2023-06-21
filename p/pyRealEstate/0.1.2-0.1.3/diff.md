# Comparing `tmp/pyRealEstate-0.1.2.tar.gz` & `tmp/pyRealEstate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.1.2.tar", last modified: Wed Jun 21 00:34:24 2023, max compression
+gzip compressed data, was "pyRealEstate-0.1.3.tar", last modified: Wed Jun 21 11:41:20 2023, max compression
```

## Comparing `pyRealEstate-0.1.2.tar` & `pyRealEstate-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/Pre_Processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/Time_Trending.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 00:34:24.000000 pyRealEstate-0.1.2/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 00:34:12.000000 pyRealEstate-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-21 00:34:24.691391 pyRealEstate-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:41:20.664423 pyRealEstate-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 11:41:20.664423 pyRealEstate-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:41:20.664423 pyRealEstate-0.1.3/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/pyRealEstate/Pre_Processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/pyRealEstate/Time_Trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:41:20.664423 pyRealEstate-0.1.3/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 11:41:20.000000 pyRealEstate-0.1.3/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-21 11:41:20.000000 pyRealEstate-0.1.3/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:41:20.000000 pyRealEstate-0.1.3/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 11:41:20.000000 pyRealEstate-0.1.3/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 11:41:20.000000 pyRealEstate-0.1.3/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 11:40:59.000000 pyRealEstate-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-21 11:41:20.664423 pyRealEstate-0.1.3/setup.cfg
```

### Comparing `pyRealEstate-0.1.2/LICENSE` & `pyRealEstate-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.2/PKG-INFO` & `pyRealEstate-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.1.2
+Version: 0.1.3
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.1.2/README.md` & `pyRealEstate-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.2/pyRealEstate/Pre_Processing.py` & `pyRealEstate-0.1.3/pyRealEstate/Pre_Processing.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.2/pyRealEstate/RealEstateMetrics.py` & `pyRealEstate-0.1.3/pyRealEstate/RealEstateMetrics.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.2/pyRealEstate/Time_Trending.py` & `pyRealEstate-0.1.3/pyRealEstate/Time_Trending.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,53 +67,56 @@
 
 
 
 
 
 class SPPSF_Machine_Learning_Time_Model :
 
-  def __init__( self , attrs = None):
+  def __init__( self , attrs = None , model_Type = 'Random Forest', Return_Gaussian_Smoothing = False , Smoothing_Sigma= 2 , model_params = {'random_state' : 42 , 'min_child_samples': 20 } ):
     self.attrs = attrs
+    self.model_Type = model_Type
 
-  def fit( self ,SPPSF_ , Time_ , model_Type = 'Random Forest', Return_Gaussian_Smoothing = False , Smoothing_Sigma= 2  , return_model =False , model_params = {'random_state' : 42 , 'min_child_samples': 20 } ):
-    #Creates df for SPPSF and Months
-    
     if( (model_Type == 'Random Forest') &  ('min_child_samples' in model_params) ):
       model_params['min_samples_leaf'] = model_params['min_child_samples']
       del model_params['min_child_samples']
     
     if( (model_Type == 'LGBM') &  ('min_samples_leaf' in model_params) ):
       model_params['min_child_samples'] = model_params['min_samples_leaf']
       del model_params['min_samples_leaf']
 
+    self.model_params = model_params
+    self.Return_Gaussian_Smoothing = Return_Gaussian_Smoothing
+    self.Smoothing_Sigma = Smoothing_Sigma
+
+  
+  def fit( self ,SPPSF_ , Time_   , return_model =False  ):
+    #Creates df for SPPSF and Months    
     Time_ = Time_.rename(columns = {Time_.columns.tolist()[0] : "Months" }).copy()
 
     Time_ML_Model = None 
-    if(model_Type == 'Random Forest'):
-      rf_tt = RandomForestRegressor( **model_params )
+
+    if(self.model_Type == 'Random Forest'):
+      rf_tt = RandomForestRegressor( **self.model_params )
       rf_tt.fit(Time_ , SPPSF_ )
       Time_ML_Model = rf_tt
     else : 
-      lgbm_tt = ltb.LGBMRegressor( **model_params)
+      lgbm_tt = ltb.LGBMRegressor( **self.model_params)
       lgbm_tt.fit(Time_ , SPPSF_ )
       Time_ML_Model = lgbm_tt
 
 
     self.Time_Model = Time_ML_Model
 
-    predData = pd.DataFrame({
-                                'Months' : range(0, Time_.max()[0] + 1)} , index = range(0, Time_.max()[0] + 1))
+    predData = pd.DataFrame({  'Months' : range(0, Time_.max()[0] + 1)} , index = range(0, Time_.max()[0] + 1))
 
     self.pred_data = predData
 
-    self.Return_Gaussian_Smoothing = Return_Gaussian_Smoothing
-    self.Smoothing_Sigma = Smoothing_Sigma
-    del model_params
     if return_model ==True:
       return bestTimeModel
+
   
   def Display_Time_Trend(self): 
     plt.plot(-self.pred_data['Months'], self.Time_Model.predict(self.pred_data[['Months']]), '-', color = 'red', linewidth = 3 , label = "Machine Learning Time Trend")
     
     if (self.Return_Gaussian_Smoothing == True): 
       plt.plot(-self.pred_data['Months'], gaussian_filter1d(self.Time_Model.predict(self.pred_data[['Months']]), sigma = self.Smoothing_Sigma), color = 'blue', linewidth = 3 , label = "Time Trend with Gaussian Smoothing")
```

### Comparing `pyRealEstate-0.1.2/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.1.3/pyRealEstate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.1.2
+Version: 0.1.3
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.1.2/pypi_description.md` & `pyRealEstate-0.1.3/pypi_description.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.2/setup.cfg` & `pyRealEstate-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.1.2
+version = 0.1.3
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
```

