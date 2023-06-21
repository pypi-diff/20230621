# Comparing `tmp/panels-0.3.0.tar.gz` & `tmp/panels-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panels-0.3.0.tar", last modified: Wed Jun 21 09:21:18 2023, max compression
+gzip compressed data, was "panels-0.3.1.tar", last modified: Wed Jun 21 10:12:58 2023, max compression
```

## Comparing `panels-0.3.0.tar` & `panels-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:21:18.747223 panels-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-21 09:20:47.000000 panels-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-21 09:21:18.747223 panels-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-21 09:20:47.000000 panels-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:21:18.747223 panels-0.3.0/panels/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-21 09:20:47.000000 panels-0.3.0/panels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:21:18.735222 panels-0.3.0/panels/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:21:18.739222 panels-0.3.0/panels/core/src/
--rw-r--r--   0 runner    (1001) docker     (123)    42878 2023-06-21 09:20:47.000000 panels-0.3.0/panels/core/src/bardell_functions_uv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    43984 2023-06-21 09:20:47.000000 panels-0.3.0/panels/core/src/bardell_functions_w.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   332246 2023-06-21 09:20:47.000000 panels-0.3.0/panels/core/src/legendre_gauss_quadrature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:21:18.747223 panels-0.3.0/panels/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-21 09:20:47.000000 panels-0.3.0/panels/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-21 09:20:47.000000 panels-0.3.0/panels/dev/matrixtools.py
--rw-r--r--   0 runner    (1001) docker     (123)   856789 2023-06-21 09:21:14.000000 panels-0.3.0/panels/legendre_gauss_quadrature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-21 09:20:47.000000 panels-0.3.0/panels/legendre_gauss_quadrature.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-21 09:20:47.000000 panels-0.3.0/panels/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-21 09:20:47.000000 panels-0.3.0/panels/modelDB.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:21:18.747223 panels-0.3.0/panels/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-21 09:20:47.000000 panels-0.3.0/panels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1167819 2023-06-21 09:21:15.000000 panels-0.3.0/panels/models/clpt_bardell_field.cpp
--rw-r--r--   0 runner    (1001) docker     (123)  1095711 2023-06-21 09:21:16.000000 panels-0.3.0/panels/models/coneshell_clpt_donnell_bardell_num.cpp
--rw-r--r--   0 runner    (1001) docker     (123)  1426810 2023-06-21 09:21:17.000000 panels-0.3.0/panels/models/cylshell_clpt_donnell_bardell_num.cpp
--rw-r--r--   0 runner    (1001) docker     (123)  1566524 2023-06-21 09:21:18.000000 panels-0.3.0/panels/models/plate_clpt_donnell_bardell_num.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-21 09:20:47.000000 panels-0.3.0/panels/plot_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    37098 2023-06-21 09:20:47.000000 panels-0.3.0/panels/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-21 09:20:47.000000 panels-0.3.0/panels/shell_fext.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 09:21:13.000000 panels-0.3.0/panels/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:21:18.747223 panels-0.3.0/panels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-21 09:21:18.000000 panels-0.3.0/panels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-21 09:21:18.000000 panels-0.3.0/panels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:21:18.000000 panels-0.3.0/panels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 09:21:18.000000 panels-0.3.0/panels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 09:21:18.000000 panels-0.3.0/panels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 09:20:47.000000 panels-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:21:18.747223 panels-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-21 09:20:47.000000 panels-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.827125 panels-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-21 10:12:22.000000 panels-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-21 10:12:58.827125 panels-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-21 10:12:22.000000 panels-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.823125 panels-0.3.1/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-21 10:12:22.000000 panels-0.3.1/panels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.815125 panels-0.3.1/panels/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.823125 panels-0.3.1/panels/core/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 10:12:22.000000 panels-0.3.1/panels/core/include/bardell_functions_uv.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 10:12:22.000000 panels-0.3.1/panels/core/include/bardell_functions_w.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 10:12:22.000000 panels-0.3.1/panels/core/include/legendre_gauss_quadrature.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.815125 panels-0.3.1/panels/core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    42878 2023-06-21 10:12:22.000000 panels-0.3.1/panels/core/src/bardell_functions_uv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43984 2023-06-21 10:12:22.000000 panels-0.3.1/panels/core/src/bardell_functions_w.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   332246 2023-06-21 10:12:22.000000 panels-0.3.1/panels/core/src/legendre_gauss_quadrature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.823125 panels-0.3.1/panels/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-21 10:12:22.000000 panels-0.3.1/panels/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-21 10:12:22.000000 panels-0.3.1/panels/dev/matrixtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)   856789 2023-06-21 10:12:54.000000 panels-0.3.1/panels/legendre_gauss_quadrature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-21 10:12:22.000000 panels-0.3.1/panels/legendre_gauss_quadrature.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-21 10:12:22.000000 panels-0.3.1/panels/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-21 10:12:22.000000 panels-0.3.1/panels/modelDB.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.823125 panels-0.3.1/panels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-21 10:12:22.000000 panels-0.3.1/panels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1167819 2023-06-21 10:12:55.000000 panels-0.3.1/panels/models/clpt_bardell_field.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-06-21 10:12:22.000000 panels-0.3.1/panels/models/clpt_bardell_field.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1095711 2023-06-21 10:12:56.000000 panels-0.3.1/panels/models/coneshell_clpt_donnell_bardell_num.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31241 2023-06-21 10:12:22.000000 panels-0.3.1/panels/models/coneshell_clpt_donnell_bardell_num.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1426810 2023-06-21 10:12:57.000000 panels-0.3.1/panels/models/cylshell_clpt_donnell_bardell_num.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    37361 2023-06-21 10:12:22.000000 panels-0.3.1/panels/models/cylshell_clpt_donnell_bardell_num.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1566524 2023-06-21 10:12:58.000000 panels-0.3.1/panels/models/plate_clpt_donnell_bardell_num.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44840 2023-06-21 10:12:22.000000 panels-0.3.1/panels/models/plate_clpt_donnell_bardell_num.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-21 10:12:22.000000 panels-0.3.1/panels/plot_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37098 2023-06-21 10:12:22.000000 panels-0.3.1/panels/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-21 10:12:22.000000 panels-0.3.1/panels/shell_fext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 10:12:52.000000 panels-0.3.1/panels/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:12:58.823125 panels-0.3.1/panels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-21 10:12:58.000000 panels-0.3.1/panels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-21 10:12:58.000000 panels-0.3.1/panels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:12:58.000000 panels-0.3.1/panels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 10:12:58.000000 panels-0.3.1/panels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 10:12:58.000000 panels-0.3.1/panels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 10:12:22.000000 panels-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:12:58.827125 panels-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-21 10:12:22.000000 panels-0.3.1/setup.py
```

### Comparing `panels-0.3.0/LICENSE` & `panels-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/PKG-INFO` & `panels-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panels
-Version: 0.3.0
+Version: 0.3.1
 Summary: Semi-analytical models for plates, shells, stiffened panels
 Home-page: https://github.com/saullocastro/panels
 Author: Saullo G. P. Castro
 Author-email: S.G.P.Castro@tudelft.nl
 License: 3-Clause BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `panels-0.3.0/README.md` & `panels-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/core/src/bardell_functions_uv.cpp` & `panels-0.3.1/panels/core/src/bardell_functions_uv.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/core/src/bardell_functions_w.cpp` & `panels-0.3.1/panels/core/src/bardell_functions_w.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/core/src/legendre_gauss_quadrature.cpp` & `panels-0.3.1/panels/core/src/legendre_gauss_quadrature.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/dev/matrixtools.py` & `panels-0.3.1/panels/dev/matrixtools.py`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/legendre_gauss_quadrature.cpp` & `panels-0.3.1/panels/legendre_gauss_quadrature.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/modelDB.py` & `panels-0.3.1/panels/modelDB.py`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/models/__init__.py` & `panels-0.3.1/panels/models/__init__.py`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/models/clpt_bardell_field.cpp` & `panels-0.3.1/panels/models/clpt_bardell_field.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/models/coneshell_clpt_donnell_bardell_num.cpp` & `panels-0.3.1/panels/models/coneshell_clpt_donnell_bardell_num.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/models/cylshell_clpt_donnell_bardell_num.cpp` & `panels-0.3.1/panels/models/cylshell_clpt_donnell_bardell_num.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/models/plate_clpt_donnell_bardell_num.cpp` & `panels-0.3.1/panels/models/plate_clpt_donnell_bardell_num.cpp`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/plot_shell.py` & `panels-0.3.1/panels/plot_shell.py`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/shell.py` & `panels-0.3.1/panels/shell.py`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels/shell_fext.py` & `panels-0.3.1/panels/shell_fext.py`

 * *Files identical despite different names*

### Comparing `panels-0.3.0/panels.egg-info/PKG-INFO` & `panels-0.3.1/panels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panels
-Version: 0.3.0
+Version: 0.3.1
 Summary: Semi-analytical models for plates, shells, stiffened panels
 Home-page: https://github.com/saullocastro/panels
 Author: Saullo G. P. Castro
 Author-email: S.G.P.Castro@tudelft.nl
 License: 3-Clause BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `panels-0.3.0/panels.egg-info/SOURCES.txt` & `panels-0.3.1/panels.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,10 +19,20 @@
 panels/shell_fext.py
 panels/version.py
 panels.egg-info/PKG-INFO
 panels.egg-info/SOURCES.txt
 panels.egg-info/dependency_links.txt
 panels.egg-info/requires.txt
 panels.egg-info/top_level.txt
+panels/core/include/bardell_functions_uv.hpp
+panels/core/include/bardell_functions_w.hpp
+panels/core/include/legendre_gauss_quadrature.hpp
+panels/core/src/bardell_functions_uv.cpp
+panels/core/src/bardell_functions_w.cpp
+panels/core/src/legendre_gauss_quadrature.cpp
 panels/dev/__init__.py
 panels/dev/matrixtools.py
-panels/models/__init__.py
+panels/models/__init__.py
+panels/models/clpt_bardell_field.pyx
+panels/models/coneshell_clpt_donnell_bardell_num.pyx
+panels/models/cylshell_clpt_donnell_bardell_num.pyx
+panels/models/plate_clpt_donnell_bardell_num.pyx
```

### Comparing `panels-0.3.0/setup.py` & `panels-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Programming Language :: Python :: 3.11
 License :: OSI Approved :: BSD License
 
 """
 
 MAJOR = 0
 MINOR = 3
-MICRO = 0
+MICRO = 1
 ISRELEASED = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 
 def write_version_py(filename='panels/version.py'):
     cnt = """# This file is generated automatically by the setup.py
 short_version = '%(version)s'
@@ -192,17 +192,20 @@
 
 data_files = [('', [
         'README.md',
         'LICENSE',
         ])]
 
 package_data = {
-        'panels': ['*.py', '*.pxd', '*.pyx'],
-        'panels/models': ['*.py', '*.pxd', '*.pyx'],
-        'panels/tests/tests_shell': ['*.py'],
+        'panels': ['*.py', '*.pxd', '*.pyx',
+                   'core/include/*.hpp',
+                   'core/src/*.cpp',
+                   'models/*.pyx', 'models/*.pxd'
+                   'tests/tests_shell/*.py'
+                   ],
         }
 
 setup(
     name = 'panels',
     version = FULLVERSION,
     author = 'Saullo G. P. Castro',
     author_email = 'S.G.P.Castro@tudelft.nl',
```

