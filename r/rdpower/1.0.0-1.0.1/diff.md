# Comparing `tmp/rdpower-1.0.0.tar.gz` & `tmp/rdpower-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rmasini/Library/CloudStorage/Dropbox/rdpower/python/rdpower/dist/.tmp-pt4urhs3/rdpower-1.0.0.tar", last modified: Wed Jun 21 02:45:20 2023, max compression
+gzip compressed data, was "/Users/rmasini/Library/CloudStorage/Dropbox/rdpower/python/rdpower/dist/.tmp-433mqi4e/rdpower-1.0.1.tar", last modified: Wed Jun 21 17:29:27 2023, max compression
```

## Comparing `rdpower-1.0.0.tar` & `rdpower-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 02:45:20.022543 rdpower-1.0.0/
--rw-r--r--   0 rmasini    (501) staff       (20)     2449 2023-06-21 02:45:20.022750 rdpower-1.0.0/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)     1967 2023-06-21 02:21:35.000000 rdpower-1.0.0/README.md
--rw-r--r--   0 rmasini    (501) staff       (20)      108 2023-06-21 02:38:51.000000 rdpower-1.0.0/pyproject.toml
--rw-r--r--   0 rmasini    (501) staff       (20)      679 2023-06-21 02:45:20.023891 rdpower-1.0.0/setup.cfg
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 02:45:20.009791 rdpower-1.0.0/src/
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 02:45:20.018088 rdpower-1.0.0/src/rdpower/
--rw-r--r--   0 rmasini    (501) staff       (20)      153 2023-06-18 21:52:00.000000 rdpower-1.0.0/src/rdpower/__init__.py
--rw-r--r--   0 rmasini    (501) staff       (20)    19699 2023-06-21 02:44:14.000000 rdpower-1.0.0/src/rdpower/rdmde.py
--rw-r--r--   0 rmasini    (501) staff       (20)    20074 2023-06-21 02:44:29.000000 rdpower-1.0.0/src/rdpower/rdpower.py
--rw-r--r--   0 rmasini    (501) staff       (20)     3241 2023-06-18 21:49:42.000000 rdpower-1.0.0/src/rdpower/rdpower_fun.py
--rw-r--r--   0 rmasini    (501) staff       (20)    21602 2023-06-21 02:44:24.000000 rdpower-1.0.0/src/rdpower/rdsampsi.py
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 02:45:20.022064 rdpower-1.0.0/src/rdpower.egg-info/
--rw-r--r--   0 rmasini    (501) staff       (20)     2449 2023-06-21 02:45:19.000000 rdpower-1.0.0/src/rdpower.egg-info/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)      327 2023-06-21 02:45:20.000000 rdpower-1.0.0/src/rdpower.egg-info/SOURCES.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-21 02:45:19.000000 rdpower-1.0.0/src/rdpower.egg-info/dependency_links.txt
--rw-r--r--   0 rmasini    (501) staff       (20)       28 2023-06-21 02:45:19.000000 rdpower-1.0.0/src/rdpower.egg-info/requires.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        8 2023-06-21 02:45:19.000000 rdpower-1.0.0/src/rdpower.egg-info/top_level.txt
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 17:29:27.817705 rdpower-1.0.1/
+-rw-r--r--   0 rmasini    (501) staff       (20)     2492 2023-06-21 17:29:27.817922 rdpower-1.0.1/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)     2010 2023-06-21 17:27:20.000000 rdpower-1.0.1/README.md
+-rw-r--r--   0 rmasini    (501) staff       (20)      108 2023-06-21 02:38:51.000000 rdpower-1.0.1/pyproject.toml
+-rw-r--r--   0 rmasini    (501) staff       (20)      679 2023-06-21 17:29:27.818750 rdpower-1.0.1/setup.cfg
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 17:29:27.805175 rdpower-1.0.1/src/
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 17:29:27.813135 rdpower-1.0.1/src/rdpower/
+-rw-r--r--   0 rmasini    (501) staff       (20)      153 2023-06-18 21:52:00.000000 rdpower-1.0.1/src/rdpower/__init__.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    19699 2023-06-21 02:44:14.000000 rdpower-1.0.1/src/rdpower/rdmde.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    20074 2023-06-21 02:44:29.000000 rdpower-1.0.1/src/rdpower/rdpower.py
+-rw-r--r--   0 rmasini    (501) staff       (20)     3241 2023-06-18 21:49:42.000000 rdpower-1.0.1/src/rdpower/rdpower_fun.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    21602 2023-06-21 02:44:24.000000 rdpower-1.0.1/src/rdpower/rdsampsi.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-21 17:29:27.817179 rdpower-1.0.1/src/rdpower.egg-info/
+-rw-r--r--   0 rmasini    (501) staff       (20)     2492 2023-06-21 17:29:27.000000 rdpower-1.0.1/src/rdpower.egg-info/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)      327 2023-06-21 17:29:27.000000 rdpower-1.0.1/src/rdpower.egg-info/SOURCES.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-21 17:29:27.000000 rdpower-1.0.1/src/rdpower.egg-info/dependency_links.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)       28 2023-06-21 17:29:27.000000 rdpower-1.0.1/src/rdpower.egg-info/requires.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        8 2023-06-21 17:29:27.000000 rdpower-1.0.1/src/rdpower.egg-info/top_level.txt
```

### Comparing `rdpower-1.0.0/PKG-INFO` & `rdpower-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rdpower
-Version: 1.0.0
+Version: 1.0.1
 Summary: Power Calculations for RD Designs
 Home-page: https://github.com/rdpackages/rdpower
 Author: Ricardo Masini
 Author-email: rmasini@ucdavis.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdpower/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # rdpower: Power and Sample Size Calculations for RD Designs
 
-The regression discontinuity (RD) design is a popular quasi-experimental design for causal inference and policy evaluation. The `rdpower` package provides tools to perform power, sample size and MDE calculations in RD designs: `rdpower` calculates the power of an RD design, `rdsampsi` calculates the required sample size to achieve a desired power and `rdmde` calculates minimum detectable effects. This package relies on the `rdrobust` package. See Calonico, Cattaneo and Titiunik (2014, 2015) and Calonico, Cattaneo, Farrell and Titiunik (2017). For more details visit \url{https://rdpackages.github.io/}.
+The regression discontinuity (RD) design is a popular quasi-experimental design for causal inference and policy evaluation. The `rdpower` package provides tools to perform power, sample size and MDE calculations in RD designs: `rdpower` calculates the power of an RD design, `rdsampsi` calculates the required sample size to achieve a desired power and `rdmde` calculates minimum detectable effects. This package relies on the `rdrobust` package. See Calonico, Cattaneo and Titiunik (2014, 2015) and Calonico, Cattaneo, Farrell and Titiunik (2017). For more details visit [https://rdpackages.github.io/rdpower/](https://rdpackages.github.io/rdpower/).
 
 ## References
 
 - Calonico, S., M. D. Cattaneo, M. Farrell and R. Titiunik. (2017). [`rdrobust`: Software for Regression Discontinuity Designs](https://rdpackages.github.io/references/Calonico-Cattaneo-Farrell-Titiunik_2017_Stata.pdf). *Stata Journal* 17(2): 372-404.
 
 - Calonico, S., M. D. Cattaneo, and R. Titiunik. (2014). [`Robust Data-Driven Inference in the Regression-Discontinuity Design`](https://rdpackages.github.io/references/Calonico-Cattaneo-Titiunik_2014_Stata.pdf). *Stata Journal* 14(4): 909-946.
```

### Comparing `rdpower-1.0.0/README.md` & `rdpower-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # rdpower: Power and Sample Size Calculations for RD Designs
 
-The regression discontinuity (RD) design is a popular quasi-experimental design for causal inference and policy evaluation. The `rdpower` package provides tools to perform power, sample size and MDE calculations in RD designs: `rdpower` calculates the power of an RD design, `rdsampsi` calculates the required sample size to achieve a desired power and `rdmde` calculates minimum detectable effects. This package relies on the `rdrobust` package. See Calonico, Cattaneo and Titiunik (2014, 2015) and Calonico, Cattaneo, Farrell and Titiunik (2017). For more details visit \url{https://rdpackages.github.io/}.
+The regression discontinuity (RD) design is a popular quasi-experimental design for causal inference and policy evaluation. The `rdpower` package provides tools to perform power, sample size and MDE calculations in RD designs: `rdpower` calculates the power of an RD design, `rdsampsi` calculates the required sample size to achieve a desired power and `rdmde` calculates minimum detectable effects. This package relies on the `rdrobust` package. See Calonico, Cattaneo and Titiunik (2014, 2015) and Calonico, Cattaneo, Farrell and Titiunik (2017). For more details visit [https://rdpackages.github.io/rdpower/](https://rdpackages.github.io/rdpower/).
 
 ## References
 
 - Calonico, S., M. D. Cattaneo, M. Farrell and R. Titiunik. (2017). [`rdrobust`: Software for Regression Discontinuity Designs](https://rdpackages.github.io/references/Calonico-Cattaneo-Farrell-Titiunik_2017_Stata.pdf). *Stata Journal* 17(2): 372-404.
 
 - Calonico, S., M. D. Cattaneo, and R. Titiunik. (2014). [`Robust Data-Driven Inference in the Regression-Discontinuity Design`](https://rdpackages.github.io/references/Calonico-Cattaneo-Titiunik_2014_Stata.pdf). *Stata Journal* 14(4): 909-946.
```

### Comparing `rdpower-1.0.0/setup.cfg` & `rdpower-1.0.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rdpower
-version = 1.0.0
+version = 1.0.1
 author = Ricardo Masini
 author_email = rmasini@ucdavis.edu
 description = Power Calculations for RD Designs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rdpackages/rdpower
 project_urls =
```

### Comparing `rdpower-1.0.0/src/rdpower/rdmde.py` & `rdpower-1.0.1/src/rdpower/rdmde.py`

 * *Files identical despite different names*

### Comparing `rdpower-1.0.0/src/rdpower/rdpower.py` & `rdpower-1.0.1/src/rdpower/rdpower.py`

 * *Files identical despite different names*

### Comparing `rdpower-1.0.0/src/rdpower/rdpower_fun.py` & `rdpower-1.0.1/src/rdpower/rdpower_fun.py`

 * *Files identical despite different names*

### Comparing `rdpower-1.0.0/src/rdpower/rdsampsi.py` & `rdpower-1.0.1/src/rdpower/rdsampsi.py`

 * *Files identical despite different names*

### Comparing `rdpower-1.0.0/src/rdpower.egg-info/PKG-INFO` & `rdpower-1.0.1/src/rdpower.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rdpower
-Version: 1.0.0
+Version: 1.0.1
 Summary: Power Calculations for RD Designs
 Home-page: https://github.com/rdpackages/rdpower
 Author: Ricardo Masini
 Author-email: rmasini@ucdavis.edu
 Project-URL: Bug Tracker, https://github.com/rdpackages/rdpower/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # rdpower: Power and Sample Size Calculations for RD Designs
 
-The regression discontinuity (RD) design is a popular quasi-experimental design for causal inference and policy evaluation. The `rdpower` package provides tools to perform power, sample size and MDE calculations in RD designs: `rdpower` calculates the power of an RD design, `rdsampsi` calculates the required sample size to achieve a desired power and `rdmde` calculates minimum detectable effects. This package relies on the `rdrobust` package. See Calonico, Cattaneo and Titiunik (2014, 2015) and Calonico, Cattaneo, Farrell and Titiunik (2017). For more details visit \url{https://rdpackages.github.io/}.
+The regression discontinuity (RD) design is a popular quasi-experimental design for causal inference and policy evaluation. The `rdpower` package provides tools to perform power, sample size and MDE calculations in RD designs: `rdpower` calculates the power of an RD design, `rdsampsi` calculates the required sample size to achieve a desired power and `rdmde` calculates minimum detectable effects. This package relies on the `rdrobust` package. See Calonico, Cattaneo and Titiunik (2014, 2015) and Calonico, Cattaneo, Farrell and Titiunik (2017). For more details visit [https://rdpackages.github.io/rdpower/](https://rdpackages.github.io/rdpower/).
 
 ## References
 
 - Calonico, S., M. D. Cattaneo, M. Farrell and R. Titiunik. (2017). [`rdrobust`: Software for Regression Discontinuity Designs](https://rdpackages.github.io/references/Calonico-Cattaneo-Farrell-Titiunik_2017_Stata.pdf). *Stata Journal* 17(2): 372-404.
 
 - Calonico, S., M. D. Cattaneo, and R. Titiunik. (2014). [`Robust Data-Driven Inference in the Regression-Discontinuity Design`](https://rdpackages.github.io/references/Calonico-Cattaneo-Titiunik_2014_Stata.pdf). *Stata Journal* 14(4): 909-946.
```

