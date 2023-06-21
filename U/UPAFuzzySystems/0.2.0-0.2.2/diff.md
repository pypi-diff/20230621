# Comparing `tmp/UPAFuzzySystems-0.2.0.tar.gz` & `tmp/UPAFuzzySystems-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UPAFuzzySystems-0.2.0.tar", last modified: Thu Jan 12 16:01:51 2023, max compression
+gzip compressed data, was "UPAFuzzySystems-0.2.2.tar", last modified: Wed Jun 21 16:47:30 2023, max compression
```

## Comparing `UPAFuzzySystems-0.2.0.tar` & `UPAFuzzySystems-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 16:01:50.996456 UPAFuzzySystems-0.2.0/
--rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1073 2023-01-12 16:01:50.995463 UPAFuzzySystems-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2023-01-12 15:06:46.000000 UPAFuzzySystems-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 16:01:50.965539 UPAFuzzySystems-0.2.0/UPAFuzzySystems/
--rw-rw-rw-   0        0        0    34230 2023-01-10 21:49:58.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems/UPAFuzzySystems.py
--rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:01:50.993463 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/
--rw-rw-rw-   0        0        0     1073 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-12 16:01:50.996456 UPAFuzzySystems-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1462 2023-01-12 15:56:10.000000 UPAFuzzySystems-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:47:30.130203 UPAFuzzySystems-0.2.2/
+-rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2498 2023-06-21 16:47:30.128144 UPAFuzzySystems-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1616 2023-06-21 16:45:02.000000 UPAFuzzySystems-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 16:47:30.059993 UPAFuzzySystems-0.2.2/UPAFuzzySystems/
+-rw-rw-rw-   0        0        0    34335 2023-06-21 15:14:44.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems/UPAFuzzySystems.py
+-rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:47:30.118870 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/
+-rw-rw-rw-   0        0        0     2498 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 16:47:30.131203 UPAFuzzySystems-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-06-21 16:46:39.000000 UPAFuzzySystems-0.2.2/setup.py
```

### Comparing `UPAFuzzySystems-0.2.0/LICENSE` & `UPAFuzzySystems-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UPAFuzzySystems-0.2.0/README.md` & `UPAFuzzySystems-0.2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 <h1 align="center">
-<img src="upa.png" width="300">
+<img src="https://sii.upa.edu.mx/image/icono/logo_upp.png" width="300">
 </h1><br>
 
-
-
 [![PyPI Downloads](https://img.shields.io/pypi/dm/UPAFuzzySystems.svg?label=PyPI%20downloads)](
 https://pypi.org/project/UPAFuzzySystems/)
 
 # UPAFuzzySystems
 
 UPAFuzzySystems library that allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for the simulation of fuzzy control with transfer functions and state space models.
 
 ***Developed by Dr. Martín Montes Rivera***
 
 # Installation
 For installation, just run the command:
 
 ```
-pip install UPAFuzzySystems==0.2.0
+pip install UPAFuzzySystems==0.2.2
 ```
 # Documentation
 For now check the Jupyter Notebook notebook, PDF or HTML examples for using the UPAFuzzySystems library.
 
 [Jupyter notebook](https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/blob/main/examples/Examples-UPAFuzzySystems.ipynb)
 
 [PDF](https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/blob/main/examples/Examples-UPAFuzzySystems.pdf)
 
 [HTML](https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/blob/main/examples/Examples-UPAFuzzySystems.html)
 
+[Other examples](https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/tree/main/examples/other%20examples)
+
+# Please cite as:
+Have you found this software useful for your research?  Please cite it as:
+
+Montes Rivera, M.; Olvera-Gonzalez, E.; Escalante-Garcia, N. UPAFuzzySystems: A Python Library for Control and Simulation with Fuzzy Inference Systems. Machines 2023, 11, 572. https://doi.org/10.3390/machines11050572
```

### Comparing `UPAFuzzySystems-0.2.0/UPAFuzzySystems/UPAFuzzySystems.py` & `UPAFuzzySystems-0.2.2/UPAFuzzySystems/UPAFuzzySystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         """
         membershipvalues=[]
         X = self.structure['universe']
         membershipfuntion = self.structure[name][0]
         vertices = self.structure[name][1]
         if membershipfuntion =='gaussmf':
             exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertices[0])+','+str(vertices[1])+'))')
+        elif membershipfuntion == 'raw':
+             exec('membershipvalues.append('+str(vertices)+')')
         else:
             exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertices)+'))')
         return {'universe':X,'membership values':membershipvalues[0]}
     def view_fuzzy(self):
 
         """Plots the the corresponding universe with all its fuzzy sets.
```

### Comparing `UPAFuzzySystems-0.2.0/setup.py` & `UPAFuzzySystems-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.2.0'
+VERSION = '0.2.2'
 DESCRIPTION = 'UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.'
 LONG_DESCRIPTION = 'UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.'
+with open('README.md', 'r', encoding='utf-8') as file:
+    LONG_DESCRIPTION = file.read()
 
 # Setting up
 setup(
     name="UPAFuzzySystems",
     version=VERSION,
     author="Dr. Martin Montes Rivera (Universidad Politécnica de Aguascalientes)",
     author_email="<martin.montes@upa.edu.mx>",
     url='https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/',
     description=DESCRIPTION,
+    license='MIT',
     license_files = ('LICENSE',),
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['numpy', 'matplotlib', 'control','scikit-fuzzy'],
     keywords=['python', 'fuzzy logic', 'fuzzy control', 'fuzzy inference systems', 'artificial intelligence'],
     classifiers=[
```

