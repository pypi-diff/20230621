# Comparing `tmp/idsred-0.1.0.tar.gz` & `tmp/idsred-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idsred-0.1.0.tar", last modified: Tue Apr 18 08:53:11 2023, max compression
+gzip compressed data, was "idsred-0.1.1.tar", last modified: Wed Jun 21 11:50:27 2023, max compression
```

## Comparing `idsred-0.1.0.tar` & `idsred-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-18 08:53:11.847826 idsred-0.1.0/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      100 2023-04-18 08:53:01.000000 idsred-0.1.0/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2089 2023-04-18 08:53:11.843826 idsred-0.1.0/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1649 2023-04-18 08:44:10.000000 idsred-0.1.0/README.md
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-18 08:53:11.839827 idsred-0.1.0/idsred/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      282 2022-12-22 15:44:33.000000 idsred-0.1.0/idsred/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2022-12-22 15:44:33.000000 idsred-0.1.0/idsred/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      272 2022-12-22 15:44:33.000000 idsred-0.1.0/idsred/env.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-18 08:53:11.839827 idsred-0.1.0/idsred/extinction/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1486 2023-01-12 19:49:19.000000 idsred-0.1.0/idsred/extinction/lapalmaext.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17781 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/fluxcalib.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-18 08:53:11.839827 idsred-0.1.0/idsred/lamps/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6918 2022-12-06 09:42:16.000000 idsred-0.1.0/idsred/lamps/CuArNe_high.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1976 2022-12-06 09:42:16.000000 idsred-0.1.0/idsred/lamps/CuArNe_low.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4253 2022-12-06 09:42:16.000000 idsred-0.1.0/idsred/lamps/CuAr_high.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1287 2022-12-06 09:42:16.000000 idsred-0.1.0/idsred/lamps/CuAr_low.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2048 2022-12-06 09:42:16.000000 idsred-0.1.0/idsred/lamps/CuNe_high.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      689 2022-12-06 09:42:16.000000 idsred-0.1.0/idsred/lamps/CuNe_low.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      768 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/lamps/init_wavesol.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2350 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/lamps/init_wavesol_no_timming.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15187 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/spec1Dreduc.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17474 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/spec2Dreduc.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-18 08:53:11.843826 idsred-0.1.0/idsred/standards/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1737 2023-03-07 14:10:49.000000 idsred-0.1.0/idsred/standards/bd17.og
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1044 2022-12-06 14:53:23.000000 idsred-0.1.0/idsred/standards/bd253.sto
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      864 2022-12-06 09:42:24.000000 idsred-0.1.0/idsred/standards/bd253a.sto
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    75467 2023-03-07 14:17:59.000000 idsred-0.1.0/idsred/standards/bd254.oke
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    75464 2023-02-27 15:24:20.000000 idsred-0.1.0/idsred/standards/bd75.oke
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1026 2023-03-07 14:27:51.000000 idsred-0.1.0/idsred/standards/f25.sto
--rw-rw-r--   0 tomas     (1000) tomas     (1000)  3120022 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/standards/fGD153.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)  3120022 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/standards/fGD71.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      855 2022-12-06 14:55:27.000000 idsred-0.1.0/idsred/standards/h102a.sto
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      977 2023-03-07 14:24:44.000000 idsred-0.1.0/idsred/standards/h600.sto
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1170 2022-12-06 09:42:24.000000 idsred-0.1.0/idsred/standards/hd194a.og
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1705 2023-03-07 14:12:24.000000 idsred-0.1.0/idsred/standards/hd849.og
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      224 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/standards/standards.json
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4816 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/standards/w1346.oke
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3397 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/utils.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    27160 2023-04-18 08:42:07.000000 idsred-0.1.0/idsred/wavecalib.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-18 08:53:11.839827 idsred-0.1.0/idsred.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2089 2023-04-18 08:53:11.000000 idsred-0.1.0/idsred.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1008 2023-04-18 08:53:11.000000 idsred-0.1.0/idsred.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-04-18 08:53:11.000000 idsred-0.1.0/idsred.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       70 2023-04-18 08:53:11.000000 idsred-0.1.0/idsred.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        7 2023-04-18 08:53:11.000000 idsred-0.1.0/idsred.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      116 2022-12-06 09:52:03.000000 idsred-0.1.0/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       70 2023-04-18 08:48:21.000000 idsred-0.1.0/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-04-18 08:53:11.847826 idsred-0.1.0/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1129 2023-04-18 08:50:36.000000 idsred-0.1.0/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-21 11:50:27.119571 idsred-0.1.1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      100 2023-04-18 08:53:01.000000 idsred-0.1.1/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2560 2023-06-21 11:50:27.115571 idsred-0.1.1/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2120 2023-04-21 08:44:34.000000 idsred-0.1.1/README.md
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-21 11:50:27.071571 idsred-0.1.1/idsred/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      282 2022-12-22 15:44:33.000000 idsred-0.1.1/idsred/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-06-21 11:47:16.000000 idsred-0.1.1/idsred/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      272 2022-12-22 15:44:33.000000 idsred-0.1.1/idsred/env.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-21 11:50:27.075571 idsred-0.1.1/idsred/extinction/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1486 2023-01-12 19:49:19.000000 idsred-0.1.1/idsred/extinction/lapalmaext.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17971 2023-06-21 11:46:07.000000 idsred-0.1.1/idsred/fluxcalib.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-21 11:50:27.091571 idsred-0.1.1/idsred/lamps/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6918 2022-12-06 09:42:16.000000 idsred-0.1.1/idsred/lamps/CuArNe_high.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1976 2022-12-06 09:42:16.000000 idsred-0.1.1/idsred/lamps/CuArNe_low.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4253 2022-12-06 09:42:16.000000 idsred-0.1.1/idsred/lamps/CuAr_high.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1287 2022-12-06 09:42:16.000000 idsred-0.1.1/idsred/lamps/CuAr_low.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2048 2022-12-06 09:42:16.000000 idsred-0.1.1/idsred/lamps/CuNe_high.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      689 2022-12-06 09:42:16.000000 idsred-0.1.1/idsred/lamps/CuNe_low.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      768 2023-04-18 08:42:07.000000 idsred-0.1.1/idsred/lamps/init_wavesol.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2350 2023-04-18 08:42:07.000000 idsred-0.1.1/idsred/lamps/init_wavesol_no_timming.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15211 2023-06-18 14:28:53.000000 idsred-0.1.1/idsred/spec1Dreduc.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17851 2023-06-21 11:08:49.000000 idsred-0.1.1/idsred/spec2Dreduc.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-21 11:50:27.115571 idsred-0.1.1/idsred/standards/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1737 2023-03-07 14:10:49.000000 idsred-0.1.1/idsred/standards/bd17.og
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1044 2022-12-06 14:53:23.000000 idsred-0.1.1/idsred/standards/bd253.sto
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      864 2022-12-06 09:42:24.000000 idsred-0.1.1/idsred/standards/bd253a.sto
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    75467 2023-03-07 14:17:59.000000 idsred-0.1.1/idsred/standards/bd254.oke
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    75464 2023-02-27 15:24:20.000000 idsred-0.1.1/idsred/standards/bd75.oke
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1026 2023-03-07 14:27:51.000000 idsred-0.1.1/idsred/standards/f25.sto
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)  3120023 2023-05-31 11:28:19.000000 idsred-0.1.1/idsred/standards/fFEIGE110.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)  3120022 2023-04-18 08:42:07.000000 idsred-0.1.1/idsred/standards/fGD153.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)  3120022 2023-04-18 08:42:07.000000 idsred-0.1.1/idsred/standards/fGD71.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    75497 2023-04-21 09:46:24.000000 idsred-0.1.1/idsred/standards/g191anew.oke
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      855 2022-12-06 14:55:27.000000 idsred-0.1.1/idsred/standards/h102a.sto
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      977 2023-03-07 14:24:44.000000 idsred-0.1.1/idsred/standards/h600.sto
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1170 2022-12-06 09:42:24.000000 idsred-0.1.1/idsred/standards/hd194a.og
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1705 2023-03-07 14:12:24.000000 idsred-0.1.1/idsred/standards/hd849.og
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      251 2023-04-21 09:48:04.000000 idsred-0.1.1/idsred/standards/standards.json
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4816 2023-04-18 08:42:07.000000 idsred-0.1.1/idsred/standards/w1346.oke
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3397 2023-04-18 08:42:07.000000 idsred-0.1.1/idsred/utils.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    27132 2023-06-21 11:03:12.000000 idsred-0.1.1/idsred/wavecalib.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-21 11:50:27.075571 idsred-0.1.1/idsred.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2560 2023-06-21 11:50:27.000000 idsred-0.1.1/idsred.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1069 2023-06-21 11:50:27.000000 idsred-0.1.1/idsred.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-06-21 11:50:27.000000 idsred-0.1.1/idsred.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       70 2023-06-21 11:50:27.000000 idsred-0.1.1/idsred.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        7 2023-06-21 11:50:27.000000 idsred-0.1.1/idsred.egg-info/top_level.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      116 2022-12-06 09:52:03.000000 idsred-0.1.1/pyproject.toml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       70 2023-04-18 08:48:21.000000 idsred-0.1.1/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-06-21 11:50:27.119571 idsred-0.1.1/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1129 2023-04-18 08:50:36.000000 idsred-0.1.1/setup.py
```

### Comparing `idsred-0.1.0/PKG-INFO` & `idsred-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idsred
-Version: 0.1.0
+Version: 0.1.1
 Summary: INT-IDS data-reduction pipeline
 Home-page: https://github.com/temuller/idsred
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 This is a spectroscopic data-reduction pipeline for the Isaac Newton Telescope (INT) Intermediate Dispersion Spectrograph (IDS) instrument. 
 It is optimised for the blue detector (EEV10).
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fidsred-blue.svg?style=flat)](https://github.com/temuller/idsred)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/idsred/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/idsred?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/idsred/)
+[![DOI](https://zenodo.org/badge/574921206.svg)](https://zenodo.org/badge/latestdoi/574921206)
+
+
 
 ## Installation
 
 It is recommended to install it on an anaconda environment:
 
 ```code
 conda create -n idsred pip
@@ -55,10 +58,25 @@
 
 A notebook that explains how to use the pipeline is found in this repository [here](https://github.com/temuller/idsred/blob/main/reduction.ipynb).
 
 ## Contributing
 
 To contribute, either open an issue or send a pull request (preferred option). You can also contact me directly.
 
+## Citing IDSRED
+
+```code
+@software{tomas_e_muller_bravo_2023_7851772,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/idsred: First Release!},
+  month        = apr,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.0},
+  doi          = {10.5281/zenodo.7851772},
+  url          = {https://doi.org/10.5281/zenodo.7851772}
+}
+```
+
 ## Acknowledgement
 
 This pipeline is based on the [GROWTH school github repository](https://github.com/growth-astro/growth-school-2020), which nicely explains the entire reduction process for images and spectra, and on [INT-IDS-DataReduction](https://github.com/aayush3009/INT-IDS-DataReduction) for (long-slit) spectra reduction.
```

### Comparing `idsred-0.1.0/README.md` & `idsred-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 This is a spectroscopic data-reduction pipeline for the Isaac Newton Telescope (INT) Intermediate Dispersion Spectrograph (IDS) instrument. 
 It is optimised for the blue detector (EEV10).
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fidsred-blue.svg?style=flat)](https://github.com/temuller/idsred)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/idsred/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/idsred?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/idsred/)
+[![DOI](https://zenodo.org/badge/574921206.svg)](https://zenodo.org/badge/latestdoi/574921206)
+
+
 
 ## Installation
 
 It is recommended to install it on an anaconda environment:
 
 ```code
 conda create -n idsred pip
@@ -41,10 +44,25 @@
 
 A notebook that explains how to use the pipeline is found in this repository [here](https://github.com/temuller/idsred/blob/main/reduction.ipynb).
 
 ## Contributing
 
 To contribute, either open an issue or send a pull request (preferred option). You can also contact me directly.
 
+## Citing IDSRED
+
+```code
+@software{tomas_e_muller_bravo_2023_7851772,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/idsred: First Release!},
+  month        = apr,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.0},
+  doi          = {10.5281/zenodo.7851772},
+  url          = {https://doi.org/10.5281/zenodo.7851772}
+}
+```
+
 ## Acknowledgement
 
 This pipeline is based on the [GROWTH school github repository](https://github.com/growth-astro/growth-school-2020), which nicely explains the entire reduction process for images and spectra, and on [INT-IDS-DataReduction](https://github.com/aayush3009/INT-IDS-DataReduction) for (long-slit) spectra reduction.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idsred-0.1.0/idsred/extinction/lapalmaext.txt` & `idsred-0.1.1/idsred/extinction/lapalmaext.txt`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/fluxcalib.py` & `idsred-0.1.1/idsred/fluxcalib.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,14 +575,18 @@
 
         # apply wavelength and flux calibration
         if use_master_arc is True:
             wavesol_file = "wavesol.txt"
         else:
             wavesol_file = f"wavesol_{target_name}.txt"
         cal_wave = apply_wavesol(raw_wave, wavesol_file)
+        # correct for atmospheric extinction at Observatorio Roque de Los Muchachos
+        airmass = _calc_airmass(hdu)
+        raw_flux = _correct_extinction(cal_wave, raw_flux, airmass)
+
         cal_wave, cal_flux = apply_sensfunc(cal_wave, raw_flux)
 
         # telluric correction
         cal_flux = correct_tellurics(cal_wave, cal_flux)
 
         # apply smoothing
         if smoothing is True:
```

### Comparing `idsred-0.1.0/idsred/lamps/CuArNe_high.dat` & `idsred-0.1.1/idsred/lamps/CuArNe_high.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/lamps/CuArNe_low.dat` & `idsred-0.1.1/idsred/lamps/CuArNe_low.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/lamps/CuAr_high.dat` & `idsred-0.1.1/idsred/lamps/CuAr_high.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/lamps/CuAr_low.dat` & `idsred-0.1.1/idsred/lamps/CuAr_low.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/lamps/CuNe_high.dat` & `idsred-0.1.1/idsred/lamps/CuNe_high.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/lamps/CuNe_low.dat` & `idsred-0.1.1/idsred/lamps/CuNe_low.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/lamps/init_wavesol.txt` & `idsred-0.1.1/idsred/lamps/init_wavesol.txt`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/lamps/init_wavesol_no_timming.txt` & `idsred-0.1.1/idsred/lamps/init_wavesol_no_timming.txt`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/spec1Dreduc.py` & `idsred-0.1.1/idsred/spec1Dreduc.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,16 @@
             warnings.simplefilter("ignore", UserWarning)
             guess = (amp, center, 5, np.nanmedian(profile))
 
         results = minimize(_get_profile_chisq, guess, args=(ys, profile))
         params = results.x
         if params[2] < 20:
             ycenter[icol] = params[1]
-            ywidth[icol] = 2 * params[2]  # aperture width in sigmas units
-            bkg_width[icol] = 6 * params[2]  # beginning of bkg in sigma units
+            ywidth[icol] = 4 * params[2]  # aperture width in sigmas units
+            bkg_width[icol] = 8 * params[2]  # beginning of bkg in sigma units
             model = _get_profile_model(params, ys)
 
             # diagnostic plots for each step
             if plot_diag:
                 fig, ax = plt.subplots(figsize=(12, 6))
                 ax.plot(ys, profile, label="data")
                 ax.plot(ys, model, label="model")
@@ -285,15 +285,15 @@
     # trace aperture + background
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", UserWarning)
         trace_top = trace + np.median(ywidth)
         trace_bottom = trace - np.median(ywidth)
         bkg_top = trace + np.median(bkg_width)
         bkg_bottom = trace - np.median(bkg_width)
-        sky_width = 50
+        sky_width = 25
 
     # final diagnostic plots
     if plot_diag:
         # spline fit
         fig, ax = plt.subplots(2, figsize=(14, 4), sharex=True)
         ax[0].plot(cols, ycenter, "ro", label="data")
         ax[0].plot(xs, trace, "r", label="spline")
@@ -427,15 +427,15 @@
         ax.set_ylabel("Raw Flux", fontsize=16)
         ax.set_title(header["OBJECT"], fontsize=16)
         plt.show()
 
     return raw_spectrum
 
 
-def quick_1Dreduction(plot_diag=False, plot_trace=False):
+def quick_1Dreduction(plot_diag=False, plot_trace=False, order=3):
     """Performs a "quick" 2D image reduction.
 
     Mostly default parameters are used, but should work in most cases.
 
     Parameters
     ----------
     plot_diag: bool, default ``False``
@@ -452,15 +452,15 @@
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
             hdu = fits.open(file)
             header = hdu[0].header
 
         # extract trace
         raw_spectrum = optimised_trace(
-            hdu, plot_diag=plot_diag, plot_trace=plot_trace
+            hdu, plot_diag=plot_diag, plot_trace=plot_trace, t_order=order
         )
         hdu[0].data = raw_spectrum
         # update header
         header["NAXIS"] = 1
         header["NAXIS2"] = len(raw_spectrum)
         del header["NAXIS2"]
```

### Comparing `idsred-0.1.0/idsred/spec2Dreduc.py` & `idsred-0.1.1/idsred/spec2Dreduc.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 ccd,
                 median=True,
                 overscan_axis=0,
                 fits_section=ccd.header["BIASSEC"],
             )
         if trim_image is True:
             ccd = ccdproc.trim_image(ccd, ccd.header["TRIMSEC"])
-            # ccd = ccdproc.trim_image(ccd[360:3601, :])
+            #ccd = ccdproc.trim_image(ccd[500:3500, :])
         if master_bias is not None:
             ccd = ccdproc.subtract_bias(ccd, master_bias)
         images_list.append(ccd)
 
     return images_list
 
 
@@ -191,17 +191,30 @@
         Combined flats.
 
     Returns
     -------
     master_flat: array
         Corrected master flat.
     """
-    avcol_in = np.average(
+    avcol_in = np.nanmean(
         flat[:, 30:306].copy(), axis=1
     )  # average column value, avoiding edges
+
+    """
+    pseudo_wave = np.arange(len(avcol_in))
+    import matplotlib.pyplot as plt
+    plt.plot(pseudo_wave, avcol_in)
+    degree = 70
+    coefs = np.polyfit(pseudo_wave, np.nan_to_num(avcol_in, nan=np.nanmean(avcol_in)), degree)
+    avcol_in = np.polyval(coefs, pseudo_wave)
+    #avcol_in[avcol_in<=0] = 0.05
+    plt.plot(pseudo_wave, avcol_in)
+    plt.show()
+    """
+    
     avcol_out = np.concatenate([[avcol_in]] * flat.shape[1], axis=0).T
     master_flat = np.copy(flat / avcol_out)
 
     return master_flat
 
 
 def create_master_flat(
@@ -465,15 +478,15 @@
                         ccd,
                         median=True,
                         overscan_axis=0,
                         fits_section=ccd.header["BIASSEC"],
                     )
                 if trim_image is True:
                     ccd = ccdproc.trim_image(ccd, ccd.header["TRIMSEC"])
-                    # ccd = ccdproc.trim_image(ccd[360:3601, :])
+                    #ccd = ccdproc.trim_image(ccd[500:3500, :])
                 if master_bias is not None:
                     ccd = ccdproc.subtract_bias(ccd, master_bias)
                 if master_flat is not None:
                     ccd = ccdproc.flat_correct(
                         ccd, master_flat, min_value=0.01
                     )
```

### Comparing `idsred-0.1.0/idsred/standards/bd17.og` & `idsred-0.1.1/idsred/standards/bd17.og`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/bd253.sto` & `idsred-0.1.1/idsred/standards/bd253.sto`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/bd253a.sto` & `idsred-0.1.1/idsred/standards/bd253a.sto`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/bd254.oke` & `idsred-0.1.1/idsred/standards/bd254.oke`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/bd75.oke` & `idsred-0.1.1/idsred/standards/bd75.oke`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/f25.sto` & `idsred-0.1.1/idsred/standards/f25.sto`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/fGD153.dat` & `idsred-0.1.1/idsred/standards/fGD153.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/fGD71.dat` & `idsred-0.1.1/idsred/standards/fGD71.dat`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/h102a.sto` & `idsred-0.1.1/idsred/standards/h102a.sto`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/h600.sto` & `idsred-0.1.1/idsred/standards/h600.sto`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/hd194a.og` & `idsred-0.1.1/idsred/standards/hd194a.og`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/hd849.og` & `idsred-0.1.1/idsred/standards/hd849.og`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/standards/w1346.oke` & `idsred-0.1.1/idsred/standards/w1346.oke`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/utils.py` & `idsred-0.1.1/idsred/utils.py`

 * *Files identical despite different names*

### Comparing `idsred-0.1.0/idsred/wavecalib.py` & `idsred-0.1.1/idsred/wavecalib.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 from dotenv import dotenv_values
 
 from scipy.signal import find_peaks
 from astropy.stats import sigma_clip
 from scipy.optimize import minimize, curve_fit
 from ccdproc import CCDData
 
-import emcee
-import corner
-
 from lmfit import Minimizer, Parameters
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 import idsred
```

### Comparing `idsred-0.1.0/idsred.egg-info/PKG-INFO` & `idsred-0.1.1/idsred.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idsred
-Version: 0.1.0
+Version: 0.1.1
 Summary: INT-IDS data-reduction pipeline
 Home-page: https://github.com/temuller/idsred
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 This is a spectroscopic data-reduction pipeline for the Isaac Newton Telescope (INT) Intermediate Dispersion Spectrograph (IDS) instrument. 
 It is optimised for the blue detector (EEV10).
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fidsred-blue.svg?style=flat)](https://github.com/temuller/idsred)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/idsred/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/idsred?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/idsred/)
+[![DOI](https://zenodo.org/badge/574921206.svg)](https://zenodo.org/badge/latestdoi/574921206)
+
+
 
 ## Installation
 
 It is recommended to install it on an anaconda environment:
 
 ```code
 conda create -n idsred pip
@@ -55,10 +58,25 @@
 
 A notebook that explains how to use the pipeline is found in this repository [here](https://github.com/temuller/idsred/blob/main/reduction.ipynb).
 
 ## Contributing
 
 To contribute, either open an issue or send a pull request (preferred option). You can also contact me directly.
 
+## Citing IDSRED
+
+```code
+@software{tomas_e_muller_bravo_2023_7851772,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/idsred: First Release!},
+  month        = apr,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.0},
+  doi          = {10.5281/zenodo.7851772},
+  url          = {https://doi.org/10.5281/zenodo.7851772}
+}
+```
+
 ## Acknowledgement
 
 This pipeline is based on the [GROWTH school github repository](https://github.com/growth-astro/growth-school-2020), which nicely explains the entire reduction process for images and spectra, and on [INT-IDS-DataReduction](https://github.com/aayush3009/INT-IDS-DataReduction) for (long-slit) spectra reduction.
```

### Comparing `idsred-0.1.0/idsred.egg-info/SOURCES.txt` & `idsred-0.1.1/idsred.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 idsred/lamps/init_wavesol_no_timming.txt
 idsred/standards/bd17.og
 idsred/standards/bd253.sto
 idsred/standards/bd253a.sto
 idsred/standards/bd254.oke
 idsred/standards/bd75.oke
 idsred/standards/f25.sto
+idsred/standards/fFEIGE110.dat
 idsred/standards/fGD153.dat
 idsred/standards/fGD71.dat
+idsred/standards/g191anew.oke
 idsred/standards/h102a.sto
 idsred/standards/h600.sto
 idsred/standards/hd194a.og
 idsred/standards/hd849.og
 idsred/standards/standards.json
 idsred/standards/w1346.oke
```

### Comparing `idsred-0.1.0/setup.py` & `idsred-0.1.1/setup.py`

 * *Files identical despite different names*

