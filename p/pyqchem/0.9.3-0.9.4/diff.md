# Comparing `tmp/pyqchem-0.9.3.tar.gz` & `tmp/pyqchem-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqchem-0.9.3.tar", last modified: Thu Feb  9 14:34:18 2023, max compression
+gzip compressed data, was "pyqchem-0.9.4.tar", last modified: Wed Jun 21 10:35:30 2023, max compression
```

## Comparing `pyqchem-0.9.3.tar` & `pyqchem-0.9.4.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:34:18.555937 pyqchem-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-09 14:34:05.000000 pyqchem-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-02-09 14:34:18.555937 pyqchem-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-02-09 14:34:05.000000 pyqchem-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:34:18.555937 pyqchem-0.9.3/pyqchem/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/order_states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:34:18.555937 pyqchem-0.9.3/pyqchem/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:34:18.555937 pyqchem-0.9.3/pyqchem/parsers/common/
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/parser_cis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/parser_fchk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/parser_frequencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/parser_irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/parser_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/parsers/parser_rasci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    28322 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/qc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    21622 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/qchem_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-02-09 14:34:05.000000 pyqchem-0.9.3/pyqchem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:34:18.555937 pyqchem-0.9.3/pyqchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-02-09 14:34:18.000000 pyqchem-0.9.3/pyqchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-09 14:34:18.000000 pyqchem-0.9.3/pyqchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 14:34:18.000000 pyqchem-0.9.3/pyqchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-09 14:34:18.000000 pyqchem-0.9.3/pyqchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-09 14:34:18.000000 pyqchem-0.9.3/pyqchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 14:34:18.555937 pyqchem-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-09 14:34:05.000000 pyqchem-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:35:30.560195 pyqchem-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-21 10:35:15.000000 pyqchem-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-21 10:35:30.560195 pyqchem-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-21 10:35:15.000000 pyqchem-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:35:30.556195 pyqchem-0.9.4/pyqchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/g_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/g_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21698 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/g_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/order_states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:35:30.560195 pyqchem-0.9.4/pyqchem/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:35:30.560195 pyqchem-0.9.4/pyqchem/parsers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/parser_cis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17679 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/parser_fchk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/parser_frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/parser_irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/parser_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18099 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/parsers/parser_rasci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29297 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/qc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/qchem_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-06-21 10:35:15.000000 pyqchem-0.9.4/pyqchem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:35:30.556195 pyqchem-0.9.4/pyqchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-21 10:35:30.000000 pyqchem-0.9.4/pyqchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-21 10:35:30.000000 pyqchem-0.9.4/pyqchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:35:30.000000 pyqchem-0.9.4/pyqchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 10:35:30.000000 pyqchem-0.9.4/pyqchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 10:35:30.000000 pyqchem-0.9.4/pyqchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:35:30.560195 pyqchem-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-21 10:35:15.000000 pyqchem-0.9.4/setup.py
```

### Comparing `pyqchem-0.9.3/LICENSE` & `pyqchem-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/PKG-INFO` & `pyqchem-0.9.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,24 @@
-Metadata-Version: 2.1
-Name: pyqchem
-Version: 0.9.3
-Summary: Python wrapper for Q-Chem
-Home-page: https://github.com/abelcarreras/PyQchem
-Author: Abel Carreras
-Author-email: abelcarreras83@gmail.com
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.com/abelcarreras/PyQchem.svg?branch=master)](https://app.travis-ci.com/github/abelcarreras/PyQchem)
+[![Build, Test & Upload](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml/badge.svg)](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/abelcarreras/PyQchem/badge.svg?branch=master)](https://coveralls.io/github/abelcarreras/PyQchem?branch=master)
 [![PyPI version](https://badge.fury.io/py/pyqchem.svg)](https://badge.fury.io/py/pyqchem)
 [![Documentation Status](https://readthedocs.org/projects/pyqchem/badge/?version=master)](https://pyqchem.readthedocs.io/en/master/?badge=master)
-[![Build, Test & Upload](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml/badge.svg)](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml)
 
 PyQchem
 =======
 Python wrapper for Q-Chem (https://www.q-chem.com)  
 Online manual: https://pyqchem.readthedocs.io/
 
 Main features
 -------------
 - Easy to use clean python interface for Q-Chem
-- No special q-chem compilation needed (reads Q-Chem environment)
-- Output parser support
-- Cache system for calculations
+- No special q-chem installation needed (reads Q-Chem environment)
+- Output parsers for different type of calculations 
+- Custom basis set and guess support using high level interface
+- Calculation Cache system powered by SQLite database
 - python 2.7.x/3.5+ compatibility
 
 Installation instructions
 -------------------------
 1. Requirements
 
 - numpy
@@ -38,23 +26,23 @@
 - matplolib
 - requests
 - lxml
 - wfnsympy (optional)
 - paramiko (optional)
 - pymatgen (optional)
 
-2a. Installation from source
-
+2a. From pypi repository (recommended)
 ```shell
-python setup.py install --user
+pip install pyqchem --user
 ```
 
-2b. From pypi repository 
+2b. Installation from source
+
 ```shell
-pip install pyqchem --user
+python setup.py install --user
 ```
 
 Examples 
 --------
 **Simple pythonic API to define your input**
 
 ```python
@@ -116,15 +104,15 @@
 
 for i, mode in enumerate(parsed_data['modes']):
     print('mode:                      {}'.format(i+1))
     print('frequency (cm-1):          {:10.2f}'.format(mode['frequency']))
     print('force constant (mdyne/A):  {:10.5f}\n'.format(mode['force_constant']))
 
 ```
-**Custom basis without pain**
+**Custom basis support**
 
 ```python
 from pyqchem import QchemInput, Structure
 from pyqchem.basis import get_basis_from_BSE
 
 
 molecule = Structure(coordinates=[[0.0, 0.0, 0.0000],
@@ -138,15 +126,15 @@
 qc_input = QchemInput(molecule,
                       jobtype='sp',
                       exchange='hf',
                       basis=basis_custom)
 
 ```
 
-**Handle qchem errors like a pro!**
+**Handle qchem errors**
 
 
 ```python
 from pyqchem import get_output_from_qchem
 from pyqchem.errors import OutputError, ParserError
 from pyqchem.parsers.parser_rasci import parser_rasci
 
@@ -166,15 +154,16 @@
     except ParserError:
         print('Failed parsing')
         exit()
 
 
 print('Energy: ', parsed_data['scf_energy'])
 ```
+Additional example scripts are found at the [examples folder](/examples)
 
 Contact info
 ------------
 Abel Carreras  
 abelcarreras83@gmail.com
 
 Donostia International Physics Center (DIPC)  
-Donostia-San Sebastian (Spain)
+Donostia-San Sebastian (Spain)
```

### Comparing `pyqchem-0.9.3/README.md` & `pyqchem-0.9.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,36 @@
-[![Build Status](https://travis-ci.com/abelcarreras/PyQchem.svg?branch=master)](https://app.travis-ci.com/github/abelcarreras/PyQchem)
+Metadata-Version: 2.1
+Name: pyqchem
+Version: 0.9.4
+Summary: Python wrapper for Q-Chem
+Home-page: https://github.com/abelcarreras/PyQchem
+Author: Abel Carreras
+Author-email: abelcarreras83@gmail.com
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build, Test & Upload](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml/badge.svg)](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/abelcarreras/PyQchem/badge.svg?branch=master)](https://coveralls.io/github/abelcarreras/PyQchem?branch=master)
 [![PyPI version](https://badge.fury.io/py/pyqchem.svg)](https://badge.fury.io/py/pyqchem)
 [![Documentation Status](https://readthedocs.org/projects/pyqchem/badge/?version=master)](https://pyqchem.readthedocs.io/en/master/?badge=master)
-[![Build, Test & Upload](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml/badge.svg)](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml)
 
 PyQchem
 =======
 Python wrapper for Q-Chem (https://www.q-chem.com)  
 Online manual: https://pyqchem.readthedocs.io/
 
 Main features
 -------------
 - Easy to use clean python interface for Q-Chem
-- No special q-chem compilation needed (reads Q-Chem environment)
-- Output parser support
-- Cache system for calculations
+- No special q-chem installation needed (reads Q-Chem environment)
+- Output parsers for different type of calculations 
+- Custom basis set and guess support using high level interface
+- Calculation Cache system powered by SQLite database
 - python 2.7.x/3.5+ compatibility
 
 Installation instructions
 -------------------------
 1. Requirements
 
 - numpy
@@ -26,23 +38,23 @@
 - matplolib
 - requests
 - lxml
 - wfnsympy (optional)
 - paramiko (optional)
 - pymatgen (optional)
 
-2a. Installation from source
-
+2a. From pypi repository (recommended)
 ```shell
-python setup.py install --user
+pip install pyqchem --user
 ```
 
-2b. From pypi repository 
+2b. Installation from source
+
 ```shell
-pip install pyqchem --user
+python setup.py install --user
 ```
 
 Examples 
 --------
 **Simple pythonic API to define your input**
 
 ```python
@@ -104,15 +116,15 @@
 
 for i, mode in enumerate(parsed_data['modes']):
     print('mode:                      {}'.format(i+1))
     print('frequency (cm-1):          {:10.2f}'.format(mode['frequency']))
     print('force constant (mdyne/A):  {:10.5f}\n'.format(mode['force_constant']))
 
 ```
-**Custom basis without pain**
+**Custom basis support**
 
 ```python
 from pyqchem import QchemInput, Structure
 from pyqchem.basis import get_basis_from_BSE
 
 
 molecule = Structure(coordinates=[[0.0, 0.0, 0.0000],
@@ -126,15 +138,15 @@
 qc_input = QchemInput(molecule,
                       jobtype='sp',
                       exchange='hf',
                       basis=basis_custom)
 
 ```
 
-**Handle qchem errors like a pro!**
+**Handle qchem errors**
 
 
 ```python
 from pyqchem import get_output_from_qchem
 from pyqchem.errors import OutputError, ParserError
 from pyqchem.parsers.parser_rasci import parser_rasci
 
@@ -154,15 +166,16 @@
     except ParserError:
         print('Failed parsing')
         exit()
 
 
 print('Energy: ', parsed_data['scf_energy'])
 ```
+Additional example scripts are found at the [examples folder](/examples)
 
 Contact info
 ------------
 Abel Carreras  
 abelcarreras83@gmail.com
 
 Donostia International Physics Center (DIPC)  
-Donostia-San Sebastian (Spain)
+Donostia-San Sebastian (Spain)
```

### Comparing `pyqchem-0.9.3/pyqchem/basis.py` & `pyqchem-0.9.4/pyqchem/basis.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/cache.py` & `pyqchem-0.9.4/pyqchem/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import pickle
 import time
 import sys
 import sqlite3
 import numpy as np
 from datetime import datetime
+import zlib
 
 
 # Singleton classes to handle cache
 
 
 class SimpleCache(object):
     """
     Class that makes use of pickle module to hadle data cache
 
     :param filename: name of the file storing the cache data
     """
 
     class __SimpleCache:
-        def __init__(self, filename='calculation_data.pkl'):
+        def __init__(self, filename='calculation_data.pkl', compress=False):
             self._calculation_data_filename = filename
             self._pickle_protocol = pickle.HIGHEST_PROTOCOL
+            self._compress = compress
 
             # Py2 compatibility
             if 'BlockingIOError' not in vars():
                 BlockingIOError = IOError
 
             try:
                 with open(self._calculation_data_filename, 'rb') as input:
@@ -83,14 +85,17 @@
                     self.calculation_data = {}
                 except (BlockingIOError, IOError, EOFError):
                     # print('read_try: {}'.format(iter))
                     time.sleep(timeout / 100)
                     continue
                 break
 
+            if self._compress:
+                data = zlib.compress(pickle.dumps(data, protocol=2))
+
             self.calculation_data[(hash(input_qchem), keyword)] = data
 
             for iter in range(100):
                 try:
                     with open(self._calculation_data_filename, 'wb') as f:
                         if sys.platform not in ["win32", "cygwin"]:
                             import fcntl
@@ -106,31 +111,40 @@
             """
             retrieve calculation data from cache file
 
             :param input_qchem: QchemInput instance
             :param keyword: string that was used as a key to store the data
             :return:
             """
-            return self.calculation_data[(hash(input_qchem), keyword)] if (hash(input_qchem),
+            data = self.calculation_data[(hash(input_qchem), keyword)] if (hash(input_qchem),
                                                                            keyword) in self.calculation_data else None
 
+            if self._compress and data is not None:
+                data = pickle.loads(zlib.decompress(data))
+
+            return data
+
         def get_all_data(self):
             """
             return a list of all data stored in the cache file
 
             :return: list of data
             """
 
             calc_id_list = np.unique([r[0] for r in self.calculation_data.keys()])
             calc_list = []
             for id in calc_id_list:
                 data_dict = {}
                 for r in self.calculation_data:
                     if r[0] == id:
-                        data_dict.update({r[1]: self.calculation_data[(id, r[1])]})
+                        value = self.calculation_data[(id, r[1])]
+                        if self._compress:
+                            data_dict.update({r[1]: pickle.loads(zlib.decompress(value))})
+                        else:
+                            data_dict.update({r[1]: value})
                 calc_list.append(data_dict)
 
             return calc_list
 
     instance = None
 
     def __new__(cls, **arguments):
@@ -158,18 +172,19 @@
             return cls.__instance__
 
         cls._calculation_data_filename = 'calculation_data.db'
 
         cls.__instance__ = super(SqlCache, cls, ).__new__(cls)
         return cls.__instance__
 
-    def __init__(self, filename=None):
+    def __init__(self, filename=None, compress=False):
         """
         Constructor
         """
+        self._compress = compress
 
         if filename is not None:
             self._calculation_data_filename = filename
 
         # python 2 compatibility
         if not '_calculation_data_filename' in dir(self):
             print('python 2')
@@ -218,17 +233,20 @@
 
         date_time = datetime.now()
 
         self._conn = sqlite3.connect(self._calculation_data_filename)
 
         serialized_data = pickle.dumps(data, protocol=2)
 
+        if self._compress:
+            serialized_data = zlib.compress(serialized_data)
+
         # python 2 compatibility
         if sys.version_info[0] < 3:
-            serialized_data = buffer(serialized_data)
+            serialized_data = buffer(serialized_data) # noqa
 
         self._conn.execute("DELETE FROM DATA_TABLE WHERE input_hash=? AND parser=?",
                            (hash(input_qchem), keyword))
 
         try:
             self._conn.execute("INSERT into DATA_TABLE (input_hash, parser, qcdata, date)  VALUES (?, ?, ?, ?)",
                                (hash(input_qchem),  keyword, serialized_data, date_time))
@@ -251,14 +269,17 @@
 
         cursor = self._conn.execute("SELECT qcdata FROM DATA_TABLE WHERE input_hash=? AND parser=?",
                                     (hash(input_qchem), keyword))
         rows = cursor.fetchall()
 
         self._conn.close()
 
+        if self._compress:
+            return pickle.loads(zlib.decompress(rows[0][0])) if len(rows) > 0 else None
+
         return pickle.loads(rows[0][0]) if len(rows) > 0 else None
 
     def retrieve_calculation_data_from_id(self, id, keyword=None):
         """
         return data using database entry ID
         [Only for SQL database cache]
 
@@ -278,17 +299,23 @@
             rows = cursor.fetchall()
 
         self._conn.close()
 
         if len(rows) <= 0:
             return None
         elif len(rows) == 1:
-            return pickle.loads(rows[0][0]) if len(rows) > 0 else None
+            if self._compress:
+                return pickle.loads(zlib.decompress(rows[0][0])) if len(rows) > 0 else None
+            else:
+                return pickle.loads(rows[0][0]) if len(rows) > 0 else None
         else:
-            return [pickle.loads(r[0]) for r in rows]
+            if self._compress:
+                return [pickle.loads(zlib.decompress(r[0])) for r in rows]
+            else:
+                return [pickle.loads(r[0]) for r in rows]
 
     def list_database(self):
         """
         prints data inside database
         [Only for SQL databse cache]
 
         :return: None
@@ -403,42 +430,54 @@
         calc_id_list = np.unique([r[0] for r in rows])
 
         calc_list = []
         for id in calc_id_list:
             data_dict = {}
             for r in rows:
                 if r[0] == id:
-                    data_dict.update({r[1]: pickle.loads(r[2])})
+                    if self._compress:
+                        data_dict.update({r[1]: pickle.loads(zlib.decompress(r[2]))})
+                    else:
+                        data_dict.update({r[1]: pickle.loads(r[2])})
             calc_list.append(data_dict)
 
         return calc_list
 
     @property
     def calculation_data(self):
 
         self._conn = sqlite3.connect(self._calculation_data_filename)
 
         cursor = self._conn.execute("SELECT input_hash, parser, qcdata from DATA_TABLE")
 
         self._calculation_data = {}
         for row in cursor:
-            self._calculation_data[(row[0], row[1])] = pickle.loads(row[2])
+
+            if self._compress:
+                self._calculation_data[(row[0], row[1])] = pickle.loads(zlib.decompress(row[2]))
+            else:
+                self._calculation_data[(row[0], row[1])] = pickle.loads(row[2])
 
         self._conn.close()
 
         return self._calculation_data
 
     @calculation_data.setter
     def calculation_data(self, calculation_data):
 
         self._conn = sqlite3.connect(self._calculation_data_filename)
 
         for key, value in calculation_data.items():
+
+            serialized_data = pickle.dumps(value, protocol=2)
+            if self._compress:
+                serialized_data = zlib.compress(serialized_data)
+
             self._conn.execute("INSERT or REPLACE into DATA_TABLE (input_hash, parser, qcdata)  VALUES (?, ?, ?)",
-                               (key[0], key[1], pickle.dumps(value, protocol=2)))
+                               (key[0], key[1], serialized_data))
 
         self._conn.commit()
         self._conn.close()
 
 
 if __name__ == '__main__':
     a = SqlCache()
```

### Comparing `pyqchem-0.9.3/pyqchem/errors.py` & `pyqchem-0.9.4/pyqchem/errors.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/file_io.py` & `pyqchem-0.9.4/pyqchem/file_io.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/order_states.py` & `pyqchem-0.9.4/pyqchem/order_states.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/parsers/basic.py` & `pyqchem-0.9.4/pyqchem/parsers/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def basic_parser_qchem(output):
     """
     This showcases the format of  Q-Chem version parser compatibility.
     Just by creating a docstring with the following line:
 
-    compatibility: 5.1, 5.2+
+    compatibility: 5.1, 5.2+, 6.0
 
     will activate the check for parser-qchem version compatibility.
     If they are not compatible a warning will rise.
 
     """
     data_dict = {}
```

### Comparing `pyqchem-0.9.3/pyqchem/parsers/parser_cis.py` & `pyqchem-0.9.4/pyqchem/parsers/parser_cis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = 'Abel Carreras'
 AU_TO_EV = 27.21138
 
 from pyqchem.structure import Structure
 from pyqchem.errors import ParserError
 from pyqchem.parsers.common import search_bars, standardize_vector
-from pyqchem.parsers.common import read_basic_info, get_cis_occupations_list, read_symmetry_info
+from pyqchem.parsers.common import read_basic_info, get_cis_occupations_list, read_symmetry_info, read_input_structure
 import numpy as np
 import re
 
 
 def _list_to_complex(list):
     real = list[0].replace('(', '').replace(')', '')
     if real[:2] == '--':
@@ -28,38 +28,16 @@
 
     :param output:
     :return:
     """
     data_dict = {}
 
     # Molecule
-    n = output.find('$molecule')
-    n2 = output[n:].find('$end')
-
-    molecule_region = output[n:n+n2-1].replace('\t', ' ').split('\n')[1:]
-    charge, multiplicity = [int(num) for num in molecule_region[0].split()]
-    coordinates = [[float(l) for l in line.split()[1:4]] for line in molecule_region[1:]]
-    symbols = [line.split()[0].capitalize() for line in molecule_region[1:]]
-    n_atoms = len(symbols)
-
-    # structure
-    structure_input = Structure(coordinates=coordinates,
-                                symbols=symbols,
-                                charge=charge,
-                                multiplicity=multiplicity)
-
-    enum = output.find('Standard Nuclear Orientation')
-    section_structure = output[enum:enum + 200*structure_input.get_number_of_atoms()].split('\n')
-    section_structure = section_structure[3:structure_input.get_number_of_atoms()+3]
-    coordinates = [[float(num) for num in s.split()[2:]] for s in section_structure]
-
-    data_dict['structure'] = Structure(coordinates=coordinates,
-                                       symbols=symbols,
-                                       charge=charge,
-                                       multiplicity=multiplicity)
+    data_dict['structure'] = read_input_structure(output)
+    n_atoms = data_dict['structure'].get_number_of_atoms()
 
     # scf_energy
     enum = output.find('Total energy in the final basis set')
     try:
         data_dict['scf_energy'] = float(output[enum:enum+100].split()[8])
     except IndexError:
         pass
@@ -86,28 +64,32 @@
 
         for m in re.finditer('Excited state ', output_cis):
             state_cis_section = output_cis[m.end():]
             state_cis_lines = state_cis_section.split('\n')
 
             exc_energy = float(state_cis_lines[0].split()[5])
             exc_energy_units = state_cis_lines[0].split()[3][1:-1]
-            tot_energy = float(state_cis_lines[1].split()[5])
 
             try:
-                tot_energy_units = state_cis_lines[1].split()[6]
+                tot_energy = float(state_cis_lines[1].split()[5])
+            except ValueError:
+                tot_energy = float(state_cis_lines[1].split()[4])
+
+            tot_energy_units = 'au'
+
+            try:
                 mul = state_cis_lines[2].split()[-1]
 
                 trans_mom = [float(mom) for mom in [state_cis_lines[3].split()[2],
                                                     state_cis_lines[3].split()[4],
                                                     state_cis_lines[3].split()[6]]]
                 strength = float(state_cis_lines[4].split()[2])
             except ValueError:
                 # old version of qchem (< 5.01)
                 state_cis_words = output_cis[m.end():].split()
-                tot_energy_units = 'au'
                 mul = state_cis_words[13]
                 trans_mom = [float(mom) for mom in [state_cis_words[16],
                                                     state_cis_words[18],
                                                     state_cis_words[20]]]
                 strength = float(state_cis_words[24])
 
             transitions = []
@@ -118,62 +100,70 @@
                     amplitude = float(line.split('=')[1].split()[0])
 
                     alpha_transitions = []
                     beta_transitions = []
                     try:
                         spin = line[21:].split()[-1]
                         if spin == 'alpha':
-                            alpha_transitions.append({'origin': origin, 'target': target + basic_data['n_alpha']})
+                            target = target + basic_data['n_alpha']
+                            alpha_transitions.append({'origin': origin, 'target': target})
                         elif spin == 'beta':
-                            beta_transitions.append({'origin': origin, 'target': target + basic_data['n_beta']})
+                            target = target + basic_data['n_beta']
+                            beta_transitions.append({'origin': origin, 'target': target})
                         else:
                             raise ParserError('basic_cis', 'Error reading configurations', output)
 
-                        transitions.append({'origin': origin,
+                        transitions.append({'spin': spin,
+                                            'origin': origin,
                                             'target': target,
                                             'amplitude': amplitude,
                                             'occupations': get_cis_occupations_list(basic_data['n_basis_functions'],
                                                                                     basic_data['n_alpha'],
                                                                                     basic_data['n_beta'],
                                                                                     alpha_transitions=alpha_transitions,
                                                                                     beta_transitions=beta_transitions)})
 
                     except (IndexError, ParserError):
                         # This supposes single electron transition
                         alpha_transitions.append({'origin': origin, 'target': target + basic_data['n_alpha']})
 
-                        transitions.append({'origin': origin,
-                                            'target': target,
+                        transitions.append({'spin': 'alpha',
+                                            'origin': origin,
+                                            'target': target + basic_data['n_alpha'],
                                             'amplitude': amplitude/np.sqrt(2),
                                             'occupations': get_cis_occupations_list(basic_data['n_basis_functions'],
                                                                                     basic_data['n_alpha'],
                                                                                     basic_data['n_beta'],
                                                                                     alpha_transitions=alpha_transitions,
                                                                                     beta_transitions=beta_transitions)})
 
-                        transitions.append({'origin': origin,
-                                            'target': target,
+                        transitions.append({'spin': 'beta',
+                                            'origin': origin,
+                                            'target': target + basic_data['n_beta'],
                                             'amplitude': amplitude/np.sqrt(2) if mul == 'Singlet' else -amplitude/np.sqrt(2),
                                             'occupations': get_cis_occupations_list(basic_data['n_basis_functions'],
                                                                                     basic_data['n_alpha'],
                                                                                     basic_data['n_beta'],
                                                                                     alpha_transitions=beta_transitions,
                                                                                     beta_transitions=alpha_transitions)})
 
                 if len(line) < 5:
                     break
 
+            # sort transitions by amplitude
+            sorted_transitions = sorted(transitions, key=lambda x: abs(x['amplitude']), reverse=True)
+
             excited_states.append({'total_energy': tot_energy,
                                    'total_energy_units': tot_energy_units,
                                    'excitation_energy': exc_energy,
                                    'excitation_energy_units': exc_energy_units,
                                    'multiplicity': mul,
                                    'transition_moment': standardize_vector(trans_mom),
-                                   'strength': strength,
-                                   'configurations': transitions})
+                                   'oscillator_strength': strength,
+                                   'configurations': sorted_transitions})
 
     data_dict['excited_states'] = excited_states
 
     # Spin-Orbit coupling
     initial = output.find('*********SPIN-ORBIT COUPLING JOB BEGINS HERE*********')
     final = output.find('*********SOC CODE ENDS HERE*********')
```

### Comparing `pyqchem-0.9.3/pyqchem/parsers/parser_fchk.py` & `pyqchem-0.9.4/pyqchem/parsers/parser_fchk.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,25 +172,37 @@
         n_elements = int(output[m.end():m.end() + 100].replace('\n', ' ').split()[2])
         nbas = int(np.sqrt(n_elements))
         data = output[m.end(): m.end() + n_elements*50].split()[3:n_elements+3]
         nto_coefficients_list[i]['V'] = np.array(data, dtype=float).reshape(nbas, nbas).tolist()
 
     return nto_coefficients_list, nto_occupancies_list
 
+
 def _get_all_fod(output):
 
     fod_list = []
     for i, m in enumerate(re.finditer('Fractional occupation density', output)):
         n_elements = int(output[m.end():m.end() + 100].replace('\n', ' ').split()[2])
         data = output[m.end(): m.end() + n_elements*50].split()[3:n_elements+3]
         fod_list.append(vect_to_mat(np.array(data, dtype=float)).tolist())
 
     return fod_list
 
 
+def _get_all_scf(output):
+
+    scf_list = []
+    for i, m in enumerate(re.finditer('Total SCF Density', output)):
+        n_elements = int(output[m.end():m.end() + 100].replace('\n', ' ').split()[2])
+        data = output[m.end(): m.end() + n_elements*50].split()[3:n_elements+3]
+        scf_list.append(vect_to_mat(np.array(data, dtype=float)).tolist())
+
+    return scf_list
+
+
 def _get_all_nto_new_format(output, label):
 
     nto_data_dict = {}
     for m in re.finditer('NTOs U coefficients {}'.format(label), output):
         indices = np.array(output[m.end() :m.end() + 100].replace('\n', ' ').split(')')[0].split('(')[1].split(','), dtype=int)
         n_elements = int(output[m.end() :m.end() + 100].replace('\n', ' ').split(')')[1].split()[2])
         nbas = int(np.sqrt(n_elements))
@@ -308,25 +320,14 @@
         final_dict['coefficients'] = {'alpha': np.array(data['Alpha MO coefficients']).reshape(-1, nbas).tolist()}
         final_dict['mo_energies'] = {'alpha': data['Alpha Orbital Energies']}
 
     if 'Beta MO coefficients' in data:
         final_dict['coefficients']['beta'] = np.array(data['Beta MO coefficients']).reshape(-1, nbas).tolist()
         final_dict['mo_energies']['beta'] = data['Beta Orbital Energies']
 
-    if 'Total SCF Density' in data:
-        total = vect_to_mat(data['Total SCF Density'])
-        if 'Spin SCF Density' in data:
-            spin = vect_to_mat(data['Spin SCF Density'])
-            final_dict['scf_density'] = {'alpha': np.ndarray.tolist((total + spin)/2),
-                                         'beta': np.ndarray.tolist((total - spin)/2)}
-        else:
-            final_dict['scf_density'] = {'alpha': np.ndarray.tolist(total/2),
-                                         'beta': np.ndarray.tolist(total/2)}
-
-        final_dict['total_scf_density'] = vect_to_mat(data['Total SCF Density']).tolist()
 
     if 'Spin SCF Density' in data:
         final_dict['spin_density'] = vect_to_mat(data['Spin SCF Density']).tolist()
 
     if 'Fractional occupation density' in data:
         final_dict['fractional_occupation_density'] = vect_to_mat(data['Fractional occupation density']).tolist()
 
@@ -359,14 +360,33 @@
             final_dict['nto_occupancies_multi'] = nat_occupancies_list
 
     if 'Fractional occupation density' in data:
         fod_list = _get_all_fod(output)
         if len(fod_list) > 1:
             final_dict['fractional_occupation_density_multi'] = fod_list
 
+    if 'Total SCF Density' in data:
+        scf_list = _get_all_scf(output)
+        if len(scf_list) > 1:
+            final_dict['total_scf_density_multi'] = scf_list
+            total = np.array(scf_list[-1])
+
+        else:
+            total = np.array(vect_to_mat(data['Total SCF Density']))
+
+        if 'Spin SCF Density' in data:
+            spin = np.array(vect_to_mat(data['Spin SCF Density']))
+            final_dict['scf_density'] = {'alpha': ((total + spin)/2).tolist(),
+                                         'beta': ((total - spin)/2).tolist()}
+        else:
+            final_dict['scf_density'] = {'alpha':(total/2).tolist(),
+                                         'beta': (total/2).tolist()}
+
+        final_dict['total_scf_density'] = total.tolist()
+
     # Parse new format RAS SOC NTO's
     NTOS_dict = dict(filter(lambda item: "NTOs occupancies SOC" in item[0], data.items()))
     if len(NTOS_dict) > 0:
         final_dict['ntos_soc'] = _get_all_nto_new_format(output, 'SOC')
 
     # Parse new format RAS NTO's
     NTOS_dict = dict(filter(lambda item: "NTOs occupancies RAS" in item[0], data.items()))
```

### Comparing `pyqchem-0.9.3/pyqchem/parsers/parser_frequencies.py` & `pyqchem-0.9.4/pyqchem/parsers/parser_frequencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,25 @@
 import re
 import numpy as np
-from pyqchem.structure import Structure
+from pyqchem.parsers.common import read_input_structure
 
 
 # parser for frequencies calculations
 def basic_frequencies(output, print_data=False):
     """
     Parser for frequencies calculations
 
     :param output:
     :param print_data:
     :return:
     """
 
-    # Input moelcular data
-    n = output.find('$molecule')
-    n2 = output[n:].find('$end')
-    molecule_region = output[n:n+n2-1].replace('\t', ' ').split('\n')[1:]
-    charge, multiplicity = [int(num) for num in molecule_region[0].split()]
-    coordinates_input = np.array([ np.array(line.split()[1:4], dtype=float) for line in molecule_region[1:]])
-    symbols = [line.split()[0].capitalize() for line in molecule_region[1:]]
-    n_atoms = len(coordinates_input)
-
-    # Standard oriented structure
-    enum = output.find('Standard Nuclear Orientation')
-    section_structure = output[enum:enum + 200*n_atoms].split('\n')
-    section_structure = section_structure[3:n_atoms+3]
-    coordinates = [[float(num) for num in s.split()[2:]] for s in section_structure]
-
-    structure = Structure(coordinates=coordinates,
-                          symbols=symbols,
-                          charge=charge,
-                          multiplicity=multiplicity)
+    # Molecule
+    structure = read_input_structure(output)
+    n_atoms = structure.get_number_of_atoms()
 
     # Energy
     n = output.find('Total energy in the final basis set =')
     energy = float(output[n:n+70].split()[8])
 
     n_hess = output.find('Hessian of the SCF Energy')
     n_van = output.find('VIBRATIONAL ANALYSIS')
```

### Comparing `pyqchem-0.9.3/pyqchem/parsers/parser_irc.py` & `pyqchem-0.9.4/pyqchem/parsers/parser_irc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from pyqchem.structure import Structure
+from pyqchem.parsers.common import read_input_structure
 import numpy as np
 import re
 
 
 def basic_irc(output, print_data=False):
 
     branch_mark = True
     data_dict = {}
-    # Molecule
-    n = output.find('$molecule')
-    n2 = output[n:].find('$end')
 
-    molecule_region = output[n:n+n2-1].replace('\t', ' ').split('\n')[1:]
-    charge, multiplicity = [int(num) for num in molecule_region[0].split()]
-    coordinates = np.array([np.array(line.split()[1:4], dtype=float) for line in molecule_region[1:]])
-    symbols = [line.split()[0].capitalize() for line in molecule_region[1:]]
-    n_atoms = len(coordinates)
+    # Molecule
+    structure = read_input_structure(output)
+    n_atoms = structure.get_number_of_atoms()
 
     forward_steps = []
     backward_steps = []
 
     list_iterations = [l.end() for l in re.finditer('Reaction path following', output)]
     for ini, fin in zip(list_iterations, list_iterations[1:] + [len(output)]):
         step_section = output[ini:fin]
@@ -28,17 +24,17 @@
         coordinates_step = np.array([atom.split()[2:] for atom in atoms_list], dtype=float).tolist()
 
         step_energy = None
         for l in re.finditer('Total energy in the final basis set', step_section):
             step_energy = float(step_section[l.end(): l.end()+50].split()[1])
 
         step_molecule = Structure(coordinates=coordinates_step,
-                                  symbols=symbols,
-                                  charge=charge,
-                                  multiplicity=multiplicity)
+                                  symbols=structure.get_symbols(),
+                                  charge=structure.charge,
+                                  multiplicity=structure.multiplicity)
 
         if (step_section.find('IRC -- maximum number of cycles reached') > 0
                 or step_section.find('IRC -- convergence criterion reached') > 0):
             if branch_mark:
                 #forward_steps = forward_steps[::-1]
                 branch_mark = False
             else:
```

### Comparing `pyqchem-0.9.3/pyqchem/parsers/parser_optimization.py` & `pyqchem-0.9.4/pyqchem/parsers/parser_optimization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pyqchem.structure import Structure
+from pyqchem.parsers.common import read_input_structure
 import numpy as np
 import re
 
 
 def parse_molecule(opt_section, charge=0, multiplicity=0):
 
     num = opt_section.find('Coordinates')
@@ -31,33 +32,27 @@
 
     return molecule
 
 
 def basic_optimization(output, print_data=False):
 
     data_dict = {}
-    # Molecule
-    n = output.find('$molecule')
-    n2 = output[n:].find('$end')
 
-    molecule_region = output[n:n+n2-1].replace('\t', ' ').split('\n')[1:]
-    charge, multiplicity = [int(num) for num in molecule_region[0].split()]
-    coordinates = np.array([np.array(line.split()[1:4], dtype=float) for line in molecule_region[1:]])
-    symbols = [line.split()[0].capitalize() for line in molecule_region[1:]]
-    n_atoms = len(coordinates)
+    # Molecule
+    structure = read_input_structure(output)
 
     step_s2 = None
     # Optimization steps
     optimization_steps = []
-    list_iterations = [l.end() for l in re.finditer('Optimization Cycle', output)]
+    list_iterations = [l.end() for l in re.finditer('Optimization Cycle', output, re.IGNORECASE)]
     for ini, fin in zip(list_iterations, list_iterations[1:] + [len(output)]):
         step_section = output[ini:fin]
         enum = step_section.find('Coordinates (Angstroms)')
 
-        step_molecule = parse_molecule(step_section, charge, multiplicity)
+        step_molecule = parse_molecule(step_section, structure.charge, structure.multiplicity)
 
         enum = step_section.find('Energy is')
         step_energy = float(step_section[enum: enum+50].split()[2])
         enum = step_section.find('      Gradient')
         step_gradient = float(step_section[enum: enum+50].split()[1])
         enum = step_section.find('      Displacement')
         step_displacement = float(step_section[enum: enum+50].split()[1])
@@ -77,15 +72,15 @@
     enum = output.find('**  OPTIMIZATION CONVERGED  **')
     if enum > 0:
         ne = output[enum-200:enum].find('Final energy')
 
         final_energy = float(output[ne+enum-200: enum].split()[3])
         optimization_section = output[enum:]
 
-        optimized_molecule = parse_molecule(optimization_section, charge, multiplicity)
+        optimized_molecule = parse_molecule(optimization_section, structure.charge, structure.multiplicity)
 
         data_dict['optimized_molecule'] = optimized_molecule
         data_dict['energy'] = final_energy
         data_dict['s2'] = step_s2
 
     return data_dict
```

### Comparing `pyqchem-0.9.3/pyqchem/parsers/parser_rasci.py` & `pyqchem-0.9.4/pyqchem/parsers/parser_rasci.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 __author__ = 'Abel Carreras'
 
 import re
 import operator
+import warnings
+
 import numpy as np
-from pyqchem.structure import Structure
-from pyqchem.parsers.common import read_basic_info, get_rasci_occupations_list, search_bars, standardize_vector
+from pyqchem.parsers.common import read_basic_info, get_rasci_occupations_list
+from pyqchem.parsers.common import search_bars, standardize_vector, read_input_structure
+from pyqchem.parsers.common import float_asterisk as float
+
 
 
 def _read_simple_matrix(header, output, maxchar=10000, foot='-------'):
     matrix_list = []
     for m in re.finditer(header, output):
         section_state = output[m.end():m.end() + maxchar]  # 10000: assumed to max of section
         section_state = section_state[:section_state.find(foot)]
@@ -35,53 +39,61 @@
 
         row = [float(r) + float(c[:-1]) * 1j for r, c in zip(real, complex)]
         matrix.append(row)
 
     return matrix
 
 
+def _complete_interstate_pairs(interstate_dict):
+    additional_items = {}
+    for key, value in interstate_dict.items():
+        if not key[::-1] in interstate_dict:
+            dict_entry = {}
+            for k, v in interstate_dict[key].items():
+                if k == 'state_a':
+                    dict_entry.update({k: key[1]})
+                elif k == 'state_b':
+                    dict_entry.update({k: key[0]})
+                elif k == 'angular_momentum':
+                    dict_entry.update({k: np.conjugate(v).tolist()})
+                elif k == '1e_soc_mat':
+                    dict_entry.update({k: np.conjugate(v).T.tolist()})
+                elif k == 'hso_l-':
+                    dict_entry.update({k: (-np.array(v)).tolist()})
+                elif k == 'hso_l+':
+                    dict_entry.update({k: (-np.array(v)).tolist()})
+                elif k == '2e_soc_mat':
+                    dict_entry.update({k: np.conjugate(v).T.tolist()})
+                elif k == 'total_soc_mat':
+                    dict_entry.update({k: np.conjugate(v).T.tolist()})
+                else:
+                    dict_entry.update({k: v})
+            additional_items.update({key[::-1]: dict_entry})
+
+    interstate_dict.update(additional_items)
+
+
 def parser_rasci(output):
     """
     Parser for RAS-CI calculations
     Include:
     - Diabatization scheme data
     - Structure
     - Adiabatic states
     - SOC
 
     :param output:
     :return:
     """
 
     data_dict = {}
-    # Molecule
-    n = output.find('$molecule')
-    n2 = output[n:].find('$end')
 
-    molecule_region = output[n:n+n2-1].replace('\t', ' ').split('\n')[1:]
-    charge, multiplicity = [int(num) for num in molecule_region[0].split()]
-    coordinates = [[float(l) for l in line.split()[1:4]] for line in molecule_region[1:]]
-    symbols = [line.split()[0].capitalize() for line in molecule_region[1:]]
-    n_atoms = len(symbols)
-
-    # structure
-    structure_input = Structure(coordinates=coordinates,
-                                symbols=symbols,
-                                charge=charge,
-                                multiplicity=multiplicity)
-
-    enum = output.find('Standard Nuclear Orientation')
-    section_structure = output[enum:enum + 200*structure_input.get_number_of_atoms()].split('\n')
-    section_structure = section_structure[3:structure_input.get_number_of_atoms()+3]
-    coordinates = [[float(num) for num in s.split()[2:]] for s in section_structure]
-
-    data_dict['structure'] = Structure(coordinates=coordinates,
-                                       symbols=symbols,
-                                       charge=charge,
-                                       multiplicity=multiplicity)
+    # Molecule
+    data_dict['structure'] = read_input_structure(output)
+    n_atoms = data_dict['structure'].get_number_of_atoms()
 
     # basic info
     enum = output.find('Nuclear Repulsion Energy')
     basic_data = read_basic_info(output[enum:enum + 5000])
 
     # scf_energy
     enum = output.find('SCF   energy in the final basis set')
@@ -90,15 +102,15 @@
     data_dict['scf_energy'] = scf_energy
     # total energy
     # enum = output.find('Total energy in the final basis set')
     # total_energy = float(output[enum:enum+100].split()[8])
 
     # RASCI dimensions
     ini_section = output.find('RAS-CI Dimensions')
-    end_section = search_bars(output, from_position=ini_section, bar_type='\*\*\*')[0]
+    end_section = search_bars(output, from_position=ini_section, bar_type=r'\*\*\*')[0]
     dimension_section = output[ini_section: end_section]
 
     enum = dimension_section.find('Doubly Occ')
     doubly_occ = int(dimension_section[enum: enum+50].split()[3])
     enum = dimension_section.find('Doubly Vir')
     doubly_vir = int(dimension_section[enum: enum+50].split()[2])
     enum = dimension_section.find('Frozen Occ')
@@ -132,40 +144,46 @@
         rot_matrix = _read_simple_matrix('showmatrix final adiabatic -> diabatic', output)[-1]
         adiabatic_matrix = _read_simple_matrix('showing H in adiabatic representation: NO coupling elements', output)[-1]
         diabatic_matrix = _read_simple_matrix('showing H in diabatic representation: WITH coupling elements', output)[-1]
 
         mulliken_adiabatic = []
         enum = output.find('Mulliken analysis of Adiabatic State')
         for m in re.finditer('Mulliken analysis of Adiabatic State', output[enum:]):
-            section_mulliken = output[m.end() + enum: m.end() + 10000 + enum]  # 10000: assumed to max of section
+            end_section = search_bars(output, from_position=m.end(), bar_type=r'\-\-\-\-\-\-')[3]
+            section_mulliken = output[m.end() + enum: m.end() + enum + end_section]
+
+            #section_mulliken = output[m.end() + enum: m.end() + 20000 + enum]  # 10000: assumed to max of section
             section_mulliken = section_mulliken[:section_mulliken.find('Natural Orbitals stored in FCHK')]
             section_attachment = section_mulliken.split('\n')[9+n_atoms:9+n_atoms*2]
 
             mulliken_adiabatic.append({'attach': [float(l.split()[1]) for l in section_attachment],
                                        'detach': [float(l.split()[2]) for l in section_attachment],
                                        'total': [float(l.split()[3]) for l in section_attachment]})
 
         mulliken_diabatic = []
         enum = output.find('showing H in diabatic representation')
         for m in re.finditer('Mulliken Analysis of Diabatic State', output[enum:]):
-            section_mulliken = output[m.end() + enum: m.end() + 10000 + enum]  # 10000: assumed to max of section
+            end_section = search_bars(output, from_position=m.end(), bar_type=r'\-\-\-\-\-\-')[3]
+            section_mulliken = output[m.end() + enum: m.end() + enum + end_section]
+
+            # section_mulliken = output[m.end() + enum: m.end() + 10000 + enum]  # 10000: assumed to max of section
             section_mulliken = section_mulliken[:section_mulliken.find('Natural Orbitals stored in FCHK')]
             section_attachment = section_mulliken.split('\n')[9+n_atoms:9+n_atoms*2]
 
             mulliken_diabatic.append({'attach': [float(l.split()[1]) for l in section_attachment],
                                       'detach': [float(l.split()[2]) for l in section_attachment],
                                       'total': [float(l.split()[3]) for l in section_attachment]})
 
         enum = output.find('Transition dipole moment - diabatic states')
 
         tdm_section = output[enum: enum + 70 * len(rot_matrix)]
 
         diabatic_tdm = []
         for m in re.finditer('TDM', tdm_section):
-            diabatic_tdm.append([float(n) for n in tdm_section[m.end(): m.end()+70][14:].split()[:3]])
+            diabatic_tdm.append([float(n) for n in tdm_section[m.end(): m.end()+70].split(':')[1].split()[:3]])
 
         diabatic_states = []
         for i, tdm in enumerate(diabatic_tdm):
             diabatic_states.append({'excitation_energy': diabatic_matrix[i][i],
                                     'excitation_energy_units': 'eV',
                                     'transition_moment': tdm,
                                     'dipole_moment_units': 'ua',
@@ -178,23 +196,23 @@
                                       'mulliken_adiabatic': mulliken_adiabatic}
 
     # excited states data
     excited_states = []
     for m in re.finditer('RAS-CI total energy for state', output):
         # print('ll found', m.start(), m.end())
 
-        end_section = search_bars(output, from_position=m.start(), bar_type='\*\*\*\*\*\*\*')[0]
+        end_section = search_bars(output, from_position=m.start(), bar_type=r'\*\*\*\*\*\*\*')[0]
         section_state = output[m.start():end_section]
 
         # energies
         enum = section_state.find('total energy for state')
         tot_energy = float(section_state[enum: enum + 50].split()[5])
         enum = section_state.find('Excitation energy')
         exc_energy_units = section_state[enum: enum + 30].split()[2].strip('(').strip(')')
-        exc_energy = float(section_state[enum: enum + 30].split()[4])
+        exc_energy = float(section_state[enum: enum + 50].split()[4])
 
         # multiplicity
         n_multi = section_state.find('<S^2>')
         multi_data = section_state[n_multi:n_multi + 30].split(':')[1]
         state_multiplicity = float(multi_data.split()[0])
 
         # dipole moment
@@ -209,14 +227,28 @@
         if enum > -1:
             trans_mom = [float(section_state[enum:].split()[2]) + 0.0,
                          float(section_state[enum:].split()[4]) + 0.0,
                          float(section_state[enum:].split()[6]) + 0.0]
             trans_mom = standardize_vector(trans_mom)
             strength = float(section_state[enum:].split()[10])
 
+        # Mulliken population analysis
+        mulliken_population = None
+        enum = section_state.find('Mulliken population analysis')
+        if enum > -1:
+            max = search_bars(section_state, from_position=enum, bar_type=r'\-'*30)
+            pop_charges = []
+            pop_spin = []
+            for line in section_state[max[1]: max[2]].split('\n')[1:n_atoms+1]:
+                c, s = line.split()[2:4]
+                pop_charges.append(float(c))
+                pop_spin.append(float(s))
+
+            mulliken_population = {'charge': pop_charges, 'spin': pop_spin, 'units': 'au'}
+
         # Natural orbitals
         nato_occ = None
         enum = section_state.find('NATURAL OCCUPATION NUMBERS')
         if enum > -1:
             lines = []
             for line in section_state[enum:].split('\n')[2::2]:
                 if len(line) == 0:
@@ -241,14 +273,15 @@
                           'part': row.split('|')[4].strip(),
                           'amplitude': float(row.split('|')[5]) + 0.0})
             table[-1]['occupations'] = get_rasci_occupations_list(table[-1],
                                                                   doubly_occ,
                                                                   basic_data['n_basis_functions'])
 
         table = sorted(table, key=operator.itemgetter('hole', 'alpha', 'beta', 'part'))
+        table = sorted(table, key=lambda x: abs(x['amplitude']), reverse=True)
 
         # Contributions RASCI wfn
         contributions_section = section_state[enum2:]
         contributions = {'active' : float(contributions_section.split()[4]),
                          'hole': float(contributions_section.split()[6]),
                          'part': float(contributions_section.split()[8])}
 
@@ -266,29 +299,33 @@
                       'oscillator_strength': strength,
                       'configurations': table,
                       'contributions_fwn': contributions}
 
         if nato_occ is not None:
             state_dict.update({'natural_occupation_numbers': nato_occ})
 
+        if mulliken_population is not None:
+            state_dict.update({'mulliken_population': mulliken_population})
+
         excited_states.append(state_dict)
 
     data_dict.update({'excited_states': excited_states})
 
     # Interstate transition properties
     done_interstate = bool(output.find('Interstate Transition Properties')+1)
     if done_interstate:
         ini_section = output.find('Interstate Transition Properties')
         end_section = search_bars(output, from_position=ini_section)[1]
         interstate_section = output[ini_section: end_section]
 
         interstate_dict = {}
         for m in re.finditer('State A: Root', interstate_section):
             section_pair = interstate_section[m.start():m.start() + 10000]
-            section_pair = section_pair[:section_pair.find('********')]
+            end_section = search_bars(section_pair, bar_type=r'\*'*20)[0]
+            section_pair = section_pair[:end_section]
 
             lines = section_pair.split('\n')
 
             state_a = int(lines[0].split()[-1])
             state_b = int(lines[1].split()[-1])
 
             pair_dict = {'state_a': state_a,
@@ -309,25 +346,30 @@
                     s_a = float(lines[i].split('=')[1].split()[0])
                     s_b = float(lines[i+1].split('=')[1].split()[0])
 
                 na = int(2 * s_a + 1)
                 nb = int(2 * s_b + 1)
 
                 if 'Spin Matrices' in line:
+                    warnings.warn('Spin Matrices parsing is deprecated')
                     spinmat_x = _read_soc_matrix(lines[i + 2:], [nb, na])
                     spinmat_y = _read_soc_matrix(lines[i + 4 + nb:], [nb, na])
                     spinmat_z = _read_soc_matrix(lines[i + 6 + 2*nb:], [nb, na])
                     pair_dict['spin_matrices'] = [spinmat_x, spinmat_y, spinmat_z]
 
                 if 'Spin matrices Sx, Sy and Sz for states' in line:
+                    warnings.warn('Spin Matrices parsing is deprecated')
                     pair_dict['spin_matrices'] = [np.zeros((nb, na)).tolist()]*3
 
                 if '1-elec SOC matrix (cm-1)' in line:
                     pair_dict['1e_soc_mat'] = _read_soc_matrix(lines[i+1:], [nb, na])
-                    pair_dict['1e_socc'] = float(lines[i+2 + nb].split()[-2:][0])
+
+                if '1-elec SOCC' in line:
+                    pair_dict['1e_socc'] = float(line.split()[3])
+
                 if '2e-SOMF Reduced matrix elements (cm-1)' in line:
                     r, c = lines[i+1].split()[-2:]
                     pair_dict['hso_l-'] = float(r) + float(c) * 1j
                     r, c = lines[i+2].split()[-2:]
                     pair_dict['hso_l0'] = float(r) + float(c) * 1j
                     r, c = lines[i+3].split()[-2:]
                     pair_dict['hso_l+'] = float(r) + float(c) * 1j
@@ -336,11 +378,27 @@
                     pair_dict['2e_soc_mat'] = _read_soc_matrix(lines[i + 1:], [nb, na])
                 if 'Total mean-field SOC matrix (cm-1)' in line:
                     pair_dict['total_soc_mat'] = _read_soc_matrix(lines[i + 1:], [nb, na])
                 if 'Mean-Field SOCC' in line:
                     pair_dict['mf_socc'] = float(line.split()[-2])
                     pair_dict['units'] = line.split()[-1]
 
+                if 'Skipping SOCs between states' in line:
+                    pair_dict['1e_soc_mat'] = np.zeros((nb, na)).tolist()
+                    pair_dict['1e_socc'] = 0.0
+
+                    pair_dict['hso_l-'] = complex(0.0)
+                    pair_dict['hso_l0'] = complex(0.0)
+                    pair_dict['hso_l+'] = complex(0.0)
+
+                    pair_dict['2e_soc_mat'] = np.zeros((nb, na)).tolist()
+                    pair_dict['total_soc_mat'] = np.zeros((nb, na)).tolist()
+
+                    pair_dict['mf_socc'] = 0.0
+                    pair_dict['units'] = 'cm-1'
+
             interstate_dict[(state_a, state_b)] = pair_dict
+
+        _complete_interstate_pairs(interstate_dict)
         data_dict.update({'interstate_properties': interstate_dict})
 
     return data_dict
```

### Comparing `pyqchem-0.9.3/pyqchem/plots.py` & `pyqchem-0.9.4/pyqchem/plots.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/qc_input.py` & `pyqchem-0.9.4/pyqchem/qc_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from copy import deepcopy
 from pyqchem.basis import basis_to_txt, get_purecard
 import hashlib, json
 import warnings
 from pyqchem.errors import QchemInputWarning, QchemInputError
+warnings.filterwarnings("default", category=DeprecationWarning)  # make DeprecationWarning visible
 
 
 def normalize_values(value):
     """
     Set all string values (including keys and values of dictionaries) to lower case
 
     :param value: the values
@@ -55,14 +56,16 @@
                  ras_sts_tm=False,
                  ras_fod=False,
                  ras_natorb=False,
                  ras_natorb_state=None,
                  ras_print=1,
                  ras_diabatization_scheme=None,
                  ras_diabatization_states=None,
+                 ras_guess=None,
+                 use_reduced_ras_guess=False,
                  # RASCI SrDFT
                  ras_omega=400,
                  ras_srdft=None,
                  ras_srdft_damp=0.5,
                  ras_srdft_exc=None,
                  ras_srdft_cor=None,
                  ras_srdft_spinpol=0,
@@ -117,15 +120,16 @@
                  rpath_tol_displacement=5000,
                  # symmetry
                  symmetry=True,
                  sym_ignore=False,
                  # other
                  nto_pairs=None,
                  n_frozen_core=None,
-                 n_frozen_virt=0,
+                 n_frozen_virt=None,  # to be deprecated in the future
+                 n_frozen_virtual=0,
                  mom_start=False,
                  reorder_orbitals=None,
                  namd_nsurfaces=None,
                  scf_print=None,
                  scf_guess=None,
                  scf_energies=None,
                  scf_density=None,
@@ -263,25 +267,29 @@
 
         if self._exchange is not None:
             input_file += 'exchange {}\n'.format(self._exchange)
 
         if self._method:
             input_file += 'method {}\n'.format(self._method)
 
+        if self._n_frozen_virt is not None:
+            self._n_frozen_virtual = self._n_frozen_virt
+            warnings.warn('"n_frozen_virt" keyword will be deprecated. Use "n_frozen_virtual" instead', DeprecationWarning)
+
         input_file += 'basis {}\n'.format(self._basis)
         input_file += 'thresh {}\n'.format(self._thresh)
         input_file += 'scf_convergence {}\n'.format(self._scf_convergence)
         input_file += 'scf_algorithm {}\n'.format(self._scf_algorithm)
         input_file += 'max_scf_cycles {}\n'.format(self._max_scf_cycles)
         input_file += 'gui {}\n'.format(self.gui)
         input_file += 'set_iter {}\n'.format(self._set_iter)
         input_file += 'RPA {}\n'.format(self._RPA)
         input_file += 'mem_total {}\n'.format(self._mem_total)
         input_file += 'mem_static {}\n'.format(self._mem_static)
-        input_file += 'n_frozen_virtual {}\n'.format(self._n_frozen_virt)
+        input_file += 'n_frozen_virtual {}\n'.format(self._n_frozen_virtual)
         input_file += 'mom_start {}\n'.format(self._mom_start)
         input_file += 'skip_scfman {}\n'.format(self._skip_scfman)
         input_file += 'scf_guess_mix {}\n'.format(self._scf_guess_mix)
 
         if self._basis2 is not None:
             input_file += 'basis2 {}\n'.format(self._basis2)
 
@@ -365,14 +373,21 @@
                     input_file += '{} '.format([num for num in seq['states']] +
                                                [diab_methods[seq['method']]] +
                                                [seq['parameters'] if 'parameters' in seq else 0.0]).replace(' ', '')[1:-1]
                     input_file += ','
                 input_file = input_file[:-1] + ']\n'
                 input_file += 'ras_diab_seq_list ' + '{}\n'.format([len(seq['states']) for seq in self._ras_diabatization_scheme]).replace(' ', '')
 
+            # RAS guess
+            if self._ras_guess is not None:
+                if self._use_reduced_ras_guess:
+                    input_file += 'set_redo {}\n'.format(1)
+                else:
+                    input_file += 'set_redo {}\n'.format(2)
+
             # Borrowed keywords
             input_file += 'cis_convergence {}\n'.format(self._cis_convergence)
 
         #if self._method.upper() in ['EOM-CCSD'] or self._correlation.upper() in ['CCSD']:
         if self._method is not None:
 
             # EOM
@@ -579,40 +594,39 @@
         return input_file + "\n"
 
     def store_mo_file(self, path='.'):
         guess_coeff = self._mo_coefficients
         guess_energies = self._scf_energies
 
         # set guess in place
-        mo_coeffa = np.array(guess_coeff['alpha'], dtype=np.float)
+        mo_coeffa = np.array(guess_coeff['alpha'], dtype=float)
 
         if 'beta' in guess_coeff:
-            mo_coeffb = np.array(guess_coeff['beta'], dtype=np.float)
+            mo_coeffb = np.array(guess_coeff['beta'], dtype=float)
         else:
             mo_coeffb = mo_coeffa
 
         if 'qchem_order' in guess_coeff:
             indices = guess_coeff['qchem_order']
             reverse_indices = [list(indices).index(j) for j in range(len(indices))]
             mo_coeffa = mo_coeffa[:, reverse_indices]
             mo_coeffb = mo_coeffb[:, reverse_indices]
 
         if guess_energies is not None:
-            mo_enea = np.array(guess_energies['alpha'], dtype=np.float)
+            mo_enea = np.array(guess_energies['alpha'], dtype=float)
             if 'beta' in guess_coeff:
-                mo_coeffb = np.array(guess_coeff['beta'], dtype=np.float)
-                mo_eneb = np.array(guess_energies['beta'], dtype=np.float)
+                mo_coeffb = np.array(guess_coeff['beta'], dtype=float)
+                mo_eneb = np.array(guess_energies['beta'], dtype=float)
             else:
                 mo_eneb = mo_enea
 
         else:
-            # here we set orbital energies to 0 (no problem if skip_scfman=False)
-            # since they will be recalculated
-            mo_enea = np.zeros(len(mo_coeffa))
-            mo_eneb = np.zeros(len(mo_coeffb))
+            # energies set with increasing values for q-chem to keep the order of orbitals
+            mo_enea = list(range(len(mo_coeffa)))
+            mo_eneb = list(range(len(mo_coeffb)))
 
         guess_file = np.vstack([mo_coeffa, mo_coeffb, mo_enea, mo_eneb]).flatten()
         with open(path + '/53.0', 'w') as f:
             guess_file.tofile(f, sep='')
 
     def store_density_file(self, path='.'):
         guess_density = self._scf_density
@@ -625,25 +639,29 @@
 
         guess_file = np.vstack([density_alpha, density_beta]).flatten()
         with open(path + '/54.0', 'w') as f:
             guess_file.tofile(f, sep='')
 
     def store_energy_file(self, path='.'):
         energy_file = np.zeros(12)
-        warnings.warn('warining: FILE_ENERGY will be set to zeros, this may affect post HF methods')
+        warnings.warn('warning: FILE_ENERGY will be set to zeros, this may affect post HF methods')
         with open(path + '/99.0', 'w') as f:
             energy_file.tofile(f, sep='')
 
     def store_hessian_file(self, path='.'):
         hessian_triu = np.array(self._hessian)
         with open(path + '/132.0', 'w') as f:
             hessian_triu.tofile(f, sep='')
 
-    # Access to properties (only a reduced set should be accessible/editable)
+    def store_ras_guess_file(self, path='.'):
+        ras_guess_file = np.array(self._ras_guess, dtype=float).flatten()
+        with open(path + '/704.0', 'w') as f:
+            ras_guess_file.tofile(f, sep='')
 
+    # Access to properties (only a reduced set should be accessible/editable)
     @property
     def molecule(self):
         return self._molecule
 
     @property
     def mo_coefficients(self):
         return self._mo_coefficients
@@ -657,14 +675,18 @@
         return self._scf_density
 
     @property
     def hessian(self):
         return self._hessian
 
     @property
+    def ras_guess(self):
+        return self._ras_guess
+
+    @property
     def gui(self):
         return self._gui
 
     @gui.setter
     def gui(self, value):
         value = int(value)
         if value < 0 or value > 10:
```

### Comparing `pyqchem-0.9.3/pyqchem/qchem_core.py` & `pyqchem-0.9.4/pyqchem/qchem_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from pyqchem.qc_input import QchemInput
 from pyqchem.errors import ParserError, OutputError
 from pyqchem.utils import get_sdm
 from subprocess import Popen, PIPE
-import os, shutil
+from pathlib import Path
+import os, shutil, sys
 import numpy as np
 import hashlib
 import pickle
 import warnings
-import sys
+
 
 if sys.version_info[0] < 3 or sys.platform in ["win32", "cygwin"] or os.getenv('PYQCHEM_CACHE') == '1':
     # For python 2.x or Windows use pickle based cache system
     from pyqchem.cache import SimpleCache as CacheSystem
     warnings.warn('Using SimpleCache')
 else:
     # For python 3.x use SQL Database based cache system
     from pyqchem.cache import SqlCache as CacheSystem
 
 
 # Backwards Compatibility
-def redefine_calculation_data_filename(filename):
-    cache = CacheSystem(filename=filename)
+def redefine_calculation_data_filename(filename, compress=False):
+    cache = CacheSystem(filename=filename, compress=compress)
 
 
 # Check if calculation finished ok
 def finish_ok(output):
     return output[-1000:].find('Thank you very much for using Q-Chem') != -1
 
 
@@ -177,19 +178,20 @@
     if not use_mpi:
         os.environ["QCTHREADS"] = "{}".format(processors)
         os.environ["OMP_NUM_THREADS"] = "{}".format(processors)
         os.environ["MKL_NUM_THREADS"] = "1"
 
     os.environ["GUIFILE"] = fchk_file
     qc_dir = os.getenv('QC')
-    binary = "{}/exe/qcprog.exe".format(qc_dir)
-    # command = binary + ' {} {} '.format(flag, processors) + ' {} '.format(temp_file_name)
-    command = binary + ' {} '.format(os.path.join(work_dir, input_file_name)) + ' {} '.format(work_dir)
+    exe_dir = os.getenv('QC_EXE_DIR') if 'QC_EXE_DIR' in os.environ else 'exe'
+
+    binary = Path(qc_dir).joinpath(exe_dir).joinpath('qcprog.exe')
+    command = [binary, Path(work_dir).joinpath(input_file_name), Path(work_dir)]
 
-    qchem_process = Popen(command, stdout=PIPE, stdin=PIPE, stderr=PIPE, shell=True, cwd=work_dir)
+    qchem_process = Popen(command, stdout=PIPE, stdin=PIPE, stderr=PIPE, cwd=work_dir)
     (output, err) = qchem_process.communicate()
     qchem_process.wait()
     output = output.decode(errors='ignore')
     err = err.decode()
 
     return output, err
 
@@ -209,19 +211,20 @@
     if not use_mpi:
         os.environ["QCTHREADS"] = "{}".format(processors)
         os.environ["OMP_NUM_THREADS"] = "{}".format(processors)
         os.environ["MKL_NUM_THREADS"] = "1"
 
     os.environ["GUIFILE"] = fchk_file
     qc_dir = os.getenv('QC')
-    binary = "{}/exe/qcprog.exe".format(qc_dir)
-    # command = binary + ' {} {} '.format(flag, processors) + ' {} '.format(temp_file_name)
-    command = binary + ' {} '.format(os.path.join(work_dir, input_file_name)) + ' {} '.format(work_dir)
 
-    qchem_process = Popen(command, stdout=PIPE, stdin=PIPE, stderr=PIPE, shell=True, cwd=work_dir)
+    exe_dir = os.getenv('QC_EXE_DIR') if 'QC_EXE_DIR' in os.environ else 'exe'
+    binary = Path(qc_dir).joinpath(exe_dir).joinpath('qcprog.exe')
+    command = [binary, Path(work_dir).joinpath(input_file_name), Path(work_dir)]
+
+    qchem_process = Popen(command, stdout=PIPE, stdin=PIPE, stderr=PIPE, cwd=work_dir)
 
     output = ''
     err = ''
     while True:
         line_out = qchem_process.stdout.readline()
         line_err = qchem_process.stderr.readline()
 
@@ -268,15 +271,15 @@
 
     # Define temp remote dir
     _, stdout, _ = ssh.exec_command('pwd', get_pty=True)
 
     if remote_scratch is None:
         remote_scratch = stdout.read().decode().strip('\n').strip('\r')
 
-    remote_dir = '{}/temp_pyqchem_remote/'.format(remote_scratch)
+    remote_dir = os.path.join(remote_scratch, 'temp_pyqchem_remote')
 
     # Create temp directory in remote machine
     try:
         sftp.mkdir(remote_dir)
     except OSError:
         pass
     sftp.chdir(remote_dir)
@@ -337,22 +340,27 @@
             raise Exception('Explicit MO guess has to be provided for scf_skip')
         input_qchem.store_energy_file(work_dir)
 
     # Write hessian
     if input_qchem.hessian is not None:
         input_qchem.store_hessian_file(work_dir)
 
+    # write RAS-GUESS
+    if input_qchem.ras_guess is not None:
+        input_qchem.store_ras_guess_file(work_dir)
 
-def retrieve_additional_files(input_qchem, data_fchk, work_dir):
+
+def retrieve_additional_files(input_qchem, data_fchk, work_dir, scratch_read_level=0):
     """
     retrieve data from files in scratch data (on development, currently for test only)
 
     :param input_qchem: QChem input object
     :param data_fchk: FCHK parsed dictionary
     :param work_dir: scratch directory
+    :param scratch_read_level: defines what data to retrieve
     :return: dictionary with additional data
     """
 
     additional_data = {}
 
     natom = len(input_qchem.molecule.get_coordinates())
     file_list = os.listdir(work_dir)
@@ -366,15 +374,15 @@
             nbas = norb  # assumption
     else:
         norb = np.shape(data_fchk['coefficients']['alpha'])[0]
         nbas = np.shape(data_fchk['coefficients']['alpha'])[1]
 
 
     # MO_COEFS (Already in fchk) in internal order
-    if '53.0' in file_list:
+    if '53.0' in file_list and 'coefficients' in data_fchk:
         with open(work_dir + '53.0', 'r') as f:
             data = np.fromfile(f, dtype=float)
             mo_alpha = data[:norb*nbas].reshape(-1, norb).tolist()
             mo_beta = data[norb*nbas: 2*norb_beta*nbas].reshape(-1, norb_beta).tolist()
             # additional_data['coefficients_internal'] = {'alpha': mo_alpha, 'beta': mo_beta}
 
             # obtain the order indices between fchk order and Q-Chem internal order of basis functions
@@ -398,61 +406,74 @@
     # FOCK_MATRIX
     if '58.0' in file_list:
         with open(work_dir + '58.0', 'r') as f:
             data = np.fromfile(f, dtype=float)
             fock_alpha = data[:nbas*nbas].reshape(-1, nbas)
             fock_beta = data[nbas*nbas: 2*nbas*nbas].reshape(-1, nbas)
 
-            # put in fchk order
+            # set basis functions in fchk order
             fock_alpha = fock_alpha[:, indices]
             fock_alpha = fock_alpha[indices, :]
             fock_beta = fock_beta[:, indices]
             fock_beta = fock_beta[indices, :]
 
             additional_data['fock_matrix'] = {'alpha': fock_alpha.tolist(), 'beta': fock_beta.tolist()}
 
-    # # FILE_ENERGY (Not really worth to read it)
-    # if '99.0' in file_list:
-    #     with open(work_dir + '99.0', 'r') as f:
-    #         data = np.fromfile(f, dtype=float)
-
-    # # FILE_DENSITY_MATRIX (Already in fchk)
-    # if '54.0' in file_list:
-    #     with open(work_dir + '54.0', 'r') as f:
-    #         data = np.fromfile(f, dtype=float)
-    #         density_alpha = data[:nbas*nbas].reshape(-1, nbas)
-    #         density_beta = data[nbas*nbas: 2*nbas*nbas].reshape(-1, nbas)
-    #         put in fchk order
-    #         density_alpha = density_alpha[:, indices]
-    #         density_alpha = density_alpha[indices, :]
-    #         density_beta = density_beta[:, indices]
-    #         density_beta = density_beta[indices, :]
-    #         additional_data['scf_density_internal'] = {'alpha': density_alpha.tolist(), 'beta': density_beta.tolist()}
+    if scratch_read_level == -1:
+        # FILE_ENERGY (Not really worth to read it)
+        if '99.0' in file_list:
+            with open(work_dir + '99.0', 'r') as f:
+                data = np.fromfile(f, dtype=float)
+
+        # FILE_DENSITY_MATRIX (Already in fchk)
+        if '54.0' in file_list:
+            with open(work_dir + '54.0', 'r') as f:
+                data = np.fromfile(f, dtype=float)
+                density_alpha = data[:nbas*nbas].reshape(-1, nbas)
+                density_beta = data[nbas*nbas: 2*nbas*nbas].reshape(-1, nbas)
+                # set basis functions in fchk order
+                density_alpha = density_alpha[:, indices]
+                density_alpha = density_alpha[indices, :]
+                density_beta = density_beta[:, indices]
+                density_beta = density_beta[indices, :]
+                additional_data['scf_density_internal'] = {'alpha': density_alpha.tolist(), 'beta': density_beta.tolist()}
 
     # HESSIAN_MATRIX
     if '132.0' in file_list:
         with open(work_dir + '132.0', 'r') as f:
             data = np.fromfile(f, dtype=float)
             hessian = data.reshape(-1, natom*3)
             additional_data['hessian'] = hessian.tolist()
 
     # AO_INTS_DEBUG
     if '21.0' in file_list:
         with open(work_dir + '21.0', 'r') as f:
             data = np.fromfile(f, dtype=float)
             ao_integrals = data.reshape(-1, nbas, nbas, nbas)
 
-            # put in fchk order
+            # set basis functions in fchk order
             ao_integrals = ao_integrals[:, :, :, indices]
             ao_integrals = ao_integrals[:, :, indices, :]
             ao_integrals = ao_integrals[:, indices, :, :]
             ao_integrals = ao_integrals[indices, :, :, :]
 
             additional_data['ao_integrals'] = ao_integrals.tolist()
 
+    if scratch_read_level > 0:
+        # FILE_RAS_AMP
+        if '704.0' in file_list:
+            with open(work_dir + '705.0', 'r') as f:
+                ras_energies = np.fromfile(f, dtype=float)
+                n_ras_roots = len(ras_energies)
+
+            with open(work_dir + '704.0', 'r') as f:
+                data = np.fromfile(f, dtype=float)
+                ras_amplitudes = data.reshape(n_ras_roots, -1)
+                additional_data['ras_amplitudes'] = ras_amplitudes.tolist()
+
     return additional_data
 
 
 def get_output_from_qchem(input_qchem,
                           processors=1,
                           use_mpi=False,
                           scratch=None,
@@ -460,15 +481,17 @@
                           return_electronic_structure=False,
                           parser=None,
                           parser_parameters=None,
                           force_recalculation=False,
                           fchk_only=False,
                           store_full_output=False,
                           delete_scratch=True,
-                          remote=None):
+                          remote=None,
+                          scratch_read_level=0):
+
     """
     Runs qchem and returns the output in the following format:
 
     1) If return_electronic_structure is requested:
         [output, parsed_fchk]
     2) If return_electronic_structure is not requested:
         [output]
@@ -572,15 +595,18 @@
         if not os.path.isfile(os.path.join(work_dir, fchk_filename)):
             warnings.warn('fchk not found! something may be wrong in calculation')
         else:
             with open(os.path.join(work_dir, fchk_filename)) as f:
                 fchk_txt = f.read()
 
             elect_struct_data = parser_fchk(fchk_txt)
-            elect_struct_data.update(retrieve_additional_files(input_qchem, elect_struct_data, work_dir))
+            elect_struct_data.update(retrieve_additional_files(input_qchem,
+                                                               elect_struct_data,
+                                                               work_dir,
+                                                               scratch_read_level))
             cache.store_calculation_data(input_qchem, 'fchk', elect_struct_data)
 
         if store_full_output:
             cache.store_calculation_data(input_qchem, 'fullout', output)
 
     if parser is not None:
```

### Comparing `pyqchem-0.9.3/pyqchem/structure.py` & `pyqchem-0.9.4/pyqchem/structure.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/symmetry.py` & `pyqchem-0.9.4/pyqchem/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/test.py` & `pyqchem-0.9.4/pyqchem/test.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem/utils.py` & `pyqchem-0.9.4/pyqchem/utils.py`

 * *Files identical despite different names*

### Comparing `pyqchem-0.9.3/pyqchem.egg-info/PKG-INFO` & `pyqchem-0.9.4/pyqchem.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyqchem
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python wrapper for Q-Chem
 Home-page: https://github.com/abelcarreras/PyQchem
 Author: Abel Carreras
 Author-email: abelcarreras83@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://travis-ci.com/abelcarreras/PyQchem.svg?branch=master)](https://app.travis-ci.com/github/abelcarreras/PyQchem)
+[![Build, Test & Upload](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml/badge.svg)](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/abelcarreras/PyQchem/badge.svg?branch=master)](https://coveralls.io/github/abelcarreras/PyQchem?branch=master)
 [![PyPI version](https://badge.fury.io/py/pyqchem.svg)](https://badge.fury.io/py/pyqchem)
 [![Documentation Status](https://readthedocs.org/projects/pyqchem/badge/?version=master)](https://pyqchem.readthedocs.io/en/master/?badge=master)
-[![Build, Test & Upload](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml/badge.svg)](https://github.com/abelcarreras/PyQchem/actions/workflows/test-publish.yaml)
 
 PyQchem
 =======
 Python wrapper for Q-Chem (https://www.q-chem.com)  
 Online manual: https://pyqchem.readthedocs.io/
 
 Main features
 -------------
 - Easy to use clean python interface for Q-Chem
-- No special q-chem compilation needed (reads Q-Chem environment)
-- Output parser support
-- Cache system for calculations
+- No special q-chem installation needed (reads Q-Chem environment)
+- Output parsers for different type of calculations 
+- Custom basis set and guess support using high level interface
+- Calculation Cache system powered by SQLite database
 - python 2.7.x/3.5+ compatibility
 
 Installation instructions
 -------------------------
 1. Requirements
 
 - numpy
@@ -38,23 +38,23 @@
 - matplolib
 - requests
 - lxml
 - wfnsympy (optional)
 - paramiko (optional)
 - pymatgen (optional)
 
-2a. Installation from source
-
+2a. From pypi repository (recommended)
 ```shell
-python setup.py install --user
+pip install pyqchem --user
 ```
 
-2b. From pypi repository 
+2b. Installation from source
+
 ```shell
-pip install pyqchem --user
+python setup.py install --user
 ```
 
 Examples 
 --------
 **Simple pythonic API to define your input**
 
 ```python
@@ -116,15 +116,15 @@
 
 for i, mode in enumerate(parsed_data['modes']):
     print('mode:                      {}'.format(i+1))
     print('frequency (cm-1):          {:10.2f}'.format(mode['frequency']))
     print('force constant (mdyne/A):  {:10.5f}\n'.format(mode['force_constant']))
 
 ```
-**Custom basis without pain**
+**Custom basis support**
 
 ```python
 from pyqchem import QchemInput, Structure
 from pyqchem.basis import get_basis_from_BSE
 
 
 molecule = Structure(coordinates=[[0.0, 0.0, 0.0000],
@@ -138,15 +138,15 @@
 qc_input = QchemInput(molecule,
                       jobtype='sp',
                       exchange='hf',
                       basis=basis_custom)
 
 ```
 
-**Handle qchem errors like a pro!**
+**Handle qchem errors**
 
 
 ```python
 from pyqchem import get_output_from_qchem
 from pyqchem.errors import OutputError, ParserError
 from pyqchem.parsers.parser_rasci import parser_rasci
 
@@ -166,14 +166,15 @@
     except ParserError:
         print('Failed parsing')
         exit()
 
 
 print('Energy: ', parsed_data['scf_energy'])
 ```
+Additional example scripts are found at the [examples folder](/examples)
 
 Contact info
 ------------
 Abel Carreras  
 abelcarreras83@gmail.com
 
 Donostia International Physics Center (DIPC)
```

### Comparing `pyqchem-0.9.3/pyqchem.egg-info/SOURCES.txt` & `pyqchem-0.9.4/pyqchem.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 README.md
 setup.py
 pyqchem/__init__.py
 pyqchem/basis.py
 pyqchem/cache.py
 pyqchem/errors.py
 pyqchem/file_io.py
+pyqchem/g_main.py
+pyqchem/g_operations.py
+pyqchem/g_read.py
 pyqchem/order_states.py
 pyqchem/plots.py
 pyqchem/qc_input.py
 pyqchem/qchem_core.py
 pyqchem/structure.py
 pyqchem/symmetry.py
 pyqchem/test.py
```

### Comparing `pyqchem-0.9.3/setup.py` & `pyqchem-0.9.4/setup.py`

 * *Files identical despite different names*

