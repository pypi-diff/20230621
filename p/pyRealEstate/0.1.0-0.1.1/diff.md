# Comparing `tmp/pyRealEstate-0.1.0.tar.gz` & `tmp/pyRealEstate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.1.0.tar", last modified: Tue Jun 20 19:00:39 2023, max compression
+gzip compressed data, was "pyRealEstate-0.1.1.tar", last modified: Tue Jun 20 23:52:10 2023, max compression
```

## Comparing `pyRealEstate-0.1.0.tar` & `pyRealEstate-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/Pre_Processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/Time_Trending.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 19:00:39.000000 pyRealEstate-0.1.0/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 19:00:23.000000 pyRealEstate-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-20 19:00:39.082808 pyRealEstate-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/Pre_Processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/Time_Trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 23:52:10.000000 pyRealEstate-0.1.1/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 23:51:55.000000 pyRealEstate-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 23:52:10.453568 pyRealEstate-0.1.1/setup.cfg
```

### Comparing `pyRealEstate-0.1.0/LICENSE` & `pyRealEstate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.0/PKG-INFO` & `pyRealEstate-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.1.0
+Version: 0.1.1
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.1.0/README.md` & `pyRealEstate-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.0/pyRealEstate/Pre_Processing.py` & `pyRealEstate-0.1.1/pyRealEstate/Pre_Processing.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.0/pyRealEstate/RealEstateMetrics.py` & `pyRealEstate-0.1.1/pyRealEstate/RealEstateMetrics.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.0/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.1.1/pyRealEstate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.1.0
+Version: 0.1.1
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.1.0/pypi_description.md` & `pyRealEstate-0.1.1/pypi_description.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.1.0/setup.cfg` & `pyRealEstate-0.1.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.1.0
+version = 0.1.1
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 
 [options]
 install_requires = scikit-learn
 	numpy
 	pandas
 	statsmodels
 	matplotlib
+	lightgbm
 packages = find:
 python_requires = >=3.4
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

