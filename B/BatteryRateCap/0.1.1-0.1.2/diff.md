# Comparing `tmp/BatteryRateCap-0.1.1.tar.gz` & `tmp/BatteryRateCap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/user/Downloads/BatteryRateCap/dist/.tmp-jl8lpx5f/BatteryRateCap-0.1.1.tar", last modified: Wed Jun  7 19:05:41 2023, max compression
+gzip compressed data, was "/home/user/Downloads/BatteryRateCap/dist/.tmp-y9k4n9_c/BatteryRateCap-0.1.2.tar", last modified: Wed Jun 21 00:02:44 2023, max compression
```

## Comparing `BatteryRateCap-0.1.1.tar` & `BatteryRateCap-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     8166 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      300 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       15 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/BatteryRateCap.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1059 2023-05-30 18:15:22.000000 BatteryRateCap-0.1.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8166 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     6154 2023-05-31 17:45:04.000000 BatteryRateCap-0.1.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-06-07 19:04:49.000000 BatteryRateCap-0.1.1/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 19:05:41.000000 BatteryRateCap-0.1.1/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     2157 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_correlationtest.py
--rw-rw-r--   0 user      (1000) user      (1000)     4128 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_data_converter.py
--rw-rw-r--   0 user      (1000) user      (1000)     3821 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_fitcaprate.py
--rw-rw-r--   0 user      (1000) user      (1000)     1445 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.1/tests/test_visualization.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/BatteryRateCap.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     8165 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/BatteryRateCap.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      300 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/BatteryRateCap.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/BatteryRateCap.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       15 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/BatteryRateCap.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1059 2023-05-30 18:15:22.000000 BatteryRateCap-0.1.2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8165 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     6153 2023-06-20 23:39:14.000000 BatteryRateCap-0.1.2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-06-20 23:55:32.000000 BatteryRateCap-0.1.2/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-21 00:02:44.000000 BatteryRateCap-0.1.2/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     2157 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.2/tests/test_correlationtest.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4128 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.2/tests/test_data_converter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3821 2023-05-30 21:10:46.000000 BatteryRateCap-0.1.2/tests/test_fitcaprate.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1448 2023-06-20 23:53:54.000000 BatteryRateCap-0.1.2/tests/test_visualization.py
```

### Comparing `BatteryRateCap-0.1.1/BatteryRateCap.egg-info/PKG-INFO` & `BatteryRateCap-0.1.2/BatteryRateCap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BatteryRateCap
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for battery rate capability analysis.
 Author-email: Chih-Hsuan Hung <dhung@uw.edu>, Praise Anyanwu <anyanc@uw.edu>, "Kevin G. Lee" <gskl92@uw.edu>, "Matthew J. Canin" <matthewcanin@gmail.com>, Kevin Martinez-Chavez <martikev@protonmail.com>
 Maintainer-email: Chih-Hsuan Hung <dhung@uw.edu>
 License: MIT License
         
         Copyright (c) 2021 c.
         
@@ -88,36 +88,36 @@
 ## Example Use Cases for Battery Researchers
 ### Use case 1. Data Conversion
 The *data_converter* module converts charge/discharge data (voltage versus capacity) and capacity-cycle data 
 into rate-capacity data. Complete procedures and example codes on how to use the *data_converter* module are 
 detailed in Demo/Demo_data_converter.ipynb. Below is an excerpt of the *data_converter* demo notebook, showing 
 the output of how *data_converter* categorizes capacity data by their C-rate in a capacity-cycle dataset. 
 The conversion from voltage-capacity to capacity-rate data does not involve any visuals, so no figures are shown here.<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/data_converter_grouped.png)   
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/data_converter_grouped.png)   
 ### Use case 2. Data Fitting
 The *fitcaprate* module fits capacity-rate data and attains fitting parameters, including charatersitic time, 
 *n* value, and capacity *Q* as described in the introduction. Complete procedures and example codes on how to 
 use the *fitcaprate* module can be found in Demo/Demo_fitcaprate.ipynb. Below is an excerpt of the *fitcaprate* 
 demo notebook, showing the results of fitted curves (red dashed curves) found by *fitcaprate* for a set of 
 battery capcity-rate data (blue dots).<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/fitcaprate_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/fitcaprate_example.png)
 ### Use case 3: Data visulization
 The *visualization* module creates a panel plot that lays out 2D scatter plots of fitting parameters versus 
 available battery design parameters realated to geometry and materials. Complete procedures and example 
 codes on how to use the *visualization* module are detailed in Demo/Demo_visualization.ipynb. Below is an 
 excerpt of the *visualization* demo notebook, showing the output panel plot.<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/visualization_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/visualization_example.png)
 ### Use case 4: Hypothesis testing
 The *correlationtest* module determines whether a statistically-signicificant linear relationship exisits 
 between found battery fitting parameters, which indicate the battery performance, and their desgin parameters
 related to geometry and materials. Complete procedures and example codes on how to use the *correlationtest* 
 module are detailed in Demo/Demo_correlationtest. Below is an excerpt of the *correlationtest* demo notebook, 
 showing how the module plots the best-fit linear regression line (in blue) between two target parameters 
 and highlights potential outliers (in red) to the linear relationship.
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/correlation_test_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/correlation_test_example.png)
 
  
 ## How to Install
 *BatteryRateCap* can be installed by cloning the entire repoitory or via pip:</br>
 ```
 pip install BatteryRateCap
 ```
@@ -126,10 +126,10 @@
 - Python >=3.6
 - See environment.yml for all Python package dependencies
 
 
 ## Community Guidelines
 If you encounter any issue using *BatteryRateCap* or would like to request an additional feature, please report using a [Github 
 issue](https://github.com/BatteryDesign/BatteryRateCap/issues). If you would like to directly contribute to this project, please email the 
-reporsitory maintainer Doris Hung at dhung@uw.edu.
+reporsitory maintainers Doris Hung (dhung@uw.edu) and Praise Anyanwu (anyanc@uw.edu).
```

### Comparing `BatteryRateCap-0.1.1/LICENSE.txt` & `BatteryRateCap-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.1/PKG-INFO` & `BatteryRateCap-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BatteryRateCap
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for battery rate capability analysis.
 Author-email: Chih-Hsuan Hung <dhung@uw.edu>, Praise Anyanwu <anyanc@uw.edu>, "Kevin G. Lee" <gskl92@uw.edu>, "Matthew J. Canin" <matthewcanin@gmail.com>, Kevin Martinez-Chavez <martikev@protonmail.com>
 Maintainer-email: Chih-Hsuan Hung <dhung@uw.edu>
 License: MIT License
         
         Copyright (c) 2021 c.
         
@@ -88,36 +88,36 @@
 ## Example Use Cases for Battery Researchers
 ### Use case 1. Data Conversion
 The *data_converter* module converts charge/discharge data (voltage versus capacity) and capacity-cycle data 
 into rate-capacity data. Complete procedures and example codes on how to use the *data_converter* module are 
 detailed in Demo/Demo_data_converter.ipynb. Below is an excerpt of the *data_converter* demo notebook, showing 
 the output of how *data_converter* categorizes capacity data by their C-rate in a capacity-cycle dataset. 
 The conversion from voltage-capacity to capacity-rate data does not involve any visuals, so no figures are shown here.<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/data_converter_grouped.png)   
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/data_converter_grouped.png)   
 ### Use case 2. Data Fitting
 The *fitcaprate* module fits capacity-rate data and attains fitting parameters, including charatersitic time, 
 *n* value, and capacity *Q* as described in the introduction. Complete procedures and example codes on how to 
 use the *fitcaprate* module can be found in Demo/Demo_fitcaprate.ipynb. Below is an excerpt of the *fitcaprate* 
 demo notebook, showing the results of fitted curves (red dashed curves) found by *fitcaprate* for a set of 
 battery capcity-rate data (blue dots).<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/fitcaprate_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/fitcaprate_example.png)
 ### Use case 3: Data visulization
 The *visualization* module creates a panel plot that lays out 2D scatter plots of fitting parameters versus 
 available battery design parameters realated to geometry and materials. Complete procedures and example 
 codes on how to use the *visualization* module are detailed in Demo/Demo_visualization.ipynb. Below is an 
 excerpt of the *visualization* demo notebook, showing the output panel plot.<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/visualization_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/visualization_example.png)
 ### Use case 4: Hypothesis testing
 The *correlationtest* module determines whether a statistically-signicificant linear relationship exisits 
 between found battery fitting parameters, which indicate the battery performance, and their desgin parameters
 related to geometry and materials. Complete procedures and example codes on how to use the *correlationtest* 
 module are detailed in Demo/Demo_correlationtest. Below is an excerpt of the *correlationtest* demo notebook, 
 showing how the module plots the best-fit linear regression line (in blue) between two target parameters 
 and highlights potential outliers (in red) to the linear relationship.
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/correlation_test_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/correlation_test_example.png)
 
  
 ## How to Install
 *BatteryRateCap* can be installed by cloning the entire repoitory or via pip:</br>
 ```
 pip install BatteryRateCap
 ```
@@ -126,10 +126,10 @@
 - Python >=3.6
 - See environment.yml for all Python package dependencies
 
 
 ## Community Guidelines
 If you encounter any issue using *BatteryRateCap* or would like to request an additional feature, please report using a [Github 
 issue](https://github.com/BatteryDesign/BatteryRateCap/issues). If you would like to directly contribute to this project, please email the 
-reporsitory maintainer Doris Hung at dhung@uw.edu.
+reporsitory maintainers Doris Hung (dhung@uw.edu) and Praise Anyanwu (anyanc@uw.edu).
```

### Comparing `BatteryRateCap-0.1.1/README.md` & `BatteryRateCap-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,36 +50,36 @@
 ## Example Use Cases for Battery Researchers
 ### Use case 1. Data Conversion
 The *data_converter* module converts charge/discharge data (voltage versus capacity) and capacity-cycle data 
 into rate-capacity data. Complete procedures and example codes on how to use the *data_converter* module are 
 detailed in Demo/Demo_data_converter.ipynb. Below is an excerpt of the *data_converter* demo notebook, showing 
 the output of how *data_converter* categorizes capacity data by their C-rate in a capacity-cycle dataset. 
 The conversion from voltage-capacity to capacity-rate data does not involve any visuals, so no figures are shown here.<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/data_converter_grouped.png)   
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/data_converter_grouped.png)   
 ### Use case 2. Data Fitting
 The *fitcaprate* module fits capacity-rate data and attains fitting parameters, including charatersitic time, 
 *n* value, and capacity *Q* as described in the introduction. Complete procedures and example codes on how to 
 use the *fitcaprate* module can be found in Demo/Demo_fitcaprate.ipynb. Below is an excerpt of the *fitcaprate* 
 demo notebook, showing the results of fitted curves (red dashed curves) found by *fitcaprate* for a set of 
 battery capcity-rate data (blue dots).<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/fitcaprate_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/fitcaprate_example.png)
 ### Use case 3: Data visulization
 The *visualization* module creates a panel plot that lays out 2D scatter plots of fitting parameters versus 
 available battery design parameters realated to geometry and materials. Complete procedures and example 
 codes on how to use the *visualization* module are detailed in Demo/Demo_visualization.ipynb. Below is an 
 excerpt of the *visualization* demo notebook, showing the output panel plot.<br/>
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/visualization_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/visualization_example.png)
 ### Use case 4: Hypothesis testing
 The *correlationtest* module determines whether a statistically-signicificant linear relationship exisits 
 between found battery fitting parameters, which indicate the battery performance, and their desgin parameters
 related to geometry and materials. Complete procedures and example codes on how to use the *correlationtest* 
 module are detailed in Demo/Demo_correlationtest. Below is an excerpt of the *correlationtest* demo notebook, 
 showing how the module plots the best-fit linear regression line (in blue) between two target parameters 
 and highlights potential outliers (in red) to the linear relationship.
-![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/documentation/demo/correlation_test_example.png)
+![alt text](https://github.com/BatteryDesign/BatteryRateCap/blob/main/demo/correlation_test_example.png)
 
  
 ## How to Install
 *BatteryRateCap* can be installed by cloning the entire repoitory or via pip:</br>
 ```
 pip install BatteryRateCap
 ```
@@ -88,10 +88,10 @@
 - Python >=3.6
 - See environment.yml for all Python package dependencies
 
 
 ## Community Guidelines
 If you encounter any issue using *BatteryRateCap* or would like to request an additional feature, please report using a [Github 
 issue](https://github.com/BatteryDesign/BatteryRateCap/issues). If you would like to directly contribute to this project, please email the 
-reporsitory maintainer Doris Hung at dhung@uw.edu.
+reporsitory maintainers Doris Hung (dhung@uw.edu) and Praise Anyanwu (anyanc@uw.edu).
```

### Comparing `BatteryRateCap-0.1.1/pyproject.toml` & `BatteryRateCap-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "BatteryRateCap"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python package for battery rate capability analysis."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 keywords = ["battery", "rate analysis", "rate capability"]
 authors = [
     {name = "Chih-Hsuan Hung", email = "dhung@uw.edu"},
```

### Comparing `BatteryRateCap-0.1.1/tests/test_correlationtest.py` & `BatteryRateCap-0.1.2/tests/test_correlationtest.py`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.1/tests/test_data_converter.py` & `BatteryRateCap-0.1.2/tests/test_data_converter.py`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.1/tests/test_fitcaprate.py` & `BatteryRateCap-0.1.2/tests/test_fitcaprate.py`

 * *Files identical despite different names*

### Comparing `BatteryRateCap-0.1.1/tests/test_visualization.py` & `BatteryRateCap-0.1.2/tests/test_visualization.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     This function tests the raised error type when
     the column names for fitting parameters are wrong.
     This function also uses a test case to ensure the
     function returns the correct figure grid number.
     '''
     df1 = pd.DataFrame({'n': [1, 2, 3],
                         'tau': [0.1, 0.2, 0.3],
-                        'Q': [100, 200, 300],
+                        'Qmax': [100, 200, 300],
                         'cathode_thickness': [20, 30, 40]})
     df2 = pd.DataFrame({'n': [1, 2, 3],
                         'cathode_thickness': [20, 30, 40]})
     # Test that the function output the correct
     # error type whem missing columns 'n', 'tau', and 'Q'
     try:
         feature_vs_n_tau_q(df2, ['cathode_thickness'])
```

