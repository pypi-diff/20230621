# Comparing `tmp/robotools-1.6.1.tar.gz` & `tmp/robotools-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotools-1.6.1.tar", last modified: Wed Jun  7 12:53:36 2023, max compression
+gzip compressed data, was "robotools-1.7.0.tar", last modified: Wed Jun 21 12:52:01 2023, max compression
```

## Comparing `robotools-1.6.1.tar` & `robotools-1.7.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-06-07 12:53:10.000000 robotools-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-07 12:53:36.287405 robotools-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 12:53:10.000000 robotools-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 12:53:10.000000 robotools-1.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.283405 robotools-1.6.1/robotools/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/test_transform.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/transform.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/__pycache__/utils.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/evotools/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/evotools/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    26749 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/commands.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 runner    (1001) docker     (123)   172857 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/test_worklist.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/types.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    52678 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/evotools/__pycache__/worklist.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    59566 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/test_worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45274 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/evotools/worklist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/liquidhandling/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.287405 robotools-1.6.1/robotools/liquidhandling/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/composition.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    21401 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/labware.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    56943 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/test_composition.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    44659 2023-06-07 12:53:33.000000 robotools-1.6.1/robotools/liquidhandling/__pycache__/test_labware.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/labware.py
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/liquidhandling/test_labware.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-06-07 12:53:10.000000 robotools-1.6.1/robotools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:53:36.283405 robotools-1.6.1/robotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 12:53:36.000000 robotools-1.6.1/robotools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:53:36.287405 robotools-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-07 12:53:10.000000 robotools-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.482763 robotools-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-06-21 12:51:35.000000 robotools-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-21 12:52:01.482763 robotools-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-21 12:51:35.000000 robotools-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 12:51:35.000000 robotools-1.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.478762 robotools-1.7.0/robotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.478762 robotools-1.7.0/robotools/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/__pycache__/test_transform.cpython-311-pytest-7.3.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/__pycache__/test_utils.cpython-311-pytest-7.3.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/__pycache__/transform.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/__pycache__/utils.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.478762 robotools-1.7.0/robotools/evotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.478762 robotools-1.7.0/robotools/evotools/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    27020 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/commands.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    28275 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/test_commands.cpython-311-pytest-7.3.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)   172857 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/test_worklist.cpython-311-pytest-7.3.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/types.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    52678 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/evotools/__pycache__/worklist.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    24581 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59566 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/test_worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45274 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/evotools/worklist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.482763 robotools-1.7.0/robotools/liquidhandling/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/liquidhandling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.482763 robotools-1.7.0/robotools/liquidhandling/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/liquidhandling/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/liquidhandling/__pycache__/composition.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/liquidhandling/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    21401 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/liquidhandling/__pycache__/labware.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    56943 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/liquidhandling/__pycache__/test_composition.cpython-311-pytest-7.3.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    44659 2023-06-21 12:51:59.000000 robotools-1.7.0/robotools/liquidhandling/__pycache__/test_labware.cpython-311-pytest-7.3.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/liquidhandling/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/liquidhandling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/liquidhandling/labware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/liquidhandling/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/liquidhandling/test_labware.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.000000 robotools-1.7.0/robotools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-06-21 12:51:35.000000 robotools-1.7.0/robotools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:52:01.478762 robotools-1.7.0/robotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-21 12:52:01.000000 robotools-1.7.0/robotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-21 12:52:01.000000 robotools-1.7.0/robotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:52:01.000000 robotools-1.7.0/robotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 12:52:01.000000 robotools-1.7.0/robotools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 12:52:01.000000 robotools-1.7.0/robotools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:52:01.482763 robotools-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-21 12:51:35.000000 robotools-1.7.0/setup.py
```

### Comparing `robotools-1.6.1/LICENSE` & `robotools-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/PKG-INFO` & `robotools-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotools
-Version: 1.6.1
+Version: 1.7.0
 Summary: Pythonic in-silico liquid handling and creation of Tecan FreedomEVO worklists.
 Home-page: https://github.com/jubiotech/robotools
-Download-URL: https://github.com/jubiotech/robotools/tarball/1.6.1
+Download-URL: https://github.com/jubiotech/robotools/tarball/1.7.0
 Author: Michael Osthege
 Author-email: m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `robotools-1.6.1/README.md` & `robotools-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/__pycache__/__init__.cpython-311.pyc` & `robotools-1.7.0/robotools/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 438
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -76,27 +76,27 @@
                110 IMPORT_NAME             19 (utils)
                112 IMPORT_FROM             20 (DilutionPlan)
                114 STORE_NAME              20 (DilutionPlan)
                116 IMPORT_FROM             21 (get_trough_wells)
                118 STORE_NAME              21 (get_trough_wells)
                120 POP_TOP
    
-    14         122 LOAD_CONST               7 ('1.6.1')
+    14         122 LOAD_CONST               7 ('1.7.0')
                124 STORE_NAME              22 (__version__)
                126 LOAD_CONST               8 (None)
                128 RETURN_VALUE
    consts
       1
       ('evotools', 'liquidhandling')
       ('InvalidOperationError', 'Labwares', 'Tip', 'Worklist')
       ('commands',)
       ('Labware', 'Trough', 'VolumeOverflowError', 'VolumeUnderflowError')
       ('WellRandomizer', 'WellRotator', 'WellShifter', 'make_well_array', 'make_well_index_dict')
       ('DilutionPlan', 'get_trough_wells')
-      '1.6.1'
+      '1.7.0'
       None
    names      ('', 'evotools', 'liquidhandling', 'InvalidOperationError', 'Labwares', 'Tip', 'Worklist', 'commands', 'evo_cmd', 'Labware', 'Trough', 'VolumeOverflowError', 'VolumeUnderflowError', 'transform', 'WellRandomizer', 'WellRotator', 'WellShifter', 'make_well_array', 'make_well_index_dict', 'utils', 'DilutionPlan', 'get_trough_wells', '__version__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/robotools/robotools/robotools/__init__.py'
    name       '<module>'
```

### Comparing `robotools-1.6.1/robotools/__pycache__/test_transform.cpython-311-pytest-7.3.1.pyc` & `robotools-1.7.0/robotools/__pycache__/test_transform.cpython-311-pytest-7.3.2.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 5266
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc` & `robotools-1.7.0/robotools/__pycache__/test_utils.cpython-311-pytest-7.3.2.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 9019
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/__pycache__/transform.cpython-311.pyc` & `robotools-1.7.0/robotools/__pycache__/transform.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 8732
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/__pycache__/utils.cpython-311.pyc` & `robotools-1.7.0/robotools/__pycache__/utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 15815
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/evotools/__pycache__/commands.cpython-311.pyc` & `robotools-1.7.0/robotools/evotools/__pycache__/commands.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,577 +1,595 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
-files sz: 24022
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
+files sz: 24581
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 42
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a036d045a046d055a056d
-      065a060100640164036c075a08640164046c096d0a5a0a0100640164056c
-      0b6d0c5a0c6d0d5a0d0100640164066c0e6d0f5a0f0100640764086c106d
-      115a11010064095a12640a6513640b6513640c65086a1400000000000000
-      006606640d84045a15640a6513640e6513640f65086a1400000000000000
-      006606641084045a16640364119c01640c65066517650465171900000000
-      000000000065086a14000000000000000066031900000000000000000064
-      126505651365136602190000000000000000006413650665186502651819
-      000000000000000000651366031900000000000000000064146517641565
-      066502650c19000000000000000000650265131900000000000000000066
-      021900000000000000000064166503651319000000000000000000641765
-      056519651a651865176519660519000000000000000000660e641884065a
-      1b64196513641a6513640c65066517650265171900000000000000000066
-      021900000000000000000064126505651365136602190000000000000000
-      006413650665186502651819000000000000000000651366031900000000
-      000000000064146517641565066502650c19000000000000000000650265
-      131900000000000000000066021900000000000000000064166518641764
-      036612641b84045a1c64196513641a6513640c6506651765026517190000
-      000000000000006602190000000000000000006412650565136513660219
-      000000000000000000641365066518650265181900000000000000000065
-      1366031900000000000000000064146517641565066502650c1900000000
-      000000000065026513190000000000000000006602190000000000000000
-      0064166518641765176612641c84045a1d6401641d641e641f641e642064
-      2164226423640164249c0a641565066502650c1900000000000000000065
-      026513190000000000000000006602190000000000000000006425650565
-      136513660219000000000000000000642665056513651366021900000000
-      0000000000642765136428651864296513642a6518642b6513642c651364
-      2d6513642e6513642f651364306513641765056519651a651a6513651865
-      136518651365136513651365136513660d19000000000000000000661c64
-      3184065a1e6401641d641e641f641e6420642164226423640164249c0a64
-      1565066502650c1900000000000000000065026513190000000000000000
-      006602190000000000000000006425650565136513660219000000000000
-      000000642665056513651366021900000000000000000064276513642865
-      1864296513642a6518642b6513642c6513642d6513642e6513642f651364
-      30651364176517661c643284065a1f64035300
+      065a066d075a070100640164036c085a09640164046c0a6d0b5a0b010064
+      0164056c0c6d0d5a0d6d0e5a0e0100640164066c0f6d105a100100640764
+      086c116d125a12010064095a13640a6514640b6514640c65076502651519
+      00000000000000000065096a160000000000000000660219000000000000
+      000000640d65096a1600000000000000006608640e84045a17640a651464
+      0f6514641065096a160000000000000000640d65156608641184045a1864
+      0364129c01640c65076515650565151900000000000000000065096a1600
+      000000000000006603190000000000000000006413650665146514660219
+      000000000000000000641465076519650365191900000000000000000065
+      1466031900000000000000000064156515641665076503650d1900000000
+      000000000065036514190000000000000000006602190000000000000000
+      0064176504651419000000000000000000640d6506651a651b6519651565
+      1a660519000000000000000000660e641884065a1c64196514641a651464
+      0c6507651565036515190000000000000000006602190000000000000000
+      006413650665146514660219000000000000000000641465076519650365
+      191900000000000000000065146603190000000000000000006415651564
+      1665076503650d1900000000000000000065036514190000000000000000
+      0066021900000000000000000064176519640d64036612641b84045a1d64
+      196514641a6514640c650765156503651519000000000000000000660219
+      000000000000000000641365066514651466021900000000000000000064
+      146507651965036519190000000000000000006514660319000000000000
+      00000064156515641665076503650d190000000000000000006503651419
+      00000000000000000066021900000000000000000064176519640d651566
+      12641c84045a1e6401641d641e641f641e6420642164226423640164249c
+      0a641665076503650d190000000000000000006503651419000000000000
+      000000660219000000000000000000642565066514651466021900000000
+      000000000064266506651465146602190000000000000000006427651464
+      28651964296514642a6519642b6514642c6514642d6514642e6514642f65
+      1464306514640d6506651a651b651b651465196514651965146514651465
+      1465146514660d19000000000000000000661c643184065a1f6401641d64
+      1e641f641e6420642164226423640164249c0a641665076503650d190000
+      000000000000006503651419000000000000000000660219000000000000
+      000000642565066514651466021900000000000000000064266506651465
+      14660219000000000000000000642765146428651964296514642a651964
+      2b6514642c6514642d6514642e6514642f651464306514640d6515661c64
+      3284065a2064035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('This module implements functions to create advanced worklist commands.')
                  4 STORE_NAME               0 (__doc__)
    
      2           6 LOAD_CONST               1 (0)
-                 8 LOAD_CONST               2 (('List', 'Optional', 'Sequence', 'Tuple', 'Union'))
+                 8 LOAD_CONST               2 (('Iterable', 'List', 'Optional', 'Sequence', 'Tuple', 'Union'))
                 10 IMPORT_NAME              1 (typing)
-                12 IMPORT_FROM              2 (List)
-                14 STORE_NAME               2 (List)
-                16 IMPORT_FROM              3 (Optional)
-                18 STORE_NAME               3 (Optional)
-                20 IMPORT_FROM              4 (Sequence)
-                22 STORE_NAME               4 (Sequence)
-                24 IMPORT_FROM              5 (Tuple)
-                26 STORE_NAME               5 (Tuple)
-                28 IMPORT_FROM              6 (Union)
-                30 STORE_NAME               6 (Union)
-                32 POP_TOP
-   
-     4          34 LOAD_CONST               1 (0)
-                36 LOAD_CONST               3 (None)
-                38 IMPORT_NAME              7 (numpy)
-                40 STORE_NAME               8 (np)
-   
-     6          42 LOAD_CONST               1 (0)
-                44 LOAD_CONST               4 (('InvalidOperationError',))
-                46 IMPORT_NAME              9 (robotools.evotools.exceptions)
-                48 IMPORT_FROM             10 (InvalidOperationError)
-                50 STORE_NAME              10 (InvalidOperationError)
-                52 POP_TOP
-   
-     7          54 LOAD_CONST               1 (0)
-                56 LOAD_CONST               5 (('Tip', 'int_to_tip'))
-                58 IMPORT_NAME             11 (robotools.evotools.types)
-                60 IMPORT_FROM             12 (Tip)
-                62 STORE_NAME              12 (Tip)
-                64 IMPORT_FROM             13 (int_to_tip)
-                66 STORE_NAME              13 (int_to_tip)
-                68 POP_TOP
-   
-     8          70 LOAD_CONST               1 (0)
-                72 LOAD_CONST               6 (('to_hex',))
-                74 IMPORT_NAME             14 (robotools.evotools.utils)
-                76 IMPORT_FROM             15 (to_hex)
-                78 STORE_NAME              15 (to_hex)
-                80 POP_TOP
-   
-    10          82 LOAD_CONST               7 (2)
-                84 LOAD_CONST               8 (('transform',))
-                86 IMPORT_NAME             16
-                88 IMPORT_FROM             17 (transform)
-                90 STORE_NAME              17 (transform)
-                92 POP_TOP
-   
-    12          94 LOAD_CONST               9 (('evo_make_selection_array', 'evo_get_selection', 'evo_aspirate', 'evo_wash'))
-                96 STORE_NAME              18 (__all__)
-   
-    20          98 LOAD_CONST              10 ('rows')
-               100 LOAD_NAME               19 (int)
-               102 LOAD_CONST              11 ('columns')
-               104 LOAD_NAME               19 (int)
-               106 LOAD_CONST              12 ('wells')
-               108 LOAD_NAME                8 (np)
-               110 LOAD_ATTR               20 (ndarray)
-               120 BUILD_TUPLE              6
-               122 LOAD_CONST              13 (<code object evo_make_selection_array, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 20>)
-               124 MAKE_FUNCTION            4 (annotations)
-               126 STORE_NAME              21 (evo_make_selection_array)
-   
-    47         128 LOAD_CONST              10 ('rows')
-               130 LOAD_NAME               19 (int)
-               132 LOAD_CONST              14 ('cols')
-               134 LOAD_NAME               19 (int)
-               136 LOAD_CONST              15 ('selected')
-               138 LOAD_NAME                8 (np)
-               140 LOAD_ATTR               20 (ndarray)
-               150 BUILD_TUPLE              6
-               152 LOAD_CONST              16 (<code object evo_get_selection, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 47>)
-               154 MAKE_FUNCTION            4 (annotations)
-               156 STORE_NAME              22 (evo_get_selection)
-   
-   102         158 LOAD_CONST               3 (None)
-   
-    95         160 LOAD_CONST              17 (('max_volume',))
-               162 BUILD_CONST_KEY_MAP      1
-               164 LOAD_CONST              12 ('wells')
-   
-    96         166 LOAD_NAME                6 (Union)
-               168 LOAD_NAME               23 (str)
-               170 LOAD_NAME                4 (Sequence)
-               172 LOAD_NAME               23 (str)
-               174 BINARY_SUBSCR
-               184 LOAD_NAME                8 (np)
-               186 LOAD_ATTR               20 (ndarray)
-               196 BUILD_TUPLE              3
-               198 BINARY_SUBSCR
-   
-    95         208 LOAD_CONST              18 ('labware_position')
-   
-    98         210 LOAD_NAME                5 (Tuple)
-               212 LOAD_NAME               19 (int)
-               214 LOAD_NAME               19 (int)
-               216 BUILD_TUPLE              2
-               218 BINARY_SUBSCR
-   
-    95         228 LOAD_CONST              19 ('volume')
-   
-    99         230 LOAD_NAME                6 (Union)
-               232 LOAD_NAME               24 (float)
-               234 LOAD_NAME                2 (List)
-               236 LOAD_NAME               24 (float)
-               238 BINARY_SUBSCR
-               248 LOAD_NAME               19 (int)
-               250 BUILD_TUPLE              3
-               252 BINARY_SUBSCR
-   
-    95         262 LOAD_CONST              20 ('liquid_class')
-   
-   100         264 LOAD_NAME               23 (str)
-   
-    95         266 LOAD_CONST              21 ('tips')
-   
-   101         268 LOAD_NAME                6 (Union)
-               270 LOAD_NAME                2 (List)
-               272 LOAD_NAME               12 (Tip)
-               274 BINARY_SUBSCR
-               284 LOAD_NAME                2 (List)
-               286 LOAD_NAME               19 (int)
+                12 IMPORT_FROM              2 (Iterable)
+                14 STORE_NAME               2 (Iterable)
+                16 IMPORT_FROM              3 (List)
+                18 STORE_NAME               3 (List)
+                20 IMPORT_FROM              4 (Optional)
+                22 STORE_NAME               4 (Optional)
+                24 IMPORT_FROM              5 (Sequence)
+                26 STORE_NAME               5 (Sequence)
+                28 IMPORT_FROM              6 (Tuple)
+                30 STORE_NAME               6 (Tuple)
+                32 IMPORT_FROM              7 (Union)
+                34 STORE_NAME               7 (Union)
+                36 POP_TOP
+   
+     4          38 LOAD_CONST               1 (0)
+                40 LOAD_CONST               3 (None)
+                42 IMPORT_NAME              8 (numpy)
+                44 STORE_NAME               9 (np)
+   
+     6          46 LOAD_CONST               1 (0)
+                48 LOAD_CONST               4 (('InvalidOperationError',))
+                50 IMPORT_NAME             10 (robotools.evotools.exceptions)
+                52 IMPORT_FROM             11 (InvalidOperationError)
+                54 STORE_NAME              11 (InvalidOperationError)
+                56 POP_TOP
+   
+     7          58 LOAD_CONST               1 (0)
+                60 LOAD_CONST               5 (('Tip', 'int_to_tip'))
+                62 IMPORT_NAME             12 (robotools.evotools.types)
+                64 IMPORT_FROM             13 (Tip)
+                66 STORE_NAME              13 (Tip)
+                68 IMPORT_FROM             14 (int_to_tip)
+                70 STORE_NAME              14 (int_to_tip)
+                72 POP_TOP
+   
+     8          74 LOAD_CONST               1 (0)
+                76 LOAD_CONST               6 (('to_hex',))
+                78 IMPORT_NAME             15 (robotools.evotools.utils)
+                80 IMPORT_FROM             16 (to_hex)
+                82 STORE_NAME              16 (to_hex)
+                84 POP_TOP
+   
+    10          86 LOAD_CONST               7 (2)
+                88 LOAD_CONST               8 (('transform',))
+                90 IMPORT_NAME             17
+                92 IMPORT_FROM             18 (transform)
+                94 STORE_NAME              18 (transform)
+                96 POP_TOP
+   
+    12          98 LOAD_CONST               9 (('evo_make_selection_array', 'evo_get_selection', 'evo_aspirate', 'evo_wash'))
+               100 STORE_NAME              19 (__all__)
+   
+    20         102 LOAD_CONST              10 ('rows')
+               104 LOAD_NAME               20 (int)
+               106 LOAD_CONST              11 ('columns')
+               108 LOAD_NAME               20 (int)
+               110 LOAD_CONST              12 ('wells')
+               112 LOAD_NAME                7 (Union)
+               114 LOAD_NAME                2 (Iterable)
+               116 LOAD_NAME               21 (str)
+               118 BINARY_SUBSCR
+               128 LOAD_NAME                9 (np)
+               130 LOAD_ATTR               22 (ndarray)
+               140 BUILD_TUPLE              2
+               142 BINARY_SUBSCR
+               152 LOAD_CONST              13 ('return')
+               154 LOAD_NAME                9 (np)
+               156 LOAD_ATTR               22 (ndarray)
+               166 BUILD_TUPLE              8
+               168 LOAD_CONST              14 (<code object evo_make_selection_array, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 20>)
+               170 MAKE_FUNCTION            4 (annotations)
+               172 STORE_NAME              23 (evo_make_selection_array)
+   
+    47         174 LOAD_CONST              10 ('rows')
+               176 LOAD_NAME               20 (int)
+               178 LOAD_CONST              15 ('cols')
+               180 LOAD_NAME               20 (int)
+               182 LOAD_CONST              16 ('selected')
+               184 LOAD_NAME                9 (np)
+               186 LOAD_ATTR               22 (ndarray)
+               196 LOAD_CONST              13 ('return')
+               198 LOAD_NAME               21 (str)
+               200 BUILD_TUPLE              8
+               202 LOAD_CONST              17 (<code object evo_get_selection, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 47>)
+               204 MAKE_FUNCTION            4 (annotations)
+               206 STORE_NAME              24 (evo_get_selection)
+   
+   102         208 LOAD_CONST               3 (None)
+   
+    95         210 LOAD_CONST              18 (('max_volume',))
+               212 BUILD_CONST_KEY_MAP      1
+               214 LOAD_CONST              12 ('wells')
+   
+    96         216 LOAD_NAME                7 (Union)
+               218 LOAD_NAME               21 (str)
+               220 LOAD_NAME                5 (Sequence)
+               222 LOAD_NAME               21 (str)
+               224 BINARY_SUBSCR
+               234 LOAD_NAME                9 (np)
+               236 LOAD_ATTR               22 (ndarray)
+               246 BUILD_TUPLE              3
+               248 BINARY_SUBSCR
+   
+    95         258 LOAD_CONST              19 ('labware_position')
+   
+    98         260 LOAD_NAME                6 (Tuple)
+               262 LOAD_NAME               20 (int)
+               264 LOAD_NAME               20 (int)
+               266 BUILD_TUPLE              2
+               268 BINARY_SUBSCR
+   
+    95         278 LOAD_CONST              20 ('volume')
+   
+    99         280 LOAD_NAME                7 (Union)
+               282 LOAD_NAME               25 (float)
+               284 LOAD_NAME                3 (List)
+               286 LOAD_NAME               25 (float)
                288 BINARY_SUBSCR
-               298 BUILD_TUPLE              2
-               300 BINARY_SUBSCR
+               298 LOAD_NAME               20 (int)
+               300 BUILD_TUPLE              3
+               302 BINARY_SUBSCR
    
-    95         310 LOAD_CONST              22 ('max_volume')
+    95         312 LOAD_CONST              21 ('liquid_class')
    
-   102         312 LOAD_NAME                3 (Optional)
-               314 LOAD_NAME               19 (int)
-               316 BINARY_SUBSCR
+   100         314 LOAD_NAME               21 (str)
    
-    95         326 LOAD_CONST              23 ('return')
+    95         316 LOAD_CONST              22 ('tips')
    
-   103         328 LOAD_NAME                5 (Tuple)
-               330 LOAD_NAME               25 (list)
-               332 LOAD_NAME               26 (tuple)
-               334 LOAD_NAME               24 (float)
-               336 LOAD_NAME               23 (str)
-               338 LOAD_NAME               25 (list)
-               340 BUILD_TUPLE              5
-               342 BINARY_SUBSCR
+   101         318 LOAD_NAME                7 (Union)
+               320 LOAD_NAME                3 (List)
+               322 LOAD_NAME               13 (Tip)
+               324 BINARY_SUBSCR
+               334 LOAD_NAME                3 (List)
+               336 LOAD_NAME               20 (int)
+               338 BINARY_SUBSCR
+               348 BUILD_TUPLE              2
+               350 BINARY_SUBSCR
    
-    95         352 BUILD_TUPLE             14
-               354 LOAD_CONST              24 (<code object prepare_evo_aspirate_dispense_parameters, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 95>)
-               356 MAKE_FUNCTION            6 (kwdefaults, annotations)
-               358 STORE_NAME              27 (prepare_evo_aspirate_dispense_parameters)
+    95         360 LOAD_CONST              23 ('max_volume')
    
-   197         360 LOAD_CONST              25 ('n_rows')
+   102         362 LOAD_NAME                4 (Optional)
+               364 LOAD_NAME               20 (int)
+               366 BINARY_SUBSCR
    
-   199         362 LOAD_NAME               19 (int)
+    95         376 LOAD_CONST              13 ('return')
    
-   197         364 LOAD_CONST              26 ('n_columns')
+   103         378 LOAD_NAME                6 (Tuple)
+               380 LOAD_NAME               26 (list)
+               382 LOAD_NAME               27 (tuple)
+               384 LOAD_NAME               25 (float)
+               386 LOAD_NAME               21 (str)
+               388 LOAD_NAME               26 (list)
+               390 BUILD_TUPLE              5
+               392 BINARY_SUBSCR
    
-   200         366 LOAD_NAME               19 (int)
+    95         402 BUILD_TUPLE             14
+               404 LOAD_CONST              24 (<code object prepare_evo_aspirate_dispense_parameters, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 95>)
+               406 MAKE_FUNCTION            6 (kwdefaults, annotations)
+               408 STORE_NAME              28 (prepare_evo_aspirate_dispense_parameters)
    
-   197         368 LOAD_CONST              12 ('wells')
+   201         410 LOAD_CONST              25 ('n_rows')
    
-   201         370 LOAD_NAME                6 (Union)
-               372 LOAD_NAME               23 (str)
-               374 LOAD_NAME                2 (List)
-               376 LOAD_NAME               23 (str)
-               378 BINARY_SUBSCR
-               388 BUILD_TUPLE              2
-               390 BINARY_SUBSCR
+   203         412 LOAD_NAME               20 (int)
    
-   197         400 LOAD_CONST              18 ('labware_position')
+   201         414 LOAD_CONST              26 ('n_columns')
    
-   202         402 LOAD_NAME                5 (Tuple)
-               404 LOAD_NAME               19 (int)
-               406 LOAD_NAME               19 (int)
-               408 BUILD_TUPLE              2
-               410 BINARY_SUBSCR
+   204         416 LOAD_NAME               20 (int)
    
-   197         420 LOAD_CONST              19 ('volume')
+   201         418 LOAD_CONST              12 ('wells')
    
-   203         422 LOAD_NAME                6 (Union)
-               424 LOAD_NAME               24 (float)
-               426 LOAD_NAME                2 (List)
-               428 LOAD_NAME               24 (float)
-               430 BINARY_SUBSCR
-               440 LOAD_NAME               19 (int)
-               442 BUILD_TUPLE              3
-               444 BINARY_SUBSCR
+   205         420 LOAD_NAME                7 (Union)
+               422 LOAD_NAME               21 (str)
+               424 LOAD_NAME                3 (List)
+               426 LOAD_NAME               21 (str)
+               428 BINARY_SUBSCR
+               438 BUILD_TUPLE              2
+               440 BINARY_SUBSCR
    
-   197         454 LOAD_CONST              20 ('liquid_class')
+   201         450 LOAD_CONST              19 ('labware_position')
    
-   204         456 LOAD_NAME               23 (str)
+   206         452 LOAD_NAME                6 (Tuple)
+               454 LOAD_NAME               20 (int)
+               456 LOAD_NAME               20 (int)
+               458 BUILD_TUPLE              2
+               460 BINARY_SUBSCR
    
-   197         458 LOAD_CONST              21 ('tips')
+   201         470 LOAD_CONST              20 ('volume')
    
-   205         460 LOAD_NAME                6 (Union)
-               462 LOAD_NAME                2 (List)
-               464 LOAD_NAME               12 (Tip)
-               466 BINARY_SUBSCR
-               476 LOAD_NAME                2 (List)
-               478 LOAD_NAME               19 (int)
+   207         472 LOAD_NAME                7 (Union)
+               474 LOAD_NAME               25 (float)
+               476 LOAD_NAME                3 (List)
+               478 LOAD_NAME               25 (float)
                480 BINARY_SUBSCR
-               490 BUILD_TUPLE              2
-               492 BINARY_SUBSCR
+               490 LOAD_NAME               20 (int)
+               492 BUILD_TUPLE              3
+               494 BINARY_SUBSCR
    
-   197         502 LOAD_CONST              22 ('max_volume')
+   201         504 LOAD_CONST              21 ('liquid_class')
    
-   206         504 LOAD_NAME               24 (float)
+   208         506 LOAD_NAME               21 (str)
    
-   197         506 LOAD_CONST              23 ('return')
+   201         508 LOAD_CONST              22 ('tips')
    
-   207         508 LOAD_CONST               3 (None)
+   209         510 LOAD_NAME                7 (Union)
+               512 LOAD_NAME                3 (List)
+               514 LOAD_NAME               13 (Tip)
+               516 BINARY_SUBSCR
+               526 LOAD_NAME                3 (List)
+               528 LOAD_NAME               20 (int)
+               530 BINARY_SUBSCR
+               540 BUILD_TUPLE              2
+               542 BINARY_SUBSCR
    
-   197         510 BUILD_TUPLE             18
-               512 LOAD_CONST              27 (<code object evo_aspirate, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 197>)
-               514 MAKE_FUNCTION            4 (annotations)
-               516 STORE_NAME              28 (evo_aspirate)
+   201         552 LOAD_CONST              23 ('max_volume')
    
-   270         518 LOAD_CONST              25 ('n_rows')
+   210         554 LOAD_NAME               25 (float)
    
-   272         520 LOAD_NAME               19 (int)
+   201         556 LOAD_CONST              13 ('return')
    
-   270         522 LOAD_CONST              26 ('n_columns')
+   211         558 LOAD_CONST               3 (None)
    
-   273         524 LOAD_NAME               19 (int)
+   201         560 BUILD_TUPLE             18
+               562 LOAD_CONST              27 (<code object evo_aspirate, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 201>)
+               564 MAKE_FUNCTION            4 (annotations)
+               566 STORE_NAME              29 (evo_aspirate)
    
-   270         526 LOAD_CONST              12 ('wells')
+   275         568 LOAD_CONST              25 ('n_rows')
    
-   274         528 LOAD_NAME                6 (Union)
-               530 LOAD_NAME               23 (str)
-               532 LOAD_NAME                2 (List)
-               534 LOAD_NAME               23 (str)
-               536 BINARY_SUBSCR
-               546 BUILD_TUPLE              2
-               548 BINARY_SUBSCR
+   277         570 LOAD_NAME               20 (int)
    
-   270         558 LOAD_CONST              18 ('labware_position')
+   275         572 LOAD_CONST              26 ('n_columns')
    
-   275         560 LOAD_NAME                5 (Tuple)
-               562 LOAD_NAME               19 (int)
-               564 LOAD_NAME               19 (int)
-               566 BUILD_TUPLE              2
-               568 BINARY_SUBSCR
+   278         574 LOAD_NAME               20 (int)
    
-   270         578 LOAD_CONST              19 ('volume')
+   275         576 LOAD_CONST              12 ('wells')
    
-   276         580 LOAD_NAME                6 (Union)
-               582 LOAD_NAME               24 (float)
-               584 LOAD_NAME                2 (List)
-               586 LOAD_NAME               24 (float)
-               588 BINARY_SUBSCR
-               598 LOAD_NAME               19 (int)
-               600 BUILD_TUPLE              3
-               602 BINARY_SUBSCR
+   279         578 LOAD_NAME                7 (Union)
+               580 LOAD_NAME               21 (str)
+               582 LOAD_NAME                3 (List)
+               584 LOAD_NAME               21 (str)
+               586 BINARY_SUBSCR
+               596 BUILD_TUPLE              2
+               598 BINARY_SUBSCR
    
-   270         612 LOAD_CONST              20 ('liquid_class')
+   275         608 LOAD_CONST              19 ('labware_position')
    
-   277         614 LOAD_NAME               23 (str)
+   280         610 LOAD_NAME                6 (Tuple)
+               612 LOAD_NAME               20 (int)
+               614 LOAD_NAME               20 (int)
+               616 BUILD_TUPLE              2
+               618 BINARY_SUBSCR
    
-   270         616 LOAD_CONST              21 ('tips')
+   275         628 LOAD_CONST              20 ('volume')
    
-   278         618 LOAD_NAME                6 (Union)
-               620 LOAD_NAME                2 (List)
-               622 LOAD_NAME               12 (Tip)
-               624 BINARY_SUBSCR
-               634 LOAD_NAME                2 (List)
-               636 LOAD_NAME               19 (int)
+   281         630 LOAD_NAME                7 (Union)
+               632 LOAD_NAME               25 (float)
+               634 LOAD_NAME                3 (List)
+               636 LOAD_NAME               25 (float)
                638 BINARY_SUBSCR
-               648 BUILD_TUPLE              2
-               650 BINARY_SUBSCR
+               648 LOAD_NAME               20 (int)
+               650 BUILD_TUPLE              3
+               652 BINARY_SUBSCR
    
-   270         660 LOAD_CONST              22 ('max_volume')
+   275         662 LOAD_CONST              21 ('liquid_class')
    
-   279         662 LOAD_NAME               24 (float)
+   282         664 LOAD_NAME               21 (str)
    
-   270         664 LOAD_CONST              23 ('return')
+   275         666 LOAD_CONST              22 ('tips')
    
-   280         666 LOAD_NAME               23 (str)
+   283         668 LOAD_NAME                7 (Union)
+               670 LOAD_NAME                3 (List)
+               672 LOAD_NAME               13 (Tip)
+               674 BINARY_SUBSCR
+               684 LOAD_NAME                3 (List)
+               686 LOAD_NAME               20 (int)
+               688 BINARY_SUBSCR
+               698 BUILD_TUPLE              2
+               700 BINARY_SUBSCR
    
-   270         668 BUILD_TUPLE             18
-               670 LOAD_CONST              28 (<code object evo_dispense, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 270>)
-               672 MAKE_FUNCTION            4 (annotations)
-               674 STORE_NAME              29 (evo_dispense)
+   275         710 LOAD_CONST              23 ('max_volume')
    
-   348         676 LOAD_CONST               1 (0)
+   284         712 LOAD_NAME               25 (float)
    
-   349         678 LOAD_CONST              29 (3.0)
+   275         714 LOAD_CONST              13 ('return')
    
-   350         680 LOAD_CONST              30 (500)
+   285         716 LOAD_NAME               21 (str)
    
-   351         682 LOAD_CONST              31 (4.0)
+   275         718 BUILD_TUPLE             18
+               720 LOAD_CONST              28 (<code object evo_dispense, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 275>)
+               722 MAKE_FUNCTION            4 (annotations)
+               724 STORE_NAME              30 (evo_dispense)
    
-   352         684 LOAD_CONST              30 (500)
+   354         726 LOAD_CONST               1 (0)
    
-   353         686 LOAD_CONST              32 (10)
+   355         728 LOAD_CONST              29 (3.0)
    
-   354         688 LOAD_CONST              33 (70)
+   356         730 LOAD_CONST              30 (500)
    
-   355         690 LOAD_CONST              34 (30)
+   357         732 LOAD_CONST              31 (4.0)
    
-   356         692 LOAD_CONST              35 (1)
+   358         734 LOAD_CONST              30 (500)
    
-   357         694 LOAD_CONST               1 (0)
+   359         736 LOAD_CONST              32 (10)
    
-   343         696 LOAD_CONST              36 (('arm', 'waste_vol', 'waste_delay', 'cleaner_vol', 'cleaner_delay', 'airgap', 'airgap_speed', 'retract_speed', 'fastwash', 'low_volume'))
-               698 BUILD_CONST_KEY_MAP     10
-               700 LOAD_CONST              21 ('tips')
+   360         738 LOAD_CONST              33 (70)
    
-   345         702 LOAD_NAME                6 (Union)
-               704 LOAD_NAME                2 (List)
-               706 LOAD_NAME               12 (Tip)
-               708 BINARY_SUBSCR
-               718 LOAD_NAME                2 (List)
-               720 LOAD_NAME               19 (int)
-               722 BINARY_SUBSCR
-               732 BUILD_TUPLE              2
-               734 BINARY_SUBSCR
+   361         740 LOAD_CONST              34 (30)
    
-   343         744 LOAD_CONST              37 ('waste_location')
+   362         742 LOAD_CONST              35 (1)
    
-   346         746 LOAD_NAME                5 (Tuple)
-               748 LOAD_NAME               19 (int)
-               750 LOAD_NAME               19 (int)
-               752 BUILD_TUPLE              2
-               754 BINARY_SUBSCR
+   363         744 LOAD_CONST               1 (0)
    
-   343         764 LOAD_CONST              38 ('cleaner_location')
+   349         746 LOAD_CONST              36 (('arm', 'waste_vol', 'waste_delay', 'cleaner_vol', 'cleaner_delay', 'airgap', 'airgap_speed', 'retract_speed', 'fastwash', 'low_volume'))
+               748 BUILD_CONST_KEY_MAP     10
+               750 LOAD_CONST              22 ('tips')
    
-   347         766 LOAD_NAME                5 (Tuple)
-               768 LOAD_NAME               19 (int)
-               770 LOAD_NAME               19 (int)
-               772 BUILD_TUPLE              2
-               774 BINARY_SUBSCR
+   351         752 LOAD_NAME                7 (Union)
+               754 LOAD_NAME                3 (List)
+               756 LOAD_NAME               13 (Tip)
+               758 BINARY_SUBSCR
+               768 LOAD_NAME                3 (List)
+               770 LOAD_NAME               20 (int)
+               772 BINARY_SUBSCR
+               782 BUILD_TUPLE              2
+               784 BINARY_SUBSCR
    
-   343         784 LOAD_CONST              39 ('arm')
+   349         794 LOAD_CONST              37 ('waste_location')
    
-   348         786 LOAD_NAME               19 (int)
+   352         796 LOAD_NAME                6 (Tuple)
+               798 LOAD_NAME               20 (int)
+               800 LOAD_NAME               20 (int)
+               802 BUILD_TUPLE              2
+               804 BINARY_SUBSCR
    
-   343         788 LOAD_CONST              40 ('waste_vol')
+   349         814 LOAD_CONST              38 ('cleaner_location')
    
-   349         790 LOAD_NAME               24 (float)
+   353         816 LOAD_NAME                6 (Tuple)
+               818 LOAD_NAME               20 (int)
+               820 LOAD_NAME               20 (int)
+               822 BUILD_TUPLE              2
+               824 BINARY_SUBSCR
    
-   343         792 LOAD_CONST              41 ('waste_delay')
+   349         834 LOAD_CONST              39 ('arm')
    
-   350         794 LOAD_NAME               19 (int)
+   354         836 LOAD_NAME               20 (int)
    
-   343         796 LOAD_CONST              42 ('cleaner_vol')
+   349         838 LOAD_CONST              40 ('waste_vol')
    
-   351         798 LOAD_NAME               24 (float)
+   355         840 LOAD_NAME               25 (float)
    
-   343         800 LOAD_CONST              43 ('cleaner_delay')
+   349         842 LOAD_CONST              41 ('waste_delay')
    
-   352         802 LOAD_NAME               19 (int)
+   356         844 LOAD_NAME               20 (int)
    
-   343         804 LOAD_CONST              44 ('airgap')
+   349         846 LOAD_CONST              42 ('cleaner_vol')
    
-   353         806 LOAD_NAME               19 (int)
+   357         848 LOAD_NAME               25 (float)
    
-   343         808 LOAD_CONST              45 ('airgap_speed')
+   349         850 LOAD_CONST              43 ('cleaner_delay')
    
-   354         810 LOAD_NAME               19 (int)
+   358         852 LOAD_NAME               20 (int)
    
-   343         812 LOAD_CONST              46 ('retract_speed')
+   349         854 LOAD_CONST              44 ('airgap')
    
-   355         814 LOAD_NAME               19 (int)
+   359         856 LOAD_NAME               20 (int)
    
-   343         816 LOAD_CONST              47 ('fastwash')
+   349         858 LOAD_CONST              45 ('airgap_speed')
    
-   356         818 LOAD_NAME               19 (int)
+   360         860 LOAD_NAME               20 (int)
    
-   343         820 LOAD_CONST              48 ('low_volume')
+   349         862 LOAD_CONST              46 ('retract_speed')
    
-   357         822 LOAD_NAME               19 (int)
+   361         864 LOAD_NAME               20 (int)
    
-   343         824 LOAD_CONST              23 ('return')
+   349         866 LOAD_CONST              47 ('fastwash')
    
-   358         826 LOAD_NAME                5 (Tuple)
-               828 LOAD_NAME               25 (list)
-               830 LOAD_NAME               26 (tuple)
-               832 LOAD_NAME               26 (tuple)
-               834 LOAD_NAME               19 (int)
-               836 LOAD_NAME               24 (float)
-               838 LOAD_NAME               19 (int)
-               840 LOAD_NAME               24 (float)
-               842 LOAD_NAME               19 (int)
-               844 LOAD_NAME               19 (int)
-               846 LOAD_NAME               19 (int)
-               848 LOAD_NAME               19 (int)
-               850 LOAD_NAME               19 (int)
-               852 LOAD_NAME               19 (int)
-               854 BUILD_TUPLE             13
-               856 BINARY_SUBSCR
+   362         868 LOAD_NAME               20 (int)
    
-   343         866 BUILD_TUPLE             28
-               868 LOAD_CONST              49 (<code object prepare_evo_wash_parameters, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 343>)
-               870 MAKE_FUNCTION            6 (kwdefaults, annotations)
-               872 STORE_NAME              30 (prepare_evo_wash_parameters)
+   349         870 LOAD_CONST              48 ('low_volume')
    
-   527         874 LOAD_CONST               1 (0)
+   363         872 LOAD_NAME               20 (int)
    
-   528         876 LOAD_CONST              29 (3.0)
+   349         874 LOAD_CONST              13 ('return')
    
-   529         878 LOAD_CONST              30 (500)
+   364         876 LOAD_NAME                6 (Tuple)
+               878 LOAD_NAME               26 (list)
+               880 LOAD_NAME               27 (tuple)
+               882 LOAD_NAME               27 (tuple)
+               884 LOAD_NAME               20 (int)
+               886 LOAD_NAME               25 (float)
+               888 LOAD_NAME               20 (int)
+               890 LOAD_NAME               25 (float)
+               892 LOAD_NAME               20 (int)
+               894 LOAD_NAME               20 (int)
+               896 LOAD_NAME               20 (int)
+               898 LOAD_NAME               20 (int)
+               900 LOAD_NAME               20 (int)
+               902 LOAD_NAME               20 (int)
+               904 BUILD_TUPLE             13
+               906 BINARY_SUBSCR
    
-   530         880 LOAD_CONST              31 (4.0)
+   349         916 BUILD_TUPLE             28
+               918 LOAD_CONST              49 (<code object prepare_evo_wash_parameters, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 349>)
+               920 MAKE_FUNCTION            6 (kwdefaults, annotations)
+               922 STORE_NAME              31 (prepare_evo_wash_parameters)
    
-   531         882 LOAD_CONST              30 (500)
+   535         924 LOAD_CONST               1 (0)
    
-   532         884 LOAD_CONST              32 (10)
+   536         926 LOAD_CONST              29 (3.0)
    
-   533         886 LOAD_CONST              33 (70)
+   537         928 LOAD_CONST              30 (500)
    
-   534         888 LOAD_CONST              34 (30)
+   538         930 LOAD_CONST              31 (4.0)
    
-   535         890 LOAD_CONST              35 (1)
+   539         932 LOAD_CONST              30 (500)
    
-   536         892 LOAD_CONST               1 (0)
+   540         934 LOAD_CONST              32 (10)
    
-   522         894 LOAD_CONST              36 (('arm', 'waste_vol', 'waste_delay', 'cleaner_vol', 'cleaner_delay', 'airgap', 'airgap_speed', 'retract_speed', 'fastwash', 'low_volume'))
-               896 BUILD_CONST_KEY_MAP     10
-               898 LOAD_CONST              21 ('tips')
+   541         936 LOAD_CONST              33 (70)
    
-   524         900 LOAD_NAME                6 (Union)
-               902 LOAD_NAME                2 (List)
-               904 LOAD_NAME               12 (Tip)
-               906 BINARY_SUBSCR
-               916 LOAD_NAME                2 (List)
-               918 LOAD_NAME               19 (int)
-               920 BINARY_SUBSCR
-               930 BUILD_TUPLE              2
-               932 BINARY_SUBSCR
+   542         938 LOAD_CONST              34 (30)
+   
+   543         940 LOAD_CONST              35 (1)
+   
+   544         942 LOAD_CONST               1 (0)
    
-   522         942 LOAD_CONST              37 ('waste_location')
+   530         944 LOAD_CONST              36 (('arm', 'waste_vol', 'waste_delay', 'cleaner_vol', 'cleaner_delay', 'airgap', 'airgap_speed', 'retract_speed', 'fastwash', 'low_volume'))
+               946 BUILD_CONST_KEY_MAP     10
+               948 LOAD_CONST              22 ('tips')
    
-   525         944 LOAD_NAME                5 (Tuple)
-               946 LOAD_NAME               19 (int)
-               948 LOAD_NAME               19 (int)
-               950 BUILD_TUPLE              2
-               952 BINARY_SUBSCR
+   532         950 LOAD_NAME                7 (Union)
+               952 LOAD_NAME                3 (List)
+               954 LOAD_NAME               13 (Tip)
+               956 BINARY_SUBSCR
+               966 LOAD_NAME                3 (List)
+               968 LOAD_NAME               20 (int)
+               970 BINARY_SUBSCR
+               980 BUILD_TUPLE              2
+               982 BINARY_SUBSCR
    
-   522         962 LOAD_CONST              38 ('cleaner_location')
+   530         992 LOAD_CONST              37 ('waste_location')
    
-   526         964 LOAD_NAME                5 (Tuple)
-               966 LOAD_NAME               19 (int)
-               968 LOAD_NAME               19 (int)
-               970 BUILD_TUPLE              2
-               972 BINARY_SUBSCR
+   533         994 LOAD_NAME                6 (Tuple)
+               996 LOAD_NAME               20 (int)
+               998 LOAD_NAME               20 (int)
+              1000 BUILD_TUPLE              2
+              1002 BINARY_SUBSCR
    
-   522         982 LOAD_CONST              39 ('arm')
+   530        1012 LOAD_CONST              38 ('cleaner_location')
    
-   527         984 LOAD_NAME               19 (int)
+   534        1014 LOAD_NAME                6 (Tuple)
+              1016 LOAD_NAME               20 (int)
+              1018 LOAD_NAME               20 (int)
+              1020 BUILD_TUPLE              2
+              1022 BINARY_SUBSCR
    
-   522         986 LOAD_CONST              40 ('waste_vol')
+   530        1032 LOAD_CONST              39 ('arm')
    
-   528         988 LOAD_NAME               24 (float)
+   535        1034 LOAD_NAME               20 (int)
    
-   522         990 LOAD_CONST              41 ('waste_delay')
+   530        1036 LOAD_CONST              40 ('waste_vol')
    
-   529         992 LOAD_NAME               19 (int)
+   536        1038 LOAD_NAME               25 (float)
    
-   522         994 LOAD_CONST              42 ('cleaner_vol')
+   530        1040 LOAD_CONST              41 ('waste_delay')
    
-   530         996 LOAD_NAME               24 (float)
+   537        1042 LOAD_NAME               20 (int)
    
-   522         998 LOAD_CONST              43 ('cleaner_delay')
+   530        1044 LOAD_CONST              42 ('cleaner_vol')
    
-   531        1000 LOAD_NAME               19 (int)
+   538        1046 LOAD_NAME               25 (float)
    
-   522        1002 LOAD_CONST              44 ('airgap')
+   530        1048 LOAD_CONST              43 ('cleaner_delay')
    
-   532        1004 LOAD_NAME               19 (int)
+   539        1050 LOAD_NAME               20 (int)
    
-   522        1006 LOAD_CONST              45 ('airgap_speed')
+   530        1052 LOAD_CONST              44 ('airgap')
    
-   533        1008 LOAD_NAME               19 (int)
+   540        1054 LOAD_NAME               20 (int)
    
-   522        1010 LOAD_CONST              46 ('retract_speed')
+   530        1056 LOAD_CONST              45 ('airgap_speed')
    
-   534        1012 LOAD_NAME               19 (int)
+   541        1058 LOAD_NAME               20 (int)
    
-   522        1014 LOAD_CONST              47 ('fastwash')
+   530        1060 LOAD_CONST              46 ('retract_speed')
    
-   535        1016 LOAD_NAME               19 (int)
+   542        1062 LOAD_NAME               20 (int)
    
-   522        1018 LOAD_CONST              48 ('low_volume')
+   530        1064 LOAD_CONST              47 ('fastwash')
    
-   536        1020 LOAD_NAME               19 (int)
+   543        1066 LOAD_NAME               20 (int)
    
-   522        1022 LOAD_CONST              23 ('return')
+   530        1068 LOAD_CONST              48 ('low_volume')
    
-   537        1024 LOAD_NAME               23 (str)
+   544        1070 LOAD_NAME               20 (int)
    
-   522        1026 BUILD_TUPLE             28
-              1028 LOAD_CONST              50 (<code object evo_wash, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 522>)
-              1030 MAKE_FUNCTION            6 (kwdefaults, annotations)
-              1032 STORE_NAME              31 (evo_wash)
-              1034 LOAD_CONST               3 (None)
-              1036 RETURN_VALUE
+   530        1072 LOAD_CONST              13 ('return')
+   
+   545        1074 LOAD_NAME               21 (str)
+   
+   530        1076 BUILD_TUPLE             28
+              1078 LOAD_CONST              50 (<code object evo_wash, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 530>)
+              1080 MAKE_FUNCTION            6 (kwdefaults, annotations)
+              1082 STORE_NAME              32 (evo_wash)
+              1084 LOAD_CONST               3 (None)
+              1086 RETURN_VALUE
    consts
       'This module implements functions to create advanced worklist commands.'
       0
-      ('List', 'Optional', 'Sequence', 'Tuple', 'Union')
+      ('Iterable', 'List', 'Optional', 'Sequence', 'Tuple', 'Union')
       None
       ('InvalidOperationError',)
       ('Tip', 'int_to_tip')
       ('to_hex',)
       2
       ('transform',)
       ('evo_make_selection_array', 'evo_get_selection', 'evo_aspirate', 'evo_wash')
       'rows'
       'columns'
       'wells'
+      'return'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c007c0166
             02a6010000ab0100000000000000007d037405000000000000000000006a
-            0300000000000000007c007c01a6020000ab0200000000000000007d047c
-            0244005d0d7d0564017c037c047c05190000000000000000003c0000008c
-            0e7c035300
+            0300000000000000007c007c01a6020000ab0200000000000000007d0474
+            01000000000000000000006a0400000000000000007c02a6010000ab0100
+            00000000000000a0050000000000000000000000000000000000000000a6
+            000000ab00000000000000000044005d0d7d0564017c037c047c05190000
+            000000000000003c0000008c0e7c035300
           20           0 RESUME                   0
          
           38           2 LOAD_GLOBAL              1 (NULL + np)
                       14 LOAD_ATTR                1 (zeros)
                       24 LOAD_FAST                0 (rows)
                       26 LOAD_FAST                1 (columns)
                       28 BUILD_TUPLE              2
@@ -583,40 +601,47 @@
                       58 LOAD_ATTR                3 (make_well_index_dict)
                       68 LOAD_FAST                0 (rows)
                       70 LOAD_FAST                1 (columns)
                       72 PRECALL                  2
                       76 CALL                     2
                       86 STORE_FAST               4 (well_index_dict)
          
-          42          88 LOAD_FAST                2 (wells)
-                      90 GET_ITER
-                 >>   92 FOR_ITER                13 (to 120)
-                      94 STORE_FAST               5 (well)
-         
-          43          96 LOAD_CONST               1 (1)
-                      98 LOAD_FAST                3 (selection_array)
-                     100 LOAD_FAST                4 (well_index_dict)
-                     102 LOAD_FAST                5 (well)
-                     104 BINARY_SUBSCR
-                     114 STORE_SUBSCR
-                     118 JUMP_BACKWARD           14 (to 92)
+          42          88 LOAD_GLOBAL              1 (NULL + np)
+                     100 LOAD_ATTR                4 (asarray)
+                     110 LOAD_FAST                2 (wells)
+                     112 PRECALL                  1
+                     116 CALL                     1
+                     126 LOAD_METHOD              5 (flatten)
+                     148 PRECALL                  0
+                     152 CALL                     0
+                     162 GET_ITER
+                 >>  164 FOR_ITER                13 (to 192)
+                     166 STORE_FAST               5 (well)
+         
+          43         168 LOAD_CONST               1 (1)
+                     170 LOAD_FAST                3 (selection_array)
+                     172 LOAD_FAST                4 (well_index_dict)
+                     174 LOAD_FAST                5 (well)
+                     176 BINARY_SUBSCR
+                     186 STORE_SUBSCR
+                     190 JUMP_BACKWARD           14 (to 164)
          
-          44     >>  120 LOAD_FAST                3 (selection_array)
-                     122 RETURN_VALUE
+          44     >>  192 LOAD_FAST                3 (selection_array)
+                     194 RETURN_VALUE
          consts
-            'Translate well IDs to a numpy array with 1s (selected) and 0s (not selected).\n\n    Parameters\n    ----------\n    rows : int\n        Number of rows of target labware object\n    cols : int\n        Number of columns of target labware object\n    wells : List[str]\n        Selected wells by well IDs as strings (e.g. ["A01", "B01"])\n\n    Returns\n    -------\n    selection_array : np.ndarray\n        Numpy array in labware dimensions with selected wells as 1 and others as 0\n    '
+            'Translate well IDs to a numpy array with 1s (selected) and 0s (not selected).\n\n    Parameters\n    ----------\n    rows : int\n        Number of rows of target labware object\n    cols : int\n        Number of columns of target labware object\n    wells : Union[Iterable[str], np.ndarray]\n        Selected wells by well IDs as strings (e.g. ["A01", "B01"])\n\n    Returns\n    -------\n    selection_array : np.ndarray\n        Numpy array in labware dimensions with selected wells as 1 and others as 0\n    '
             1
-         names      ('np', 'zeros', 'transform', 'make_well_index_dict')
+         names      ('np', 'zeros', 'transform', 'make_well_index_dict', 'asarray', 'flatten')
          varnames   ('rows', 'columns', 'wells', 'selection_array', 'well_index_dict', 'well')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
          name       'evo_make_selection_array'
          firstlineno 20
-         lnotab 0x02122c022a0208011801
+         lnotab 0x02122c022a0250011801
       'cols'
       'selected'
       code
          argcount  : 3
          nlocals   : 10
          stacksize : 7
          flags     : 3
@@ -794,586 +819,548 @@
             012a0304012c0126010c010c010c0102ff1004
       ('max_volume',)
       'labware_position'
       'volume'
       'liquid_class'
       'tips'
       'max_volume'
-      'return'
       code
          argcount  : 1
-         nlocals   : 9
+         nlocals   : 11
          stacksize : 10
          flags     : 3
          code
             0x97007c00800f7401000000000000000000006402a6010000ab01000000
             000000000082017403000000000000000000007c00740400000000000000
             000000740600000000000000000000740800000000000000000000740a00
             0000000000000000006a0600000000000000006604a6020000ab02000000
             0000000000731274010000000000000000000064037c009b009d02a60100
             00ab0100000000000000008201740f000000000000000000007c00a60100
             00ab010000000000000000740f000000000000000000007c04a6010000ab
             0100000000000000006b0200000000730f74010000000000000000000064
             04a6010000ab01000000000000000082017c01800f740100000000000000
-            0000006405a6010000ab0100000000000000008201741100000000000000
-            000000640684007c014400a6000000ab000000000000000000a6010000ab
-            0100000000000000007219741300000000000000000000640784007c0144
-            00a6000000ab000000000000000000a6010000ab01000000000000000072
-            1274010000000000000000000064087c019b009d02a6010000ab01000000
-            000000000082017c02800f7401000000000000000000006409a6010000ab
-            01000000000000000082017403000000000000000000007c027406000000
-            00000000000000a6020000ab02000000000000000072f17c0244005d777d
-            0609007415000000000000000000007c06a6010000ab0100000000000000
-            007d066e1723000100740100000000000000000000640a7c069b009d02a6
-            010000ab01000000000000000082017803590077017c06640b6b00000000
-            00731a7c06640c6b04000000007314740b000000000000000000006a0b00
-            000000000000007c06a6010000ab01000000000000000072127401000000
-            00000000000000640a7c069b009d02a6010000ab01000000000000000082
-            017c0581197c067c056b0400000000721374190000000000000000000064
-            0d7c069b00640e9d03a6010000ab01000000000000000082018c78740f00
-            0000000000000000007c02a6010000ab010000000000000000740f000000
-            000000000000007c04a6010000ab010000000000000000630278026b0200
-            0000007213740f000000000000000000007c00a6010000ab010000000000
-            0000006b020000000073426e010100741b00000000000000000000640f74
-            0f000000000000000000007c04a6010000ab0100000000000000009b0064
-            10740f000000000000000000007c00a6010000ab0100000000000000009b
-            006411740f000000000000000000007c02a6010000ab0100000000000000
-            009b0064129d07a6010000ab01000000000000000082016e9c7403000000
-            000000000000007c02741400000000000000000000741c00000000000000
-            0000006602a6020000ab020000000000000000726e7c02640b6b00000000
-            00731a7c02640c6b04000000007314740b000000000000000000006a0b00
-            000000000000007c02a6010000ab01000000000000000072127401000000
-            00000000000000640a7c029b009d02a6010000ab01000000000000000082
-            017c0581197c027c056b0400000000721374190000000000000000000064
-            0d7c029b00640e9d03a6010000ab01000000000000000082017415000000
-            000000000000007c02a6010000ab0100000000000000006701740f000000
-            000000000000007c00a6010000ab0100000000000000007a0500007d026e
-            12740100000000000000000000640a7c029b009d02a6010000ab01000000
-            00000000008201740b000000000000000000006a0f00000000000000007c
-            026413ac14a6020000ab020000000000000000a010000000000000000000
-            0000000000000000000000a6000000ab0000000000000000007d027c0380
-            0f7401000000000000000000006415a6010000ab01000000000000000082
-            017403000000000000000000007c03740400000000000000000000a60200
-            00ab020000000000000000720464167c0376007212740100000000000000
-            00000064177c039b009d02a6010000ab01000000000000000082017c0480
-            0f7401000000000000000000006418a6010000ab01000000000000000082
-            017c0444005d3e7d077403000000000000000000007c07741c0000000000
-            00000000007422000000000000000000006602a6020000ab020000000000
-            000000732074010000000000000000000064197425000000000000000000
-            007c07a6010000ab0100000000000000009b00641a9d03a6010000ab0100
-            0000000000000082018c3f67007d087c0444005d507d0774030000000000
-            00000000007c07741c00000000000000000000a6020000ab020000000000
-            00000072247403000000000000000000007c077422000000000000000000
-            00a6020000ab020000000000000000730f7427000000000000000000007c
-            07a6010000ab0100000000000000007d077c08a014000000000000000000
-            00000000000000000000007c07a6010000ab01000000000000000001008c
-            517c007c017c027c037c0866055300
+            0000006405a6010000ab01000000000000000082017c015c0200007d067d
+            077403000000000000000000007c06741000000000000000000000a60200
+            00ab020000000000000000720f64067c06630278026b0100000000720664
+            076b010000000073116e0101007401000000000000000000006408a60100
+            00ab01000000000000000082017403000000000000000000007c07741000
+            000000000000000000a6020000ab020000000000000000720f64067c0763
+            0278026b0100000000720664096b010000000073116e0101007401000000
+            00000000000000640aa6010000ab01000000000000000082017c067c0764
+            067a0a000066027d017c02800f740100000000000000000000640ba60100
+            00ab01000000000000000082017403000000000000000000007c02740600
+            000000000000000000a6020000ab02000000000000000072f17c0244005d
+            777d0809007413000000000000000000007c08a6010000ab010000000000
+            0000007d086e1723000100740100000000000000000000640c7c089b009d
+            02a6010000ab01000000000000000082017803590077017c08640d6b0000
+            000000731a7c08640e6b04000000007314740b000000000000000000006a
+            0a00000000000000007c08a6010000ab0100000000000000007212740100
+            000000000000000000640c7c089b009d02a6010000ab0100000000000000
+            0082017c0581197c087c056b040000000072137417000000000000000000
+            00640f7c089b0064109d03a6010000ab01000000000000000082018c7874
+            0f000000000000000000007c02a6010000ab010000000000000000740f00
+            0000000000000000007c04a6010000ab010000000000000000630278026b
+            02000000007213740f000000000000000000007c00a6010000ab01000000
+            00000000006b020000000073426e01010074190000000000000000000064
+            11740f000000000000000000007c04a6010000ab0100000000000000009b
+            006412740f000000000000000000007c00a6010000ab0100000000000000
+            009b006413740f000000000000000000007c02a6010000ab010000000000
+            0000009b0064149d07a6010000ab01000000000000000082016e9c740300
+            0000000000000000007c0274120000000000000000000074100000000000
+            00000000006602a6020000ab020000000000000000726e7c02640d6b0000
+            000000731a7c02640e6b04000000007314740b000000000000000000006a
+            0a00000000000000007c02a6010000ab0100000000000000007212740100
+            000000000000000000640c7c029b009d02a6010000ab0100000000000000
+            0082017c0581197c027c056b040000000072137417000000000000000000
+            00640f7c029b0064109d03a6010000ab0100000000000000008201741300
+            0000000000000000007c02a6010000ab0100000000000000006701740f00
+            0000000000000000007c00a6010000ab0100000000000000007a0500007d
+            026e12740100000000000000000000640c7c029b009d02a6010000ab0100
+            000000000000008201740b000000000000000000006a0d00000000000000
+            007c026415ac16a6020000ab020000000000000000a00e00000000000000
+            00000000000000000000000000a6000000ab0000000000000000007d027c
+            03800f7401000000000000000000006417a6010000ab0100000000000000
+            0082017403000000000000000000007c03740400000000000000000000a6
+            020000ab020000000000000000720464187c037600721274010000000000
+            000000000064197c039b009d02a6010000ab01000000000000000082017c
+            04800f740100000000000000000000641aa6010000ab0100000000000000
+            0082017c0444005d3e7d097403000000000000000000007c097410000000
+            00000000000000741e000000000000000000006602a6020000ab02000000
+            00000000007320740100000000000000000000641b742100000000000000
+            0000007c09a6010000ab0100000000000000009b00641c9d03a6010000ab
+            01000000000000000082018c3f67007d0a7c0444005d507d097403000000
+            000000000000007c09741000000000000000000000a6020000ab02000000
+            000000000072247403000000000000000000007c09741e00000000000000
+            000000a6020000ab020000000000000000730f7423000000000000000000
+            007c09a6010000ab0100000000000000007d097c0aa01200000000000000
+            000000000000000000000000007c09a6010000ab01000000000000000001
+            008c517c007c017c027c037c0a66055300
           95           0 RESUME                   0
          
-         134           2 LOAD_FAST                0 (wells)
+         136           2 LOAD_FAST                0 (wells)
                        4 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 36)
          
-         135           6 LOAD_GLOBAL              1 (NULL + ValueError)
+         137           6 LOAD_GLOBAL              1 (NULL + ValueError)
                       18 LOAD_CONST               2 ('Missing required parameter: wells')
                       20 PRECALL                  1
                       24 CALL                     1
                       34 RAISE_VARARGS            1
          
-         136     >>   36 LOAD_GLOBAL              3 (NULL + isinstance)
+         138     >>   36 LOAD_GLOBAL              3 (NULL + isinstance)
                       48 LOAD_FAST                0 (wells)
                       50 LOAD_GLOBAL              4 (str)
                       62 LOAD_GLOBAL              6 (list)
                       74 LOAD_GLOBAL              8 (tuple)
                       86 LOAD_GLOBAL             10 (np)
                       98 LOAD_ATTR                6 (ndarray)
                      108 BUILD_TUPLE              4
                      110 PRECALL                  2
                      114 CALL                     2
                      124 POP_JUMP_FORWARD_IF_TRUE    18 (to 162)
          
-         137         126 LOAD_GLOBAL              1 (NULL + ValueError)
+         139         126 LOAD_GLOBAL              1 (NULL + ValueError)
                      138 LOAD_CONST               3 ('Invalid wells: ')
                      140 LOAD_FAST                0 (wells)
                      142 FORMAT_VALUE             0
                      144 BUILD_STRING             2
                      146 PRECALL                  1
                      150 CALL                     1
                      160 RAISE_VARARGS            1
          
-         138     >>  162 LOAD_GLOBAL             15 (NULL + len)
+         140     >>  162 LOAD_GLOBAL             15 (NULL + len)
                      174 LOAD_FAST                0 (wells)
                      176 PRECALL                  1
                      180 CALL                     1
                      190 LOAD_GLOBAL             15 (NULL + len)
                      202 LOAD_FAST                4 (tips)
                      204 PRECALL                  1
                      208 CALL                     1
                      218 COMPARE_OP               2 (==)
                      224 POP_JUMP_FORWARD_IF_TRUE    15 (to 256)
          
-         139         226 LOAD_GLOBAL              1 (NULL + ValueError)
+         141         226 LOAD_GLOBAL              1 (NULL + ValueError)
                      238 LOAD_CONST               4 ('Invalid wells: wells and tips need to have the same length.')
                      240 PRECALL                  1
                      244 CALL                     1
                      254 RAISE_VARARGS            1
          
-         140     >>  256 LOAD_FAST                1 (labware_position)
+         142     >>  256 LOAD_FAST                1 (labware_position)
                      258 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 290)
          
-         141         260 LOAD_GLOBAL              1 (NULL + ValueError)
+         143         260 LOAD_GLOBAL              1 (NULL + ValueError)
                      272 LOAD_CONST               5 ('Missing required parameter: position')
                      274 PRECALL                  1
                      278 CALL                     1
                      288 RAISE_VARARGS            1
          
-         142     >>  290 LOAD_GLOBAL             17 (NULL + all)
-                     302 LOAD_CONST               6 (<code object <genexpr>, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 142>)
-                     304 MAKE_FUNCTION            0
-                     306 LOAD_FAST                1 (labware_position)
-                     308 GET_ITER
-                     310 PRECALL                  0
-                     314 CALL                     0
-                     324 PRECALL                  1
-                     328 CALL                     1
-                     338 POP_JUMP_FORWARD_IF_FALSE    25 (to 390)
-                     340 LOAD_GLOBAL             19 (NULL + any)
-                     352 LOAD_CONST               7 (<code object <genexpr>, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 142>)
-                     354 MAKE_FUNCTION            0
-         
-         143         356 LOAD_FAST                1 (labware_position)
-         
-         142         358 GET_ITER
-                     360 PRECALL                  0
-                     364 CALL                     0
-                     374 PRECALL                  1
-                     378 CALL                     1
-                     388 POP_JUMP_FORWARD_IF_FALSE    18 (to 426)
-         
-         145     >>  390 LOAD_GLOBAL              1 (NULL + ValueError)
-                     402 LOAD_CONST               8 ('Invalid position: ')
-                     404 LOAD_FAST                1 (labware_position)
-                     406 FORMAT_VALUE             0
-                     408 BUILD_STRING             2
-                     410 PRECALL                  1
-                     414 CALL                     1
-                     424 RAISE_VARARGS            1
-         
-         147     >>  426 LOAD_FAST                2 (volume)
-                     428 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 460)
-         
-         148         430 LOAD_GLOBAL              1 (NULL + ValueError)
-                     442 LOAD_CONST               9 ('Missing required parameter: volume')
-                     444 PRECALL                  1
-                     448 CALL                     1
-                     458 RAISE_VARARGS            1
-         
-         149     >>  460 LOAD_GLOBAL              3 (NULL + isinstance)
-                     472 LOAD_FAST                2 (volume)
-                     474 LOAD_GLOBAL              6 (list)
-                     486 PRECALL                  2
-                     490 CALL                     2
-                     500 POP_JUMP_FORWARD_IF_FALSE   241 (to 984)
-         
-         150         502 LOAD_FAST                2 (volume)
-                     504 GET_ITER
-                 >>  506 FOR_ITER               119 (to 746)
-                     508 STORE_FAST               6 (vol)
-         
-         151         510 NOP
-         
-         152         512 LOAD_GLOBAL             21 (NULL + float)
-                     524 LOAD_FAST                6 (vol)
-                     526 PRECALL                  1
-                     530 CALL                     1
-                     540 STORE_FAST               6 (vol)
-                     542 JUMP_FORWARD            23 (to 590)
-                 >>  544 PUSH_EXC_INFO
-         
-         153         546 POP_TOP
-         
-         154         548 LOAD_GLOBAL              1 (NULL + ValueError)
-                     560 LOAD_CONST              10 ('Invalid volume: ')
-                     562 LOAD_FAST                6 (vol)
-                     564 FORMAT_VALUE             0
-                     566 BUILD_STRING             2
-                     568 PRECALL                  1
-                     572 CALL                     1
-                     582 RAISE_VARARGS            1
-                 >>  584 COPY                     3
-                     586 POP_EXCEPT
-                     588 RERAISE                  1
-         
-         155     >>  590 LOAD_FAST                6 (vol)
-                     592 LOAD_CONST              11 (0)
-                     594 COMPARE_OP               0 (<)
-                     600 POP_JUMP_FORWARD_IF_TRUE    26 (to 654)
-                     602 LOAD_FAST                6 (vol)
-                     604 LOAD_CONST              12 (7158278)
-                     606 COMPARE_OP               4 (>)
-                     612 POP_JUMP_FORWARD_IF_TRUE    20 (to 654)
-                     614 LOAD_GLOBAL             11 (NULL + np)
-                     626 LOAD_ATTR               11 (isnan)
-                     636 LOAD_FAST                6 (vol)
-                     638 PRECALL                  1
-                     642 CALL                     1
-                     652 POP_JUMP_FORWARD_IF_FALSE    18 (to 690)
-         
-         156     >>  654 LOAD_GLOBAL              1 (NULL + ValueError)
-                     666 LOAD_CONST              10 ('Invalid volume: ')
-                     668 LOAD_FAST                6 (vol)
-                     670 FORMAT_VALUE             0
-                     672 BUILD_STRING             2
-                     674 PRECALL                  1
-                     678 CALL                     1
-                     688 RAISE_VARARGS            1
-         
-         157     >>  690 LOAD_FAST                5 (max_volume)
-                     692 POP_JUMP_FORWARD_IF_NONE    25 (to 744)
-                     694 LOAD_FAST                6 (vol)
-                     696 LOAD_FAST                5 (max_volume)
+         144     >>  290 LOAD_FAST                1 (labware_position)
+                     292 UNPACK_SEQUENCE          2
+                     296 STORE_FAST               6 (grid)
+                     298 STORE_FAST               7 (site)
+         
+         145         300 LOAD_GLOBAL              3 (NULL + isinstance)
+                     312 LOAD_FAST                6 (grid)
+                     314 LOAD_GLOBAL             16 (int)
+                     326 PRECALL                  2
+                     330 CALL                     2
+                     340 POP_JUMP_FORWARD_IF_FALSE    15 (to 372)
+                     342 LOAD_CONST               6 (1)
+                     344 LOAD_FAST                6 (grid)
+                     346 SWAP                     2
+                     348 COPY                     2
+                     350 COMPARE_OP               1 (<=)
+                     356 POP_JUMP_FORWARD_IF_FALSE     6 (to 370)
+                     358 LOAD_CONST               7 (67)
+                     360 COMPARE_OP               1 (<=)
+                     366 POP_JUMP_FORWARD_IF_TRUE    17 (to 402)
+                     368 JUMP_FORWARD             1 (to 372)
+                 >>  370 POP_TOP
+         
+         146     >>  372 LOAD_GLOBAL              1 (NULL + ValueError)
+                     384 LOAD_CONST               8 ('Grid (first number in labware_position tuple) has to be an int from 1 - 67.')
+                     386 PRECALL                  1
+                     390 CALL                     1
+                     400 RAISE_VARARGS            1
+         
+         147     >>  402 LOAD_GLOBAL              3 (NULL + isinstance)
+                     414 LOAD_FAST                7 (site)
+                     416 LOAD_GLOBAL             16 (int)
+                     428 PRECALL                  2
+                     432 CALL                     2
+                     442 POP_JUMP_FORWARD_IF_FALSE    15 (to 474)
+                     444 LOAD_CONST               6 (1)
+                     446 LOAD_FAST                7 (site)
+                     448 SWAP                     2
+                     450 COPY                     2
+                     452 COMPARE_OP               1 (<=)
+                     458 POP_JUMP_FORWARD_IF_FALSE     6 (to 472)
+                     460 LOAD_CONST               9 (128)
+                     462 COMPARE_OP               1 (<=)
+                     468 POP_JUMP_FORWARD_IF_TRUE    17 (to 504)
+                     470 JUMP_FORWARD             1 (to 474)
+                 >>  472 POP_TOP
+         
+         148     >>  474 LOAD_GLOBAL              1 (NULL + ValueError)
+                     486 LOAD_CONST              10 ('Site (second number in labware_position tuple) has to be an int from 1 - 128.')
+                     488 PRECALL                  1
+                     492 CALL                     1
+                     502 RAISE_VARARGS            1
+         
+         149     >>  504 LOAD_FAST                6 (grid)
+                     506 LOAD_FAST                7 (site)
+                     508 LOAD_CONST               6 (1)
+                     510 BINARY_OP               10 (-)
+                     514 BUILD_TUPLE              2
+                     516 STORE_FAST               1 (labware_position)
+         
+         151         518 LOAD_FAST                2 (volume)
+                     520 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 552)
+         
+         152         522 LOAD_GLOBAL              1 (NULL + ValueError)
+                     534 LOAD_CONST              11 ('Missing required parameter: volume')
+                     536 PRECALL                  1
+                     540 CALL                     1
+                     550 RAISE_VARARGS            1
+         
+         153     >>  552 LOAD_GLOBAL              3 (NULL + isinstance)
+                     564 LOAD_FAST                2 (volume)
+                     566 LOAD_GLOBAL              6 (list)
+                     578 PRECALL                  2
+                     582 CALL                     2
+                     592 POP_JUMP_FORWARD_IF_FALSE   241 (to 1076)
+         
+         154         594 LOAD_FAST                2 (volume)
+                     596 GET_ITER
+                 >>  598 FOR_ITER               119 (to 838)
+                     600 STORE_FAST               8 (vol)
+         
+         155         602 NOP
+         
+         156         604 LOAD_GLOBAL             19 (NULL + float)
+                     616 LOAD_FAST                8 (vol)
+                     618 PRECALL                  1
+                     622 CALL                     1
+                     632 STORE_FAST               8 (vol)
+                     634 JUMP_FORWARD            23 (to 682)
+                 >>  636 PUSH_EXC_INFO
+         
+         157         638 POP_TOP
+         
+         158         640 LOAD_GLOBAL              1 (NULL + ValueError)
+                     652 LOAD_CONST              12 ('Invalid volume: ')
+                     654 LOAD_FAST                8 (vol)
+                     656 FORMAT_VALUE             0
+                     658 BUILD_STRING             2
+                     660 PRECALL                  1
+                     664 CALL                     1
+                     674 RAISE_VARARGS            1
+                 >>  676 COPY                     3
+                     678 POP_EXCEPT
+                     680 RERAISE                  1
+         
+         159     >>  682 LOAD_FAST                8 (vol)
+                     684 LOAD_CONST              13 (0)
+                     686 COMPARE_OP               0 (<)
+                     692 POP_JUMP_FORWARD_IF_TRUE    26 (to 746)
+                     694 LOAD_FAST                8 (vol)
+                     696 LOAD_CONST              14 (7158278)
                      698 COMPARE_OP               4 (>)
-                     704 POP_JUMP_FORWARD_IF_FALSE    19 (to 744)
+                     704 POP_JUMP_FORWARD_IF_TRUE    20 (to 746)
+                     706 LOAD_GLOBAL             11 (NULL + np)
+                     718 LOAD_ATTR               10 (isnan)
+                     728 LOAD_FAST                8 (vol)
+                     730 PRECALL                  1
+                     734 CALL                     1
+                     744 POP_JUMP_FORWARD_IF_FALSE    18 (to 782)
+         
+         160     >>  746 LOAD_GLOBAL              1 (NULL + ValueError)
+                     758 LOAD_CONST              12 ('Invalid volume: ')
+                     760 LOAD_FAST                8 (vol)
+                     762 FORMAT_VALUE             0
+                     764 BUILD_STRING             2
+                     766 PRECALL                  1
+                     770 CALL                     1
+                     780 RAISE_VARARGS            1
+         
+         161     >>  782 LOAD_FAST                5 (max_volume)
+                     784 POP_JUMP_FORWARD_IF_NONE    25 (to 836)
+                     786 LOAD_FAST                8 (vol)
+                     788 LOAD_FAST                5 (max_volume)
+                     790 COMPARE_OP               4 (>)
+                     796 POP_JUMP_FORWARD_IF_FALSE    19 (to 836)
+         
+         162         798 LOAD_GLOBAL             23 (NULL + InvalidOperationError)
+                     810 LOAD_CONST              15 ('Invalid volume: volume of ')
+                     812 LOAD_FAST                8 (vol)
+                     814 FORMAT_VALUE             0
+                     816 LOAD_CONST              16 (' exceeds max_volume.')
+                     818 BUILD_STRING             3
+                     820 PRECALL                  1
+                     824 CALL                     1
+                     834 RAISE_VARARGS            1
+                 >>  836 JUMP_BACKWARD          120 (to 598)
+         
+         163     >>  838 LOAD_GLOBAL             15 (NULL + len)
+                     850 LOAD_FAST                2 (volume)
+                     852 PRECALL                  1
+                     856 CALL                     1
+                     866 LOAD_GLOBAL             15 (NULL + len)
+                     878 LOAD_FAST                4 (tips)
+                     880 PRECALL                  1
+                     884 CALL                     1
+                     894 SWAP                     2
+                     896 COPY                     2
+                     898 COMPARE_OP               2 (==)
+                     904 POP_JUMP_FORWARD_IF_FALSE    19 (to 944)
+                     906 LOAD_GLOBAL             15 (NULL + len)
+                     918 LOAD_FAST                0 (wells)
+                     920 PRECALL                  1
+                     924 CALL                     1
+                     934 COMPARE_OP               2 (==)
+                     940 POP_JUMP_FORWARD_IF_TRUE    66 (to 1074)
+                     942 JUMP_FORWARD             1 (to 946)
+                 >>  944 POP_TOP
+         
+         164     >>  946 LOAD_GLOBAL             25 (NULL + Exception)
+         
+         165         958 LOAD_CONST              17 ('Invalid volume: Tips, wells, and volume lists have different lengths (')
+                     960 LOAD_GLOBAL             15 (NULL + len)
+                     972 LOAD_FAST                4 (tips)
+                     974 PRECALL                  1
+                     978 CALL                     1
+                     988 FORMAT_VALUE             0
+                     990 LOAD_CONST              18 (', ')
+                     992 LOAD_GLOBAL             15 (NULL + len)
+                    1004 LOAD_FAST                0 (wells)
+                    1006 PRECALL                  1
+                    1010 CALL                     1
+                    1020 FORMAT_VALUE             0
+                    1022 LOAD_CONST              19 (' and ')
+                    1024 LOAD_GLOBAL             15 (NULL + len)
+                    1036 LOAD_FAST                2 (volume)
+                    1038 PRECALL                  1
+                    1042 CALL                     1
+                    1052 FORMAT_VALUE             0
+                    1054 LOAD_CONST              20 (', respectively).')
+                    1056 BUILD_STRING             7
          
-         158         706 LOAD_GLOBAL             25 (NULL + InvalidOperationError)
-                     718 LOAD_CONST              13 ('Invalid volume: volume of ')
-                     720 LOAD_FAST                6 (vol)
-                     722 FORMAT_VALUE             0
-                     724 LOAD_CONST              14 (' exceeds max_volume.')
-                     726 BUILD_STRING             3
-                     728 PRECALL                  1
-                     732 CALL                     1
-                     742 RAISE_VARARGS            1
-                 >>  744 JUMP_BACKWARD          120 (to 506)
-         
-         159     >>  746 LOAD_GLOBAL             15 (NULL + len)
-                     758 LOAD_FAST                2 (volume)
-                     760 PRECALL                  1
-                     764 CALL                     1
-                     774 LOAD_GLOBAL             15 (NULL + len)
-                     786 LOAD_FAST                4 (tips)
-                     788 PRECALL                  1
-                     792 CALL                     1
-                     802 SWAP                     2
-                     804 COPY                     2
-                     806 COMPARE_OP               2 (==)
-                     812 POP_JUMP_FORWARD_IF_FALSE    19 (to 852)
-                     814 LOAD_GLOBAL             15 (NULL + len)
-                     826 LOAD_FAST                0 (wells)
-                     828 PRECALL                  1
-                     832 CALL                     1
-                     842 COMPARE_OP               2 (==)
-                     848 POP_JUMP_FORWARD_IF_TRUE    66 (to 982)
-                     850 JUMP_FORWARD             1 (to 854)
-                 >>  852 POP_TOP
-         
-         160     >>  854 LOAD_GLOBAL             27 (NULL + Exception)
-         
-         161         866 LOAD_CONST              15 ('Invalid volume: Tips, wells, and volume lists have different lengths (')
-                     868 LOAD_GLOBAL             15 (NULL + len)
-                     880 LOAD_FAST                4 (tips)
-                     882 PRECALL                  1
-                     886 CALL                     1
-                     896 FORMAT_VALUE             0
-                     898 LOAD_CONST              16 (', ')
-                     900 LOAD_GLOBAL             15 (NULL + len)
-                     912 LOAD_FAST                0 (wells)
-                     914 PRECALL                  1
-                     918 CALL                     1
-                     928 FORMAT_VALUE             0
-                     930 LOAD_CONST              17 (' and ')
-                     932 LOAD_GLOBAL             15 (NULL + len)
-                     944 LOAD_FAST                2 (volume)
-                     946 PRECALL                  1
-                     950 CALL                     1
-                     960 FORMAT_VALUE             0
-                     962 LOAD_CONST              18 (', respectively).')
-                     964 BUILD_STRING             7
-         
-         160         966 PRECALL                  1
-                     970 CALL                     1
-                     980 RAISE_VARARGS            1
-         
-         159     >>  982 JUMP_FORWARD           156 (to 1296)
-         
-         163     >>  984 LOAD_GLOBAL              3 (NULL + isinstance)
-                     996 LOAD_FAST                2 (volume)
-                     998 LOAD_GLOBAL             20 (float)
-                    1010 LOAD_GLOBAL             28 (int)
-                    1022 BUILD_TUPLE              2
-                    1024 PRECALL                  2
-                    1028 CALL                     2
-                    1038 POP_JUMP_FORWARD_IF_FALSE   110 (to 1260)
-         
-         165        1040 LOAD_FAST                2 (volume)
-                    1042 LOAD_CONST              11 (0)
-                    1044 COMPARE_OP               0 (<)
-                    1050 POP_JUMP_FORWARD_IF_TRUE    26 (to 1104)
-                    1052 LOAD_FAST                2 (volume)
-                    1054 LOAD_CONST              12 (7158278)
-                    1056 COMPARE_OP               4 (>)
-                    1062 POP_JUMP_FORWARD_IF_TRUE    20 (to 1104)
-                    1064 LOAD_GLOBAL             11 (NULL + np)
-                    1076 LOAD_ATTR               11 (isnan)
-                    1086 LOAD_FAST                2 (volume)
-                    1088 PRECALL                  1
-                    1092 CALL                     1
-                    1102 POP_JUMP_FORWARD_IF_FALSE    18 (to 1140)
-         
-         166     >> 1104 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1116 LOAD_CONST              10 ('Invalid volume: ')
-                    1118 LOAD_FAST                2 (volume)
-                    1120 FORMAT_VALUE             0
-                    1122 BUILD_STRING             2
-                    1124 PRECALL                  1
-                    1128 CALL                     1
-                    1138 RAISE_VARARGS            1
+         164        1058 PRECALL                  1
+                    1062 CALL                     1
+                    1072 RAISE_VARARGS            1
+         
+         163     >> 1074 JUMP_FORWARD           156 (to 1388)
          
-         167     >> 1140 LOAD_FAST                5 (max_volume)
-                    1142 POP_JUMP_FORWARD_IF_NONE    25 (to 1194)
+         167     >> 1076 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1088 LOAD_FAST                2 (volume)
+                    1090 LOAD_GLOBAL             18 (float)
+                    1102 LOAD_GLOBAL             16 (int)
+                    1114 BUILD_TUPLE              2
+                    1116 PRECALL                  2
+                    1120 CALL                     2
+                    1130 POP_JUMP_FORWARD_IF_FALSE   110 (to 1352)
+         
+         169        1132 LOAD_FAST                2 (volume)
+                    1134 LOAD_CONST              13 (0)
+                    1136 COMPARE_OP               0 (<)
+                    1142 POP_JUMP_FORWARD_IF_TRUE    26 (to 1196)
                     1144 LOAD_FAST                2 (volume)
-                    1146 LOAD_FAST                5 (max_volume)
+                    1146 LOAD_CONST              14 (7158278)
                     1148 COMPARE_OP               4 (>)
-                    1154 POP_JUMP_FORWARD_IF_FALSE    19 (to 1194)
-         
-         168        1156 LOAD_GLOBAL             25 (NULL + InvalidOperationError)
-                    1168 LOAD_CONST              13 ('Invalid volume: volume of ')
-                    1170 LOAD_FAST                2 (volume)
-                    1172 FORMAT_VALUE             0
-                    1174 LOAD_CONST              14 (' exceeds max_volume.')
-                    1176 BUILD_STRING             3
-                    1178 PRECALL                  1
-                    1182 CALL                     1
-                    1192 RAISE_VARARGS            1
-         
-         170     >> 1194 LOAD_GLOBAL             21 (NULL + float)
-                    1206 LOAD_FAST                2 (volume)
-                    1208 PRECALL                  1
-                    1212 CALL                     1
-                    1222 BUILD_LIST               1
-                    1224 LOAD_GLOBAL             15 (NULL + len)
-                    1236 LOAD_FAST                0 (wells)
-                    1238 PRECALL                  1
-                    1242 CALL                     1
-                    1252 BINARY_OP                5 (*)
-                    1256 STORE_FAST               2 (volume)
-                    1258 JUMP_FORWARD            18 (to 1296)
-         
-         172     >> 1260 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1272 LOAD_CONST              10 ('Invalid volume: ')
-                    1274 LOAD_FAST                2 (volume)
-                    1276 FORMAT_VALUE             0
-                    1278 BUILD_STRING             2
-                    1280 PRECALL                  1
-                    1284 CALL                     1
-                    1294 RAISE_VARARGS            1
-         
-         175     >> 1296 LOAD_GLOBAL             11 (NULL + np)
-                    1308 LOAD_ATTR               15 (round)
-                    1318 LOAD_FAST                2 (volume)
-                    1320 LOAD_CONST              19 (2)
-                    1322 KW_NAMES                20
-                    1324 PRECALL                  2
-                    1328 CALL                     2
-                    1338 LOAD_METHOD             16 (tolist)
-                    1360 PRECALL                  0
-                    1364 CALL                     0
-                    1374 STORE_FAST               2 (volume)
-         
-         177        1376 LOAD_FAST                3 (liquid_class)
-                    1378 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1410)
-         
-         178        1380 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1392 LOAD_CONST              21 ('Missing required parameter: liquid_class')
-                    1394 PRECALL                  1
-                    1398 CALL                     1
-                    1408 RAISE_VARARGS            1
-         
-         179     >> 1410 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1422 LOAD_FAST                3 (liquid_class)
-                    1424 LOAD_GLOBAL              4 (str)
-                    1436 PRECALL                  2
-                    1440 CALL                     2
-                    1450 POP_JUMP_FORWARD_IF_FALSE     4 (to 1460)
-                    1452 LOAD_CONST              22 (';')
-                    1454 LOAD_FAST                3 (liquid_class)
-                    1456 CONTAINS_OP              0
-                    1458 POP_JUMP_FORWARD_IF_FALSE    18 (to 1496)
-         
-         180     >> 1460 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1472 LOAD_CONST              23 ('Invalid liquid_class: ')
-                    1474 LOAD_FAST                3 (liquid_class)
-                    1476 FORMAT_VALUE             0
-                    1478 BUILD_STRING             2
-                    1480 PRECALL                  1
-                    1484 CALL                     1
-                    1494 RAISE_VARARGS            1
-         
-         182     >> 1496 LOAD_FAST                4 (tips)
-                    1498 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1530)
-         
-         183        1500 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1512 LOAD_CONST              24 ('Missing required parameter: tips')
-                    1514 PRECALL                  1
-                    1518 CALL                     1
-                    1528 RAISE_VARARGS            1
-         
-         184     >> 1530 LOAD_FAST                4 (tips)
-                    1532 GET_ITER
-                 >> 1534 FOR_ITER                62 (to 1660)
-                    1536 STORE_FAST               7 (tip)
-         
-         185        1538 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1550 LOAD_FAST                7 (tip)
-                    1552 LOAD_GLOBAL             28 (int)
-                    1564 LOAD_GLOBAL             34 (Tip)
-                    1576 BUILD_TUPLE              2
-                    1578 PRECALL                  2
-                    1582 CALL                     2
-                    1592 POP_JUMP_FORWARD_IF_TRUE    32 (to 1658)
+                    1154 POP_JUMP_FORWARD_IF_TRUE    20 (to 1196)
+                    1156 LOAD_GLOBAL             11 (NULL + np)
+                    1168 LOAD_ATTR               10 (isnan)
+                    1178 LOAD_FAST                2 (volume)
+                    1180 PRECALL                  1
+                    1184 CALL                     1
+                    1194 POP_JUMP_FORWARD_IF_FALSE    18 (to 1232)
+         
+         170     >> 1196 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1208 LOAD_CONST              12 ('Invalid volume: ')
+                    1210 LOAD_FAST                2 (volume)
+                    1212 FORMAT_VALUE             0
+                    1214 BUILD_STRING             2
+                    1216 PRECALL                  1
+                    1220 CALL                     1
+                    1230 RAISE_VARARGS            1
+         
+         171     >> 1232 LOAD_FAST                5 (max_volume)
+                    1234 POP_JUMP_FORWARD_IF_NONE    25 (to 1286)
+                    1236 LOAD_FAST                2 (volume)
+                    1238 LOAD_FAST                5 (max_volume)
+                    1240 COMPARE_OP               4 (>)
+                    1246 POP_JUMP_FORWARD_IF_FALSE    19 (to 1286)
+         
+         172        1248 LOAD_GLOBAL             23 (NULL + InvalidOperationError)
+                    1260 LOAD_CONST              15 ('Invalid volume: volume of ')
+                    1262 LOAD_FAST                2 (volume)
+                    1264 FORMAT_VALUE             0
+                    1266 LOAD_CONST              16 (' exceeds max_volume.')
+                    1268 BUILD_STRING             3
+                    1270 PRECALL                  1
+                    1274 CALL                     1
+                    1284 RAISE_VARARGS            1
+         
+         174     >> 1286 LOAD_GLOBAL             19 (NULL + float)
+                    1298 LOAD_FAST                2 (volume)
+                    1300 PRECALL                  1
+                    1304 CALL                     1
+                    1314 BUILD_LIST               1
+                    1316 LOAD_GLOBAL             15 (NULL + len)
+                    1328 LOAD_FAST                0 (wells)
+                    1330 PRECALL                  1
+                    1334 CALL                     1
+                    1344 BINARY_OP                5 (*)
+                    1348 STORE_FAST               2 (volume)
+                    1350 JUMP_FORWARD            18 (to 1388)
+         
+         176     >> 1352 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1364 LOAD_CONST              12 ('Invalid volume: ')
+                    1366 LOAD_FAST                2 (volume)
+                    1368 FORMAT_VALUE             0
+                    1370 BUILD_STRING             2
+                    1372 PRECALL                  1
+                    1376 CALL                     1
+                    1386 RAISE_VARARGS            1
          
-         186        1594 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1606 LOAD_CONST              25 ('Invalid type of tips: ')
-                    1608 LOAD_GLOBAL             37 (NULL + type)
-                    1620 LOAD_FAST                7 (tip)
-                    1622 PRECALL                  1
-                    1626 CALL                     1
-                    1636 FORMAT_VALUE             0
-                    1638 LOAD_CONST              26 ('. Has to be int or Tip.')
-                    1640 BUILD_STRING             3
-                    1642 PRECALL                  1
-                    1646 CALL                     1
-                    1656 RAISE_VARARGS            1
-         
-         185     >> 1658 JUMP_BACKWARD           63 (to 1534)
-         
-         187     >> 1660 BUILD_LIST               0
-                    1662 STORE_FAST               8 (tecan_tips)
-         
-         188        1664 LOAD_FAST                4 (tips)
-                    1666 GET_ITER
-                 >> 1668 FOR_ITER                80 (to 1830)
-                    1670 STORE_FAST               7 (tip)
-         
-         189        1672 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1684 LOAD_FAST                7 (tip)
-                    1686 LOAD_GLOBAL             28 (int)
-                    1698 PRECALL                  2
-                    1702 CALL                     2
-                    1712 POP_JUMP_FORWARD_IF_FALSE    36 (to 1786)
-                    1714 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1726 LOAD_FAST                7 (tip)
-                    1728 LOAD_GLOBAL             34 (Tip)
-                    1740 PRECALL                  2
-                    1744 CALL                     2
-                    1754 POP_JUMP_FORWARD_IF_TRUE    15 (to 1786)
-         
-         191        1756 LOAD_GLOBAL             39 (NULL + int_to_tip)
-                    1768 LOAD_FAST                7 (tip)
-                    1770 PRECALL                  1
-                    1774 CALL                     1
-                    1784 STORE_FAST               7 (tip)
-         
-         192     >> 1786 LOAD_FAST                8 (tecan_tips)
-                    1788 LOAD_METHOD             20 (append)
-                    1810 LOAD_FAST                7 (tip)
-                    1812 PRECALL                  1
-                    1816 CALL                     1
-                    1826 POP_TOP
-                    1828 JUMP_BACKWARD           81 (to 1668)
-         
-         194     >> 1830 LOAD_FAST                0 (wells)
-                    1832 LOAD_FAST                1 (labware_position)
-                    1834 LOAD_FAST                2 (volume)
-                    1836 LOAD_FAST                3 (liquid_class)
-                    1838 LOAD_FAST                8 (tecan_tips)
-                    1840 BUILD_TUPLE              5
-                    1842 RETURN_VALUE
+         179     >> 1388 LOAD_GLOBAL             11 (NULL + np)
+                    1400 LOAD_ATTR               13 (round)
+                    1410 LOAD_FAST                2 (volume)
+                    1412 LOAD_CONST              21 (2)
+                    1414 KW_NAMES                22
+                    1416 PRECALL                  2
+                    1420 CALL                     2
+                    1430 LOAD_METHOD             14 (tolist)
+                    1452 PRECALL                  0
+                    1456 CALL                     0
+                    1466 STORE_FAST               2 (volume)
+         
+         181        1468 LOAD_FAST                3 (liquid_class)
+                    1470 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1502)
+         
+         182        1472 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1484 LOAD_CONST              23 ('Missing required parameter: liquid_class')
+                    1486 PRECALL                  1
+                    1490 CALL                     1
+                    1500 RAISE_VARARGS            1
+         
+         183     >> 1502 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1514 LOAD_FAST                3 (liquid_class)
+                    1516 LOAD_GLOBAL              4 (str)
+                    1528 PRECALL                  2
+                    1532 CALL                     2
+                    1542 POP_JUMP_FORWARD_IF_FALSE     4 (to 1552)
+                    1544 LOAD_CONST              24 (';')
+                    1546 LOAD_FAST                3 (liquid_class)
+                    1548 CONTAINS_OP              0
+                    1550 POP_JUMP_FORWARD_IF_FALSE    18 (to 1588)
+         
+         184     >> 1552 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1564 LOAD_CONST              25 ('Invalid liquid_class: ')
+                    1566 LOAD_FAST                3 (liquid_class)
+                    1568 FORMAT_VALUE             0
+                    1570 BUILD_STRING             2
+                    1572 PRECALL                  1
+                    1576 CALL                     1
+                    1586 RAISE_VARARGS            1
+         
+         186     >> 1588 LOAD_FAST                4 (tips)
+                    1590 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1622)
+         
+         187        1592 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1604 LOAD_CONST              26 ('Missing required parameter: tips')
+                    1606 PRECALL                  1
+                    1610 CALL                     1
+                    1620 RAISE_VARARGS            1
+         
+         188     >> 1622 LOAD_FAST                4 (tips)
+                    1624 GET_ITER
+                 >> 1626 FOR_ITER                62 (to 1752)
+                    1628 STORE_FAST               9 (tip)
+         
+         189        1630 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1642 LOAD_FAST                9 (tip)
+                    1644 LOAD_GLOBAL             16 (int)
+                    1656 LOAD_GLOBAL             30 (Tip)
+                    1668 BUILD_TUPLE              2
+                    1670 PRECALL                  2
+                    1674 CALL                     2
+                    1684 POP_JUMP_FORWARD_IF_TRUE    32 (to 1750)
+         
+         190        1686 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1698 LOAD_CONST              27 ('Invalid type of tips: ')
+                    1700 LOAD_GLOBAL             33 (NULL + type)
+                    1712 LOAD_FAST                9 (tip)
+                    1714 PRECALL                  1
+                    1718 CALL                     1
+                    1728 FORMAT_VALUE             0
+                    1730 LOAD_CONST              28 ('. Has to be int or Tip.')
+                    1732 BUILD_STRING             3
+                    1734 PRECALL                  1
+                    1738 CALL                     1
+                    1748 RAISE_VARARGS            1
+         
+         189     >> 1750 JUMP_BACKWARD           63 (to 1626)
+         
+         191     >> 1752 BUILD_LIST               0
+                    1754 STORE_FAST              10 (tecan_tips)
+         
+         192        1756 LOAD_FAST                4 (tips)
+                    1758 GET_ITER
+                 >> 1760 FOR_ITER                80 (to 1922)
+                    1762 STORE_FAST               9 (tip)
+         
+         193        1764 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1776 LOAD_FAST                9 (tip)
+                    1778 LOAD_GLOBAL             16 (int)
+                    1790 PRECALL                  2
+                    1794 CALL                     2
+                    1804 POP_JUMP_FORWARD_IF_FALSE    36 (to 1878)
+                    1806 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1818 LOAD_FAST                9 (tip)
+                    1820 LOAD_GLOBAL             30 (Tip)
+                    1832 PRECALL                  2
+                    1836 CALL                     2
+                    1846 POP_JUMP_FORWARD_IF_TRUE    15 (to 1878)
+         
+         195        1848 LOAD_GLOBAL             35 (NULL + int_to_tip)
+                    1860 LOAD_FAST                9 (tip)
+                    1862 PRECALL                  1
+                    1866 CALL                     1
+                    1876 STORE_FAST               9 (tip)
+         
+         196     >> 1878 LOAD_FAST               10 (tecan_tips)
+                    1880 LOAD_METHOD             18 (append)
+                    1902 LOAD_FAST                9 (tip)
+                    1904 PRECALL                  1
+                    1908 CALL                     1
+                    1918 POP_TOP
+                    1920 JUMP_BACKWARD           81 (to 1760)
+         
+         198     >> 1922 LOAD_FAST                0 (wells)
+                    1924 LOAD_FAST                1 (labware_position)
+                    1926 LOAD_FAST                2 (volume)
+                    1928 LOAD_FAST                3 (liquid_class)
+                    1930 LOAD_FAST               10 (tecan_tips)
+                    1932 BUILD_TUPLE              5
+                    1934 RETURN_VALUE
          ExceptionTable:
-           512 to 540 -> 544 [1]
-           544 to 582 -> 584 [2] lasti
+           604 to 632 -> 636 [1]
+           636 to 674 -> 676 [2] lasti
          consts
-            'Validates and prepares aspirate/dispense parameters.\n\n    Parameters\n    ----------\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)\n    volume : int, float or list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list of int\n        Tip(s) that will be selected (out of tips 1-8)\n    max_volume : int, optional\n        Maximum allowed volume\n\n    Returns\n    -------\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)\n    volume : list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list of int\n        Tip(s) that will be selected (out of tips 1-8)\n    '
+            'Validates and prepares aspirate/dispense parameters.\n\n    Parameters\n    ----------\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).\n        NOTE: The site numbering starts at 1.\n    volume : int, float or list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list of int\n        Tip(s) that will be selected (out of tips 1-8)\n    max_volume : int, optional\n        Maximum allowed volume\n\n    Returns\n    -------\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).\n        NOTE: The returned site number starts at 1.\n    volume : list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list of int\n        Tip(s) that will be selected (out of tips 1-8)\n    '
             None
             'Missing required parameter: wells'
             'Invalid wells: '
             'Invalid wells: wells and tips need to have the same length.'
             'Missing required parameter: position'
-            code
-               argcount  : 1
-               nlocals   : 2
-               stacksize : 5
-               flags     : 51
-               code
-                  0x4b00010097007c005d197d017401000000000000000000007c01740200
-                  000000000000000000a6020000ab0200000000000000005600970101008c
-                  1a64005300
-               142           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-                             6 LOAD_FAST                0 (.0)
-                       >>    8 FOR_ITER                25 (to 60)
-                            10 STORE_FAST               1 (position)
-                            12 LOAD_GLOBAL              1 (NULL + isinstance)
-                            24 LOAD_FAST                1 (position)
-                            26 LOAD_GLOBAL              2 (int)
-                            38 PRECALL                  2
-                            42 CALL                     2
-                            52 YIELD_VALUE
-                            54 RESUME                   1
-                            56 POP_TOP
-                            58 JUMP_BACKWARD           26 (to 8)
-                       >>   60 LOAD_CONST               0 (None)
-                            62 RETURN_VALUE
-               consts
-                  None
-               names      ('isinstance', 'int')
-               varnames   ('.0', 'position')
-               freevars   ()
-               cellvars   ()
-               filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
-               name       '<genexpr>'
-               firstlineno 142
-               lnotab 0x
-            code
-               argcount  : 1
-               nlocals   : 2
-               stacksize : 3
-               flags     : 51
-               code
-                  0x4b00010097007c005d0a7d017c0164006b00000000005600970101008c
-                  0b64015300
-               142           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-                             6 LOAD_FAST                0 (.0)
-                       >>    8 FOR_ITER                10 (to 30)
-               
-               143          10 STORE_FAST               1 (position)
-                            12 LOAD_FAST                1 (position)
-                            14 LOAD_CONST               0 (0)
-                            16 COMPARE_OP               0 (<)
-               
-               142          22 YIELD_VALUE
-                            24 RESUME                   1
-                            26 POP_TOP
-                            28 JUMP_BACKWARD           11 (to 8)
-                       >>   30 LOAD_CONST               1 (None)
-                            32 RETURN_VALUE
-               consts
-                  0
-                  None
-               names      ()
-               varnames   ('.0', 'position')
-               freevars   ()
-               cellvars   ()
-               filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
-               name       '<genexpr>'
-               firstlineno 142
-               lnotab 0x0a010cff
-            'Invalid position: '
+            1
+            67
+            'Grid (first number in labware_position tuple) has to be an int from 1 - 67.'
+            128
+            'Site (second number in labware_position tuple) has to be an int from 1 - 128.'
             'Missing required parameter: volume'
             'Invalid volume: '
             0
             7158278
             'Invalid volume: volume of '
             ' exceeds max_volume.'
             'Invalid volume: Tips, wells, and volume lists have different lengths ('
@@ -1384,26 +1371,26 @@
             ('decimals',)
             'Missing required parameter: liquid_class'
             ';'
             'Invalid liquid_class: '
             'Missing required parameter: tips'
             'Invalid type of tips: '
             '. Has to be int or Tip.'
-         names      ('ValueError', 'isinstance', 'str', 'list', 'tuple', 'np', 'ndarray', 'len', 'all', 'any', 'float', 'isnan', 'InvalidOperationError', 'Exception', 'int', 'round', 'tolist', 'Tip', 'type', 'int_to_tip', 'append')
-         varnames   ('wells', 'labware_position', 'volume', 'liquid_class', 'tips', 'max_volume', 'vol', 'tip', 'tecan_tips')
+         names      ('ValueError', 'isinstance', 'str', 'list', 'tuple', 'np', 'ndarray', 'len', 'int', 'float', 'isnan', 'InvalidOperationError', 'Exception', 'round', 'tolist', 'Tip', 'type', 'int_to_tip', 'append')
+         varnames   ('wells', 'labware_position', 'volume', 'liquid_class', 'tips', 'max_volume', 'grid', 'site', 'vol', 'tip', 'tecan_tips')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
          name       'prepare_evo_aspirate_dispense_parameters'
          firstlineno 95
          lnotab
-            0x022704011e015a01240140011e0104011e01420102ff2003240204011e
-            012a0108010201220102012a0140012401100128016c010c0164ff10ff02
-            043802400124011001260242022403500204011e013201240204011e0108
-            01380140ff02020401080154021e012c02
+            0x022904011e015a01240140011e0104011e010a0148011e0148011e010e
+            0204011e012a0108010201220102012a0140012401100128016c010c0164
+            ff10ff02043802400124011001260242022403500204011e013201240204
+            011e010801380140ff02020401080154021e012c02
       'n_rows'
       'n_columns'
       code
          argcount  : 0
          nlocals   : 14
          stacksize : 13
          flags     : 3
@@ -1417,131 +1404,131 @@
             0064089d037a0d00007d0b7c04a003000000000000000000000000000000
             00000000006403a6010000ab01000000000000000001008c357c0b64097a
             0d00007d0b8c3b7409000000000000000000007c007c017c02a6030000ab
             0300000000000000007d0c740b000000000000000000007c007c017c0ca6
             030000ab0300000000000000007d0d640a7c099b00640b7c059b0064087c
             0b9b00640c7c036403190000000000000000009b00640d7c03640e190000
             000000000000009b00640f7c0d9b0064109d0d5300
-         197           0 RESUME                   0
+         201           0 RESUME                   0
          
-         234           2 LOAD_GLOBAL              1 (NULL + dict)
+         239           2 LOAD_GLOBAL              1 (NULL + dict)
          
-         235          14 LOAD_FAST                2 (wells)
+         240          14 LOAD_FAST                2 (wells)
          
-         236          16 LOAD_FAST                3 (labware_position)
+         241          16 LOAD_FAST                3 (labware_position)
          
-         237          18 LOAD_FAST                4 (volume)
+         242          18 LOAD_FAST                4 (volume)
          
-         238          20 LOAD_FAST                5 (liquid_class)
+         243          20 LOAD_FAST                5 (liquid_class)
          
-         239          22 LOAD_FAST                6 (tips)
+         244          22 LOAD_FAST                6 (tips)
          
-         234          24 KW_NAMES                 1
+         239          24 KW_NAMES                 1
                       26 PRECALL                  5
                       30 CALL                     5
                       40 STORE_FAST               8 (kwargs)
          
-         247          42 LOAD_GLOBAL              3 (NULL + prepare_evo_aspirate_dispense_parameters)
+         252          42 LOAD_GLOBAL              3 (NULL + prepare_evo_aspirate_dispense_parameters)
                       54 LOAD_CONST              17 (())
                       56 BUILD_MAP                0
                       58 LOAD_FAST                8 (kwargs)
                       60 DICT_MERGE               1
                       62 LOAD_CONST               2 ('max_volume')
                       64 LOAD_FAST                7 (max_volume)
                       66 BUILD_MAP                1
                       68 DICT_MERGE               1
                       70 CALL_FUNCTION_EX         1
          
-         241          72 UNPACK_SEQUENCE          5
+         246          72 UNPACK_SEQUENCE          5
          
-         242          76 STORE_FAST               2 (wells)
+         247          76 STORE_FAST               2 (wells)
          
-         243          78 STORE_FAST               3 (labware_position)
+         248          78 STORE_FAST               3 (labware_position)
          
-         244          80 STORE_FAST               4 (volume)
+         249          80 STORE_FAST               4 (volume)
          
-         245          82 STORE_FAST               5 (liquid_class)
+         250          82 STORE_FAST               5 (liquid_class)
          
-         246          84 STORE_FAST               6 (tips)
+         251          84 STORE_FAST               6 (tips)
          
-         250          86 LOAD_CONST               3 (0)
+         255          86 LOAD_CONST               3 (0)
                       88 STORE_FAST               9 (tip_selection)
          
-         251          90 LOAD_FAST                6 (tips)
+         256          90 LOAD_FAST                6 (tips)
                       92 GET_ITER
                  >>   94 FOR_ITER                12 (to 120)
                       96 STORE_FAST              10 (tip)
          
-         252          98 LOAD_FAST                9 (tip_selection)
+         257          98 LOAD_FAST                9 (tip_selection)
                      100 LOAD_FAST               10 (tip)
                      102 LOAD_ATTR                2 (value)
                      112 BINARY_OP               13 (+=)
                      116 STORE_FAST               9 (tip_selection)
                      118 JUMP_BACKWARD           13 (to 94)
          
-         255     >>  120 LOAD_CONST               4 ('')
+         260     >>  120 LOAD_CONST               4 ('')
                      122 STORE_FAST              11 (tip_volumes)
          
-         256         124 LOAD_CONST               5 ((1, 2, 4, 8, 16, 32, 64, 128))
+         261         124 LOAD_CONST               5 ((1, 2, 4, 8, 16, 32, 64, 128))
                      126 GET_ITER
                  >>  128 FOR_ITER                58 (to 246)
                      130 STORE_FAST              10 (tip)
          
-         257         132 LOAD_FAST               10 (tip)
-                     134 LOAD_CONST               6 (<code object <listcomp>, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 257>)
+         262         132 LOAD_FAST               10 (tip)
+                     134 LOAD_CONST               6 (<code object <listcomp>, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 262>)
                      136 MAKE_FUNCTION            0
                      138 LOAD_FAST                6 (tips)
                      140 GET_ITER
                      142 PRECALL                  0
                      146 CALL                     0
                      156 CONTAINS_OP              0
                      158 POP_JUMP_FORWARD_IF_FALSE    37 (to 234)
          
-         258         160 LOAD_FAST               11 (tip_volumes)
+         263         160 LOAD_FAST               11 (tip_volumes)
                      162 LOAD_CONST               7 ('"')
                      164 LOAD_FAST                4 (volume)
                      166 LOAD_CONST               3 (0)
                      168 BINARY_SUBSCR
                      178 FORMAT_VALUE             0
                      180 LOAD_CONST               8 ('",')
                      182 BUILD_STRING             3
                      184 BINARY_OP               13 (+=)
                      188 STORE_FAST              11 (tip_volumes)
          
-         259         190 LOAD_FAST                4 (volume)
+         264         190 LOAD_FAST                4 (volume)
                      192 LOAD_METHOD              3 (pop)
                      214 LOAD_CONST               3 (0)
                      216 PRECALL                  1
                      220 CALL                     1
                      230 POP_TOP
                      232 JUMP_BACKWARD           53 (to 128)
          
-         261     >>  234 LOAD_FAST               11 (tip_volumes)
+         266     >>  234 LOAD_FAST               11 (tip_volumes)
                      236 LOAD_CONST               9 ('0,')
                      238 BINARY_OP               13 (+=)
                      242 STORE_FAST              11 (tip_volumes)
                      244 JUMP_BACKWARD           59 (to 128)
          
-         264     >>  246 LOAD_GLOBAL              9 (NULL + evo_make_selection_array)
+         269     >>  246 LOAD_GLOBAL              9 (NULL + evo_make_selection_array)
                      258 LOAD_FAST                0 (n_rows)
                      260 LOAD_FAST                1 (n_columns)
                      262 LOAD_FAST                2 (wells)
                      264 PRECALL                  3
                      268 CALL                     3
                      278 STORE_FAST              12 (selected)
          
-         266         280 LOAD_GLOBAL             11 (NULL + evo_get_selection)
+         271         280 LOAD_GLOBAL             11 (NULL + evo_get_selection)
                      292 LOAD_FAST                0 (n_rows)
                      294 LOAD_FAST                1 (n_columns)
                      296 LOAD_FAST               12 (selected)
                      298 PRECALL                  3
                      302 CALL                     3
                      312 STORE_FAST              13 (code_string)
          
-         267         314 LOAD_CONST              10 ('B;Aspirate(')
+         272         314 LOAD_CONST              10 ('B;Aspirate(')
                      316 LOAD_FAST                9 (tip_selection)
                      318 FORMAT_VALUE             0
                      320 LOAD_CONST              11 (',"')
                      322 LOAD_FAST                5 (liquid_class)
                      324 FORMAT_VALUE             0
                      326 LOAD_CONST               8 ('",')
                      328 LOAD_FAST               11 (tip_volumes)
@@ -1559,27 +1546,27 @@
                      368 LOAD_CONST              15 (',1,"')
                      370 LOAD_FAST               13 (code_string)
                      372 FORMAT_VALUE             0
                      374 LOAD_CONST              16 ('",0,0);')
                      376 BUILD_STRING            13
                      378 RETURN_VALUE
          consts
-            'Command for aspirating with the EvoWARE aspirate command WITHOUT digital volume tracking.\n\n    As many wells in one column may be selected as your liquid handling arm has pipettes.\n    This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string\n    specifying the target wells.\n\n    Parameters\n    ----------\n    n_rows\n        Number of rows in the labware.\n    n_columns\n        Number of columns in the labware.\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)\n    volume : int, float or list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    max_volume\n        Maximum allowed dilutor volume.\n    '
+            'Command for aspirating with the EvoWARE aspirate command WITHOUT digital volume tracking.\n\n    As many wells in one column may be selected as your liquid handling arm has pipettes.\n    This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string\n    specifying the target wells.\n\n    Parameters\n    ----------\n    n_rows\n        Number of rows in the labware.\n    n_columns\n        Number of columns in the labware.\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).\n        NOTE: The site numbering starts at 1.\n    volume : int, float or list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    max_volume\n        Maximum allowed dilutor volume.\n    '
             ('wells', 'labware_position', 'volume', 'liquid_class', 'tips')
             'max_volume'
             0
             ''
             (1, 2, 4, 8, 16, 32, 64, 128)
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-               257           0 RESUME                   0
+               262           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                 9 (to 26)
                              8 STORE_FAST               1 (tecantip)
                             10 LOAD_FAST                1 (tecantip)
                             12 LOAD_ATTR                0 (value)
                             22 LIST_APPEND              2
@@ -1588,15 +1575,15 @@
                consts
                names      ('value',)
                varnames   ('.0', 'tecantip')
                freevars   ()
                cellvars   ()
                filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
                name       '<listcomp>'
-               firstlineno 257
+               firstlineno 262
                lnotab 0x
             '"'
             '",'
             '0,'
             'B;Aspirate('
             ',"'
             '0,0,0,0,'
@@ -1607,17 +1594,17 @@
             ()
          names      ('dict', 'prepare_evo_aspirate_dispense_parameters', 'value', 'pop', 'evo_make_selection_array', 'evo_get_selection')
          varnames   ('n_rows', 'n_columns', 'wells', 'labware_position', 'volume', 'liquid_class', 'tips', 'max_volume', 'kwargs', 'tip_selection', 'tip', 'tip_volumes', 'selected', 'code_string')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
          name       'evo_aspirate'
-         firstlineno 197
+         firstlineno 201
          lnotab
-            0x02250c01020102010201020102fb120d1efa0401020102010201020102
+            0x02260c01020102010201020102fb120d1efa0401020102010201020102
             04040108011603040108011c011e012c020c0322022201
       code
          argcount  : 0
          nlocals   : 14
          stacksize : 13
          flags     : 3
          code
@@ -1630,131 +1617,131 @@
             0064089d037a0d00007d0b7c04a003000000000000000000000000000000
             00000000006403a6010000ab01000000000000000001008c357c0b64097a
             0d00007d0b8c3b7409000000000000000000007c007c017c02a6030000ab
             0300000000000000007d0c740b000000000000000000007c007c017c0ca6
             030000ab0300000000000000007d0d640a7c099b00640b7c059b0064087c
             0b9b00640c7c036403190000000000000000009b00640d7c03640e190000
             000000000000009b00640f7c0d9b0064109d0d5300
-         270           0 RESUME                   0
+         275           0 RESUME                   0
          
-         307           2 LOAD_GLOBAL              1 (NULL + dict)
+         313           2 LOAD_GLOBAL              1 (NULL + dict)
          
-         308          14 LOAD_FAST                2 (wells)
+         314          14 LOAD_FAST                2 (wells)
          
-         309          16 LOAD_FAST                3 (labware_position)
+         315          16 LOAD_FAST                3 (labware_position)
          
-         310          18 LOAD_FAST                4 (volume)
+         316          18 LOAD_FAST                4 (volume)
          
-         311          20 LOAD_FAST                5 (liquid_class)
+         317          20 LOAD_FAST                5 (liquid_class)
          
-         312          22 LOAD_FAST                6 (tips)
+         318          22 LOAD_FAST                6 (tips)
          
-         307          24 KW_NAMES                 1
+         313          24 KW_NAMES                 1
                       26 PRECALL                  5
                       30 CALL                     5
                       40 STORE_FAST               8 (kwargs)
          
-         320          42 LOAD_GLOBAL              3 (NULL + prepare_evo_aspirate_dispense_parameters)
+         326          42 LOAD_GLOBAL              3 (NULL + prepare_evo_aspirate_dispense_parameters)
                       54 LOAD_CONST              17 (())
                       56 BUILD_MAP                0
                       58 LOAD_FAST                8 (kwargs)
                       60 DICT_MERGE               1
                       62 LOAD_CONST               2 ('max_volume')
                       64 LOAD_FAST                7 (max_volume)
                       66 BUILD_MAP                1
                       68 DICT_MERGE               1
                       70 CALL_FUNCTION_EX         1
          
-         314          72 UNPACK_SEQUENCE          5
+         320          72 UNPACK_SEQUENCE          5
          
-         315          76 STORE_FAST               2 (wells)
+         321          76 STORE_FAST               2 (wells)
          
-         316          78 STORE_FAST               3 (labware_position)
+         322          78 STORE_FAST               3 (labware_position)
          
-         317          80 STORE_FAST               4 (volume)
+         323          80 STORE_FAST               4 (volume)
          
-         318          82 STORE_FAST               5 (liquid_class)
+         324          82 STORE_FAST               5 (liquid_class)
          
-         319          84 STORE_FAST               6 (tips)
+         325          84 STORE_FAST               6 (tips)
          
-         323          86 LOAD_CONST               3 (0)
+         329          86 LOAD_CONST               3 (0)
                       88 STORE_FAST               9 (tip_selection)
          
-         324          90 LOAD_FAST                6 (tips)
+         330          90 LOAD_FAST                6 (tips)
                       92 GET_ITER
                  >>   94 FOR_ITER                12 (to 120)
                       96 STORE_FAST              10 (tip)
          
-         325          98 LOAD_FAST                9 (tip_selection)
+         331          98 LOAD_FAST                9 (tip_selection)
                      100 LOAD_FAST               10 (tip)
                      102 LOAD_ATTR                2 (value)
                      112 BINARY_OP               13 (+=)
                      116 STORE_FAST               9 (tip_selection)
                      118 JUMP_BACKWARD           13 (to 94)
          
-         328     >>  120 LOAD_CONST               4 ('')
+         334     >>  120 LOAD_CONST               4 ('')
                      122 STORE_FAST              11 (tip_volumes)
          
-         329         124 LOAD_CONST               5 ((1, 2, 4, 8, 16, 32, 64, 128))
+         335         124 LOAD_CONST               5 ((1, 2, 4, 8, 16, 32, 64, 128))
                      126 GET_ITER
                  >>  128 FOR_ITER                58 (to 246)
                      130 STORE_FAST              10 (tip)
          
-         330         132 LOAD_FAST               10 (tip)
-                     134 LOAD_CONST               6 (<code object <listcomp>, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 330>)
+         336         132 LOAD_FAST               10 (tip)
+                     134 LOAD_CONST               6 (<code object <listcomp>, file "/home/runner/work/robotools/robotools/robotools/evotools/commands.py", line 336>)
                      136 MAKE_FUNCTION            0
                      138 LOAD_FAST                6 (tips)
                      140 GET_ITER
                      142 PRECALL                  0
                      146 CALL                     0
                      156 CONTAINS_OP              0
                      158 POP_JUMP_FORWARD_IF_FALSE    37 (to 234)
          
-         331         160 LOAD_FAST               11 (tip_volumes)
+         337         160 LOAD_FAST               11 (tip_volumes)
                      162 LOAD_CONST               7 ('"')
                      164 LOAD_FAST                4 (volume)
                      166 LOAD_CONST               3 (0)
                      168 BINARY_SUBSCR
                      178 FORMAT_VALUE             0
                      180 LOAD_CONST               8 ('",')
                      182 BUILD_STRING             3
                      184 BINARY_OP               13 (+=)
                      188 STORE_FAST              11 (tip_volumes)
          
-         332         190 LOAD_FAST                4 (volume)
+         338         190 LOAD_FAST                4 (volume)
                      192 LOAD_METHOD              3 (pop)
                      214 LOAD_CONST               3 (0)
                      216 PRECALL                  1
                      220 CALL                     1
                      230 POP_TOP
                      232 JUMP_BACKWARD           53 (to 128)
          
-         334     >>  234 LOAD_FAST               11 (tip_volumes)
+         340     >>  234 LOAD_FAST               11 (tip_volumes)
                      236 LOAD_CONST               9 ('0,')
                      238 BINARY_OP               13 (+=)
                      242 STORE_FAST              11 (tip_volumes)
                      244 JUMP_BACKWARD           59 (to 128)
          
-         337     >>  246 LOAD_GLOBAL              9 (NULL + evo_make_selection_array)
+         343     >>  246 LOAD_GLOBAL              9 (NULL + evo_make_selection_array)
                      258 LOAD_FAST                0 (n_rows)
                      260 LOAD_FAST                1 (n_columns)
                      262 LOAD_FAST                2 (wells)
                      264 PRECALL                  3
                      268 CALL                     3
                      278 STORE_FAST              12 (selected)
          
-         339         280 LOAD_GLOBAL             11 (NULL + evo_get_selection)
+         345         280 LOAD_GLOBAL             11 (NULL + evo_get_selection)
                      292 LOAD_FAST                0 (n_rows)
                      294 LOAD_FAST                1 (n_columns)
                      296 LOAD_FAST               12 (selected)
                      298 PRECALL                  3
                      302 CALL                     3
                      312 STORE_FAST              13 (code_string)
          
-         340         314 LOAD_CONST              10 ('B;Dispense(')
+         346         314 LOAD_CONST              10 ('B;Dispense(')
                      316 LOAD_FAST                9 (tip_selection)
                      318 FORMAT_VALUE             0
                      320 LOAD_CONST              11 (',"')
                      322 LOAD_FAST                5 (liquid_class)
                      324 FORMAT_VALUE             0
                      326 LOAD_CONST               8 ('",')
                      328 LOAD_FAST               11 (tip_volumes)
@@ -1772,27 +1759,27 @@
                      368 LOAD_CONST              15 (',1,"')
                      370 LOAD_FAST               13 (code_string)
                      372 FORMAT_VALUE             0
                      374 LOAD_CONST              16 ('",0,0);')
                      376 BUILD_STRING            13
                      378 RETURN_VALUE
          consts
-            'Command for dispensing using the EvoWARE dispense command WITHOUT digital volume tracking.\n\n    As many wells in one column may be selected as your liquid handling arm has pipettes.\n    This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string\n    specifying the target wells.\n\n    Parameters\n    ----------\n    n_rows\n        Number of rows in the labware.\n    n_columns\n        Number of columns in the labware.\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)\n    volume : int, float or list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    max_volume\n        Maximum allowed dilutor volume.\n    '
+            'Command for dispensing using the EvoWARE dispense command WITHOUT digital volume tracking.\n\n    As many wells in one column may be selected as your liquid handling arm has pipettes.\n    This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string\n    specifying the target wells.\n\n    Parameters\n    ----------\n    n_rows\n        Number of rows in the labware.\n    n_columns\n        Number of columns in the labware.\n    wells : list of str\n        List with target well ID(s)\n    labware_position : tuple\n        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).\n        NOTE: The site numbering starts at 1.\n    volume : int, float or list\n        Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases\n    liquid_class : str, optional\n        Overwrites the liquid class for this step (max 32 characters)\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    max_volume\n        Maximum allowed dilutor volume.\n    '
             ('wells', 'labware_position', 'volume', 'liquid_class', 'tips')
             'max_volume'
             0
             ''
             (1, 2, 4, 8, 16, 32, 64, 128)
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-               330           0 RESUME                   0
+               336           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                 9 (to 26)
                              8 STORE_FAST               1 (tecantip)
                             10 LOAD_FAST                1 (tecantip)
                             12 LOAD_ATTR                0 (value)
                             22 LIST_APPEND              2
@@ -1801,15 +1788,15 @@
                consts
                names      ('value',)
                varnames   ('.0', 'tecantip')
                freevars   ()
                cellvars   ()
                filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
                name       '<listcomp>'
-               firstlineno 330
+               firstlineno 336
                lnotab 0x
             '"'
             '",'
             '0,'
             'B;Dispense('
             ',"'
             '0,0,0,0,'
@@ -1820,17 +1807,17 @@
             ()
          names      ('dict', 'prepare_evo_aspirate_dispense_parameters', 'value', 'pop', 'evo_make_selection_array', 'evo_get_selection')
          varnames   ('n_rows', 'n_columns', 'wells', 'labware_position', 'volume', 'liquid_class', 'tips', 'max_volume', 'kwargs', 'tip_selection', 'tip', 'tip_volumes', 'selected', 'code_string')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
          name       'evo_dispense'
-         firstlineno 270
+         firstlineno 275
          lnotab
-            0x02250c01020102010201020102fb120d1efa0401020102010201020102
+            0x02260c01020102010201020102fb120d1efa0401020102010201020102
             04040108011603040108011c011e012c020c0322022201
       3.0
       500
       4.0
       10
       70
       30
@@ -1863,137 +1850,138 @@
             000000000000007c0ea6010000ab01000000000000000001008c517c0180
             0f7401000000000000000000006403a6010000ab01000000000000000082
             017c015c0200007d0f7d107403000000000000000000007c0f7404000000
             00000000000000a6020000ab020000000000000000720f64047c0f630278
             026b0100000000720664056b010000000073116e01010074010000000000
             00000000006406a6010000ab010000000000000000820174030000000000
             00000000007c10740400000000000000000000a6020000ab020000000000
-            000000720f64077c10630278026b0100000000720664086b010000000073
-            116e0101007401000000000000000000006409a6010000ab010000000000
-            00000082017c02800f740100000000000000000000640aa6010000ab0100
-            0000000000000082017c025c0200007d0f7d107403000000000000000000
-            007c0f740400000000000000000000a6020000ab02000000000000000072
-            0f64047c0f630278026b0100000000720664056b010000000073116e0101
-            00740100000000000000000000640ba6010000ab01000000000000000082
-            017403000000000000000000007c10740400000000000000000000a60200
-            00ab020000000000000000720f64077c10630278026b0100000000720664
-            086b010000000073116e010100740100000000000000000000640ca60100
-            00ab01000000000000000082017c03800f74010000000000000000000064
-            0da6010000ab01000000000000000082017403000000000000000000007c
-            03740400000000000000000000a6020000ab020000000000000000730f74
-            0100000000000000000000640ea6010000ab01000000000000000082017c
-            0364076b020000000073157c0364046b0200000000730f74010000000000
-            0000000000640fa6010000ab01000000000000000082017c04800f740100
-            0000000000000000006410a6010000ab0100000000000000008201740300
-            0000000000000000007c04740c00000000000000000000a6020000ab0200
-            00000000000000720f64077c04630278026b0100000000720664116b0100
-            00000073116e0101007401000000000000000000006412a6010000ab0100
-            000000000000008201740f000000000000000000006a0800000000000000
-            007c046404a6020000ab0200000000000000007d047c05800f7401000000
-            000000000000006413a6010000ab01000000000000000082017403000000
-            000000000000007c05740400000000000000000000a6020000ab02000000
-            0000000000720f64077c05630278026b0100000000720664146b01000000
-            0073116e0101007401000000000000000000006415a6010000ab01000000
-            000000000082017c06800f7401000000000000000000006416a6010000ab
-            01000000000000000082017403000000000000000000007c06740c000000
-            00000000000000a6020000ab020000000000000000720f64077c06630278
-            026b0100000000720664116b010000000073116e01010074010000000000
-            00000000006417a6010000ab0100000000000000008201740f0000000000
-            00000000006a0800000000000000007c066404a6020000ab020000000000
-            0000007d067c07800f7401000000000000000000006418a6010000ab0100
-            0000000000000082017403000000000000000000007c0774040000000000
-            0000000000a6020000ab020000000000000000720f64077c07630278026b
+            000000720f64047c10630278026b0100000000720664076b010000000073
+            116e0101007401000000000000000000006408a6010000ab010000000000
+            00000082017c0f7c1064047a0a000066027d017c02800f74010000000000
+            00000000006409a6010000ab01000000000000000082017c025c0200007d
+            0f7d107403000000000000000000007c0f740400000000000000000000a6
+            020000ab020000000000000000720f64047c0f630278026b010000000072
+            0664056b010000000073116e010100740100000000000000000000640aa6
+            010000ab01000000000000000082017403000000000000000000007c1074
+            0400000000000000000000a6020000ab020000000000000000720f64047c
+            10630278026b0100000000720664076b010000000073116e010100740100
+            000000000000000000640ba6010000ab01000000000000000082017c0f7c
+            1064047a0a000066027d027c03800f740100000000000000000000640ca6
+            010000ab01000000000000000082017403000000000000000000007c0374
+            0400000000000000000000a6020000ab020000000000000000730f740100
+            000000000000000000640da6010000ab01000000000000000082017c0364
+            0e6b020000000073157c0364046b0200000000730f740100000000000000
+            000000640fa6010000ab01000000000000000082017c04800f7401000000
+            000000000000006410a6010000ab01000000000000000082017403000000
+            000000000000007c04740c00000000000000000000a6020000ab02000000
+            0000000000720f640e7c04630278026b0100000000720664116b01000000
+            0073116e0101007401000000000000000000006412a6010000ab01000000
+            00000000008201740f000000000000000000006a0800000000000000007c
+            046404a6020000ab0200000000000000007d047c05800f74010000000000
+            00000000006413a6010000ab010000000000000000820174030000000000
+            00000000007c05740400000000000000000000a6020000ab020000000000
+            000000720f640e7c05630278026b0100000000720664146b010000000073
+            116e0101007401000000000000000000006415a6010000ab010000000000
+            00000082017c06800f7401000000000000000000006416a6010000ab0100
+            0000000000000082017403000000000000000000007c06740c0000000000
+            0000000000a6020000ab020000000000000000720f640e7c06630278026b
+            0100000000720664116b010000000073116e010100740100000000000000
+            0000006417a6010000ab0100000000000000008201740f00000000000000
+            0000006a0800000000000000007c066404a6020000ab0200000000000000
+            007d067c07800f7401000000000000000000006418a6010000ab01000000
+            000000000082017403000000000000000000007c07740400000000000000
+            000000a6020000ab020000000000000000720f640e7c07630278026b0100
+            000000720664146b010000000073116e0101007401000000000000000000
+            006419a6010000ab01000000000000000082017c08800f74010000000000
+            0000000000641aa6010000ab010000000000000000820174030000000000
+            00000000007c08740400000000000000000000a6020000ab020000000000
+            000000720f640e7c08630278026b0100000000720664116b010000000073
+            116e010100740100000000000000000000641ba6010000ab010000000000
+            00000082017c09800f740100000000000000000000641ca6010000ab0100
+            0000000000000082017403000000000000000000007c0974040000000000
+            0000000000a6020000ab020000000000000000720f64047c09630278026b
             0100000000720664146b010000000073116e010100740100000000000000
-            0000006419a6010000ab01000000000000000082017c08800f7401000000
-            00000000000000641aa6010000ab01000000000000000082017403000000
-            000000000000007c08740400000000000000000000a6020000ab02000000
-            0000000000720f64077c08630278026b0100000000720664116b01000000
-            0073116e010100740100000000000000000000641ba6010000ab01000000
-            000000000082017c09800f740100000000000000000000641ca6010000ab
-            01000000000000000082017403000000000000000000007c097404000000
-            00000000000000a6020000ab020000000000000000720f64047c09630278
-            026b0100000000720664146b010000000073116e01010074010000000000
-            0000000000641da6010000ab01000000000000000082017c0a800f740100
-            000000000000000000641ea6010000ab0100000000000000008201740300
-            0000000000000000007c0a740400000000000000000000a6020000ab0200
-            00000000000000720f64047c0a630278026b0100000000720664116b0100
-            00000073116e010100740100000000000000000000641fa6010000ab0100
-            0000000000000082017c0b800f7401000000000000000000006420a60100
-            00ab01000000000000000082017403000000000000000000007c0b740400
-            000000000000000000a6020000ab020000000000000000730f7401000000
-            000000000000006421a6010000ab01000000000000000082017c0b64076b
-            020000000073157c0b64046b0200000000730f7401000000000000000000
-            006422a6010000ab01000000000000000082017c0c800f74010000000000
-            00000000006423a6010000ab010000000000000000820174030000000000
-            00000000007c0c740400000000000000000000a6020000ab020000000000
-            000000730f7401000000000000000000006424a6010000ab010000000000
-            00000082017c0c64076b020000000073157c0c64046b0200000000730f74
-            01000000000000000000006425a6010000ab01000000000000000082017c
-            0d7c017c027c037c047c057c067c077c087c097c0a7c0b7c0c660d5300
-         343           0 RESUME                   0
+            000000641da6010000ab01000000000000000082017c0a800f7401000000
+            00000000000000641ea6010000ab01000000000000000082017403000000
+            000000000000007c0a740400000000000000000000a6020000ab02000000
+            0000000000720f64047c0a630278026b0100000000720664116b01000000
+            0073116e010100740100000000000000000000641fa6010000ab01000000
+            000000000082017c0b800f7401000000000000000000006420a6010000ab
+            01000000000000000082017403000000000000000000007c0b7404000000
+            00000000000000a6020000ab020000000000000000730f74010000000000
+            00000000006421a6010000ab01000000000000000082017c0b640e6b0200
+            00000073157c0b64046b0200000000730f74010000000000000000000064
+            22a6010000ab01000000000000000082017c0c800f740100000000000000
+            0000006423a6010000ab0100000000000000008201740300000000000000
+            0000007c0c740400000000000000000000a6020000ab0200000000000000
+            00730f7401000000000000000000006424a6010000ab0100000000000000
+            0082017c0c640e6b020000000073157c0c64046b0200000000730f740100
+            0000000000000000006425a6010000ab01000000000000000082017c0d7c
+            017c027c037c047c057c067c077c087c097c0a7c0b7c0c660d5300
+         349           0 RESUME                   0
          
-         419           2 LOAD_FAST                0 (tips)
+         425           2 LOAD_FAST                0 (tips)
                        4 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 36)
          
-         420           6 LOAD_GLOBAL              1 (NULL + ValueError)
+         426           6 LOAD_GLOBAL              1 (NULL + ValueError)
                       18 LOAD_CONST               2 ('Missing required parameter: tips')
                       20 PRECALL                  1
                       24 CALL                     1
                       34 RAISE_VARARGS            1
          
-         422     >>   36 BUILD_LIST               0
+         428     >>   36 BUILD_LIST               0
                       38 STORE_FAST              13 (tecan_tips)
          
-         423          40 LOAD_FAST                0 (tips)
+         429          40 LOAD_FAST                0 (tips)
                       42 GET_ITER
                  >>   44 FOR_ITER                80 (to 206)
                       46 STORE_FAST              14 (tip)
          
-         424          48 LOAD_GLOBAL              3 (NULL + isinstance)
+         430          48 LOAD_GLOBAL              3 (NULL + isinstance)
                       60 LOAD_FAST               14 (tip)
                       62 LOAD_GLOBAL              4 (int)
                       74 PRECALL                  2
                       78 CALL                     2
                       88 POP_JUMP_FORWARD_IF_FALSE    36 (to 162)
                       90 LOAD_GLOBAL              3 (NULL + isinstance)
                      102 LOAD_FAST               14 (tip)
                      104 LOAD_GLOBAL              6 (Tip)
                      116 PRECALL                  2
                      120 CALL                     2
                      130 POP_JUMP_FORWARD_IF_TRUE    15 (to 162)
          
-         426         132 LOAD_GLOBAL              9 (NULL + int_to_tip)
+         432         132 LOAD_GLOBAL              9 (NULL + int_to_tip)
                      144 LOAD_FAST               14 (tip)
                      146 PRECALL                  1
                      150 CALL                     1
                      160 STORE_FAST              14 (tip)
          
-         427     >>  162 LOAD_FAST               13 (tecan_tips)
+         433     >>  162 LOAD_FAST               13 (tecan_tips)
                      164 LOAD_METHOD              5 (append)
                      186 LOAD_FAST               14 (tip)
                      188 PRECALL                  1
                      192 CALL                     1
                      202 POP_TOP
                      204 JUMP_BACKWARD           81 (to 44)
          
-         429     >>  206 LOAD_FAST                1 (waste_location)
+         435     >>  206 LOAD_FAST                1 (waste_location)
                      208 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 240)
          
-         430         210 LOAD_GLOBAL              1 (NULL + ValueError)
+         436         210 LOAD_GLOBAL              1 (NULL + ValueError)
                      222 LOAD_CONST               3 ('Missing required parameter: waste_location')
                      224 PRECALL                  1
                      228 CALL                     1
                      238 RAISE_VARARGS            1
          
-         431     >>  240 LOAD_FAST                1 (waste_location)
+         437     >>  240 LOAD_FAST                1 (waste_location)
                      242 UNPACK_SEQUENCE          2
                      246 STORE_FAST              15 (grid)
                      248 STORE_FAST              16 (site)
          
-         432         250 LOAD_GLOBAL              3 (NULL + isinstance)
+         438         250 LOAD_GLOBAL              3 (NULL + isinstance)
                      262 LOAD_FAST               15 (grid)
                      264 LOAD_GLOBAL              4 (int)
                      276 PRECALL                  2
                      280 CALL                     2
                      290 POP_JUMP_FORWARD_IF_FALSE    15 (to 322)
                      292 LOAD_CONST               4 (1)
                      294 LOAD_FAST               15 (grid)
@@ -2003,508 +1991,522 @@
                      306 POP_JUMP_FORWARD_IF_FALSE     6 (to 320)
                      308 LOAD_CONST               5 (67)
                      310 COMPARE_OP               1 (<=)
                      316 POP_JUMP_FORWARD_IF_TRUE    17 (to 352)
                      318 JUMP_FORWARD             1 (to 322)
                  >>  320 POP_TOP
          
-         433     >>  322 LOAD_GLOBAL              1 (NULL + ValueError)
+         439     >>  322 LOAD_GLOBAL              1 (NULL + ValueError)
                      334 LOAD_CONST               6 ('Grid (first number in waste_location tuple) has to be an int from 1 - 67.')
                      336 PRECALL                  1
                      340 CALL                     1
                      350 RAISE_VARARGS            1
          
-         434     >>  352 LOAD_GLOBAL              3 (NULL + isinstance)
+         440     >>  352 LOAD_GLOBAL              3 (NULL + isinstance)
                      364 LOAD_FAST               16 (site)
                      366 LOAD_GLOBAL              4 (int)
                      378 PRECALL                  2
                      382 CALL                     2
                      392 POP_JUMP_FORWARD_IF_FALSE    15 (to 424)
-                     394 LOAD_CONST               7 (0)
+                     394 LOAD_CONST               4 (1)
                      396 LOAD_FAST               16 (site)
                      398 SWAP                     2
                      400 COPY                     2
                      402 COMPARE_OP               1 (<=)
                      408 POP_JUMP_FORWARD_IF_FALSE     6 (to 422)
-                     410 LOAD_CONST               8 (127)
+                     410 LOAD_CONST               7 (128)
                      412 COMPARE_OP               1 (<=)
                      418 POP_JUMP_FORWARD_IF_TRUE    17 (to 454)
                      420 JUMP_FORWARD             1 (to 424)
                  >>  422 POP_TOP
          
-         435     >>  424 LOAD_GLOBAL              1 (NULL + ValueError)
-                     436 LOAD_CONST               9 ('Site (second number in waste_location tuple) has to be an int from 0 - 127.')
+         441     >>  424 LOAD_GLOBAL              1 (NULL + ValueError)
+                     436 LOAD_CONST               8 ('Site (second number in waste_location tuple) has to be an int from 1 - 128.')
                      438 PRECALL                  1
                      442 CALL                     1
                      452 RAISE_VARARGS            1
          
-         437     >>  454 LOAD_FAST                2 (cleaner_location)
-                     456 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 488)
-         
-         438         458 LOAD_GLOBAL              1 (NULL + ValueError)
-                     470 LOAD_CONST              10 ('Missing required parameter: cleaner_location')
-                     472 PRECALL                  1
-                     476 CALL                     1
-                     486 RAISE_VARARGS            1
-         
-         439     >>  488 LOAD_FAST                2 (cleaner_location)
-                     490 UNPACK_SEQUENCE          2
-                     494 STORE_FAST              15 (grid)
-                     496 STORE_FAST              16 (site)
-         
-         440         498 LOAD_GLOBAL              3 (NULL + isinstance)
-                     510 LOAD_FAST               15 (grid)
-                     512 LOAD_GLOBAL              4 (int)
-                     524 PRECALL                  2
-                     528 CALL                     2
-                     538 POP_JUMP_FORWARD_IF_FALSE    15 (to 570)
-                     540 LOAD_CONST               4 (1)
-                     542 LOAD_FAST               15 (grid)
-                     544 SWAP                     2
-                     546 COPY                     2
-                     548 COMPARE_OP               1 (<=)
-                     554 POP_JUMP_FORWARD_IF_FALSE     6 (to 568)
-                     556 LOAD_CONST               5 (67)
-                     558 COMPARE_OP               1 (<=)
-                     564 POP_JUMP_FORWARD_IF_TRUE    17 (to 600)
-                     566 JUMP_FORWARD             1 (to 570)
-                 >>  568 POP_TOP
-         
-         441     >>  570 LOAD_GLOBAL              1 (NULL + ValueError)
-                     582 LOAD_CONST              11 ('Grid (first number in cleaner_location tuple) has to be an int from 1 - 67.')
-                     584 PRECALL                  1
-                     588 CALL                     1
-                     598 RAISE_VARARGS            1
-         
-         442     >>  600 LOAD_GLOBAL              3 (NULL + isinstance)
-                     612 LOAD_FAST               16 (site)
-                     614 LOAD_GLOBAL              4 (int)
-                     626 PRECALL                  2
-                     630 CALL                     2
-                     640 POP_JUMP_FORWARD_IF_FALSE    15 (to 672)
-                     642 LOAD_CONST               7 (0)
-                     644 LOAD_FAST               16 (site)
-                     646 SWAP                     2
-                     648 COPY                     2
-                     650 COMPARE_OP               1 (<=)
-                     656 POP_JUMP_FORWARD_IF_FALSE     6 (to 670)
-                     658 LOAD_CONST               8 (127)
-                     660 COMPARE_OP               1 (<=)
-                     666 POP_JUMP_FORWARD_IF_TRUE    17 (to 702)
-                     668 JUMP_FORWARD             1 (to 672)
-                 >>  670 POP_TOP
-         
-         443     >>  672 LOAD_GLOBAL              1 (NULL + ValueError)
-                     684 LOAD_CONST              12 ('Site (second number in cleaner_location tuple) has to be an int from 0 - 127.')
-                     686 PRECALL                  1
-                     690 CALL                     1
-                     700 RAISE_VARARGS            1
-         
-         445     >>  702 LOAD_FAST                3 (arm)
-                     704 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 736)
-         
-         446         706 LOAD_GLOBAL              1 (NULL + ValueError)
-                     718 LOAD_CONST              13 ('Missing required paramter: arm')
-                     720 PRECALL                  1
-                     724 CALL                     1
-                     734 RAISE_VARARGS            1
-         
-         447     >>  736 LOAD_GLOBAL              3 (NULL + isinstance)
-                     748 LOAD_FAST                3 (arm)
-                     750 LOAD_GLOBAL              4 (int)
-                     762 PRECALL                  2
-                     766 CALL                     2
-                     776 POP_JUMP_FORWARD_IF_TRUE    15 (to 808)
-         
-         448         778 LOAD_GLOBAL              1 (NULL + ValueError)
-                     790 LOAD_CONST              14 ('Parameter arm is not int.')
-                     792 PRECALL                  1
-                     796 CALL                     1
-                     806 RAISE_VARARGS            1
-         
-         449     >>  808 LOAD_FAST                3 (arm)
-                     810 LOAD_CONST               7 (0)
-                     812 COMPARE_OP               2 (==)
-                     818 POP_JUMP_FORWARD_IF_TRUE    21 (to 862)
-                     820 LOAD_FAST                3 (arm)
-                     822 LOAD_CONST               4 (1)
-                     824 COMPARE_OP               2 (==)
-                     830 POP_JUMP_FORWARD_IF_TRUE    15 (to 862)
-         
-         450         832 LOAD_GLOBAL              1 (NULL + ValueError)
-                     844 LOAD_CONST              15 ('Parameter arm has to be 0 (LiHa 1) or 1 (LiHa 2).')
-                     846 PRECALL                  1
-                     850 CALL                     1
-                     860 RAISE_VARARGS            1
-         
-         452     >>  862 LOAD_FAST                4 (waste_vol)
-                     864 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 896)
-         
-         453         866 LOAD_GLOBAL              1 (NULL + ValueError)
-                     878 LOAD_CONST              16 ('Missing required parameter: waste_vol')
-                     880 PRECALL                  1
-                     884 CALL                     1
-                     894 RAISE_VARARGS            1
-         
-         454     >>  896 LOAD_GLOBAL              3 (NULL + isinstance)
-                     908 LOAD_FAST                4 (waste_vol)
-                     910 LOAD_GLOBAL             12 (float)
-                     922 PRECALL                  2
-                     926 CALL                     2
-                     936 POP_JUMP_FORWARD_IF_FALSE    15 (to 968)
-                     938 LOAD_CONST               7 (0)
-                     940 LOAD_FAST                4 (waste_vol)
-                     942 SWAP                     2
-                     944 COPY                     2
-                     946 COMPARE_OP               1 (<=)
-                     952 POP_JUMP_FORWARD_IF_FALSE     6 (to 966)
-                     954 LOAD_CONST              17 (100)
-                     956 COMPARE_OP               1 (<=)
-                     962 POP_JUMP_FORWARD_IF_TRUE    17 (to 998)
-                     964 JUMP_FORWARD             1 (to 968)
-                 >>  966 POP_TOP
-         
-         455     >>  968 LOAD_GLOBAL              1 (NULL + ValueError)
-                     980 LOAD_CONST              18 ('waste_vol has to be a float from 0 - 100.')
-                     982 PRECALL                  1
-                     986 CALL                     1
-                     996 RAISE_VARARGS            1
-         
-         457     >>  998 LOAD_GLOBAL             15 (NULL + np)
-                    1010 LOAD_ATTR                8 (round)
-                    1020 LOAD_FAST                4 (waste_vol)
-                    1022 LOAD_CONST               4 (1)
-                    1024 PRECALL                  2
-                    1028 CALL                     2
-                    1038 STORE_FAST               4 (waste_vol)
-         
-         459        1040 LOAD_FAST                5 (waste_delay)
-                    1042 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1074)
-         
-         460        1044 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1056 LOAD_CONST              19 ('Missing required parameter: waste_delay')
-                    1058 PRECALL                  1
-                    1062 CALL                     1
-                    1072 RAISE_VARARGS            1
-         
-         461     >> 1074 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1086 LOAD_FAST                5 (waste_delay)
-                    1088 LOAD_GLOBAL              4 (int)
-                    1100 PRECALL                  2
-                    1104 CALL                     2
-                    1114 POP_JUMP_FORWARD_IF_FALSE    15 (to 1146)
-                    1116 LOAD_CONST               7 (0)
-                    1118 LOAD_FAST                5 (waste_delay)
-                    1120 SWAP                     2
-                    1122 COPY                     2
-                    1124 COMPARE_OP               1 (<=)
-                    1130 POP_JUMP_FORWARD_IF_FALSE     6 (to 1144)
-                    1132 LOAD_CONST              20 (1000)
-                    1134 COMPARE_OP               1 (<=)
-                    1140 POP_JUMP_FORWARD_IF_TRUE    17 (to 1176)
-                    1142 JUMP_FORWARD             1 (to 1146)
-                 >> 1144 POP_TOP
-         
-         462     >> 1146 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1158 LOAD_CONST              21 ('waste_delay has to be an int from 0 - 1000.')
-                    1160 PRECALL                  1
-                    1164 CALL                     1
-                    1174 RAISE_VARARGS            1
-         
-         464     >> 1176 LOAD_FAST                6 (cleaner_vol)
-                    1178 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1210)
-         
-         465        1180 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1192 LOAD_CONST              22 ('Missing required parameter: cleaner_vol')
-                    1194 PRECALL                  1
-                    1198 CALL                     1
-                    1208 RAISE_VARARGS            1
-         
-         466     >> 1210 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1222 LOAD_FAST                6 (cleaner_vol)
-                    1224 LOAD_GLOBAL             12 (float)
-                    1236 PRECALL                  2
-                    1240 CALL                     2
-                    1250 POP_JUMP_FORWARD_IF_FALSE    15 (to 1282)
-                    1252 LOAD_CONST               7 (0)
-                    1254 LOAD_FAST                6 (cleaner_vol)
-                    1256 SWAP                     2
-                    1258 COPY                     2
-                    1260 COMPARE_OP               1 (<=)
-                    1266 POP_JUMP_FORWARD_IF_FALSE     6 (to 1280)
-                    1268 LOAD_CONST              17 (100)
-                    1270 COMPARE_OP               1 (<=)
-                    1276 POP_JUMP_FORWARD_IF_TRUE    17 (to 1312)
-                    1278 JUMP_FORWARD             1 (to 1282)
-                 >> 1280 POP_TOP
-         
-         467     >> 1282 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1294 LOAD_CONST              23 ('cleaner_vol has to be a float from 0 - 100.')
-                    1296 PRECALL                  1
-                    1300 CALL                     1
-                    1310 RAISE_VARARGS            1
-         
-         469     >> 1312 LOAD_GLOBAL             15 (NULL + np)
-                    1324 LOAD_ATTR                8 (round)
-                    1334 LOAD_FAST                6 (cleaner_vol)
-                    1336 LOAD_CONST               4 (1)
-                    1338 PRECALL                  2
-                    1342 CALL                     2
-                    1352 STORE_FAST               6 (cleaner_vol)
-         
-         471        1354 LOAD_FAST                7 (cleaner_delay)
-                    1356 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1388)
-         
-         472        1358 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1370 LOAD_CONST              24 ('Missing required parameter: cleaner_delay')
-                    1372 PRECALL                  1
-                    1376 CALL                     1
-                    1386 RAISE_VARARGS            1
-         
-         473     >> 1388 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1400 LOAD_FAST                7 (cleaner_delay)
-                    1402 LOAD_GLOBAL              4 (int)
-                    1414 PRECALL                  2
-                    1418 CALL                     2
-                    1428 POP_JUMP_FORWARD_IF_FALSE    15 (to 1460)
-                    1430 LOAD_CONST               7 (0)
-                    1432 LOAD_FAST                7 (cleaner_delay)
-                    1434 SWAP                     2
-                    1436 COPY                     2
-                    1438 COMPARE_OP               1 (<=)
-                    1444 POP_JUMP_FORWARD_IF_FALSE     6 (to 1458)
-                    1446 LOAD_CONST              20 (1000)
-                    1448 COMPARE_OP               1 (<=)
-                    1454 POP_JUMP_FORWARD_IF_TRUE    17 (to 1490)
-                    1456 JUMP_FORWARD             1 (to 1460)
-                 >> 1458 POP_TOP
-         
-         474     >> 1460 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1472 LOAD_CONST              25 ('cleaner_delay has to be an int from 0 - 1000.')
-                    1474 PRECALL                  1
-                    1478 CALL                     1
-                    1488 RAISE_VARARGS            1
-         
-         476     >> 1490 LOAD_FAST                8 (airgap)
-                    1492 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1524)
-         
-         477        1494 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1506 LOAD_CONST              26 ('Missing required parameter: airgap')
-                    1508 PRECALL                  1
-                    1512 CALL                     1
-                    1522 RAISE_VARARGS            1
-         
-         478     >> 1524 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1536 LOAD_FAST                8 (airgap)
-                    1538 LOAD_GLOBAL              4 (int)
-                    1550 PRECALL                  2
-                    1554 CALL                     2
-                    1564 POP_JUMP_FORWARD_IF_FALSE    15 (to 1596)
-                    1566 LOAD_CONST               7 (0)
-                    1568 LOAD_FAST                8 (airgap)
-                    1570 SWAP                     2
-                    1572 COPY                     2
-                    1574 COMPARE_OP               1 (<=)
-                    1580 POP_JUMP_FORWARD_IF_FALSE     6 (to 1594)
-                    1582 LOAD_CONST              17 (100)
-                    1584 COMPARE_OP               1 (<=)
-                    1590 POP_JUMP_FORWARD_IF_TRUE    17 (to 1626)
-                    1592 JUMP_FORWARD             1 (to 1596)
-                 >> 1594 POP_TOP
-         
-         479     >> 1596 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1608 LOAD_CONST              27 ('airgap has to be an int from 0 - 100.')
-                    1610 PRECALL                  1
-                    1614 CALL                     1
-                    1624 RAISE_VARARGS            1
-         
-         481     >> 1626 LOAD_FAST                9 (airgap_speed)
-                    1628 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1660)
-         
-         482        1630 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1642 LOAD_CONST              28 ('Missing required parameter: airgap_speed')
-                    1644 PRECALL                  1
-                    1648 CALL                     1
-                    1658 RAISE_VARARGS            1
-         
-         483     >> 1660 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1672 LOAD_FAST                9 (airgap_speed)
-                    1674 LOAD_GLOBAL              4 (int)
-                    1686 PRECALL                  2
-                    1690 CALL                     2
-                    1700 POP_JUMP_FORWARD_IF_FALSE    15 (to 1732)
-                    1702 LOAD_CONST               4 (1)
-                    1704 LOAD_FAST                9 (airgap_speed)
-                    1706 SWAP                     2
-                    1708 COPY                     2
-                    1710 COMPARE_OP               1 (<=)
-                    1716 POP_JUMP_FORWARD_IF_FALSE     6 (to 1730)
-                    1718 LOAD_CONST              20 (1000)
-                    1720 COMPARE_OP               1 (<=)
-                    1726 POP_JUMP_FORWARD_IF_TRUE    17 (to 1762)
-                    1728 JUMP_FORWARD             1 (to 1732)
-                 >> 1730 POP_TOP
-         
-         484     >> 1732 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1744 LOAD_CONST              29 ('airgap_speed has to be an int from 1 - 1000.')
-                    1746 PRECALL                  1
-                    1750 CALL                     1
-                    1760 RAISE_VARARGS            1
-         
-         486     >> 1762 LOAD_FAST               10 (retract_speed)
-                    1764 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1796)
-         
-         487        1766 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1778 LOAD_CONST              30 ('Missing required parameter: retract_speed')
-                    1780 PRECALL                  1
-                    1784 CALL                     1
-                    1794 RAISE_VARARGS            1
-         
-         488     >> 1796 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1808 LOAD_FAST               10 (retract_speed)
-                    1810 LOAD_GLOBAL              4 (int)
-                    1822 PRECALL                  2
-                    1826 CALL                     2
-                    1836 POP_JUMP_FORWARD_IF_FALSE    15 (to 1868)
-                    1838 LOAD_CONST               4 (1)
-                    1840 LOAD_FAST               10 (retract_speed)
-                    1842 SWAP                     2
-                    1844 COPY                     2
-                    1846 COMPARE_OP               1 (<=)
-                    1852 POP_JUMP_FORWARD_IF_FALSE     6 (to 1866)
-                    1854 LOAD_CONST              17 (100)
-                    1856 COMPARE_OP               1 (<=)
-                    1862 POP_JUMP_FORWARD_IF_TRUE    17 (to 1898)
-                    1864 JUMP_FORWARD             1 (to 1868)
-                 >> 1866 POP_TOP
-         
-         489     >> 1868 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1880 LOAD_CONST              31 ('retract_speed has to be an int from 1 - 100.')
-                    1882 PRECALL                  1
-                    1886 CALL                     1
-                    1896 RAISE_VARARGS            1
-         
-         491     >> 1898 LOAD_FAST               11 (fastwash)
-                    1900 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1932)
-         
-         492        1902 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1914 LOAD_CONST              32 ('Missing required paramter: fastwash')
-                    1916 PRECALL                  1
-                    1920 CALL                     1
-                    1930 RAISE_VARARGS            1
-         
-         493     >> 1932 LOAD_GLOBAL              3 (NULL + isinstance)
-                    1944 LOAD_FAST               11 (fastwash)
-                    1946 LOAD_GLOBAL              4 (int)
-                    1958 PRECALL                  2
-                    1962 CALL                     2
-                    1972 POP_JUMP_FORWARD_IF_TRUE    15 (to 2004)
-         
-         494        1974 LOAD_GLOBAL              1 (NULL + ValueError)
-                    1986 LOAD_CONST              33 ('Parameter fastwash is not int.')
-                    1988 PRECALL                  1
-                    1992 CALL                     1
-                    2002 RAISE_VARARGS            1
-         
-         495     >> 2004 LOAD_FAST               11 (fastwash)
-                    2006 LOAD_CONST               7 (0)
-                    2008 COMPARE_OP               2 (==)
-                    2014 POP_JUMP_FORWARD_IF_TRUE    21 (to 2058)
-                    2016 LOAD_FAST               11 (fastwash)
-                    2018 LOAD_CONST               4 (1)
-                    2020 COMPARE_OP               2 (==)
-                    2026 POP_JUMP_FORWARD_IF_TRUE    15 (to 2058)
-         
-         496        2028 LOAD_GLOBAL              1 (NULL + ValueError)
-                    2040 LOAD_CONST              34 ('Parameter fastwash has to be 0 (no fast-wash) or 1 (use fast-wash).')
-                    2042 PRECALL                  1
-                    2046 CALL                     1
-                    2056 RAISE_VARARGS            1
-         
-         498     >> 2058 LOAD_FAST               12 (low_volume)
-                    2060 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 2092)
-         
-         499        2062 LOAD_GLOBAL              1 (NULL + ValueError)
-                    2074 LOAD_CONST              35 ('Missing required paramter: low_volume')
-                    2076 PRECALL                  1
-                    2080 CALL                     1
-                    2090 RAISE_VARARGS            1
-         
-         500     >> 2092 LOAD_GLOBAL              3 (NULL + isinstance)
-                    2104 LOAD_FAST               12 (low_volume)
-                    2106 LOAD_GLOBAL              4 (int)
-                    2118 PRECALL                  2
-                    2122 CALL                     2
-                    2132 POP_JUMP_FORWARD_IF_TRUE    15 (to 2164)
-         
-         501        2134 LOAD_GLOBAL              1 (NULL + ValueError)
-                    2146 LOAD_CONST              36 ('Parameter low_volume is not int.')
-                    2148 PRECALL                  1
-                    2152 CALL                     1
-                    2162 RAISE_VARARGS            1
-         
-         502     >> 2164 LOAD_FAST               12 (low_volume)
-                    2166 LOAD_CONST               7 (0)
-                    2168 COMPARE_OP               2 (==)
-                    2174 POP_JUMP_FORWARD_IF_TRUE    21 (to 2218)
-                    2176 LOAD_FAST               12 (low_volume)
-                    2178 LOAD_CONST               4 (1)
-                    2180 COMPARE_OP               2 (==)
-                    2186 POP_JUMP_FORWARD_IF_TRUE    15 (to 2218)
-         
-         503        2188 LOAD_GLOBAL              1 (NULL + ValueError)
-                    2200 LOAD_CONST              37 ('Parameter low_volume has to be 0 (no fast-wash) or 1 (use fast-wash).')
-                    2202 PRECALL                  1
-                    2206 CALL                     1
-                    2216 RAISE_VARARGS            1
-         
-         506     >> 2218 LOAD_FAST               13 (tecan_tips)
-         
-         507        2220 LOAD_FAST                1 (waste_location)
-         
-         508        2222 LOAD_FAST                2 (cleaner_location)
-         
-         509        2224 LOAD_FAST                3 (arm)
-         
-         510        2226 LOAD_FAST                4 (waste_vol)
-         
-         511        2228 LOAD_FAST                5 (waste_delay)
-         
-         512        2230 LOAD_FAST                6 (cleaner_vol)
-         
-         513        2232 LOAD_FAST                7 (cleaner_delay)
-         
-         514        2234 LOAD_FAST                8 (airgap)
-         
-         515        2236 LOAD_FAST                9 (airgap_speed)
+         442     >>  454 LOAD_FAST               15 (grid)
+                     456 LOAD_FAST               16 (site)
+                     458 LOAD_CONST               4 (1)
+                     460 BINARY_OP               10 (-)
+                     464 BUILD_TUPLE              2
+                     466 STORE_FAST               1 (waste_location)
+         
+         444         468 LOAD_FAST                2 (cleaner_location)
+                     470 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 502)
+         
+         445         472 LOAD_GLOBAL              1 (NULL + ValueError)
+                     484 LOAD_CONST               9 ('Missing required parameter: cleaner_location')
+                     486 PRECALL                  1
+                     490 CALL                     1
+                     500 RAISE_VARARGS            1
+         
+         446     >>  502 LOAD_FAST                2 (cleaner_location)
+                     504 UNPACK_SEQUENCE          2
+                     508 STORE_FAST              15 (grid)
+                     510 STORE_FAST              16 (site)
+         
+         447         512 LOAD_GLOBAL              3 (NULL + isinstance)
+                     524 LOAD_FAST               15 (grid)
+                     526 LOAD_GLOBAL              4 (int)
+                     538 PRECALL                  2
+                     542 CALL                     2
+                     552 POP_JUMP_FORWARD_IF_FALSE    15 (to 584)
+                     554 LOAD_CONST               4 (1)
+                     556 LOAD_FAST               15 (grid)
+                     558 SWAP                     2
+                     560 COPY                     2
+                     562 COMPARE_OP               1 (<=)
+                     568 POP_JUMP_FORWARD_IF_FALSE     6 (to 582)
+                     570 LOAD_CONST               5 (67)
+                     572 COMPARE_OP               1 (<=)
+                     578 POP_JUMP_FORWARD_IF_TRUE    17 (to 614)
+                     580 JUMP_FORWARD             1 (to 584)
+                 >>  582 POP_TOP
+         
+         448     >>  584 LOAD_GLOBAL              1 (NULL + ValueError)
+                     596 LOAD_CONST              10 ('Grid (first number in cleaner_location tuple) has to be an int from 1 - 67.')
+                     598 PRECALL                  1
+                     602 CALL                     1
+                     612 RAISE_VARARGS            1
+         
+         449     >>  614 LOAD_GLOBAL              3 (NULL + isinstance)
+                     626 LOAD_FAST               16 (site)
+                     628 LOAD_GLOBAL              4 (int)
+                     640 PRECALL                  2
+                     644 CALL                     2
+                     654 POP_JUMP_FORWARD_IF_FALSE    15 (to 686)
+                     656 LOAD_CONST               4 (1)
+                     658 LOAD_FAST               16 (site)
+                     660 SWAP                     2
+                     662 COPY                     2
+                     664 COMPARE_OP               1 (<=)
+                     670 POP_JUMP_FORWARD_IF_FALSE     6 (to 684)
+                     672 LOAD_CONST               7 (128)
+                     674 COMPARE_OP               1 (<=)
+                     680 POP_JUMP_FORWARD_IF_TRUE    17 (to 716)
+                     682 JUMP_FORWARD             1 (to 686)
+                 >>  684 POP_TOP
+         
+         450     >>  686 LOAD_GLOBAL              1 (NULL + ValueError)
+                     698 LOAD_CONST              11 ('Site (second number in cleaner_location tuple) has to be an int from 1 - 128.')
+                     700 PRECALL                  1
+                     704 CALL                     1
+                     714 RAISE_VARARGS            1
+         
+         451     >>  716 LOAD_FAST               15 (grid)
+                     718 LOAD_FAST               16 (site)
+                     720 LOAD_CONST               4 (1)
+                     722 BINARY_OP               10 (-)
+                     726 BUILD_TUPLE              2
+                     728 STORE_FAST               2 (cleaner_location)
+         
+         453         730 LOAD_FAST                3 (arm)
+                     732 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 764)
+         
+         454         734 LOAD_GLOBAL              1 (NULL + ValueError)
+                     746 LOAD_CONST              12 ('Missing required paramter: arm')
+                     748 PRECALL                  1
+                     752 CALL                     1
+                     762 RAISE_VARARGS            1
+         
+         455     >>  764 LOAD_GLOBAL              3 (NULL + isinstance)
+                     776 LOAD_FAST                3 (arm)
+                     778 LOAD_GLOBAL              4 (int)
+                     790 PRECALL                  2
+                     794 CALL                     2
+                     804 POP_JUMP_FORWARD_IF_TRUE    15 (to 836)
+         
+         456         806 LOAD_GLOBAL              1 (NULL + ValueError)
+                     818 LOAD_CONST              13 ('Parameter arm is not int.')
+                     820 PRECALL                  1
+                     824 CALL                     1
+                     834 RAISE_VARARGS            1
+         
+         457     >>  836 LOAD_FAST                3 (arm)
+                     838 LOAD_CONST              14 (0)
+                     840 COMPARE_OP               2 (==)
+                     846 POP_JUMP_FORWARD_IF_TRUE    21 (to 890)
+                     848 LOAD_FAST                3 (arm)
+                     850 LOAD_CONST               4 (1)
+                     852 COMPARE_OP               2 (==)
+                     858 POP_JUMP_FORWARD_IF_TRUE    15 (to 890)
+         
+         458         860 LOAD_GLOBAL              1 (NULL + ValueError)
+                     872 LOAD_CONST              15 ('Parameter arm has to be 0 (LiHa 1) or 1 (LiHa 2).')
+                     874 PRECALL                  1
+                     878 CALL                     1
+                     888 RAISE_VARARGS            1
+         
+         460     >>  890 LOAD_FAST                4 (waste_vol)
+                     892 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 924)
+         
+         461         894 LOAD_GLOBAL              1 (NULL + ValueError)
+                     906 LOAD_CONST              16 ('Missing required parameter: waste_vol')
+                     908 PRECALL                  1
+                     912 CALL                     1
+                     922 RAISE_VARARGS            1
+         
+         462     >>  924 LOAD_GLOBAL              3 (NULL + isinstance)
+                     936 LOAD_FAST                4 (waste_vol)
+                     938 LOAD_GLOBAL             12 (float)
+                     950 PRECALL                  2
+                     954 CALL                     2
+                     964 POP_JUMP_FORWARD_IF_FALSE    15 (to 996)
+                     966 LOAD_CONST              14 (0)
+                     968 LOAD_FAST                4 (waste_vol)
+                     970 SWAP                     2
+                     972 COPY                     2
+                     974 COMPARE_OP               1 (<=)
+                     980 POP_JUMP_FORWARD_IF_FALSE     6 (to 994)
+                     982 LOAD_CONST              17 (100)
+                     984 COMPARE_OP               1 (<=)
+                     990 POP_JUMP_FORWARD_IF_TRUE    17 (to 1026)
+                     992 JUMP_FORWARD             1 (to 996)
+                 >>  994 POP_TOP
+         
+         463     >>  996 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1008 LOAD_CONST              18 ('waste_vol has to be a float from 0 - 100.')
+                    1010 PRECALL                  1
+                    1014 CALL                     1
+                    1024 RAISE_VARARGS            1
+         
+         465     >> 1026 LOAD_GLOBAL             15 (NULL + np)
+                    1038 LOAD_ATTR                8 (round)
+                    1048 LOAD_FAST                4 (waste_vol)
+                    1050 LOAD_CONST               4 (1)
+                    1052 PRECALL                  2
+                    1056 CALL                     2
+                    1066 STORE_FAST               4 (waste_vol)
+         
+         467        1068 LOAD_FAST                5 (waste_delay)
+                    1070 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1102)
+         
+         468        1072 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1084 LOAD_CONST              19 ('Missing required parameter: waste_delay')
+                    1086 PRECALL                  1
+                    1090 CALL                     1
+                    1100 RAISE_VARARGS            1
+         
+         469     >> 1102 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1114 LOAD_FAST                5 (waste_delay)
+                    1116 LOAD_GLOBAL              4 (int)
+                    1128 PRECALL                  2
+                    1132 CALL                     2
+                    1142 POP_JUMP_FORWARD_IF_FALSE    15 (to 1174)
+                    1144 LOAD_CONST              14 (0)
+                    1146 LOAD_FAST                5 (waste_delay)
+                    1148 SWAP                     2
+                    1150 COPY                     2
+                    1152 COMPARE_OP               1 (<=)
+                    1158 POP_JUMP_FORWARD_IF_FALSE     6 (to 1172)
+                    1160 LOAD_CONST              20 (1000)
+                    1162 COMPARE_OP               1 (<=)
+                    1168 POP_JUMP_FORWARD_IF_TRUE    17 (to 1204)
+                    1170 JUMP_FORWARD             1 (to 1174)
+                 >> 1172 POP_TOP
+         
+         470     >> 1174 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1186 LOAD_CONST              21 ('waste_delay has to be an int from 0 - 1000.')
+                    1188 PRECALL                  1
+                    1192 CALL                     1
+                    1202 RAISE_VARARGS            1
+         
+         472     >> 1204 LOAD_FAST                6 (cleaner_vol)
+                    1206 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1238)
+         
+         473        1208 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1220 LOAD_CONST              22 ('Missing required parameter: cleaner_vol')
+                    1222 PRECALL                  1
+                    1226 CALL                     1
+                    1236 RAISE_VARARGS            1
+         
+         474     >> 1238 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1250 LOAD_FAST                6 (cleaner_vol)
+                    1252 LOAD_GLOBAL             12 (float)
+                    1264 PRECALL                  2
+                    1268 CALL                     2
+                    1278 POP_JUMP_FORWARD_IF_FALSE    15 (to 1310)
+                    1280 LOAD_CONST              14 (0)
+                    1282 LOAD_FAST                6 (cleaner_vol)
+                    1284 SWAP                     2
+                    1286 COPY                     2
+                    1288 COMPARE_OP               1 (<=)
+                    1294 POP_JUMP_FORWARD_IF_FALSE     6 (to 1308)
+                    1296 LOAD_CONST              17 (100)
+                    1298 COMPARE_OP               1 (<=)
+                    1304 POP_JUMP_FORWARD_IF_TRUE    17 (to 1340)
+                    1306 JUMP_FORWARD             1 (to 1310)
+                 >> 1308 POP_TOP
+         
+         475     >> 1310 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1322 LOAD_CONST              23 ('cleaner_vol has to be a float from 0 - 100.')
+                    1324 PRECALL                  1
+                    1328 CALL                     1
+                    1338 RAISE_VARARGS            1
+         
+         477     >> 1340 LOAD_GLOBAL             15 (NULL + np)
+                    1352 LOAD_ATTR                8 (round)
+                    1362 LOAD_FAST                6 (cleaner_vol)
+                    1364 LOAD_CONST               4 (1)
+                    1366 PRECALL                  2
+                    1370 CALL                     2
+                    1380 STORE_FAST               6 (cleaner_vol)
+         
+         479        1382 LOAD_FAST                7 (cleaner_delay)
+                    1384 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1416)
+         
+         480        1386 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1398 LOAD_CONST              24 ('Missing required parameter: cleaner_delay')
+                    1400 PRECALL                  1
+                    1404 CALL                     1
+                    1414 RAISE_VARARGS            1
+         
+         481     >> 1416 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1428 LOAD_FAST                7 (cleaner_delay)
+                    1430 LOAD_GLOBAL              4 (int)
+                    1442 PRECALL                  2
+                    1446 CALL                     2
+                    1456 POP_JUMP_FORWARD_IF_FALSE    15 (to 1488)
+                    1458 LOAD_CONST              14 (0)
+                    1460 LOAD_FAST                7 (cleaner_delay)
+                    1462 SWAP                     2
+                    1464 COPY                     2
+                    1466 COMPARE_OP               1 (<=)
+                    1472 POP_JUMP_FORWARD_IF_FALSE     6 (to 1486)
+                    1474 LOAD_CONST              20 (1000)
+                    1476 COMPARE_OP               1 (<=)
+                    1482 POP_JUMP_FORWARD_IF_TRUE    17 (to 1518)
+                    1484 JUMP_FORWARD             1 (to 1488)
+                 >> 1486 POP_TOP
+         
+         482     >> 1488 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1500 LOAD_CONST              25 ('cleaner_delay has to be an int from 0 - 1000.')
+                    1502 PRECALL                  1
+                    1506 CALL                     1
+                    1516 RAISE_VARARGS            1
+         
+         484     >> 1518 LOAD_FAST                8 (airgap)
+                    1520 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1552)
+         
+         485        1522 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1534 LOAD_CONST              26 ('Missing required parameter: airgap')
+                    1536 PRECALL                  1
+                    1540 CALL                     1
+                    1550 RAISE_VARARGS            1
+         
+         486     >> 1552 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1564 LOAD_FAST                8 (airgap)
+                    1566 LOAD_GLOBAL              4 (int)
+                    1578 PRECALL                  2
+                    1582 CALL                     2
+                    1592 POP_JUMP_FORWARD_IF_FALSE    15 (to 1624)
+                    1594 LOAD_CONST              14 (0)
+                    1596 LOAD_FAST                8 (airgap)
+                    1598 SWAP                     2
+                    1600 COPY                     2
+                    1602 COMPARE_OP               1 (<=)
+                    1608 POP_JUMP_FORWARD_IF_FALSE     6 (to 1622)
+                    1610 LOAD_CONST              17 (100)
+                    1612 COMPARE_OP               1 (<=)
+                    1618 POP_JUMP_FORWARD_IF_TRUE    17 (to 1654)
+                    1620 JUMP_FORWARD             1 (to 1624)
+                 >> 1622 POP_TOP
+         
+         487     >> 1624 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1636 LOAD_CONST              27 ('airgap has to be an int from 0 - 100.')
+                    1638 PRECALL                  1
+                    1642 CALL                     1
+                    1652 RAISE_VARARGS            1
+         
+         489     >> 1654 LOAD_FAST                9 (airgap_speed)
+                    1656 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1688)
+         
+         490        1658 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1670 LOAD_CONST              28 ('Missing required parameter: airgap_speed')
+                    1672 PRECALL                  1
+                    1676 CALL                     1
+                    1686 RAISE_VARARGS            1
+         
+         491     >> 1688 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1700 LOAD_FAST                9 (airgap_speed)
+                    1702 LOAD_GLOBAL              4 (int)
+                    1714 PRECALL                  2
+                    1718 CALL                     2
+                    1728 POP_JUMP_FORWARD_IF_FALSE    15 (to 1760)
+                    1730 LOAD_CONST               4 (1)
+                    1732 LOAD_FAST                9 (airgap_speed)
+                    1734 SWAP                     2
+                    1736 COPY                     2
+                    1738 COMPARE_OP               1 (<=)
+                    1744 POP_JUMP_FORWARD_IF_FALSE     6 (to 1758)
+                    1746 LOAD_CONST              20 (1000)
+                    1748 COMPARE_OP               1 (<=)
+                    1754 POP_JUMP_FORWARD_IF_TRUE    17 (to 1790)
+                    1756 JUMP_FORWARD             1 (to 1760)
+                 >> 1758 POP_TOP
+         
+         492     >> 1760 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1772 LOAD_CONST              29 ('airgap_speed has to be an int from 1 - 1000.')
+                    1774 PRECALL                  1
+                    1778 CALL                     1
+                    1788 RAISE_VARARGS            1
+         
+         494     >> 1790 LOAD_FAST               10 (retract_speed)
+                    1792 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1824)
+         
+         495        1794 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1806 LOAD_CONST              30 ('Missing required parameter: retract_speed')
+                    1808 PRECALL                  1
+                    1812 CALL                     1
+                    1822 RAISE_VARARGS            1
+         
+         496     >> 1824 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1836 LOAD_FAST               10 (retract_speed)
+                    1838 LOAD_GLOBAL              4 (int)
+                    1850 PRECALL                  2
+                    1854 CALL                     2
+                    1864 POP_JUMP_FORWARD_IF_FALSE    15 (to 1896)
+                    1866 LOAD_CONST               4 (1)
+                    1868 LOAD_FAST               10 (retract_speed)
+                    1870 SWAP                     2
+                    1872 COPY                     2
+                    1874 COMPARE_OP               1 (<=)
+                    1880 POP_JUMP_FORWARD_IF_FALSE     6 (to 1894)
+                    1882 LOAD_CONST              17 (100)
+                    1884 COMPARE_OP               1 (<=)
+                    1890 POP_JUMP_FORWARD_IF_TRUE    17 (to 1926)
+                    1892 JUMP_FORWARD             1 (to 1896)
+                 >> 1894 POP_TOP
+         
+         497     >> 1896 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1908 LOAD_CONST              31 ('retract_speed has to be an int from 1 - 100.')
+                    1910 PRECALL                  1
+                    1914 CALL                     1
+                    1924 RAISE_VARARGS            1
+         
+         499     >> 1926 LOAD_FAST               11 (fastwash)
+                    1928 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 1960)
+         
+         500        1930 LOAD_GLOBAL              1 (NULL + ValueError)
+                    1942 LOAD_CONST              32 ('Missing required paramter: fastwash')
+                    1944 PRECALL                  1
+                    1948 CALL                     1
+                    1958 RAISE_VARARGS            1
+         
+         501     >> 1960 LOAD_GLOBAL              3 (NULL + isinstance)
+                    1972 LOAD_FAST               11 (fastwash)
+                    1974 LOAD_GLOBAL              4 (int)
+                    1986 PRECALL                  2
+                    1990 CALL                     2
+                    2000 POP_JUMP_FORWARD_IF_TRUE    15 (to 2032)
+         
+         502        2002 LOAD_GLOBAL              1 (NULL + ValueError)
+                    2014 LOAD_CONST              33 ('Parameter fastwash is not int.')
+                    2016 PRECALL                  1
+                    2020 CALL                     1
+                    2030 RAISE_VARARGS            1
+         
+         503     >> 2032 LOAD_FAST               11 (fastwash)
+                    2034 LOAD_CONST              14 (0)
+                    2036 COMPARE_OP               2 (==)
+                    2042 POP_JUMP_FORWARD_IF_TRUE    21 (to 2086)
+                    2044 LOAD_FAST               11 (fastwash)
+                    2046 LOAD_CONST               4 (1)
+                    2048 COMPARE_OP               2 (==)
+                    2054 POP_JUMP_FORWARD_IF_TRUE    15 (to 2086)
+         
+         504        2056 LOAD_GLOBAL              1 (NULL + ValueError)
+                    2068 LOAD_CONST              34 ('Parameter fastwash has to be 0 (no fast-wash) or 1 (use fast-wash).')
+                    2070 PRECALL                  1
+                    2074 CALL                     1
+                    2084 RAISE_VARARGS            1
+         
+         506     >> 2086 LOAD_FAST               12 (low_volume)
+                    2088 POP_JUMP_FORWARD_IF_NOT_NONE    15 (to 2120)
+         
+         507        2090 LOAD_GLOBAL              1 (NULL + ValueError)
+                    2102 LOAD_CONST              35 ('Missing required paramter: low_volume')
+                    2104 PRECALL                  1
+                    2108 CALL                     1
+                    2118 RAISE_VARARGS            1
+         
+         508     >> 2120 LOAD_GLOBAL              3 (NULL + isinstance)
+                    2132 LOAD_FAST               12 (low_volume)
+                    2134 LOAD_GLOBAL              4 (int)
+                    2146 PRECALL                  2
+                    2150 CALL                     2
+                    2160 POP_JUMP_FORWARD_IF_TRUE    15 (to 2192)
+         
+         509        2162 LOAD_GLOBAL              1 (NULL + ValueError)
+                    2174 LOAD_CONST              36 ('Parameter low_volume is not int.')
+                    2176 PRECALL                  1
+                    2180 CALL                     1
+                    2190 RAISE_VARARGS            1
+         
+         510     >> 2192 LOAD_FAST               12 (low_volume)
+                    2194 LOAD_CONST              14 (0)
+                    2196 COMPARE_OP               2 (==)
+                    2202 POP_JUMP_FORWARD_IF_TRUE    21 (to 2246)
+                    2204 LOAD_FAST               12 (low_volume)
+                    2206 LOAD_CONST               4 (1)
+                    2208 COMPARE_OP               2 (==)
+                    2214 POP_JUMP_FORWARD_IF_TRUE    15 (to 2246)
+         
+         511        2216 LOAD_GLOBAL              1 (NULL + ValueError)
+                    2228 LOAD_CONST              37 ('Parameter low_volume has to be 0 (no fast-wash) or 1 (use fast-wash).')
+                    2230 PRECALL                  1
+                    2234 CALL                     1
+                    2244 RAISE_VARARGS            1
+         
+         514     >> 2246 LOAD_FAST               13 (tecan_tips)
+         
+         515        2248 LOAD_FAST                1 (waste_location)
+         
+         516        2250 LOAD_FAST                2 (cleaner_location)
+         
+         517        2252 LOAD_FAST                3 (arm)
+         
+         518        2254 LOAD_FAST                4 (waste_vol)
+         
+         519        2256 LOAD_FAST                5 (waste_delay)
+         
+         520        2258 LOAD_FAST                6 (cleaner_vol)
+         
+         521        2260 LOAD_FAST                7 (cleaner_delay)
+         
+         522        2262 LOAD_FAST                8 (airgap)
+         
+         523        2264 LOAD_FAST                9 (airgap_speed)
          
-         516        2238 LOAD_FAST               10 (retract_speed)
+         524        2266 LOAD_FAST               10 (retract_speed)
          
-         517        2240 LOAD_FAST               11 (fastwash)
+         525        2268 LOAD_FAST               11 (fastwash)
          
-         518        2242 LOAD_FAST               12 (low_volume)
+         526        2270 LOAD_FAST               12 (low_volume)
          
-         505        2244 BUILD_TUPLE             13
-                    2246 RETURN_VALUE
+         513        2272 BUILD_TUPLE             13
+                    2274 RETURN_VALUE
          consts
-            "Validates and prepares aspirate/dispense parameters.\n\n    Parameters\n    ----------\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    waste_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of waste as integers\n    cleaner_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers\n    arm : int\n        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2\n    waste_vol: float\n        Volume in waste in mL (0-100)\n    waste_delay : int\n        Delay before closing valves in waste in ms (0-1000)\n    cleaner_vol: float\n        Volume in cleaner in mL (0-100)\n    cleaner_delay : int\n        Delay before closing valves in cleaner in ms (0-1000)\n    airgap : int\n        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)\n    airgap_speed : int\n        Speed of airgap aspiration in µL/s (1-1000)\n    retract_speed : int\n        Retract speed in mm/s (1-100)\n    fastwash : int\n        Use fast-wash module = 1, don't use it = 0\n    low_volume : int\n        Use pinch valves = 1, don't use them = 0\n\n    Returns\n    -------\n    tips : list\n        Tip(s) that will be selected; have been converted to tip.T1 - tip.T8 here if they weren't originally formatted that way\n    waste_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of waste as integers\n    cleaner_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers\n    arm : int\n        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2\n    waste_vol: float\n        Volume in waste in mL (0-100)\n    waste_delay : int\n        Delay before closing valves in waste in ms (0-1000)\n    cleaner_vol: float\n        Volume in cleaner in mL (0-100)\n    cleaner_delay : int\n        Delay before closing valves in cleaner in ms (0-1000)\n    airgap : int\n        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)\n    airgap_speed : int\n        Speed of airgap aspiration in µL/s (1-1000)\n    retract_speed : int\n        Retract speed in mm/s (1-100)\n    fastwash : int\n        Use fast-wash module = 1, don't use it = 0\n    low_volume : int\n        Use pinch valves = 1, don't use them = 0\n    "
+            "Validates and prepares aspirate/dispense parameters.\n\n    Parameters\n    ----------\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    waste_location : tuple\n        Tuple with grid position (1-67) and site number (1-128) of waste as integers\n    cleaner_location : tuple\n        Tuple with grid position (1-67) and site number (1-128) of cleaner as integers\n    arm : int\n        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2\n    waste_vol: float\n        Volume in waste in mL (0-100)\n    waste_delay : int\n        Delay before closing valves in waste in ms (0-1000)\n    cleaner_vol: float\n        Volume in cleaner in mL (0-100)\n    cleaner_delay : int\n        Delay before closing valves in cleaner in ms (0-1000)\n    airgap : int\n        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)\n    airgap_speed : int\n        Speed of airgap aspiration in µL/s (1-1000)\n    retract_speed : int\n        Retract speed in mm/s (1-100)\n    fastwash : int\n        Use fast-wash module = 1, don't use it = 0\n    low_volume : int\n        Use pinch valves = 1, don't use them = 0\n\n    Returns\n    -------\n    tips : list\n        Tip(s) that will be selected; have been converted to tip.T1 - tip.T8 here if they weren't originally formatted that way\n    waste_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of waste as integers\n    cleaner_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers\n    arm : int\n        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2\n    waste_vol: float\n        Volume in waste in mL (0-100)\n    waste_delay : int\n        Delay before closing valves in waste in ms (0-1000)\n    cleaner_vol: float\n        Volume in cleaner in mL (0-100)\n    cleaner_delay : int\n        Delay before closing valves in cleaner in ms (0-1000)\n    airgap : int\n        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)\n    airgap_speed : int\n        Speed of airgap aspiration in µL/s (1-1000)\n    retract_speed : int\n        Retract speed in mm/s (1-100)\n    fastwash : int\n        Use fast-wash module = 1, don't use it = 0\n    low_volume : int\n        Use pinch valves = 1, don't use them = 0\n    "
             None
             'Missing required parameter: tips'
             'Missing required parameter: waste_location'
             1
             67
             'Grid (first number in waste_location tuple) has to be an int from 1 - 67.'
-            0
-            127
-            'Site (second number in waste_location tuple) has to be an int from 0 - 127.'
+            128
+            'Site (second number in waste_location tuple) has to be an int from 1 - 128.'
             'Missing required parameter: cleaner_location'
             'Grid (first number in cleaner_location tuple) has to be an int from 1 - 67.'
-            'Site (second number in cleaner_location tuple) has to be an int from 0 - 127.'
+            'Site (second number in cleaner_location tuple) has to be an int from 1 - 128.'
             'Missing required paramter: arm'
             'Parameter arm is not int.'
+            0
             'Parameter arm has to be 0 (LiHa 1) or 1 (LiHa 2).'
             'Missing required parameter: waste_vol'
             100
             'waste_vol has to be a float from 0 - 100.'
             'Missing required parameter: waste_delay'
             1000
             'waste_delay has to be an int from 0 - 1000.'
@@ -2526,22 +2528,22 @@
             'Parameter low_volume has to be 0 (no fast-wash) or 1 (use fast-wash).'
          names      ('ValueError', 'isinstance', 'int', 'Tip', 'int_to_tip', 'append', 'float', 'np', 'round')
          varnames   ('tips', 'waste_location', 'cleaner_location', 'arm', 'waste_vol', 'waste_delay', 'cleaner_vol', 'cleaner_delay', 'airgap', 'airgap_speed', 'retract_speed', 'fastwash', 'low_volume', 'tecan_tips', 'tip', 'grid', 'site')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
          name       'prepare_evo_wash_parameters'
-         firstlineno 343
+         firstlineno 349
          lnotab
             0x024c04011e020401080154021e012c0204011e010a0148011e0148011e
-            0204011e010a0148011e0148011e0204011e012a011e0118011e0204011e
-            0148011e022a0204011e0148011e0204011e0148011e022a0204011e0148
-            011e0204011e0148011e0204011e0148011e0204011e0148011e0204011e
-            012a011e0118011e0204011e012a011e0118011e03020102010201020102
-            01020102010201020102010201020102f3
+            010e0204011e010a0148011e0148011e010e0204011e012a011e0118011e
+            0204011e0148011e022a0204011e0148011e0204011e0148011e022a0204
+            011e0148011e0204011e0148011e0204011e0148011e0204011e0148011e
+            0204011e012a011e0118011e0204011e012a011e0118011e030201020102
+            0102010201020102010201020102010201020102f3
       code
          argcount  : 0
          nlocals   : 16
          stacksize : 15
          flags     : 3
          code
             0x97007401000000000000000000007c007c017c027c037c047c057c067c
@@ -2553,100 +2555,100 @@
             01640591017c016402190000000000000000009b009101640591017c0164
             06190000000000000000009b009101640591017c02640219000000000000
             0000009b009101640591017c026406190000000000000000009b00910164
             0791017c049b009101640891017c059b009101640791017c069b00910164
             0891017c079b009101640591017c089b009101640591017c099b00910164
             0591017c0a9b009101640591017c0b9b009101640591017c0c9b00910164
             0991017c039b009101640a9101a6010000ab0100000000000000005300
-         522           0 RESUME                   0
+         530           0 RESUME                   0
          
-         572           2 LOAD_GLOBAL              1 (NULL + dict)
+         580           2 LOAD_GLOBAL              1 (NULL + dict)
          
-         573          14 LOAD_FAST                0 (tips)
+         581          14 LOAD_FAST                0 (tips)
          
-         574          16 LOAD_FAST                1 (waste_location)
+         582          16 LOAD_FAST                1 (waste_location)
          
-         575          18 LOAD_FAST                2 (cleaner_location)
+         583          18 LOAD_FAST                2 (cleaner_location)
          
-         576          20 LOAD_FAST                3 (arm)
+         584          20 LOAD_FAST                3 (arm)
          
-         577          22 LOAD_FAST                4 (waste_vol)
+         585          22 LOAD_FAST                4 (waste_vol)
          
-         578          24 LOAD_FAST                5 (waste_delay)
+         586          24 LOAD_FAST                5 (waste_delay)
          
-         579          26 LOAD_FAST                6 (cleaner_vol)
+         587          26 LOAD_FAST                6 (cleaner_vol)
          
-         580          28 LOAD_FAST                7 (cleaner_delay)
+         588          28 LOAD_FAST                7 (cleaner_delay)
          
-         581          30 LOAD_FAST                8 (airgap)
+         589          30 LOAD_FAST                8 (airgap)
          
-         582          32 LOAD_FAST                9 (airgap_speed)
+         590          32 LOAD_FAST                9 (airgap_speed)
          
-         583          34 LOAD_FAST               10 (retract_speed)
+         591          34 LOAD_FAST               10 (retract_speed)
          
-         584          36 LOAD_FAST               11 (fastwash)
+         592          36 LOAD_FAST               11 (fastwash)
          
-         585          38 LOAD_FAST               12 (low_volume)
+         593          38 LOAD_FAST               12 (low_volume)
          
-         572          40 KW_NAMES                 1
+         580          40 KW_NAMES                 1
                       42 PRECALL                 13
                       46 CALL                    13
                       56 STORE_FAST              13 (kwargs)
          
-         601          58 LOAD_GLOBAL              3 (NULL + prepare_evo_wash_parameters)
+         609          58 LOAD_GLOBAL              3 (NULL + prepare_evo_wash_parameters)
                       70 LOAD_CONST              11 (())
                       72 BUILD_MAP                0
                       74 LOAD_FAST               13 (kwargs)
                       76 DICT_MERGE               1
                       78 CALL_FUNCTION_EX         1
          
-         587          80 UNPACK_SEQUENCE         13
+         595          80 UNPACK_SEQUENCE         13
          
-         588          84 STORE_FAST               0 (tips)
+         596          84 STORE_FAST               0 (tips)
          
-         589          86 STORE_FAST               1 (waste_location)
+         597          86 STORE_FAST               1 (waste_location)
          
-         590          88 STORE_FAST               2 (cleaner_location)
+         598          88 STORE_FAST               2 (cleaner_location)
          
-         591          90 STORE_FAST               3 (arm)
+         599          90 STORE_FAST               3 (arm)
          
-         592          92 STORE_FAST               4 (waste_vol)
+         600          92 STORE_FAST               4 (waste_vol)
          
-         593          94 STORE_FAST               5 (waste_delay)
+         601          94 STORE_FAST               5 (waste_delay)
          
-         594          96 STORE_FAST               6 (cleaner_vol)
+         602          96 STORE_FAST               6 (cleaner_vol)
          
-         595          98 STORE_FAST               7 (cleaner_delay)
+         603          98 STORE_FAST               7 (cleaner_delay)
          
-         596         100 STORE_FAST               8 (airgap)
+         604         100 STORE_FAST               8 (airgap)
          
-         597         102 STORE_FAST               9 (airgap_speed)
+         605         102 STORE_FAST               9 (airgap_speed)
          
-         598         104 STORE_FAST              10 (retract_speed)
+         606         104 STORE_FAST              10 (retract_speed)
          
-         599         106 STORE_FAST              11 (fastwash)
+         607         106 STORE_FAST              11 (fastwash)
          
-         600         108 STORE_FAST              12 (low_volume)
+         608         108 STORE_FAST              12 (low_volume)
          
-         603         110 LOAD_CONST               2 (0)
+         611         110 LOAD_CONST               2 (0)
                      112 STORE_FAST              14 (tip_selection)
          
-         604         114 LOAD_FAST                0 (tips)
+         612         114 LOAD_FAST                0 (tips)
                      116 GET_ITER
                  >>  118 FOR_ITER                12 (to 144)
                      120 STORE_FAST              15 (tip)
          
-         605         122 LOAD_FAST               14 (tip_selection)
+         613         122 LOAD_FAST               14 (tip_selection)
                      124 LOAD_FAST               15 (tip)
                      126 LOAD_ATTR                2 (value)
                      136 BINARY_OP               13 (+=)
                      140 STORE_FAST              14 (tip_selection)
                      142 JUMP_BACKWARD           13 (to 118)
          
-         606     >>  144 LOAD_CONST               3 ('')
+         614     >>  144 LOAD_CONST               3 ('')
                      146 LOAD_METHOD              3 (join)
                      168 BUILD_LIST               0
                      170 LOAD_CONST               4 ('B;Wash(')
                      172 LIST_APPEND              1
                      174 LOAD_FAST               14 (tip_selection)
                      176 FORMAT_VALUE             0
                      178 LIST_APPEND              1
@@ -2730,15 +2732,15 @@
                      366 LIST_APPEND              1
                      368 LOAD_CONST              10 (');')
                      370 LIST_APPEND              1
                      372 PRECALL                  1
                      376 CALL                     1
                      386 RETURN_VALUE
          consts
-            "Command for aspirating with the EvoWARE aspirate command. As many wells in one column may be selected as your liquid handling arm has pipettes.\n    This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string\n    specifying the target wells.\n\n    Parameters\n    ----------\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    waste_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of waste as integers\n    cleaner_location : tuple\n        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers\n    arm : int\n        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2\n    waste_vol: float\n        Volume in waste in mL (0-100)\n    waste_delay : int\n        Delay before closing valves in waste in ms (0-1000)\n    cleaner_vol: float\n        Volume in cleaner in mL (0-100)\n    cleaner_delay : int\n        Delay before closing valves in cleaner in ms (0-1000)\n    airgap : int\n        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)\n    airgap_speed : int\n        Speed of airgap aspiration in µL/s (1-1000)\n    retract_speed : int\n        Retract speed in mm/s (1-100)\n    fastwash : int\n        Use fast-wash module = 1, don't use it = 0\n    low_volume : int\n        Use pinch valves = 1, don't use them = 0\n    "
+            "Command for aspirating with the EvoWARE aspirate command. As many wells in one column may be selected as your liquid handling arm has pipettes.\n    This method generates the full command (as can be observed when opening a .esc file with an editor) and calls upon other functions to create the code string\n    specifying the target wells.\n\n    Parameters\n    ----------\n    tips : list\n        Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8\n    waste_location : tuple\n        Tuple with grid position (1-67) and site number (1-128) of waste as integers\n    cleaner_location : tuple\n        Tuple with grid position (1-67) and site number (1-128) of cleaner as integers\n    arm : int\n        number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2\n    waste_vol: float\n        Volume in waste in mL (0-100)\n    waste_delay : int\n        Delay before closing valves in waste in ms (0-1000)\n    cleaner_vol: float\n        Volume in cleaner in mL (0-100)\n    cleaner_delay : int\n        Delay before closing valves in cleaner in ms (0-1000)\n    airgap : int\n        Volume of airgap in µL which is aspirated after washing the tips (system trailing airgap) (0-100)\n    airgap_speed : int\n        Speed of airgap aspiration in µL/s (1-1000)\n    retract_speed : int\n        Retract speed in mm/s (1-100)\n    fastwash : int\n        Use fast-wash module = 1, don't use it = 0\n    low_volume : int\n        Use pinch valves = 1, don't use them = 0\n    "
             ('tips', 'waste_location', 'cleaner_location', 'arm', 'waste_vol', 'waste_delay', 'cleaner_vol', 'cleaner_delay', 'airgap', 'airgap_speed', 'retract_speed', 'fastwash', 'low_volume')
             0
             ''
             'B;Wash('
             ','
             1
             ',"'
@@ -2748,30 +2750,30 @@
             ()
          names      ('dict', 'prepare_evo_wash_parameters', 'value', 'join')
          varnames   ('tips', 'waste_location', 'cleaner_location', 'arm', 'waste_vol', 'waste_delay', 'cleaner_vol', 'cleaner_delay', 'airgap', 'airgap_speed', 'retract_speed', 'fastwash', 'low_volume', 'kwargs', 'tip_selection', 'tip')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
          name       'evo_wash'
-         firstlineno 522
+         firstlineno 530
          lnotab
             0x02320c0102010201020102010201020102010201020102010201020102
             f3121d16f204010201020102010201020102010201020102010201020102
             010203040108011601
-   names      ('__doc__', 'typing', 'List', 'Optional', 'Sequence', 'Tuple', 'Union', 'numpy', 'np', 'robotools.evotools.exceptions', 'InvalidOperationError', 'robotools.evotools.types', 'Tip', 'int_to_tip', 'robotools.evotools.utils', 'to_hex', '', 'transform', '__all__', 'int', 'ndarray', 'evo_make_selection_array', 'evo_get_selection', 'str', 'float', 'list', 'tuple', 'prepare_evo_aspirate_dispense_parameters', 'evo_aspirate', 'evo_dispense', 'prepare_evo_wash_parameters', 'evo_wash')
+   names      ('__doc__', 'typing', 'Iterable', 'List', 'Optional', 'Sequence', 'Tuple', 'Union', 'numpy', 'np', 'robotools.evotools.exceptions', 'InvalidOperationError', 'robotools.evotools.types', 'Tip', 'int_to_tip', 'robotools.evotools.utils', 'to_hex', '', 'transform', '__all__', 'int', 'str', 'ndarray', 'evo_make_selection_array', 'evo_get_selection', 'float', 'list', 'tuple', 'prepare_evo_aspirate_dispense_parameters', 'evo_aspirate', 'evo_dispense', 'prepare_evo_wash_parameters', 'evo_wash')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/robotools/robotools/robotools/evotools/commands.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104011c0208020c0110010c020c0204081e1b1e3702f906012a
-      ff020312fd020420fc020502fb02062afa02070ef9020818f80866020202
+      0x00ff02010401200208020c0110010c020c020408481b223702f906012a
+      ff020312fd020420fc020502fb02062afa02070ef9020818f8086a020202
       fe020302fd02041efc020512fb020620fa020702f902082af8020902f702
-      0a02f60849020202fe020302fd02041efc020512fb020620fa020702f902
-      082af8020902f7020a02f6084e0201020102010201020102010201020102
+      0a02f6084a020202fe020302fd02041efc020512fb020620fa020702f902
+      082af8020902f7020a02f6084f0201020102010201020102010201020102
       0102f206022afe020312fd020412fc020502fb020602fa020702f9020802
       f8020902f7020a02f6020b02f5020c02f4020d02f3020e02f2020f28f108
-      7f003902010201020102010201020102010201020102f206022afe020312
+      7f003b02010201020102010201020102010201020102f206022afe020312
       fd020412fc020502fb020602fa020702f9020802f8020902f7020a02f602
       0b02f5020c02f4020d02f3020e02f2020f02f1
```

### Comparing `robotools-1.6.1/robotools/evotools/__pycache__/exceptions.cpython-311.pyc` & `robotools-1.7.0/robotools/evotools/__pycache__/exceptions.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 149
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/evotools/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc` & `robotools-1.7.0/robotools/evotools/__pycache__/test_commands.cpython-311-pytest-7.3.2.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
-files sz: 19694
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
+files sz: 19722
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640064016c026d03630201006d045a05010064
@@ -353,69 +353,69 @@
                   00000001006e0b2300310073047702780359007701010059000100010074
                   01000000000000000000006a010000000000000000740400000000000000
                   000000640aac02a6020000ab020000000000000000350001007407000000
                   000000000000006403640b6702640c64056406640764086702ac09a60500
                   00ab0500000000000000000100640064006400a6020000ab020000000000
                   00000001006e0b2300310073047702780359007701010059000100010074
                   01000000000000000000006a010000000000000000740400000000000000
-                  000000640aac02a6020000ab020000000000000000350001007407000000
-                  000000000000006403640b6702640d64056406640764086702ac09a60500
+                  000000640dac02a6020000ab020000000000000000350001007407000000
+                  000000000000006403640b6702640e64056406640764086702ac09a60500
                   00ab0500000000000000000100640064006400a6020000ab020000000000
                   00000001006e0b2300310073047702780359007701010059000100010074
                   01000000000000000000006a010000000000000000740400000000000000
-                  000000640eac02a6020000ab020000000000000000350001007407000000
+                  000000640fac02a6020000ab020000000000000000350001007407000000
                   000000000000006403640b67026404640564066701640764086702ac09a6
                   050000ab0500000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007401000000000000000000006a01000000000000000074040000000000
-                  0000000000640eac02a6020000ab02000000000000000035000100740700
-                  0000000000000000006403640b670264046405640f640764086702ac09a6
+                  0000000000640fac02a6020000ab02000000000000000035000100740700
+                  0000000000000000006403640b6702640464056410640764086702ac09a6
                   050000ab0500000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007401000000000000000000006a01000000000000000074040000000000
-                  00000000006410ac02a6020000ab02000000000000000035000100740700
-                  0000000000000000006403640b6702640464056406640764116702ac09a6
+                  00000000006411ac02a6020000ab02000000000000000035000100740700
+                  0000000000000000006403640b6702640464056406640764126702ac09a6
                   050000ab0500000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007407000000000000000000006403640b67026404640564066407640867
                   02ac09a6050000ab0500000000000000005c0500007d017d017d017d017d
-                  02740900000000000000000000641284007c024400a6000000ab00000000
+                  02740900000000000000000000641384007c024400a6000000ab00000000
                   0000000000a6010000ab010000000000000000730f740b00000000000000
-                  0000006413a6010000ab0100000000000000008201740100000000000000
-                  0000006a0100000000000000007404000000000000000000006414ac02a6
+                  0000006414a6010000ab0100000000000000008201740100000000000000
+                  0000006a0100000000000000007404000000000000000000006415ac02a6
                   020000ab0200000000000000003500010074070000000000000000000064
-                  03640b6702640464156406640764086702ac09a6050000ab050000000000
+                  03640b6702640464166406640764086702ac09a6050000ab050000000000
                   0000000100640064006400a6020000ab02000000000000000001006e0b23
                   003100730477027803590077010100590001000100740100000000000000
-                  0000006a0100000000000000007404000000000000000000006414ac02a6
+                  0000006a0100000000000000007404000000000000000000006415ac02a6
                   020000ab0200000000000000003500010074070000000000000000000064
-                  03640b6702640464166406640764086702ac09a6050000ab050000000000
+                  03640b6702640464176406640764086702ac09a6050000ab050000000000
                   0000000100640064006400a6020000ab02000000000000000001006e0b23
                   003100730477027803590077010100590001000100740100000000000000
-                  0000006a0100000000000000007404000000000000000000006414ac02a6
+                  0000006a0100000000000000007404000000000000000000006415ac02a6
                   020000ab0200000000000000003500010074070000000000000000000064
-                  03640b6702640464176406640764086702ac09a6050000ab050000000000
+                  03640b6702640464186406640764086702ac09a6050000ab050000000000
                   0000000100640064006400a6020000ab02000000000000000001006e0b23
                   003100730477027803590077010100590001000100740700000000000000
-                  00000067006418a20164046419641a6700641ba201ac09a6050000ab0500
-                  000000000000007d0367006418a20164046700641ca201641a740c000000
+                  00000067006419a201641a641b641c6700641da201ac09a6050000ab0500
+                  000000000000007d0367006419a20164046700641ea201641c740c000000
                   000000000000006a070000000000000000740c000000000000000000006a
                   080000000000000000740c000000000000000000006a0900000000000000
                   00670366057d047c037c046b02000000007d057c0573c274150000000000
-                  00000000006a0b0000000000000000641d7c056601641e7c037c046602a6
-                  040000ab040000000000000000641f7419000000000000000000006a0d00
+                  00000000006a0b0000000000000000641f7c05660164207c037c046602a6
+                  040000ab04000000000000000064217419000000000000000000006a0d00
                   00000000000000a6000000ab000000000000000000760073147415000000
                   000000000000006a0e00000000000000007c03a6010000ab010000000000
                   00000072147415000000000000000000006a0f00000000000000007c03a6
-                  010000ab0100000000000000006e01641f64207419000000000000000000
+                  010000ab0100000000000000006e01642164227419000000000000000000
                   006a0d0000000000000000a6000000ab0000000000000000007600731474
                   15000000000000000000006a0e00000000000000007c04a6010000ab0100
                   0000000000000072147415000000000000000000006a0f00000000000000
-                  007c04a6010000ab0100000000000000006e01642064219c027a0600007d
-                  06642264237c0669017a0600007d07742100000000000000000000741500
+                  007c04a6010000ab0100000000000000006e01642264239c027a0600007d
+                  06642464257c0669017a0600007d07742100000000000000000000741500
                   0000000000000000006a1100000000000000007c07a6010000ab01000000
                   0000000000a6010000ab010000000000000000820164007d0564005300
                 42           0 RESUME                   0
                
                 44           2 LOAD_GLOBAL              1 (NULL + pytest)
                             14 LOAD_ATTR                1 (raises)
                             24 LOAD_GLOBAL              4 (ValueError)
@@ -463,28 +463,28 @@
                            142 POP_EXCEPT
                            144 POP_TOP
                            146 POP_TOP
                
                 53     >>  148 LOAD_GLOBAL              1 (NULL + pytest)
                            160 LOAD_ATTR                1 (raises)
                            170 LOAD_GLOBAL              4 (ValueError)
-                           182 LOAD_CONST              10 ('Invalid position:')
+                           182 LOAD_CONST              10 ('second number in labware_position')
                            184 KW_NAMES                 2
                            186 PRECALL                  2
                            190 CALL                     2
                            200 BEFORE_WITH
                            202 POP_TOP
                
                 54         204 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
                
                 55         216 LOAD_CONST               3 ('A01')
                            218 LOAD_CONST              11 ('B01')
                            220 BUILD_LIST               2
                
-                56         222 LOAD_CONST              12 ((38, -1))
+                56         222 LOAD_CONST              12 ((38, 0))
                
                 57         224 LOAD_CONST               5 (15)
                
                 58         226 LOAD_CONST               6 ('Water_DispZmax-1_AspZmax-1')
                
                 59         228 LOAD_CONST               7 (1)
                            230 LOAD_CONST               8 (2)
@@ -513,28 +513,28 @@
                            292 POP_EXCEPT
                            294 POP_TOP
                            296 POP_TOP
                
                 61     >>  298 LOAD_GLOBAL              1 (NULL + pytest)
                            310 LOAD_ATTR                1 (raises)
                            320 LOAD_GLOBAL              4 (ValueError)
-                           332 LOAD_CONST              10 ('Invalid position:')
+                           332 LOAD_CONST              13 ('first number in labware_position')
                            334 KW_NAMES                 2
                            336 PRECALL                  2
                            340 CALL                     2
                            350 BEFORE_WITH
                            352 POP_TOP
                
                 62         354 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
                
                 63         366 LOAD_CONST               3 ('A01')
                            368 LOAD_CONST              11 ('B01')
                            370 BUILD_LIST               2
                
-                64         372 LOAD_CONST              13 (('a', 2))
+                64         372 LOAD_CONST              14 (('a', 2))
                
                 65         374 LOAD_CONST               5 (15)
                
                 66         376 LOAD_CONST               6 ('Water_DispZmax-1_AspZmax-1')
                
                 67         378 LOAD_CONST               7 (1)
                            380 LOAD_CONST               8 (2)
@@ -563,15 +563,15 @@
                            442 POP_EXCEPT
                            444 POP_TOP
                            446 POP_TOP
                
                 70     >>  448 LOAD_GLOBAL              1 (NULL + pytest)
                            460 LOAD_ATTR                1 (raises)
                            470 LOAD_GLOBAL              4 (ValueError)
-                           482 LOAD_CONST              14 ('Invalid liquid_class:')
+                           482 LOAD_CONST              15 ('Invalid liquid_class:')
                            484 KW_NAMES                 2
                            486 PRECALL                  2
                            490 CALL                     2
                            500 BEFORE_WITH
                            502 POP_TOP
                
                 71         504 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
@@ -614,15 +614,15 @@
                            594 POP_EXCEPT
                            596 POP_TOP
                            598 POP_TOP
                
                 78     >>  600 LOAD_GLOBAL              1 (NULL + pytest)
                            612 LOAD_ATTR                1 (raises)
                            622 LOAD_GLOBAL              4 (ValueError)
-                           634 LOAD_CONST              14 ('Invalid liquid_class:')
+                           634 LOAD_CONST              15 ('Invalid liquid_class:')
                            636 KW_NAMES                 2
                            638 PRECALL                  2
                            642 CALL                     2
                            652 BEFORE_WITH
                            654 POP_TOP
                
                 79         656 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
@@ -631,15 +631,15 @@
                            670 LOAD_CONST              11 ('B01')
                            672 BUILD_LIST               2
                
                 81         674 LOAD_CONST               4 ((38, 2))
                
                 82         676 LOAD_CONST               5 (15)
                
-                83         678 LOAD_CONST              15 ('Water;DispZmax-1;AspZmax-1')
+                83         678 LOAD_CONST              16 ('Water;DispZmax-1;AspZmax-1')
                
                 84         680 LOAD_CONST               7 (1)
                            682 LOAD_CONST               8 (2)
                            684 BUILD_LIST               2
                
                 79         686 KW_NAMES                 9
                            688 PRECALL                  5
@@ -664,15 +664,15 @@
                            744 POP_EXCEPT
                            746 POP_TOP
                            748 POP_TOP
                
                 87     >>  750 LOAD_GLOBAL              1 (NULL + pytest)
                            762 LOAD_ATTR                1 (raises)
                            772 LOAD_GLOBAL              4 (ValueError)
-                           784 LOAD_CONST              16 ('Invalid type of tips:')
+                           784 LOAD_CONST              17 ('Invalid type of tips:')
                            786 KW_NAMES                 2
                            788 PRECALL                  2
                            792 CALL                     2
                            802 BEFORE_WITH
                            804 POP_TOP
                
                 88         806 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
@@ -684,15 +684,15 @@
                 90         824 LOAD_CONST               4 ((38, 2))
                
                 91         826 LOAD_CONST               5 (15)
                
                 92         828 LOAD_CONST               6 ('Water_DispZmax-1_AspZmax-1')
                
                 93         830 LOAD_CONST               7 (1)
-                           832 LOAD_CONST              17 ('2')
+                           832 LOAD_CONST              18 ('2')
                            834 BUILD_LIST               2
                
                 88         836 KW_NAMES                 9
                            838 PRECALL                  5
                            842 CALL                     5
                            852 POP_TOP
                
@@ -738,51 +738,51 @@
                            950 STORE_FAST               1 (_)
                            952 STORE_FAST               1 (_)
                            954 STORE_FAST               1 (_)
                            956 STORE_FAST               1 (_)
                            958 STORE_FAST               2 (tips)
                
                102         960 LOAD_GLOBAL              9 (NULL + all)
-                           972 LOAD_CONST              18 (<code object <genexpr>, file "/home/runner/work/robotools/robotools/robotools/evotools/test_commands.py", line 102>)
+                           972 LOAD_CONST              19 (<code object <genexpr>, file "/home/runner/work/robotools/robotools/robotools/evotools/test_commands.py", line 102>)
                            974 MAKE_FUNCTION            0
                            976 LOAD_FAST                2 (tips)
                            978 GET_ITER
                            980 PRECALL                  0
                            984 CALL                     0
                            994 PRECALL                  1
                            998 CALL                     1
                           1008 POP_JUMP_FORWARD_IF_TRUE    15 (to 1040)
                
                103        1010 LOAD_GLOBAL             11 (NULL + TypeError)
                
-               104        1022 LOAD_CONST              19 ('Even after completing the prepare_evo_aspirate_dispense_parameters method, not all tips are type Tip.')
+               104        1022 LOAD_CONST              20 ('Even after completing the prepare_evo_aspirate_dispense_parameters method, not all tips are type Tip.')
                
                103        1024 PRECALL                  1
                           1028 CALL                     1
                           1038 RAISE_VARARGS            1
                
                107     >> 1040 LOAD_GLOBAL              1 (NULL + pytest)
                           1052 LOAD_ATTR                1 (raises)
                           1062 LOAD_GLOBAL              4 (ValueError)
-                          1074 LOAD_CONST              20 ('Invalid volume:')
+                          1074 LOAD_CONST              21 ('Invalid volume:')
                           1076 KW_NAMES                 2
                           1078 PRECALL                  2
                           1082 CALL                     2
                           1092 BEFORE_WITH
                           1094 POP_TOP
                
                108        1096 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
                
                109        1108 LOAD_CONST               3 ('A01')
                           1110 LOAD_CONST              11 ('B01')
                           1112 BUILD_LIST               2
                
                110        1114 LOAD_CONST               4 ((38, 2))
                
-               111        1116 LOAD_CONST              21 ('volume')
+               111        1116 LOAD_CONST              22 ('volume')
                
                112        1118 LOAD_CONST               6 ('Water_DispZmax-1_AspZmax-1')
                
                113        1120 LOAD_CONST               7 (1)
                           1122 LOAD_CONST               8 (2)
                           1124 BUILD_LIST               2
                
@@ -809,30 +809,30 @@
                           1184 POP_EXCEPT
                           1186 POP_TOP
                           1188 POP_TOP
                
                115     >> 1190 LOAD_GLOBAL              1 (NULL + pytest)
                           1202 LOAD_ATTR                1 (raises)
                           1212 LOAD_GLOBAL              4 (ValueError)
-                          1224 LOAD_CONST              20 ('Invalid volume:')
+                          1224 LOAD_CONST              21 ('Invalid volume:')
                           1226 KW_NAMES                 2
                           1228 PRECALL                  2
                           1232 CALL                     2
                           1242 BEFORE_WITH
                           1244 POP_TOP
                
                116        1246 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
                
                117        1258 LOAD_CONST               3 ('A01')
                           1260 LOAD_CONST              11 ('B01')
                           1262 BUILD_LIST               2
                
                118        1264 LOAD_CONST               4 ((38, 2))
                
-               119        1266 LOAD_CONST              22 (-10)
+               119        1266 LOAD_CONST              23 (-10)
                
                120        1268 LOAD_CONST               6 ('Water_DispZmax-1_AspZmax-1')
                
                121        1270 LOAD_CONST               7 (1)
                           1272 LOAD_CONST               8 (2)
                           1274 BUILD_LIST               2
                
@@ -859,30 +859,30 @@
                           1334 POP_EXCEPT
                           1336 POP_TOP
                           1338 POP_TOP
                
                123     >> 1340 LOAD_GLOBAL              1 (NULL + pytest)
                           1352 LOAD_ATTR                1 (raises)
                           1362 LOAD_GLOBAL              4 (ValueError)
-                          1374 LOAD_CONST              20 ('Invalid volume:')
+                          1374 LOAD_CONST              21 ('Invalid volume:')
                           1376 KW_NAMES                 2
                           1378 PRECALL                  2
                           1382 CALL                     2
                           1392 BEFORE_WITH
                           1394 POP_TOP
                
                124        1396 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
                
                125        1408 LOAD_CONST               3 ('A01')
                           1410 LOAD_CONST              11 ('B01')
                           1412 BUILD_LIST               2
                
                126        1414 LOAD_CONST               4 ((38, 2))
                
-               127        1416 LOAD_CONST              23 (7158279)
+               127        1416 LOAD_CONST              24 (7158279)
                
                128        1418 LOAD_CONST               6 ('Water_DispZmax-1_AspZmax-1')
                
                129        1420 LOAD_CONST               7 (1)
                           1422 LOAD_CONST               8 (2)
                           1424 BUILD_LIST               2
                
@@ -909,43 +909,43 @@
                           1484 POP_EXCEPT
                           1486 POP_TOP
                           1488 POP_TOP
                
                133     >> 1490 LOAD_GLOBAL              7 (NULL + prepare_evo_aspirate_dispense_parameters)
                
                134        1502 BUILD_LIST               0
-                          1504 LOAD_CONST              24 (('E01', 'F01', 'G01'))
+                          1504 LOAD_CONST              25 (('E01', 'F01', 'G01'))
                           1506 LIST_EXTEND              1
                
-               135        1508 LOAD_CONST               4 ((38, 2))
+               135        1508 LOAD_CONST              26 ((38, 3))
                
-               136        1510 LOAD_CONST              25 (750)
+               136        1510 LOAD_CONST              27 (750)
                
-               137        1512 LOAD_CONST              26 ('Water_DispZmax_AspZmax')
+               137        1512 LOAD_CONST              28 ('Water_DispZmax_AspZmax')
                
                138        1514 BUILD_LIST               0
-                          1516 LOAD_CONST              27 ((5, 6, 7))
+                          1516 LOAD_CONST              29 ((5, 6, 7))
                           1518 LIST_EXTEND              1
                
                133        1520 KW_NAMES                 9
                           1522 PRECALL                  5
                           1526 CALL                     5
                           1536 STORE_FAST               3 (actual)
                
                141        1538 BUILD_LIST               0
-                          1540 LOAD_CONST              24 (('E01', 'F01', 'G01'))
+                          1540 LOAD_CONST              25 (('E01', 'F01', 'G01'))
                           1542 LIST_EXTEND              1
                
                142        1544 LOAD_CONST               4 ((38, 2))
                
                143        1546 BUILD_LIST               0
-                          1548 LOAD_CONST              28 ((750.0, 750.0, 750.0))
+                          1548 LOAD_CONST              30 ((750.0, 750.0, 750.0))
                           1550 LIST_EXTEND              1
                
-               144        1552 LOAD_CONST              26 ('Water_DispZmax_AspZmax')
+               144        1552 LOAD_CONST              28 ('Water_DispZmax_AspZmax')
                
                145        1554 LOAD_GLOBAL             12 (Tip)
                           1566 LOAD_ATTR                7 (T5)
                           1576 LOAD_GLOBAL             12 (Tip)
                           1588 LOAD_ATTR                8 (T6)
                           1598 LOAD_GLOBAL             12 (Tip)
                           1610 LOAD_ATTR                9 (T7)
@@ -958,24 +958,24 @@
                           1628 LOAD_FAST                4 (expected)
                           1630 COMPARE_OP               2 (==)
                           1636 STORE_FAST               5 (@py_assert1)
                           1638 LOAD_FAST                5 (@py_assert1)
                           1640 POP_JUMP_FORWARD_IF_TRUE   194 (to 2030)
                           1642 LOAD_GLOBAL             21 (NULL + @pytest_ar)
                           1654 LOAD_ATTR               11 (_call_reprcompare)
-                          1664 LOAD_CONST              29 (('==',))
+                          1664 LOAD_CONST              31 (('==',))
                           1666 LOAD_FAST                5 (@py_assert1)
                           1668 BUILD_TUPLE              1
-                          1670 LOAD_CONST              30 (('%(py0)s == %(py2)s',))
+                          1670 LOAD_CONST              32 (('%(py0)s == %(py2)s',))
                           1672 LOAD_FAST                3 (actual)
                           1674 LOAD_FAST                4 (expected)
                           1676 BUILD_TUPLE              2
                           1678 PRECALL                  4
                           1682 CALL                     4
-                          1692 LOAD_CONST              31 ('actual')
+                          1692 LOAD_CONST              33 ('actual')
                           1694 LOAD_GLOBAL             25 (NULL + @py_builtins)
                           1706 LOAD_ATTR               13 (locals)
                           1716 PRECALL                  0
                           1720 CALL                     0
                           1730 CONTAINS_OP              0
                           1732 POP_JUMP_FORWARD_IF_TRUE    20 (to 1774)
                           1734 LOAD_GLOBAL             21 (NULL + @pytest_ar)
@@ -986,16 +986,16 @@
                           1772 POP_JUMP_FORWARD_IF_FALSE    20 (to 1814)
                        >> 1774 LOAD_GLOBAL             21 (NULL + @pytest_ar)
                           1786 LOAD_ATTR               15 (_saferepr)
                           1796 LOAD_FAST                3 (actual)
                           1798 PRECALL                  1
                           1802 CALL                     1
                           1812 JUMP_FORWARD             1 (to 1816)
-                       >> 1814 LOAD_CONST              31 ('actual')
-                       >> 1816 LOAD_CONST              32 ('expected')
+                       >> 1814 LOAD_CONST              33 ('actual')
+                       >> 1816 LOAD_CONST              34 ('expected')
                           1818 LOAD_GLOBAL             25 (NULL + @py_builtins)
                           1830 LOAD_ATTR               13 (locals)
                           1840 PRECALL                  0
                           1844 CALL                     0
                           1854 CONTAINS_OP              0
                           1856 POP_JUMP_FORWARD_IF_TRUE    20 (to 1898)
                           1858 LOAD_GLOBAL             21 (NULL + @pytest_ar)
@@ -1006,21 +1006,21 @@
                           1896 POP_JUMP_FORWARD_IF_FALSE    20 (to 1938)
                        >> 1898 LOAD_GLOBAL             21 (NULL + @pytest_ar)
                           1910 LOAD_ATTR               15 (_saferepr)
                           1920 LOAD_FAST                4 (expected)
                           1922 PRECALL                  1
                           1926 CALL                     1
                           1936 JUMP_FORWARD             1 (to 1940)
-                       >> 1938 LOAD_CONST              32 ('expected')
-                       >> 1940 LOAD_CONST              33 (('py0', 'py2'))
+                       >> 1938 LOAD_CONST              34 ('expected')
+                       >> 1940 LOAD_CONST              35 (('py0', 'py2'))
                           1942 BUILD_CONST_KEY_MAP      2
                           1944 BINARY_OP                6 (%)
                           1948 STORE_FAST               6 (@py_format3)
-                          1950 LOAD_CONST              34 ('assert %(py4)s')
-                          1952 LOAD_CONST              35 ('py4')
+                          1950 LOAD_CONST              36 ('assert %(py4)s')
+                          1952 LOAD_CONST              37 ('py4')
                           1954 LOAD_FAST                6 (@py_format3)
                           1956 BUILD_MAP                1
                           1958 BINARY_OP                6 (%)
                           1962 STORE_FAST               7 (@py_format5)
                           1964 LOAD_GLOBAL             33 (NULL + AssertionError)
                           1976 LOAD_GLOBAL             21 (NULL + @pytest_ar)
                           1988 LOAD_ATTR               17 (_format_explanation)
@@ -1069,17 +1069,18 @@
                   'A01'
                   (38, 2)
                   15
                   'Water_DispZmax-1_AspZmax-1'
                   1
                   2
                   ('wells', 'labware_position', 'volume', 'liquid_class', 'tips')
-                  'Invalid position:'
+                  'second number in labware_position'
                   'B01'
-                  (38, -1)
+                  (38, 0)
+                  'first number in labware_position'
                   ('a', 2)
                   'Invalid liquid_class:'
                   'Water;DispZmax-1;AspZmax-1'
                   'Invalid type of tips:'
                   '2'
                   code
                      argcount  : 1
@@ -1119,14 +1120,15 @@
                      lnotab 0x
                   'Even after completing the prepare_evo_aspirate_dispense_parameters method, not all tips are type Tip.'
                   'Invalid volume:'
                   'volume'
                   -10
                   7158279
                   ('E01', 'F01', 'G01')
+                  (38, 3)
                   750
                   'Water_DispZmax_AspZmax'
                   (5, 6, 7)
                   (750.0, 750.0, 750.0)
                   ('==',)
                   ('%(py0)s == %(py2)s',)
                   'actual'
@@ -1219,15 +1221,15 @@
                
                154          16 LOAD_CONST               2 (12)
                
                155          18 BUILD_LIST               0
                             20 LOAD_CONST               3 (('E01', 'F01', 'G01'))
                             22 LIST_EXTEND              1
                
-               156          24 LOAD_CONST               4 ((38, 2))
+               156          24 LOAD_CONST               4 ((38, 3))
                
                157          26 BUILD_LIST               0
                             28 LOAD_CONST               5 ((5, 6, 7))
                             30 LIST_EXTEND              1
                
                158          32 LOAD_CONST               6 (750)
                
@@ -1325,15 +1327,15 @@
                164         468 LOAD_CONST               0 (None)
                            470 RETURN_VALUE
                consts
                   None
                   8
                   12
                   ('E01', 'F01', 'G01')
-                  (38, 2)
+                  (38, 3)
                   (5, 6, 7)
                   750
                   'Water_DispZmax_AspZmax'
                   950
                   ('n_rows', 'n_columns', 'wells', 'labware_position', 'tips', 'volume', 'liquid_class', 'max_volume')
                   'B;Aspirate(112,"Water_DispZmax_AspZmax",0,0,0,0,"750.0","750.0","750.0",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
                   ('==',)
@@ -1381,15 +1383,15 @@
                
                169          16 LOAD_CONST               2 (12)
                
                170          18 BUILD_LIST               0
                             20 LOAD_CONST               3 (('E01', 'F01', 'G01'))
                             22 LIST_EXTEND              1
                
-               171          24 LOAD_CONST               4 ((38, 2))
+               171          24 LOAD_CONST               4 ((38, 3))
                
                172          26 BUILD_LIST               0
                             28 LOAD_CONST               5 ((5, 6, 7))
                             30 LIST_EXTEND              1
                
                173          32 BUILD_LIST               0
                             34 LOAD_CONST               6 ((750, 730, 710))
@@ -1489,15 +1491,15 @@
                179         472 LOAD_CONST               0 (None)
                            474 RETURN_VALUE
                consts
                   None
                   8
                   12
                   ('E01', 'F01', 'G01')
-                  (38, 2)
+                  (38, 3)
                   (5, 6, 7)
                   (750, 730, 710)
                   'Water_DispZmax_AspZmax'
                   950
                   ('n_rows', 'n_columns', 'wells', 'labware_position', 'tips', 'volume', 'liquid_class', 'max_volume')
                   'B;Aspirate(112,"Water_DispZmax_AspZmax",0,0,0,0,"750","730","710",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
                   ('==',)
@@ -1584,15 +1586,15 @@
                
                186          16 LOAD_CONST               2 (12)
                
                187          18 BUILD_LIST               0
                             20 LOAD_CONST               3 (('E01', 'F01', 'G01'))
                             22 LIST_EXTEND              1
                
-               188          24 LOAD_CONST               4 ((38, 2))
+               188          24 LOAD_CONST               4 ((38, 3))
                
                189          26 BUILD_LIST               0
                             28 LOAD_CONST               5 ((5, 6, 7))
                             30 LIST_EXTEND              1
                
                190          32 LOAD_CONST               6 (750)
                
@@ -1690,15 +1692,15 @@
                196         468 LOAD_CONST               0 (None)
                            470 RETURN_VALUE
                consts
                   None
                   8
                   12
                   ('E01', 'F01', 'G01')
-                  (38, 2)
+                  (38, 3)
                   (5, 6, 7)
                   750
                   'Water_DispZmax_AspZmax'
                   950
                   ('n_rows', 'n_columns', 'wells', 'labware_position', 'tips', 'volume', 'liquid_class', 'max_volume')
                   'B;Dispense(112,"Water_DispZmax_AspZmax",0,0,0,0,"750.0","750.0","750.0",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
                   ('==',)
@@ -1746,15 +1748,15 @@
                
                201          16 LOAD_CONST               2 (12)
                
                202          18 BUILD_LIST               0
                             20 LOAD_CONST               3 (('E01', 'F01', 'G01'))
                             22 LIST_EXTEND              1
                
-               203          24 LOAD_CONST               4 ((38, 2))
+               203          24 LOAD_CONST               4 ((38, 3))
                
                204          26 BUILD_LIST               0
                             28 LOAD_CONST               5 ((5, 6, 7))
                             30 LIST_EXTEND              1
                
                205          32 BUILD_LIST               0
                             34 LOAD_CONST               6 ((750, 730, 710))
@@ -1854,15 +1856,15 @@
                211         472 LOAD_CONST               0 (None)
                            474 RETURN_VALUE
                consts
                   None
                   8
                   12
                   ('E01', 'F01', 'G01')
-                  (38, 2)
+                  (38, 3)
                   (5, 6, 7)
                   (750, 730, 710)
                   'Water_DispZmax_AspZmax'
                   950
                   ('n_rows', 'n_columns', 'wells', 'labware_position', 'tips', 'volume', 'liquid_class', 'max_volume')
                   'B;Dispense(112,"Water_DispZmax_AspZmax",0,0,0,0,"750","730","710",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
                   ('==',)
@@ -1951,199 +1953,199 @@
                   003100730477027803590077010100590001000100740700000000000000
                   0000006a040000000000000000740a00000000000000000000640dac09a6
                   020000ab0200000000000000003500010074010000000000000000000064
                   016402670264106404ac05a6030000ab0300000000000000000100640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007407000000000000000000006a04000000
                   0000000000740a000000000000000000006411ac09a6020000ab02000000
-                  000000000035000100740100000000000000000000640164026702640364
-                  0aac05a6030000ab0300000000000000000100640064006400a6020000ab
+                  000000000035000100740100000000000000000000640164026702640464
+                  12ac05a6030000ab0300000000000000000100640064006400a6020000ab
                   02000000000000000001006e0b2300310073047702780359007701010059
                   00010001007407000000000000000000006a040000000000000000740a00
                   0000000000000000006411ac09a6020000ab020000000000000000350001
-                  007401000000000000000000006401640267026403640bac05a6030000ab
+                  0074010000000000000000000064016402670264046413ac05a6030000ab
                   0300000000000000000100640064006400a6020000ab0200000000000000
                   0001006e0b23003100730477027803590077010100590001000100740700
                   0000000000000000006a040000000000000000740a000000000000000000
                   006411ac09a6020000ab0200000000000000003500010074010000000000
-                  00000000006401640267026403640cac05a6030000ab0300000000000000
+                  000000000064016402670264046414ac05a6030000ab0300000000000000
                   000100640064006400a6020000ab02000000000000000001006e0b230031
                   007304770278035900770101005900010001007407000000000000000000
-                  006a040000000000000000740a000000000000000000006412ac09a60200
+                  006a040000000000000000740a000000000000000000006415ac09a60200
                   00ab02000000000000000035000100740100000000000000000000640164
-                  0267026403640eac05a6030000ab03000000000000000001006400640064
+                  0267026404640eac05a6030000ab03000000000000000001006400640064
                   00a6020000ab02000000000000000001006e0b2300310073047702780359
                   00770101005900010001007407000000000000000000006a040000000000
-                  000000740a000000000000000000006412ac09a6020000ab020000000000
-                  000000350001007401000000000000000000006401640267026403640fac
+                  000000740a000000000000000000006415ac09a6020000ab020000000000
+                  000000350001007401000000000000000000006401640267026404640fac
                   05a6030000ab0300000000000000000100640064006400a6020000ab0200
                   0000000000000001006e0b23003100730477027803590077010100590001
                   0001007407000000000000000000006a040000000000000000740a000000
-                  000000000000006412ac09a6020000ab0200000000000000003500010074
-                  010000000000000000000064016402670264036410ac05a6030000ab0300
+                  000000000000006415ac09a6020000ab0200000000000000003500010074
+                  010000000000000000000064016402670264046410ac05a6030000ab0300
                   000000000000000100640064006400a6020000ab02000000000000000001
                   006e0b230031007304770278035900770101005900010001007407000000
                   000000000000006a040000000000000000740a0000000000000000000064
-                  13ac09a6020000ab02000000000000000035000100740100000000000000
-                  000000640164026702640364046402ac14a6040000ab0400000000000000
+                  16ac09a6020000ab02000000000000000035000100740100000000000000
+                  000000640164026702640364046402ac17a6040000ab0400000000000000
                   000100640064006400a6020000ab02000000000000000001006e0b230031
                   007304770278035900770101005900010001007407000000000000000000
-                  006a040000000000000000740a000000000000000000006415ac09a60200
+                  006a040000000000000000740a000000000000000000006418ac09a60200
                   00ab02000000000000000035000100740100000000000000000000640164
-                  026702640364046416ac17a6040000ab0400000000000000000100640064
+                  026702640364046419ac1aa6040000ab0400000000000000000100640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007407000000000000000000006a04000000
-                  0000000000740a000000000000000000006415ac09a6020000ab02000000
+                  0000000000740a000000000000000000006418ac09a6020000ab02000000
                   000000000035000100740100000000000000000000640164026702640364
-                  046418ac17a6040000ab0400000000000000000100640064006400a60200
+                  04641bac1aa6040000ab0400000000000000000100640064006400a60200
                   00ab02000000000000000001006e0b230031007304770278035900770101
                   005900010001007407000000000000000000006a04000000000000000074
-                  0a000000000000000000006415ac09a6020000ab02000000000000000035
-                  000100740100000000000000000000640164026702640364046401ac17a6
+                  0a000000000000000000006418ac09a6020000ab02000000000000000035
+                  000100740100000000000000000000640164026702640364046401ac1aa6
                   040000ab0400000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007407000000000000000000006a040000000000000000740a0000000000
-                  00000000006419ac09a6020000ab02000000000000000035000100740100
-                  00000000000000000064016402670264036404641aac1ba6040000ab0400
+                  0000000000641cac09a6020000ab02000000000000000035000100740100
+                  00000000000000000064016402670264036404641dac1ea6040000ab0400
                   000000000000000100640064006400a6020000ab02000000000000000001
                   006e0b230031007304770278035900770101005900010001007407000000
                   000000000000006a040000000000000000740a0000000000000000000064
-                  19ac09a6020000ab02000000000000000035000100740100000000000000
-                  00000064016402670264036404641cac1ba6040000ab0400000000000000
+                  1cac09a6020000ab02000000000000000035000100740100000000000000
+                  00000064016402670264036404641fac1ea6040000ab0400000000000000
                   000100640064006400a6020000ab02000000000000000001006e0b230031
                   007304770278035900770101005900010001007407000000000000000000
-                  006a040000000000000000740a000000000000000000006419ac09a60200
+                  006a040000000000000000740a00000000000000000000641cac09a60200
                   00ab02000000000000000035000100740100000000000000000000640164
-                  02670264036404641dac1ba6040000ab0400000000000000000100640064
+                  026702640364046420ac1ea6040000ab0400000000000000000100640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007407000000000000000000006a04000000
-                  0000000000740a00000000000000000000641eac09a6020000ab02000000
+                  0000000000740a000000000000000000006421ac09a6020000ab02000000
                   000000000035000100740100000000000000000000640164026702640364
-                  046416ac1fa6040000ab0400000000000000000100640064006400a60200
+                  046419ac22a6040000ab0400000000000000000100640064006400a60200
                   00ab02000000000000000001006e0b230031007304770278035900770101
                   005900010001007407000000000000000000006a04000000000000000074
-                  0a00000000000000000000641eac09a6020000ab02000000000000000035
-                  000100740100000000000000000000640164026702640364046418ac1fa6
+                  0a000000000000000000006421ac09a6020000ab02000000000000000035
+                  00010074010000000000000000000064016402670264036404641bac22a6
                   040000ab0400000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007407000000000000000000006a040000000000000000740a0000000000
-                  0000000000641eac09a6020000ab02000000000000000035000100740100
-                  000000000000000000640164026702640364046401ac1fa6040000ab0400
+                  00000000006421ac09a6020000ab02000000000000000035000100740100
+                  000000000000000000640164026702640364046401ac22a6040000ab0400
                   000000000000000100640064006400a6020000ab02000000000000000001
                   006e0b230031007304770278035900770101005900010001007407000000
                   000000000000006a040000000000000000740a0000000000000000000064
-                  20ac09a6020000ab02000000000000000035000100740100000000000000
-                  00000064016402670264036404641aac21a6040000ab0400000000000000
+                  23ac09a6020000ab02000000000000000035000100740100000000000000
+                  00000064016402670264036404641dac24a6040000ab0400000000000000
                   000100640064006400a6020000ab02000000000000000001006e0b230031
                   007304770278035900770101005900010001007407000000000000000000
-                  006a040000000000000000740a000000000000000000006420ac09a60200
+                  006a040000000000000000740a000000000000000000006423ac09a60200
                   00ab02000000000000000035000100740100000000000000000000640164
-                  02670264036404641cac21a6040000ab0400000000000000000100640064
+                  02670264036404641fac24a6040000ab0400000000000000000100640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007407000000000000000000006a04000000
-                  0000000000740a000000000000000000006420ac09a6020000ab02000000
+                  0000000000740a000000000000000000006423ac09a6020000ab02000000
                   000000000035000100740100000000000000000000640164026702640364
-                  04641dac21a6040000ab0400000000000000000100640064006400a60200
+                  046420ac24a6040000ab0400000000000000000100640064006400a60200
                   00ab02000000000000000001006e0b230031007304770278035900770101
                   005900010001007407000000000000000000006a04000000000000000074
-                  0a000000000000000000006422ac09a6020000ab02000000000000000035
-                  00010074010000000000000000000064016402670264036404641aac23a6
+                  0a000000000000000000006425ac09a6020000ab02000000000000000035
+                  00010074010000000000000000000064016402670264036404641dac26a6
                   040000ab0400000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007407000000000000000000006a040000000000000000740a0000000000
-                  00000000006422ac09a6020000ab02000000000000000035000100740100
-                  000000000000000000640164026702640364046424ac23a6040000ab0400
+                  00000000006425ac09a6020000ab02000000000000000035000100740100
+                  000000000000000000640164026702640364046427ac26a6040000ab0400
                   000000000000000100640064006400a6020000ab02000000000000000001
                   006e0b230031007304770278035900770101005900010001007407000000
                   000000000000006a040000000000000000740a0000000000000000000064
-                  22ac09a6020000ab02000000000000000035000100740100000000000000
-                  00000064016402670264036404641dac23a6040000ab0400000000000000
+                  25ac09a6020000ab02000000000000000035000100740100000000000000
+                  000000640164026702640364046420ac26a6040000ab0400000000000000
                   000100640064006400a6020000ab02000000000000000001006e0b230031
                   007304770278035900770101005900010001007407000000000000000000
-                  006a040000000000000000740a000000000000000000006425ac09a60200
+                  006a040000000000000000740a000000000000000000006428ac09a60200
                   00ab02000000000000000035000100740100000000000000000000640164
-                  026702640364046426ac27a6040000ab0400000000000000000100640064
+                  026702640364046429ac2aa6040000ab0400000000000000000100640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007407000000000000000000006a04000000
-                  0000000000740a000000000000000000006425ac09a6020000ab02000000
+                  0000000000740a000000000000000000006428ac09a6020000ab02000000
                   000000000035000100740100000000000000000000640164026702640364
-                  04641cac27a6040000ab0400000000000000000100640064006400a60200
+                  04641fac2aa6040000ab0400000000000000000100640064006400a60200
                   00ab02000000000000000001006e0b230031007304770278035900770101
                   005900010001007407000000000000000000006a04000000000000000074
-                  0a000000000000000000006425ac09a6020000ab02000000000000000035
-                  00010074010000000000000000000064016402670264036404641dac27a6
+                  0a000000000000000000006428ac09a6020000ab02000000000000000035
+                  000100740100000000000000000000640164026702640364046420ac2aa6
                   040000ab0400000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007407000000000000000000006a040000000000000000740a0000000000
-                  00000000006428ac09a6020000ab02000000000000000035000100740100
-                  000000000000000000640164026702640364046426ac29a6040000ab0400
+                  0000000000642bac09a6020000ab02000000000000000035000100740100
+                  000000000000000000640164026702640364046429ac2ca6040000ab0400
                   000000000000000100640064006400a6020000ab02000000000000000001
                   006e0b230031007304770278035900770101005900010001007407000000
                   000000000000006a040000000000000000740a0000000000000000000064
-                  28ac09a6020000ab02000000000000000035000100740100000000000000
-                  000000640164026702640364046424ac29a6040000ab0400000000000000
+                  2bac09a6020000ab02000000000000000035000100740100000000000000
+                  000000640164026702640364046427ac2ca6040000ab0400000000000000
                   000100640064006400a6020000ab02000000000000000001006e0b230031
                   007304770278035900770101005900010001007407000000000000000000
-                  006a040000000000000000740a000000000000000000006428ac09a60200
+                  006a040000000000000000740a00000000000000000000642bac09a60200
                   00ab02000000000000000035000100740100000000000000000000640164
-                  02670264036404641dac29a6040000ab0400000000000000000100640064
+                  026702640364046420ac2ca6040000ab0400000000000000000100640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007407000000000000000000006a04000000
-                  0000000000740a00000000000000000000642aac09a6020000ab02000000
+                  0000000000740a00000000000000000000642dac09a6020000ab02000000
                   000000000035000100740100000000000000000000640164026702640364
-                  046402ac2ba6040000ab0400000000000000000100640064006400a60200
+                  046402ac2ea6040000ab0400000000000000000100640064006400a60200
                   00ab02000000000000000001006e0b230031007304770278035900770101
                   005900010001007407000000000000000000006a04000000000000000074
-                  0a00000000000000000000642aac09a6020000ab02000000000000000035
-                  00010074010000000000000000000064016402670264036404642cac2ba6
+                  0a00000000000000000000642dac09a6020000ab02000000000000000035
+                  00010074010000000000000000000064016402670264036404642fac2ea6
                   040000ab0400000000000000000100640064006400a6020000ab02000000
                   000000000001006e0b230031007304770278035900770101005900010001
                   007407000000000000000000006a040000000000000000740a0000000000
-                  0000000000642dac09a6020000ab02000000000000000035000100740100
-                  000000000000000000640164026702640364046402ac2ea6040000ab0400
+                  00000000006430ac09a6020000ab02000000000000000035000100740100
+                  000000000000000000640164026702640364046402ac31a6040000ab0400
                   000000000000000100640064006400a6020000ab02000000000000000001
                   006e0b230031007304770278035900770101005900010001007407000000
                   000000000000006a040000000000000000740a0000000000000000000064
-                  2dac09a6020000ab02000000000000000035000100740100000000000000
-                  00000064016402670264036404642cac2ea6040000ab0400000000000000
+                  30ac09a6020000ab02000000000000000035000100740100000000000000
+                  00000064016402670264036404642fac31a6040000ab0400000000000000
                   000100640064006400a6020000ab02000000000000000001006e0b230031
                   007304770278035900770101005900010001007401000000000000000000
-                  006700642fa20164036404ac05a6030000ab0300000000000000007d0374
+                  0067006432a20164036404ac05a6030000ab0300000000000000007d0374
                   0c000000000000000000006a070000000000000000740c00000000000000
                   0000006a080000000000000000740c000000000000000000006a09000000
                   0000000000740c000000000000000000006a0a0000000000000000740c00
                   0000000000000000006a0b0000000000000000740c000000000000000000
                   006a0c0000000000000000740c000000000000000000006a0d0000000000
-                  000000740c000000000000000000006a0e00000000000000006708640364
-                  046426643064316432643164336434643564016426660d7d047c037c046b
+                  000000740c000000000000000000006a0e00000000000000006708640464
+                  0e6429643364346435643464366437643864016429660d7d047c037c046b
                   02000000007d057c0573c2741f000000000000000000006a100000000000
-                  00000064367c05660164377c037c046602a6040000ab0400000000000000
-                  0064387423000000000000000000006a120000000000000000a6000000ab
+                  00000064397c056601643a7c037c046602a6040000ab0400000000000000
+                  00643b7423000000000000000000006a120000000000000000a6000000ab
                   00000000000000000076007314741f000000000000000000006a13000000
                   00000000007c03a6010000ab0100000000000000007214741f0000000000
                   00000000006a1400000000000000007c03a6010000ab0100000000000000
-                  006e01643864397423000000000000000000006a120000000000000000a6
+                  006e01643b643c7423000000000000000000006a120000000000000000a6
                   000000ab00000000000000000076007314741f000000000000000000006a
                   1300000000000000007c04a6010000ab0100000000000000007214741f00
                   0000000000000000006a1400000000000000007c04a6010000ab01000000
-                  00000000006e016439643a9c027a0600007d06643b643c7c0669017a0600
+                  00000000006e01643c643d9c027a0600007d06643e643f7c0669017a0600
                   007d07742b00000000000000000000741f000000000000000000006a1600
                   000000000000007c07a6010000ab010000000000000000a6010000ab0100
                   00000000000000820164007d0564005300
                215           0 RESUME                   0
                
                217           2 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                218          14 LOAD_CONST               1 (1)
                             16 LOAD_CONST               2 (2)
                             18 BUILD_LIST               2
                
-               219          20 LOAD_CONST               3 ((52, 1))
+               219          20 LOAD_CONST               3 ((52, 2))
                
-               220          22 LOAD_CONST               4 ((52, 0))
+               220          22 LOAD_CONST               4 ((52, 1))
                
                217          24 KW_NAMES                 5
                             26 PRECALL                  3
                             30 CALL                     3
                             40 UNPACK_SEQUENCE         13
                             44 STORE_FAST               1 (tips)
                             46 STORE_FAST               2 (_)
@@ -2190,17 +2192,17 @@
                
                229         206 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                230         218 LOAD_CONST               1 (1)
                            220 LOAD_CONST               2 (2)
                            222 BUILD_LIST               2
                
-               231         224 LOAD_CONST              10 ((68, 1))
+               231         224 LOAD_CONST              10 ((68, 2))
                
-               232         226 LOAD_CONST               4 ((52, 0))
+               232         226 LOAD_CONST               4 ((52, 1))
                
                229         228 KW_NAMES                 5
                            230 PRECALL                  3
                            234 CALL                     3
                            244 POP_TOP
                
                228         246 LOAD_CONST               0 (None)
@@ -2234,17 +2236,17 @@
                
                235         348 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                236         360 LOAD_CONST               1 (1)
                            362 LOAD_CONST               2 (2)
                            364 BUILD_LIST               2
                
-               237         366 LOAD_CONST              11 ((0, 1))
+               237         366 LOAD_CONST              11 ((0, 2))
                
-               238         368 LOAD_CONST               4 ((52, 0))
+               238         368 LOAD_CONST               4 ((52, 1))
                
                235         370 KW_NAMES                 5
                            372 PRECALL                  3
                            376 CALL                     3
                            386 POP_TOP
                
                234         388 LOAD_CONST               0 (None)
@@ -2278,17 +2280,17 @@
                
                241         490 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                242         502 LOAD_CONST               1 (1)
                            504 LOAD_CONST               2 (2)
                            506 BUILD_LIST               2
                
-               243         508 LOAD_CONST              12 ((1.7, 1))
+               243         508 LOAD_CONST              12 ((1.7, 2))
                
-               244         510 LOAD_CONST               4 ((52, 0))
+               244         510 LOAD_CONST               4 ((52, 1))
                
                241         512 KW_NAMES                 5
                            514 PRECALL                  3
                            518 CALL                     3
                            528 POP_TOP
                
                240         530 LOAD_CONST               0 (None)
@@ -2322,17 +2324,17 @@
                
                247         632 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                248         644 LOAD_CONST               1 (1)
                            646 LOAD_CONST               2 (2)
                            648 BUILD_LIST               2
                
-               249         650 LOAD_CONST              14 ((52, -1))
+               249         650 LOAD_CONST              14 ((52, 0))
                
-               250         652 LOAD_CONST               4 ((52, 0))
+               250         652 LOAD_CONST               4 ((52, 1))
                
                247         654 KW_NAMES                 5
                            656 PRECALL                  3
                            660 CALL                     3
                            670 POP_TOP
                
                246         672 LOAD_CONST               0 (None)
@@ -2366,17 +2368,17 @@
                
                253         774 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                254         786 LOAD_CONST               1 (1)
                            788 LOAD_CONST               2 (2)
                            790 BUILD_LIST               2
                
-               255         792 LOAD_CONST              15 ((52, 128))
+               255         792 LOAD_CONST              15 ((52, 129))
                
-               256         794 LOAD_CONST               4 ((52, 0))
+               256         794 LOAD_CONST               4 ((52, 1))
                
                253         796 KW_NAMES                 5
                            798 PRECALL                  3
                            802 CALL                     3
                            812 POP_TOP
                
                252         814 LOAD_CONST               0 (None)
@@ -2412,15 +2414,15 @@
                
                260         928 LOAD_CONST               1 (1)
                            930 LOAD_CONST               2 (2)
                            932 BUILD_LIST               2
                
                261         934 LOAD_CONST              16 ((52, 1.7))
                
-               262         936 LOAD_CONST               4 ((52, 0))
+               262         936 LOAD_CONST               4 ((52, 1))
                
                259         938 KW_NAMES                 5
                            940 PRECALL                  3
                            944 CALL                     3
                            954 POP_TOP
                
                258         956 LOAD_CONST               0 (None)
@@ -2454,17 +2456,17 @@
                
                267        1058 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                268        1070 LOAD_CONST               1 (1)
                           1072 LOAD_CONST               2 (2)
                           1074 BUILD_LIST               2
                
-               269        1076 LOAD_CONST               3 ((52, 1))
+               269        1076 LOAD_CONST               4 ((52, 1))
                
-               270        1078 LOAD_CONST              10 ((68, 1))
+               270        1078 LOAD_CONST              18 ((68, 1))
                
                267        1080 KW_NAMES                 5
                           1082 PRECALL                  3
                           1086 CALL                     3
                           1096 POP_TOP
                
                266        1098 LOAD_CONST               0 (None)
@@ -2498,17 +2500,17 @@
                
                273        1200 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                274        1212 LOAD_CONST               1 (1)
                           1214 LOAD_CONST               2 (2)
                           1216 BUILD_LIST               2
                
-               275        1218 LOAD_CONST               3 ((52, 1))
+               275        1218 LOAD_CONST               4 ((52, 1))
                
-               276        1220 LOAD_CONST              11 ((0, 1))
+               276        1220 LOAD_CONST              19 ((0, 1))
                
                273        1222 KW_NAMES                 5
                           1224 PRECALL                  3
                           1228 CALL                     3
                           1238 POP_TOP
                
                272        1240 LOAD_CONST               0 (None)
@@ -2542,17 +2544,17 @@
                
                279        1342 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                280        1354 LOAD_CONST               1 (1)
                           1356 LOAD_CONST               2 (2)
                           1358 BUILD_LIST               2
                
-               281        1360 LOAD_CONST               3 ((52, 1))
+               281        1360 LOAD_CONST               4 ((52, 1))
                
-               282        1362 LOAD_CONST              12 ((1.7, 1))
+               282        1362 LOAD_CONST              20 ((1.7, 1))
                
                279        1364 KW_NAMES                 5
                           1366 PRECALL                  3
                           1370 CALL                     3
                           1380 POP_TOP
                
                278        1382 LOAD_CONST               0 (None)
@@ -2573,30 +2575,30 @@
                           1422 POP_EXCEPT
                           1424 POP_TOP
                           1426 POP_TOP
                
                284     >> 1428 LOAD_GLOBAL              7 (NULL + pytest)
                           1440 LOAD_ATTR                4 (raises)
                           1450 LOAD_GLOBAL             10 (ValueError)
-                          1462 LOAD_CONST              18 ('Site \\(second number in cleaner_location tuple\\)')
+                          1462 LOAD_CONST              21 ('Site \\(second number in cleaner_location tuple\\)')
                           1464 KW_NAMES                 9
                           1466 PRECALL                  2
                           1470 CALL                     2
                           1480 BEFORE_WITH
                           1482 POP_TOP
                
                285        1484 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                286        1496 LOAD_CONST               1 (1)
                           1498 LOAD_CONST               2 (2)
                           1500 BUILD_LIST               2
                
-               287        1502 LOAD_CONST               3 ((52, 1))
+               287        1502 LOAD_CONST               4 ((52, 1))
                
-               288        1504 LOAD_CONST              14 ((52, -1))
+               288        1504 LOAD_CONST              14 ((52, 0))
                
                285        1506 KW_NAMES                 5
                           1508 PRECALL                  3
                           1512 CALL                     3
                           1522 POP_TOP
                
                284        1524 LOAD_CONST               0 (None)
@@ -2617,30 +2619,30 @@
                           1564 POP_EXCEPT
                           1566 POP_TOP
                           1568 POP_TOP
                
                290     >> 1570 LOAD_GLOBAL              7 (NULL + pytest)
                           1582 LOAD_ATTR                4 (raises)
                           1592 LOAD_GLOBAL             10 (ValueError)
-                          1604 LOAD_CONST              18 ('Site \\(second number in cleaner_location tuple\\)')
+                          1604 LOAD_CONST              21 ('Site \\(second number in cleaner_location tuple\\)')
                           1606 KW_NAMES                 9
                           1608 PRECALL                  2
                           1612 CALL                     2
                           1622 BEFORE_WITH
                           1624 POP_TOP
                
                291        1626 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                292        1638 LOAD_CONST               1 (1)
                           1640 LOAD_CONST               2 (2)
                           1642 BUILD_LIST               2
                
-               293        1644 LOAD_CONST               3 ((52, 1))
+               293        1644 LOAD_CONST               4 ((52, 1))
                
-               294        1646 LOAD_CONST              15 ((52, 128))
+               294        1646 LOAD_CONST              15 ((52, 129))
                
                291        1648 KW_NAMES                 5
                           1650 PRECALL                  3
                           1654 CALL                     3
                           1664 POP_TOP
                
                290        1666 LOAD_CONST               0 (None)
@@ -2661,28 +2663,28 @@
                           1706 POP_EXCEPT
                           1708 POP_TOP
                           1710 POP_TOP
                
                296     >> 1712 LOAD_GLOBAL              7 (NULL + pytest)
                           1724 LOAD_ATTR                4 (raises)
                           1734 LOAD_GLOBAL             10 (ValueError)
-                          1746 LOAD_CONST              18 ('Site \\(second number in cleaner_location tuple\\)')
+                          1746 LOAD_CONST              21 ('Site \\(second number in cleaner_location tuple\\)')
                           1748 KW_NAMES                 9
                           1750 PRECALL                  2
                           1754 CALL                     2
                           1764 BEFORE_WITH
                           1766 POP_TOP
                
                297        1768 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                298        1780 LOAD_CONST               1 (1)
                           1782 LOAD_CONST               2 (2)
                           1784 BUILD_LIST               2
                
-               299        1786 LOAD_CONST               3 ((52, 1))
+               299        1786 LOAD_CONST               4 ((52, 1))
                
                300        1788 LOAD_CONST              16 ((52, 1.7))
                
                297        1790 KW_NAMES                 5
                           1792 PRECALL                  3
                           1796 CALL                     3
                           1806 POP_TOP
@@ -2705,34 +2707,34 @@
                           1848 POP_EXCEPT
                           1850 POP_TOP
                           1852 POP_TOP
                
                304     >> 1854 LOAD_GLOBAL              7 (NULL + pytest)
                           1866 LOAD_ATTR                4 (raises)
                           1876 LOAD_GLOBAL             10 (ValueError)
-                          1888 LOAD_CONST              19 ('Parameter arm')
+                          1888 LOAD_CONST              22 ('Parameter arm')
                           1890 KW_NAMES                 9
                           1892 PRECALL                  2
                           1896 CALL                     2
                           1906 BEFORE_WITH
                           1908 POP_TOP
                
                305        1910 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                306        1922 LOAD_CONST               1 (1)
                           1924 LOAD_CONST               2 (2)
                           1926 BUILD_LIST               2
                
-               307        1928 LOAD_CONST               3 ((52, 1))
+               307        1928 LOAD_CONST               3 ((52, 2))
                
-               308        1930 LOAD_CONST               4 ((52, 0))
+               308        1930 LOAD_CONST               4 ((52, 1))
                
                309        1932 LOAD_CONST               2 (2)
                
-               305        1934 KW_NAMES                20
+               305        1934 KW_NAMES                23
                           1936 PRECALL                  4
                           1940 CALL                     4
                           1950 POP_TOP
                
                304        1952 LOAD_CONST               0 (None)
                           1954 LOAD_CONST               0 (None)
                           1956 LOAD_CONST               0 (None)
@@ -2751,34 +2753,34 @@
                           1992 POP_EXCEPT
                           1994 POP_TOP
                           1996 POP_TOP
                
                313     >> 1998 LOAD_GLOBAL              7 (NULL + pytest)
                           2010 LOAD_ATTR                4 (raises)
                           2020 LOAD_GLOBAL             10 (ValueError)
-                          2032 LOAD_CONST              21 ('waste_vol has to be a float')
+                          2032 LOAD_CONST              24 ('waste_vol has to be a float')
                           2034 KW_NAMES                 9
                           2036 PRECALL                  2
                           2040 CALL                     2
                           2050 BEFORE_WITH
                           2052 POP_TOP
                
                314        2054 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                315        2066 LOAD_CONST               1 (1)
                           2068 LOAD_CONST               2 (2)
                           2070 BUILD_LIST               2
                
-               316        2072 LOAD_CONST               3 ((52, 1))
+               316        2072 LOAD_CONST               3 ((52, 2))
                
-               317        2074 LOAD_CONST               4 ((52, 0))
+               317        2074 LOAD_CONST               4 ((52, 1))
                
-               318        2076 LOAD_CONST              22 (-1.0)
+               318        2076 LOAD_CONST              25 (-1.0)
                
-               314        2078 KW_NAMES                23
+               314        2078 KW_NAMES                26
                           2080 PRECALL                  4
                           2084 CALL                     4
                           2094 POP_TOP
                
                313        2096 LOAD_CONST               0 (None)
                           2098 LOAD_CONST               0 (None)
                           2100 LOAD_CONST               0 (None)
@@ -2797,34 +2799,34 @@
                           2136 POP_EXCEPT
                           2138 POP_TOP
                           2140 POP_TOP
                
                320     >> 2142 LOAD_GLOBAL              7 (NULL + pytest)
                           2154 LOAD_ATTR                4 (raises)
                           2164 LOAD_GLOBAL             10 (ValueError)
-                          2176 LOAD_CONST              21 ('waste_vol has to be a float')
+                          2176 LOAD_CONST              24 ('waste_vol has to be a float')
                           2178 KW_NAMES                 9
                           2180 PRECALL                  2
                           2184 CALL                     2
                           2194 BEFORE_WITH
                           2196 POP_TOP
                
                321        2198 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                322        2210 LOAD_CONST               1 (1)
                           2212 LOAD_CONST               2 (2)
                           2214 BUILD_LIST               2
                
-               323        2216 LOAD_CONST               3 ((52, 1))
+               323        2216 LOAD_CONST               3 ((52, 2))
                
-               324        2218 LOAD_CONST               4 ((52, 0))
+               324        2218 LOAD_CONST               4 ((52, 1))
                
-               325        2220 LOAD_CONST              24 (101.0)
+               325        2220 LOAD_CONST              27 (101.0)
                
-               321        2222 KW_NAMES                23
+               321        2222 KW_NAMES                26
                           2224 PRECALL                  4
                           2228 CALL                     4
                           2238 POP_TOP
                
                320        2240 LOAD_CONST               0 (None)
                           2242 LOAD_CONST               0 (None)
                           2244 LOAD_CONST               0 (None)
@@ -2843,34 +2845,34 @@
                           2280 POP_EXCEPT
                           2282 POP_TOP
                           2284 POP_TOP
                
                327     >> 2286 LOAD_GLOBAL              7 (NULL + pytest)
                           2298 LOAD_ATTR                4 (raises)
                           2308 LOAD_GLOBAL             10 (ValueError)
-                          2320 LOAD_CONST              21 ('waste_vol has to be a float')
+                          2320 LOAD_CONST              24 ('waste_vol has to be a float')
                           2322 KW_NAMES                 9
                           2324 PRECALL                  2
                           2328 CALL                     2
                           2338 BEFORE_WITH
                           2340 POP_TOP
                
                328        2342 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                329        2354 LOAD_CONST               1 (1)
                           2356 LOAD_CONST               2 (2)
                           2358 BUILD_LIST               2
                
-               330        2360 LOAD_CONST               3 ((52, 1))
+               330        2360 LOAD_CONST               3 ((52, 2))
                
-               331        2362 LOAD_CONST               4 ((52, 0))
+               331        2362 LOAD_CONST               4 ((52, 1))
                
                332        2364 LOAD_CONST               1 (1)
                
-               328        2366 KW_NAMES                23
+               328        2366 KW_NAMES                26
                           2368 PRECALL                  4
                           2372 CALL                     4
                           2382 POP_TOP
                
                327        2384 LOAD_CONST               0 (None)
                           2386 LOAD_CONST               0 (None)
                           2388 LOAD_CONST               0 (None)
@@ -2889,34 +2891,34 @@
                           2424 POP_EXCEPT
                           2426 POP_TOP
                           2428 POP_TOP
                
                336     >> 2430 LOAD_GLOBAL              7 (NULL + pytest)
                           2442 LOAD_ATTR                4 (raises)
                           2452 LOAD_GLOBAL             10 (ValueError)
-                          2464 LOAD_CONST              25 ('waste_delay has to be an int')
+                          2464 LOAD_CONST              28 ('waste_delay has to be an int')
                           2466 KW_NAMES                 9
                           2468 PRECALL                  2
                           2472 CALL                     2
                           2482 BEFORE_WITH
                           2484 POP_TOP
                
                337        2486 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                338        2498 LOAD_CONST               1 (1)
                           2500 LOAD_CONST               2 (2)
                           2502 BUILD_LIST               2
                
-               339        2504 LOAD_CONST               3 ((52, 1))
+               339        2504 LOAD_CONST               3 ((52, 2))
                
-               340        2506 LOAD_CONST               4 ((52, 0))
+               340        2506 LOAD_CONST               4 ((52, 1))
                
-               341        2508 LOAD_CONST              26 (-1)
+               341        2508 LOAD_CONST              29 (-1)
                
-               337        2510 KW_NAMES                27
+               337        2510 KW_NAMES                30
                           2512 PRECALL                  4
                           2516 CALL                     4
                           2526 POP_TOP
                
                336        2528 LOAD_CONST               0 (None)
                           2530 LOAD_CONST               0 (None)
                           2532 LOAD_CONST               0 (None)
@@ -2935,34 +2937,34 @@
                           2568 POP_EXCEPT
                           2570 POP_TOP
                           2572 POP_TOP
                
                343     >> 2574 LOAD_GLOBAL              7 (NULL + pytest)
                           2586 LOAD_ATTR                4 (raises)
                           2596 LOAD_GLOBAL             10 (ValueError)
-                          2608 LOAD_CONST              25 ('waste_delay has to be an int')
+                          2608 LOAD_CONST              28 ('waste_delay has to be an int')
                           2610 KW_NAMES                 9
                           2612 PRECALL                  2
                           2616 CALL                     2
                           2626 BEFORE_WITH
                           2628 POP_TOP
                
                344        2630 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                345        2642 LOAD_CONST               1 (1)
                           2644 LOAD_CONST               2 (2)
                           2646 BUILD_LIST               2
                
-               346        2648 LOAD_CONST               3 ((52, 1))
+               346        2648 LOAD_CONST               3 ((52, 2))
                
-               347        2650 LOAD_CONST               4 ((52, 0))
+               347        2650 LOAD_CONST               4 ((52, 1))
                
-               348        2652 LOAD_CONST              28 (1001)
+               348        2652 LOAD_CONST              31 (1001)
                
-               344        2654 KW_NAMES                27
+               344        2654 KW_NAMES                30
                           2656 PRECALL                  4
                           2660 CALL                     4
                           2670 POP_TOP
                
                343        2672 LOAD_CONST               0 (None)
                           2674 LOAD_CONST               0 (None)
                           2676 LOAD_CONST               0 (None)
@@ -2981,34 +2983,34 @@
                           2712 POP_EXCEPT
                           2714 POP_TOP
                           2716 POP_TOP
                
                350     >> 2718 LOAD_GLOBAL              7 (NULL + pytest)
                           2730 LOAD_ATTR                4 (raises)
                           2740 LOAD_GLOBAL             10 (ValueError)
-                          2752 LOAD_CONST              25 ('waste_delay has to be an int')
+                          2752 LOAD_CONST              28 ('waste_delay has to be an int')
                           2754 KW_NAMES                 9
                           2756 PRECALL                  2
                           2760 CALL                     2
                           2770 BEFORE_WITH
                           2772 POP_TOP
                
                351        2774 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                352        2786 LOAD_CONST               1 (1)
                           2788 LOAD_CONST               2 (2)
                           2790 BUILD_LIST               2
                
-               353        2792 LOAD_CONST               3 ((52, 1))
+               353        2792 LOAD_CONST               3 ((52, 2))
                
-               354        2794 LOAD_CONST               4 ((52, 0))
+               354        2794 LOAD_CONST               4 ((52, 1))
                
-               355        2796 LOAD_CONST              29 (10.0)
+               355        2796 LOAD_CONST              32 (10.0)
                
-               351        2798 KW_NAMES                27
+               351        2798 KW_NAMES                30
                           2800 PRECALL                  4
                           2804 CALL                     4
                           2814 POP_TOP
                
                350        2816 LOAD_CONST               0 (None)
                           2818 LOAD_CONST               0 (None)
                           2820 LOAD_CONST               0 (None)
@@ -3027,34 +3029,34 @@
                           2856 POP_EXCEPT
                           2858 POP_TOP
                           2860 POP_TOP
                
                359     >> 2862 LOAD_GLOBAL              7 (NULL + pytest)
                           2874 LOAD_ATTR                4 (raises)
                           2884 LOAD_GLOBAL             10 (ValueError)
-                          2896 LOAD_CONST              30 ('cleaner_vol has to be a float')
+                          2896 LOAD_CONST              33 ('cleaner_vol has to be a float')
                           2898 KW_NAMES                 9
                           2900 PRECALL                  2
                           2904 CALL                     2
                           2914 BEFORE_WITH
                           2916 POP_TOP
                
                360        2918 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                361        2930 LOAD_CONST               1 (1)
                           2932 LOAD_CONST               2 (2)
                           2934 BUILD_LIST               2
                
-               362        2936 LOAD_CONST               3 ((52, 1))
+               362        2936 LOAD_CONST               3 ((52, 2))
                
-               363        2938 LOAD_CONST               4 ((52, 0))
+               363        2938 LOAD_CONST               4 ((52, 1))
                
-               364        2940 LOAD_CONST              22 (-1.0)
+               364        2940 LOAD_CONST              25 (-1.0)
                
-               360        2942 KW_NAMES                31
+               360        2942 KW_NAMES                34
                           2944 PRECALL                  4
                           2948 CALL                     4
                           2958 POP_TOP
                
                359        2960 LOAD_CONST               0 (None)
                           2962 LOAD_CONST               0 (None)
                           2964 LOAD_CONST               0 (None)
@@ -3073,34 +3075,34 @@
                           3000 POP_EXCEPT
                           3002 POP_TOP
                           3004 POP_TOP
                
                366     >> 3006 LOAD_GLOBAL              7 (NULL + pytest)
                           3018 LOAD_ATTR                4 (raises)
                           3028 LOAD_GLOBAL             10 (ValueError)
-                          3040 LOAD_CONST              30 ('cleaner_vol has to be a float')
+                          3040 LOAD_CONST              33 ('cleaner_vol has to be a float')
                           3042 KW_NAMES                 9
                           3044 PRECALL                  2
                           3048 CALL                     2
                           3058 BEFORE_WITH
                           3060 POP_TOP
                
                367        3062 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                368        3074 LOAD_CONST               1 (1)
                           3076 LOAD_CONST               2 (2)
                           3078 BUILD_LIST               2
                
-               369        3080 LOAD_CONST               3 ((52, 1))
+               369        3080 LOAD_CONST               3 ((52, 2))
                
-               370        3082 LOAD_CONST               4 ((52, 0))
+               370        3082 LOAD_CONST               4 ((52, 1))
                
-               371        3084 LOAD_CONST              24 (101.0)
+               371        3084 LOAD_CONST              27 (101.0)
                
-               367        3086 KW_NAMES                31
+               367        3086 KW_NAMES                34
                           3088 PRECALL                  4
                           3092 CALL                     4
                           3102 POP_TOP
                
                366        3104 LOAD_CONST               0 (None)
                           3106 LOAD_CONST               0 (None)
                           3108 LOAD_CONST               0 (None)
@@ -3119,34 +3121,34 @@
                           3144 POP_EXCEPT
                           3146 POP_TOP
                           3148 POP_TOP
                
                373     >> 3150 LOAD_GLOBAL              7 (NULL + pytest)
                           3162 LOAD_ATTR                4 (raises)
                           3172 LOAD_GLOBAL             10 (ValueError)
-                          3184 LOAD_CONST              30 ('cleaner_vol has to be a float')
+                          3184 LOAD_CONST              33 ('cleaner_vol has to be a float')
                           3186 KW_NAMES                 9
                           3188 PRECALL                  2
                           3192 CALL                     2
                           3202 BEFORE_WITH
                           3204 POP_TOP
                
                374        3206 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                375        3218 LOAD_CONST               1 (1)
                           3220 LOAD_CONST               2 (2)
                           3222 BUILD_LIST               2
                
-               376        3224 LOAD_CONST               3 ((52, 1))
+               376        3224 LOAD_CONST               3 ((52, 2))
                
-               377        3226 LOAD_CONST               4 ((52, 0))
+               377        3226 LOAD_CONST               4 ((52, 1))
                
                378        3228 LOAD_CONST               1 (1)
                
-               374        3230 KW_NAMES                31
+               374        3230 KW_NAMES                34
                           3232 PRECALL                  4
                           3236 CALL                     4
                           3246 POP_TOP
                
                373        3248 LOAD_CONST               0 (None)
                           3250 LOAD_CONST               0 (None)
                           3252 LOAD_CONST               0 (None)
@@ -3165,34 +3167,34 @@
                           3288 POP_EXCEPT
                           3290 POP_TOP
                           3292 POP_TOP
                
                382     >> 3294 LOAD_GLOBAL              7 (NULL + pytest)
                           3306 LOAD_ATTR                4 (raises)
                           3316 LOAD_GLOBAL             10 (ValueError)
-                          3328 LOAD_CONST              32 ('cleaner_delay has to be an int')
+                          3328 LOAD_CONST              35 ('cleaner_delay has to be an int')
                           3330 KW_NAMES                 9
                           3332 PRECALL                  2
                           3336 CALL                     2
                           3346 BEFORE_WITH
                           3348 POP_TOP
                
                383        3350 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                384        3362 LOAD_CONST               1 (1)
                           3364 LOAD_CONST               2 (2)
                           3366 BUILD_LIST               2
                
-               385        3368 LOAD_CONST               3 ((52, 1))
+               385        3368 LOAD_CONST               3 ((52, 2))
                
-               386        3370 LOAD_CONST               4 ((52, 0))
+               386        3370 LOAD_CONST               4 ((52, 1))
                
-               387        3372 LOAD_CONST              26 (-1)
+               387        3372 LOAD_CONST              29 (-1)
                
-               383        3374 KW_NAMES                33
+               383        3374 KW_NAMES                36
                           3376 PRECALL                  4
                           3380 CALL                     4
                           3390 POP_TOP
                
                382        3392 LOAD_CONST               0 (None)
                           3394 LOAD_CONST               0 (None)
                           3396 LOAD_CONST               0 (None)
@@ -3211,34 +3213,34 @@
                           3432 POP_EXCEPT
                           3434 POP_TOP
                           3436 POP_TOP
                
                389     >> 3438 LOAD_GLOBAL              7 (NULL + pytest)
                           3450 LOAD_ATTR                4 (raises)
                           3460 LOAD_GLOBAL             10 (ValueError)
-                          3472 LOAD_CONST              32 ('cleaner_delay has to be an int')
+                          3472 LOAD_CONST              35 ('cleaner_delay has to be an int')
                           3474 KW_NAMES                 9
                           3476 PRECALL                  2
                           3480 CALL                     2
                           3490 BEFORE_WITH
                           3492 POP_TOP
                
                390        3494 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                391        3506 LOAD_CONST               1 (1)
                           3508 LOAD_CONST               2 (2)
                           3510 BUILD_LIST               2
                
-               392        3512 LOAD_CONST               3 ((52, 1))
+               392        3512 LOAD_CONST               3 ((52, 2))
                
-               393        3514 LOAD_CONST               4 ((52, 0))
+               393        3514 LOAD_CONST               4 ((52, 1))
                
-               394        3516 LOAD_CONST              28 (1001)
+               394        3516 LOAD_CONST              31 (1001)
                
-               390        3518 KW_NAMES                33
+               390        3518 KW_NAMES                36
                           3520 PRECALL                  4
                           3524 CALL                     4
                           3534 POP_TOP
                
                389        3536 LOAD_CONST               0 (None)
                           3538 LOAD_CONST               0 (None)
                           3540 LOAD_CONST               0 (None)
@@ -3257,34 +3259,34 @@
                           3576 POP_EXCEPT
                           3578 POP_TOP
                           3580 POP_TOP
                
                396     >> 3582 LOAD_GLOBAL              7 (NULL + pytest)
                           3594 LOAD_ATTR                4 (raises)
                           3604 LOAD_GLOBAL             10 (ValueError)
-                          3616 LOAD_CONST              32 ('cleaner_delay has to be an int')
+                          3616 LOAD_CONST              35 ('cleaner_delay has to be an int')
                           3618 KW_NAMES                 9
                           3620 PRECALL                  2
                           3624 CALL                     2
                           3634 BEFORE_WITH
                           3636 POP_TOP
                
                397        3638 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                398        3650 LOAD_CONST               1 (1)
                           3652 LOAD_CONST               2 (2)
                           3654 BUILD_LIST               2
                
-               399        3656 LOAD_CONST               3 ((52, 1))
+               399        3656 LOAD_CONST               3 ((52, 2))
                
-               400        3658 LOAD_CONST               4 ((52, 0))
+               400        3658 LOAD_CONST               4 ((52, 1))
                
-               401        3660 LOAD_CONST              29 (10.0)
+               401        3660 LOAD_CONST              32 (10.0)
                
-               397        3662 KW_NAMES                33
+               397        3662 KW_NAMES                36
                           3664 PRECALL                  4
                           3668 CALL                     4
                           3678 POP_TOP
                
                396        3680 LOAD_CONST               0 (None)
                           3682 LOAD_CONST               0 (None)
                           3684 LOAD_CONST               0 (None)
@@ -3303,34 +3305,34 @@
                           3720 POP_EXCEPT
                           3722 POP_TOP
                           3724 POP_TOP
                
                405     >> 3726 LOAD_GLOBAL              7 (NULL + pytest)
                           3738 LOAD_ATTR                4 (raises)
                           3748 LOAD_GLOBAL             10 (ValueError)
-                          3760 LOAD_CONST              34 ('airgap has to be an int')
+                          3760 LOAD_CONST              37 ('airgap has to be an int')
                           3762 KW_NAMES                 9
                           3764 PRECALL                  2
                           3768 CALL                     2
                           3778 BEFORE_WITH
                           3780 POP_TOP
                
                406        3782 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                407        3794 LOAD_CONST               1 (1)
                           3796 LOAD_CONST               2 (2)
                           3798 BUILD_LIST               2
                
-               408        3800 LOAD_CONST               3 ((52, 1))
+               408        3800 LOAD_CONST               3 ((52, 2))
                
-               409        3802 LOAD_CONST               4 ((52, 0))
+               409        3802 LOAD_CONST               4 ((52, 1))
                
-               410        3804 LOAD_CONST              26 (-1)
+               410        3804 LOAD_CONST              29 (-1)
                
-               406        3806 KW_NAMES                35
+               406        3806 KW_NAMES                38
                           3808 PRECALL                  4
                           3812 CALL                     4
                           3822 POP_TOP
                
                405        3824 LOAD_CONST               0 (None)
                           3826 LOAD_CONST               0 (None)
                           3828 LOAD_CONST               0 (None)
@@ -3349,34 +3351,34 @@
                           3864 POP_EXCEPT
                           3866 POP_TOP
                           3868 POP_TOP
                
                412     >> 3870 LOAD_GLOBAL              7 (NULL + pytest)
                           3882 LOAD_ATTR                4 (raises)
                           3892 LOAD_GLOBAL             10 (ValueError)
-                          3904 LOAD_CONST              34 ('airgap has to be an int')
+                          3904 LOAD_CONST              37 ('airgap has to be an int')
                           3906 KW_NAMES                 9
                           3908 PRECALL                  2
                           3912 CALL                     2
                           3922 BEFORE_WITH
                           3924 POP_TOP
                
                413        3926 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                414        3938 LOAD_CONST               1 (1)
                           3940 LOAD_CONST               2 (2)
                           3942 BUILD_LIST               2
                
-               415        3944 LOAD_CONST               3 ((52, 1))
+               415        3944 LOAD_CONST               3 ((52, 2))
                
-               416        3946 LOAD_CONST               4 ((52, 0))
+               416        3946 LOAD_CONST               4 ((52, 1))
                
-               417        3948 LOAD_CONST              36 (101)
+               417        3948 LOAD_CONST              39 (101)
                
-               413        3950 KW_NAMES                35
+               413        3950 KW_NAMES                38
                           3952 PRECALL                  4
                           3956 CALL                     4
                           3966 POP_TOP
                
                412        3968 LOAD_CONST               0 (None)
                           3970 LOAD_CONST               0 (None)
                           3972 LOAD_CONST               0 (None)
@@ -3395,34 +3397,34 @@
                           4008 POP_EXCEPT
                           4010 POP_TOP
                           4012 POP_TOP
                
                419     >> 4014 LOAD_GLOBAL              7 (NULL + pytest)
                           4026 LOAD_ATTR                4 (raises)
                           4036 LOAD_GLOBAL             10 (ValueError)
-                          4048 LOAD_CONST              34 ('airgap has to be an int')
+                          4048 LOAD_CONST              37 ('airgap has to be an int')
                           4050 KW_NAMES                 9
                           4052 PRECALL                  2
                           4056 CALL                     2
                           4066 BEFORE_WITH
                           4068 POP_TOP
                
                420        4070 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                421        4082 LOAD_CONST               1 (1)
                           4084 LOAD_CONST               2 (2)
                           4086 BUILD_LIST               2
                
-               422        4088 LOAD_CONST               3 ((52, 1))
+               422        4088 LOAD_CONST               3 ((52, 2))
                
-               423        4090 LOAD_CONST               4 ((52, 0))
+               423        4090 LOAD_CONST               4 ((52, 1))
                
-               424        4092 LOAD_CONST              29 (10.0)
+               424        4092 LOAD_CONST              32 (10.0)
                
-               420        4094 KW_NAMES                35
+               420        4094 KW_NAMES                38
                           4096 PRECALL                  4
                           4100 CALL                     4
                           4110 POP_TOP
                
                419        4112 LOAD_CONST               0 (None)
                           4114 LOAD_CONST               0 (None)
                           4116 LOAD_CONST               0 (None)
@@ -3441,34 +3443,34 @@
                           4152 POP_EXCEPT
                           4154 POP_TOP
                           4156 POP_TOP
                
                428     >> 4158 LOAD_GLOBAL              7 (NULL + pytest)
                           4170 LOAD_ATTR                4 (raises)
                           4180 LOAD_GLOBAL             10 (ValueError)
-                          4192 LOAD_CONST              37 ('airgap_speed has to be an int')
+                          4192 LOAD_CONST              40 ('airgap_speed has to be an int')
                           4194 KW_NAMES                 9
                           4196 PRECALL                  2
                           4200 CALL                     2
                           4210 BEFORE_WITH
                           4212 POP_TOP
                
                429        4214 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                430        4226 LOAD_CONST               1 (1)
                           4228 LOAD_CONST               2 (2)
                           4230 BUILD_LIST               2
                
-               431        4232 LOAD_CONST               3 ((52, 1))
+               431        4232 LOAD_CONST               3 ((52, 2))
                
-               432        4234 LOAD_CONST               4 ((52, 0))
+               432        4234 LOAD_CONST               4 ((52, 1))
                
-               433        4236 LOAD_CONST              38 (0)
+               433        4236 LOAD_CONST              41 (0)
                
-               429        4238 KW_NAMES                39
+               429        4238 KW_NAMES                42
                           4240 PRECALL                  4
                           4244 CALL                     4
                           4254 POP_TOP
                
                428        4256 LOAD_CONST               0 (None)
                           4258 LOAD_CONST               0 (None)
                           4260 LOAD_CONST               0 (None)
@@ -3487,34 +3489,34 @@
                           4296 POP_EXCEPT
                           4298 POP_TOP
                           4300 POP_TOP
                
                435     >> 4302 LOAD_GLOBAL              7 (NULL + pytest)
                           4314 LOAD_ATTR                4 (raises)
                           4324 LOAD_GLOBAL             10 (ValueError)
-                          4336 LOAD_CONST              37 ('airgap_speed has to be an int')
+                          4336 LOAD_CONST              40 ('airgap_speed has to be an int')
                           4338 KW_NAMES                 9
                           4340 PRECALL                  2
                           4344 CALL                     2
                           4354 BEFORE_WITH
                           4356 POP_TOP
                
                436        4358 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                437        4370 LOAD_CONST               1 (1)
                           4372 LOAD_CONST               2 (2)
                           4374 BUILD_LIST               2
                
-               438        4376 LOAD_CONST               3 ((52, 1))
+               438        4376 LOAD_CONST               3 ((52, 2))
                
-               439        4378 LOAD_CONST               4 ((52, 0))
+               439        4378 LOAD_CONST               4 ((52, 1))
                
-               440        4380 LOAD_CONST              28 (1001)
+               440        4380 LOAD_CONST              31 (1001)
                
-               436        4382 KW_NAMES                39
+               436        4382 KW_NAMES                42
                           4384 PRECALL                  4
                           4388 CALL                     4
                           4398 POP_TOP
                
                435        4400 LOAD_CONST               0 (None)
                           4402 LOAD_CONST               0 (None)
                           4404 LOAD_CONST               0 (None)
@@ -3533,34 +3535,34 @@
                           4440 POP_EXCEPT
                           4442 POP_TOP
                           4444 POP_TOP
                
                442     >> 4446 LOAD_GLOBAL              7 (NULL + pytest)
                           4458 LOAD_ATTR                4 (raises)
                           4468 LOAD_GLOBAL             10 (ValueError)
-                          4480 LOAD_CONST              37 ('airgap_speed has to be an int')
+                          4480 LOAD_CONST              40 ('airgap_speed has to be an int')
                           4482 KW_NAMES                 9
                           4484 PRECALL                  2
                           4488 CALL                     2
                           4498 BEFORE_WITH
                           4500 POP_TOP
                
                443        4502 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                444        4514 LOAD_CONST               1 (1)
                           4516 LOAD_CONST               2 (2)
                           4518 BUILD_LIST               2
                
-               445        4520 LOAD_CONST               3 ((52, 1))
+               445        4520 LOAD_CONST               3 ((52, 2))
                
-               446        4522 LOAD_CONST               4 ((52, 0))
+               446        4522 LOAD_CONST               4 ((52, 1))
                
-               447        4524 LOAD_CONST              29 (10.0)
+               447        4524 LOAD_CONST              32 (10.0)
                
-               443        4526 KW_NAMES                39
+               443        4526 KW_NAMES                42
                           4528 PRECALL                  4
                           4532 CALL                     4
                           4542 POP_TOP
                
                442        4544 LOAD_CONST               0 (None)
                           4546 LOAD_CONST               0 (None)
                           4548 LOAD_CONST               0 (None)
@@ -3579,34 +3581,34 @@
                           4584 POP_EXCEPT
                           4586 POP_TOP
                           4588 POP_TOP
                
                451     >> 4590 LOAD_GLOBAL              7 (NULL + pytest)
                           4602 LOAD_ATTR                4 (raises)
                           4612 LOAD_GLOBAL             10 (ValueError)
-                          4624 LOAD_CONST              40 ('retract_speed has to be an int')
+                          4624 LOAD_CONST              43 ('retract_speed has to be an int')
                           4626 KW_NAMES                 9
                           4628 PRECALL                  2
                           4632 CALL                     2
                           4642 BEFORE_WITH
                           4644 POP_TOP
                
                452        4646 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                453        4658 LOAD_CONST               1 (1)
                           4660 LOAD_CONST               2 (2)
                           4662 BUILD_LIST               2
                
-               454        4664 LOAD_CONST               3 ((52, 1))
+               454        4664 LOAD_CONST               3 ((52, 2))
                
-               455        4666 LOAD_CONST               4 ((52, 0))
+               455        4666 LOAD_CONST               4 ((52, 1))
                
-               456        4668 LOAD_CONST              38 (0)
+               456        4668 LOAD_CONST              41 (0)
                
-               452        4670 KW_NAMES                41
+               452        4670 KW_NAMES                44
                           4672 PRECALL                  4
                           4676 CALL                     4
                           4686 POP_TOP
                
                451        4688 LOAD_CONST               0 (None)
                           4690 LOAD_CONST               0 (None)
                           4692 LOAD_CONST               0 (None)
@@ -3625,34 +3627,34 @@
                           4728 POP_EXCEPT
                           4730 POP_TOP
                           4732 POP_TOP
                
                458     >> 4734 LOAD_GLOBAL              7 (NULL + pytest)
                           4746 LOAD_ATTR                4 (raises)
                           4756 LOAD_GLOBAL             10 (ValueError)
-                          4768 LOAD_CONST              40 ('retract_speed has to be an int')
+                          4768 LOAD_CONST              43 ('retract_speed has to be an int')
                           4770 KW_NAMES                 9
                           4772 PRECALL                  2
                           4776 CALL                     2
                           4786 BEFORE_WITH
                           4788 POP_TOP
                
                459        4790 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                460        4802 LOAD_CONST               1 (1)
                           4804 LOAD_CONST               2 (2)
                           4806 BUILD_LIST               2
                
-               461        4808 LOAD_CONST               3 ((52, 1))
+               461        4808 LOAD_CONST               3 ((52, 2))
                
-               462        4810 LOAD_CONST               4 ((52, 0))
+               462        4810 LOAD_CONST               4 ((52, 1))
                
-               463        4812 LOAD_CONST              36 (101)
+               463        4812 LOAD_CONST              39 (101)
                
-               459        4814 KW_NAMES                41
+               459        4814 KW_NAMES                44
                           4816 PRECALL                  4
                           4820 CALL                     4
                           4830 POP_TOP
                
                458        4832 LOAD_CONST               0 (None)
                           4834 LOAD_CONST               0 (None)
                           4836 LOAD_CONST               0 (None)
@@ -3671,34 +3673,34 @@
                           4872 POP_EXCEPT
                           4874 POP_TOP
                           4876 POP_TOP
                
                465     >> 4878 LOAD_GLOBAL              7 (NULL + pytest)
                           4890 LOAD_ATTR                4 (raises)
                           4900 LOAD_GLOBAL             10 (ValueError)
-                          4912 LOAD_CONST              40 ('retract_speed has to be an int')
+                          4912 LOAD_CONST              43 ('retract_speed has to be an int')
                           4914 KW_NAMES                 9
                           4916 PRECALL                  2
                           4920 CALL                     2
                           4930 BEFORE_WITH
                           4932 POP_TOP
                
                466        4934 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                467        4946 LOAD_CONST               1 (1)
                           4948 LOAD_CONST               2 (2)
                           4950 BUILD_LIST               2
                
-               468        4952 LOAD_CONST               3 ((52, 1))
+               468        4952 LOAD_CONST               3 ((52, 2))
                
-               469        4954 LOAD_CONST               4 ((52, 0))
+               469        4954 LOAD_CONST               4 ((52, 1))
                
-               470        4956 LOAD_CONST              29 (10.0)
+               470        4956 LOAD_CONST              32 (10.0)
                
-               466        4958 KW_NAMES                41
+               466        4958 KW_NAMES                44
                           4960 PRECALL                  4
                           4964 CALL                     4
                           4974 POP_TOP
                
                465        4976 LOAD_CONST               0 (None)
                           4978 LOAD_CONST               0 (None)
                           4980 LOAD_CONST               0 (None)
@@ -3717,34 +3719,34 @@
                           5016 POP_EXCEPT
                           5018 POP_TOP
                           5020 POP_TOP
                
                474     >> 5022 LOAD_GLOBAL              7 (NULL + pytest)
                           5034 LOAD_ATTR                4 (raises)
                           5044 LOAD_GLOBAL             10 (ValueError)
-                          5056 LOAD_CONST              42 ('Parameter fastwash')
+                          5056 LOAD_CONST              45 ('Parameter fastwash')
                           5058 KW_NAMES                 9
                           5060 PRECALL                  2
                           5064 CALL                     2
                           5074 BEFORE_WITH
                           5076 POP_TOP
                
                475        5078 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                476        5090 LOAD_CONST               1 (1)
                           5092 LOAD_CONST               2 (2)
                           5094 BUILD_LIST               2
                
-               477        5096 LOAD_CONST               3 ((52, 1))
+               477        5096 LOAD_CONST               3 ((52, 2))
                
-               478        5098 LOAD_CONST               4 ((52, 0))
+               478        5098 LOAD_CONST               4 ((52, 1))
                
                479        5100 LOAD_CONST               2 (2)
                
-               475        5102 KW_NAMES                43
+               475        5102 KW_NAMES                46
                           5104 PRECALL                  4
                           5108 CALL                     4
                           5118 POP_TOP
                
                474        5120 LOAD_CONST               0 (None)
                           5122 LOAD_CONST               0 (None)
                           5124 LOAD_CONST               0 (None)
@@ -3763,34 +3765,34 @@
                           5160 POP_EXCEPT
                           5162 POP_TOP
                           5164 POP_TOP
                
                481     >> 5166 LOAD_GLOBAL              7 (NULL + pytest)
                           5178 LOAD_ATTR                4 (raises)
                           5188 LOAD_GLOBAL             10 (ValueError)
-                          5200 LOAD_CONST              42 ('Parameter fastwash')
+                          5200 LOAD_CONST              45 ('Parameter fastwash')
                           5202 KW_NAMES                 9
                           5204 PRECALL                  2
                           5208 CALL                     2
                           5218 BEFORE_WITH
                           5220 POP_TOP
                
                482        5222 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                483        5234 LOAD_CONST               1 (1)
                           5236 LOAD_CONST               2 (2)
                           5238 BUILD_LIST               2
                
-               484        5240 LOAD_CONST               3 ((52, 1))
+               484        5240 LOAD_CONST               3 ((52, 2))
                
-               485        5242 LOAD_CONST               4 ((52, 0))
+               485        5242 LOAD_CONST               4 ((52, 1))
                
-               486        5244 LOAD_CONST              44 (1.0)
+               486        5244 LOAD_CONST              47 (1.0)
                
-               482        5246 KW_NAMES                43
+               482        5246 KW_NAMES                46
                           5248 PRECALL                  4
                           5252 CALL                     4
                           5262 POP_TOP
                
                481        5264 LOAD_CONST               0 (None)
                           5266 LOAD_CONST               0 (None)
                           5268 LOAD_CONST               0 (None)
@@ -3809,34 +3811,34 @@
                           5304 POP_EXCEPT
                           5306 POP_TOP
                           5308 POP_TOP
                
                490     >> 5310 LOAD_GLOBAL              7 (NULL + pytest)
                           5322 LOAD_ATTR                4 (raises)
                           5332 LOAD_GLOBAL             10 (ValueError)
-                          5344 LOAD_CONST              45 ('Parameter low_volume')
+                          5344 LOAD_CONST              48 ('Parameter low_volume')
                           5346 KW_NAMES                 9
                           5348 PRECALL                  2
                           5352 CALL                     2
                           5362 BEFORE_WITH
                           5364 POP_TOP
                
                491        5366 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                492        5378 LOAD_CONST               1 (1)
                           5380 LOAD_CONST               2 (2)
                           5382 BUILD_LIST               2
                
-               493        5384 LOAD_CONST               3 ((52, 1))
+               493        5384 LOAD_CONST               3 ((52, 2))
                
-               494        5386 LOAD_CONST               4 ((52, 0))
+               494        5386 LOAD_CONST               4 ((52, 1))
                
                495        5388 LOAD_CONST               2 (2)
                
-               491        5390 KW_NAMES                46
+               491        5390 KW_NAMES                49
                           5392 PRECALL                  4
                           5396 CALL                     4
                           5406 POP_TOP
                
                490        5408 LOAD_CONST               0 (None)
                           5410 LOAD_CONST               0 (None)
                           5412 LOAD_CONST               0 (None)
@@ -3855,34 +3857,34 @@
                           5448 POP_EXCEPT
                           5450 POP_TOP
                           5452 POP_TOP
                
                497     >> 5454 LOAD_GLOBAL              7 (NULL + pytest)
                           5466 LOAD_ATTR                4 (raises)
                           5476 LOAD_GLOBAL             10 (ValueError)
-                          5488 LOAD_CONST              45 ('Parameter low_volume')
+                          5488 LOAD_CONST              48 ('Parameter low_volume')
                           5490 KW_NAMES                 9
                           5492 PRECALL                  2
                           5496 CALL                     2
                           5506 BEFORE_WITH
                           5508 POP_TOP
                
                498        5510 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                499        5522 LOAD_CONST               1 (1)
                           5524 LOAD_CONST               2 (2)
                           5526 BUILD_LIST               2
                
-               500        5528 LOAD_CONST               3 ((52, 1))
+               500        5528 LOAD_CONST               3 ((52, 2))
                
-               501        5530 LOAD_CONST               4 ((52, 0))
+               501        5530 LOAD_CONST               4 ((52, 1))
                
-               502        5532 LOAD_CONST              44 (1.0)
+               502        5532 LOAD_CONST              47 (1.0)
                
-               498        5534 KW_NAMES                46
+               498        5534 KW_NAMES                49
                           5536 PRECALL                  4
                           5540 CALL                     4
                           5550 POP_TOP
                
                497        5552 LOAD_CONST               0 (None)
                           5554 LOAD_CONST               0 (None)
                           5556 LOAD_CONST               0 (None)
@@ -3901,20 +3903,20 @@
                           5592 POP_EXCEPT
                           5594 POP_TOP
                           5596 POP_TOP
                
                506     >> 5598 LOAD_GLOBAL              1 (NULL + prepare_evo_wash_parameters)
                
                507        5610 BUILD_LIST               0
-                          5612 LOAD_CONST              47 ((1, 2, 3, 4, 5, 6, 7, 8))
+                          5612 LOAD_CONST              50 ((1, 2, 3, 4, 5, 6, 7, 8))
                           5614 LIST_EXTEND              1
                
-               508        5616 LOAD_CONST               3 ((52, 1))
+               508        5616 LOAD_CONST               3 ((52, 2))
                
-               509        5618 LOAD_CONST               4 ((52, 0))
+               509        5618 LOAD_CONST               4 ((52, 1))
                
                506        5620 KW_NAMES                 5
                           5622 PRECALL                  3
                           5626 CALL                     3
                           5636 STORE_FAST               3 (actual)
                
                513        5638 LOAD_GLOBAL             12 (Tip)
@@ -3939,59 +3941,59 @@
                           5782 LOAD_ATTR               13 (T7)
                
                520        5792 LOAD_GLOBAL             12 (Tip)
                           5804 LOAD_ATTR               14 (T8)
                
                512        5814 BUILD_LIST               8
                
-               522        5816 LOAD_CONST               3 ((52, 1))
+               522        5816 LOAD_CONST               4 ((52, 1))
                
-               523        5818 LOAD_CONST               4 ((52, 0))
+               523        5818 LOAD_CONST              14 ((52, 0))
                
-               524        5820 LOAD_CONST              38 (0)
+               524        5820 LOAD_CONST              41 (0)
                
-               525        5822 LOAD_CONST              48 (3.0)
+               525        5822 LOAD_CONST              51 (3.0)
                
-               526        5824 LOAD_CONST              49 (500)
+               526        5824 LOAD_CONST              52 (500)
                
-               527        5826 LOAD_CONST              50 (4.0)
+               527        5826 LOAD_CONST              53 (4.0)
                
-               528        5828 LOAD_CONST              49 (500)
+               528        5828 LOAD_CONST              52 (500)
                
-               529        5830 LOAD_CONST              51 (10)
+               529        5830 LOAD_CONST              54 (10)
                
-               530        5832 LOAD_CONST              52 (70)
+               530        5832 LOAD_CONST              55 (70)
                
-               531        5834 LOAD_CONST              53 (30)
+               531        5834 LOAD_CONST              56 (30)
                
                532        5836 LOAD_CONST               1 (1)
                
-               533        5838 LOAD_CONST              38 (0)
+               533        5838 LOAD_CONST              41 (0)
                
                511        5840 BUILD_TUPLE             13
                           5842 STORE_FAST               4 (expected)
                
                535        5844 LOAD_FAST                3 (actual)
                           5846 LOAD_FAST                4 (expected)
                           5848 COMPARE_OP               2 (==)
                           5854 STORE_FAST               5 (@py_assert1)
                           5856 LOAD_FAST                5 (@py_assert1)
                           5858 POP_JUMP_FORWARD_IF_TRUE   194 (to 6248)
                           5860 LOAD_GLOBAL             31 (NULL + @pytest_ar)
                           5872 LOAD_ATTR               16 (_call_reprcompare)
-                          5882 LOAD_CONST              54 (('==',))
+                          5882 LOAD_CONST              57 (('==',))
                           5884 LOAD_FAST                5 (@py_assert1)
                           5886 BUILD_TUPLE              1
-                          5888 LOAD_CONST              55 (('%(py0)s == %(py2)s',))
+                          5888 LOAD_CONST              58 (('%(py0)s == %(py2)s',))
                           5890 LOAD_FAST                3 (actual)
                           5892 LOAD_FAST                4 (expected)
                           5894 BUILD_TUPLE              2
                           5896 PRECALL                  4
                           5900 CALL                     4
-                          5910 LOAD_CONST              56 ('actual')
+                          5910 LOAD_CONST              59 ('actual')
                           5912 LOAD_GLOBAL             35 (NULL + @py_builtins)
                           5924 LOAD_ATTR               18 (locals)
                           5934 PRECALL                  0
                           5938 CALL                     0
                           5948 CONTAINS_OP              0
                           5950 POP_JUMP_FORWARD_IF_TRUE    20 (to 5992)
                           5952 LOAD_GLOBAL             31 (NULL + @pytest_ar)
@@ -4002,16 +4004,16 @@
                           5990 POP_JUMP_FORWARD_IF_FALSE    20 (to 6032)
                        >> 5992 LOAD_GLOBAL             31 (NULL + @pytest_ar)
                           6004 LOAD_ATTR               20 (_saferepr)
                           6014 LOAD_FAST                3 (actual)
                           6016 PRECALL                  1
                           6020 CALL                     1
                           6030 JUMP_FORWARD             1 (to 6034)
-                       >> 6032 LOAD_CONST              56 ('actual')
-                       >> 6034 LOAD_CONST              57 ('expected')
+                       >> 6032 LOAD_CONST              59 ('actual')
+                       >> 6034 LOAD_CONST              60 ('expected')
                           6036 LOAD_GLOBAL             35 (NULL + @py_builtins)
                           6048 LOAD_ATTR               18 (locals)
                           6058 PRECALL                  0
                           6062 CALL                     0
                           6072 CONTAINS_OP              0
                           6074 POP_JUMP_FORWARD_IF_TRUE    20 (to 6116)
                           6076 LOAD_GLOBAL             31 (NULL + @pytest_ar)
@@ -4022,21 +4024,21 @@
                           6114 POP_JUMP_FORWARD_IF_FALSE    20 (to 6156)
                        >> 6116 LOAD_GLOBAL             31 (NULL + @pytest_ar)
                           6128 LOAD_ATTR               20 (_saferepr)
                           6138 LOAD_FAST                4 (expected)
                           6140 PRECALL                  1
                           6144 CALL                     1
                           6154 JUMP_FORWARD             1 (to 6158)
-                       >> 6156 LOAD_CONST              57 ('expected')
-                       >> 6158 LOAD_CONST              58 (('py0', 'py2'))
+                       >> 6156 LOAD_CONST              60 ('expected')
+                       >> 6158 LOAD_CONST              61 (('py0', 'py2'))
                           6160 BUILD_CONST_KEY_MAP      2
                           6162 BINARY_OP                6 (%)
                           6166 STORE_FAST               6 (@py_format3)
-                          6168 LOAD_CONST              59 ('assert %(py4)s')
-                          6170 LOAD_CONST              60 ('py4')
+                          6168 LOAD_CONST              62 ('assert %(py4)s')
+                          6170 LOAD_CONST              63 ('py4')
                           6172 LOAD_FAST                6 (@py_format3)
                           6174 BUILD_MAP                1
                           6176 BINARY_OP                6 (%)
                           6180 STORE_FAST               7 (@py_format5)
                           6182 LOAD_GLOBAL             43 (NULL + AssertionError)
                           6194 LOAD_GLOBAL             31 (NULL + @pytest_ar)
                           6206 LOAD_ATTR               22 (_format_explanation)
@@ -4166,16 +4168,16 @@
                  5508 to 5550 -> 5576 [1] lasti
                  5576 to 5582 -> 5584 [3] lasti
                  5590 to 5590 -> 5584 [3] lasti
                consts
                   None
                   1
                   2
+                  (52, 2)
                   (52, 1)
-                  (52, 0)
                   ('tips', 'waste_location', 'cleaner_location')
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 51
                      code
@@ -4208,22 +4210,25 @@
                      filename   '/home/runner/work/robotools/robotools/robotools/evotools/test_commands.py'
                      name       '<genexpr>'
                      firstlineno 222
                      lnotab 0x
                   'Even after completing the prepare_evo_aspirate_dispense_parameters method, not all tips are type Tip.'
                   'Grid \\(first number in waste_location tuple\\)'
                   ('match',)
-                  (68, 1)
-                  (0, 1)
-                  (1.7, 1)
+                  (68, 2)
+                  (0, 2)
+                  (1.7, 2)
                   'Site \\(second number in waste_location tuple\\)'
-                  (52, -1)
-                  (52, 128)
+                  (52, 0)
+                  (52, 129)
                   (52, 1.7)
                   'Grid \\(first number in cleaner_location tuple\\)'
+                  (68, 1)
+                  (0, 1)
+                  (1.7, 1)
                   'Site \\(second number in cleaner_location tuple\\)'
                   'Parameter arm'
                   ('tips', 'waste_location', 'cleaner_location', 'arm')
                   'waste_vol has to be a float'
                   -1.0
                   ('tips', 'waste_location', 'cleaner_location', 'waste_vol')
                   101.0
@@ -4319,17 +4324,17 @@
                
                539           2 LOAD_GLOBAL              1 (NULL + evo_wash)
                
                540          14 BUILD_LIST               0
                             16 LOAD_CONST               1 ((1, 2, 3, 4, 5, 6, 7, 8))
                             18 LIST_EXTEND              1
                
-               541          20 LOAD_CONST               2 ((52, 1))
+               541          20 LOAD_CONST               2 ((52, 2))
                
-               542          22 LOAD_CONST               3 ((52, 0))
+               542          22 LOAD_CONST               3 ((52, 1))
                
                539          24 KW_NAMES                 4
                             26 PRECALL                  3
                             30 CALL                     3
                             40 STORE_FAST               1 (cmd)
                
                544          42 LOAD_CONST               5 ('B;Wash(255,52,1,52,0,"3.0",500,"4.0",500,10,70,30,1,0,1000,0);')
@@ -4401,16 +4406,16 @@
                            370 STORE_FAST               2 (@py_assert2)
                
                545         372 LOAD_CONST               0 (None)
                            374 RETURN_VALUE
                consts
                   None
                   (1, 2, 3, 4, 5, 6, 7, 8)
+                  (52, 2)
                   (52, 1)
-                  (52, 0)
                   ('tips', 'waste_location', 'cleaner_location')
                   'B;Wash(255,52,1,52,0,"3.0",500,"4.0",500,10,70,30,1,0,1000,0);'
                   ('==',)
                   ('%(py0)s == %(py3)s',)
                   'cmd'
                   ('py0', 'py3')
                   'assert %(py5)s'
```

### Comparing `robotools-1.6.1/robotools/evotools/__pycache__/test_worklist.cpython-311-pytest-7.3.1.pyc` & `robotools-1.7.0/robotools/evotools/__pycache__/test_worklist.cpython-311-pytest-7.3.2.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 59566
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/evotools/__pycache__/types.cpython-311.pyc` & `robotools-1.7.0/robotools/evotools/__pycache__/types.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 1048
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/evotools/__pycache__/utils.cpython-311.pyc` & `robotools-1.7.0/robotools/evotools/__pycache__/utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 416
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x970064005a00640165016602640284045a0264035300
```

### Comparing `robotools-1.6.1/robotools/evotools/__pycache__/worklist.cpython-311.pyc` & `robotools-1.7.0/robotools/evotools/__pycache__/worklist.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 45274
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 32
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/evotools/commands.py` & `robotools-1.7.0/robotools/evotools/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module implements functions to create advanced worklist commands."""
-from typing import List, Optional, Sequence, Tuple, Union
+from typing import Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from robotools.evotools.exceptions import InvalidOperationError
 from robotools.evotools.types import Tip, int_to_tip
 from robotools.evotools.utils import to_hex
 
@@ -13,42 +13,42 @@
     "evo_make_selection_array",
     "evo_get_selection",
     "evo_aspirate",
     "evo_wash",
 )
 
 
-def evo_make_selection_array(rows: int, columns: int, wells: np.ndarray):
+def evo_make_selection_array(rows: int, columns: int, wells: Union[Iterable[str], np.ndarray]) -> np.ndarray:
     """Translate well IDs to a numpy array with 1s (selected) and 0s (not selected).
 
     Parameters
     ----------
     rows : int
         Number of rows of target labware object
     cols : int
         Number of columns of target labware object
-    wells : List[str]
+    wells : Union[Iterable[str], np.ndarray]
         Selected wells by well IDs as strings (e.g. ["A01", "B01"])
 
     Returns
     -------
     selection_array : np.ndarray
         Numpy array in labware dimensions with selected wells as 1 and others as 0
     """
     # create array with a shape beffiting the labware dimensions
     selection_array = np.zeros((rows, columns))
     # get a dictionary with the "coordinates" of well IDs (A01, B01 etc) as tuples
     well_index_dict = transform.make_well_index_dict(rows, columns)
     # insert 1s for all selected wells
-    for well in wells:
+    for well in np.asarray(wells).flatten():
         selection_array[well_index_dict[well]] = 1
     return selection_array
 
 
-def evo_get_selection(rows: int, cols: int, selected: np.ndarray):
+def evo_get_selection(rows: int, cols: int, selected: np.ndarray) -> str:
     """Function to generate the code string for the well selection of pipetting actions in EvoWare scripts (.esc).
 
     Adapted from the C++ function detailed in the EvoWare manual to Python by Martin Beyß (except the test at the end).
 
     Parameters
     ----------
     rows : int
@@ -104,30 +104,32 @@
     """Validates and prepares aspirate/dispense parameters.
 
     Parameters
     ----------
     wells : list of str
         List with target well ID(s)
     labware_position : tuple
-        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
+        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).
+        NOTE: The site numbering starts at 1.
     volume : int, float or list
         Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
     liquid_class : str, optional
         Overwrites the liquid class for this step (max 32 characters)
     tips : list of int
         Tip(s) that will be selected (out of tips 1-8)
     max_volume : int, optional
         Maximum allowed volume
 
     Returns
     -------
     wells : list of str
         List with target well ID(s)
     labware_position : tuple
-        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
+        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).
+        NOTE: The returned site number starts at 1.
     volume : list
         Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
     liquid_class : str, optional
         Overwrites the liquid class for this step (max 32 characters)
     tips : list of int
         Tip(s) that will be selected (out of tips 1-8)
     """
@@ -135,18 +137,20 @@
         raise ValueError("Missing required parameter: wells")
     if not isinstance(wells, (str, list, tuple, np.ndarray)):
         raise ValueError(f"Invalid wells: {wells}")
     if not len(wells) == len(tips):
         raise ValueError(f"Invalid wells: wells and tips need to have the same length.")
     if labware_position is None:
         raise ValueError("Missing required parameter: position")
-    if not all(isinstance(position, int) for position in labware_position) or any(
-        position < 0 for position in labware_position
-    ):
-        raise ValueError(f"Invalid position: {labware_position}")
+    grid, site = labware_position
+    if not isinstance(grid, int) or not 1 <= grid <= 67:
+        raise ValueError("Grid (first number in labware_position tuple) has to be an int from 1 - 67.")
+    if not isinstance(site, int) or not 1 <= site <= 128:
+        raise ValueError("Site (second number in labware_position tuple) has to be an int from 1 - 128.")
+    labware_position = (grid, site - 1)
 
     if volume is None:
         raise ValueError("Missing required parameter: volume")
     if isinstance(volume, list):
         for vol in volume:
             try:
                 vol = float(vol)
@@ -216,15 +220,16 @@
     n_rows
         Number of rows in the labware.
     n_columns
         Number of columns in the labware.
     wells : list of str
         List with target well ID(s)
     labware_position : tuple
-        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
+        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).
+        NOTE: The site numbering starts at 1.
     volume : int, float or list
         Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
     liquid_class : str, optional
         Overwrites the liquid class for this step (max 32 characters)
     tips : list
         Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8
     max_volume
@@ -289,15 +294,16 @@
     n_rows
         Number of rows in the labware.
     n_columns
         Number of columns in the labware.
     wells : list of str
         List with target well ID(s)
     labware_position : tuple
-        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2)
+        Grid position of the target labware on the robotic deck and site position on its carrier, e.g. labware on grid 38, site 2 -> (38,2).
+        NOTE: The site numbering starts at 1.
     volume : int, float or list
         Volume in microliters (will be rounded to 2 decimal places); if several tips are used, these tips may aspirate individual volumes -> use list in these cases
     liquid_class : str, optional
         Overwrites the liquid class for this step (max 32 characters)
     tips : list
         Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8
     max_volume
@@ -359,17 +365,17 @@
     """Validates and prepares aspirate/dispense parameters.
 
     Parameters
     ----------
     tips : list
         Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8
     waste_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of waste as integers
+        Tuple with grid position (1-67) and site number (1-128) of waste as integers
     cleaner_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers
+        Tuple with grid position (1-67) and site number (1-128) of cleaner as integers
     arm : int
         number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2
     waste_vol: float
         Volume in waste in mL (0-100)
     waste_delay : int
         Delay before closing valves in waste in ms (0-1000)
     cleaner_vol: float
@@ -427,24 +433,26 @@
         tecan_tips.append(tip)
 
     if waste_location is None:
         raise ValueError("Missing required parameter: waste_location")
     grid, site = waste_location
     if not isinstance(grid, int) or not 1 <= grid <= 67:
         raise ValueError("Grid (first number in waste_location tuple) has to be an int from 1 - 67.")
-    if not isinstance(site, int) or not 0 <= site <= 127:
-        raise ValueError("Site (second number in waste_location tuple) has to be an int from 0 - 127.")
+    if not isinstance(site, int) or not 1 <= site <= 128:
+        raise ValueError("Site (second number in waste_location tuple) has to be an int from 1 - 128.")
+    waste_location = (grid, site - 1)
 
     if cleaner_location is None:
         raise ValueError("Missing required parameter: cleaner_location")
     grid, site = cleaner_location
     if not isinstance(grid, int) or not 1 <= grid <= 67:
         raise ValueError("Grid (first number in cleaner_location tuple) has to be an int from 1 - 67.")
-    if not isinstance(site, int) or not 0 <= site <= 127:
-        raise ValueError("Site (second number in cleaner_location tuple) has to be an int from 0 - 127.")
+    if not isinstance(site, int) or not 1 <= site <= 128:
+        raise ValueError("Site (second number in cleaner_location tuple) has to be an int from 1 - 128.")
+    cleaner_location = (grid, site - 1)
 
     if arm is None:
         raise ValueError("Missing required paramter: arm")
     if not isinstance(arm, int):
         raise ValueError("Parameter arm is not int.")
     if not arm == 0 and not arm == 1:
         raise ValueError("Parameter arm has to be 0 (LiHa 1) or 1 (LiHa 2).")
@@ -540,17 +548,17 @@
     specifying the target wells.
 
     Parameters
     ----------
     tips : list
         Tip(s) that will be selected; use either a list with integers from 1 - 8 or with tip.T1 - tip.T8
     waste_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of waste as integers
+        Tuple with grid position (1-67) and site number (1-128) of waste as integers
     cleaner_location : tuple
-        Tuple with grid position (1-67) and site number (0-127) of cleaner as integers
+        Tuple with grid position (1-67) and site number (1-128) of cleaner as integers
     arm : int
         number of the LiHa performing the action: 0 = LiHa 1, 1 = LiHa 2
     waste_vol: float
         Volume in waste in mL (0-100)
     waste_delay : int
         Delay before closing valves in waste in ms (0-1000)
     cleaner_vol: float
```

### Comparing `robotools-1.6.1/robotools/evotools/test_commands.py` & `robotools-1.7.0/robotools/evotools/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,23 +46,23 @@
                 wells="A01",
                 labware_position=(38, 2),
                 volume=15,
                 liquid_class="Water_DispZmax-1_AspZmax-1",
                 tips=[1, 2],
             )
         # test labware_position argument checks
-        with pytest.raises(ValueError, match="Invalid position:"):
+        with pytest.raises(ValueError, match="second number in labware_position"):
             prepare_evo_aspirate_dispense_parameters(
                 wells=["A01", "B01"],
-                labware_position=(38, -1),
+                labware_position=(38, 0),
                 volume=15,
                 liquid_class="Water_DispZmax-1_AspZmax-1",
                 tips=[1, 2],
             )
-        with pytest.raises(ValueError, match="Invalid position:"):
+        with pytest.raises(ValueError, match="first number in labware_position"):
             prepare_evo_aspirate_dispense_parameters(
                 wells=["A01", "B01"],
                 labware_position=("a", 2),
                 volume=15,
                 liquid_class="Water_DispZmax-1_AspZmax-1",
                 tips=[1, 2],
             )
@@ -128,15 +128,15 @@
                 liquid_class="Water_DispZmax-1_AspZmax-1",
                 tips=[1, 2],
             )
 
         # test complete prepare_evo_aspirate_dispense_parameters() command
         actual = prepare_evo_aspirate_dispense_parameters(
             wells=["E01", "F01", "G01"],
-            labware_position=(38, 2),
+            labware_position=(38, 3),
             volume=750,
             liquid_class="Water_DispZmax_AspZmax",
             tips=[5, 6, 7],
         )
         expected = (
             ["E01", "F01", "G01"],
             (38, 2),
@@ -149,30 +149,30 @@
 
 class TestEvoAspirate:
     def test_evo_aspirate1(self) -> None:
         cmd = evo_aspirate(
             n_rows=8,
             n_columns=12,
             wells=["E01", "F01", "G01"],
-            labware_position=(38, 2),
+            labware_position=(38, 3),
             tips=[5, 6, 7],
             volume=750,
             liquid_class="Water_DispZmax_AspZmax",
             max_volume=950,
         )
         exp = 'B;Aspirate(112,"Water_DispZmax_AspZmax",0,0,0,0,"750.0","750.0","750.0",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
         assert cmd == exp
         return
 
     def test_evo_aspirate2(self) -> None:
         cmd = evo_aspirate(
             n_rows=8,
             n_columns=12,
             wells=["E01", "F01", "G01"],
-            labware_position=(38, 2),
+            labware_position=(38, 3),
             tips=[5, 6, 7],
             volume=[750, 730, 710],
             liquid_class="Water_DispZmax_AspZmax",
             max_volume=950,
         )
         exp = 'B;Aspirate(112,"Water_DispZmax_AspZmax",0,0,0,0,"750","730","710",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
         assert cmd == exp
@@ -181,30 +181,30 @@
 
 class TestEvoDispense:
     def test_evo_dispense1(self) -> None:
         cmd = evo_dispense(
             n_rows=8,
             n_columns=12,
             wells=["E01", "F01", "G01"],
-            labware_position=(38, 2),
+            labware_position=(38, 3),
             tips=[5, 6, 7],
             volume=750,
             liquid_class="Water_DispZmax_AspZmax",
             max_volume=950,
         )
         exp = 'B;Dispense(112,"Water_DispZmax_AspZmax",0,0,0,0,"750.0","750.0","750.0",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
         assert cmd == exp
         return
 
     def test_evo_dispense2(self) -> None:
         cmd = evo_dispense(
             n_rows=8,
             n_columns=12,
             wells=["E01", "F01", "G01"],
-            labware_position=(38, 2),
+            labware_position=(38, 3),
             tips=[5, 6, 7],
             volume=[750, 730, 710],
             liquid_class="Water_DispZmax_AspZmax",
             max_volume=950,
         )
         exp = 'B;Dispense(112,"Water_DispZmax_AspZmax",0,0,0,0,"750","730","710",0,0,0,0,0,38,2,1,"0C08\xa00000000000000",0,0);'
         assert cmd == exp
@@ -212,58 +212,58 @@
 
 
 class TestEvoWash:
     def test_prepare_evo_wash_parameters_checking(self):
         # test tips argument checks
         tips, _, _, _, _, _, _, _, _, _, _, _, _ = prepare_evo_wash_parameters(
             tips=[1, 2],
-            waste_location=(52, 1),
-            cleaner_location=(52, 0),
+            waste_location=(52, 2),
+            cleaner_location=(52, 1),
         )
         if not all(isinstance(n, Tip) for n in tips):
             raise TypeError(
                 f"Even after completing the prepare_evo_aspirate_dispense_parameters method, not all tips are type Tip."
             )
 
         # test waste_location argument checks
         with pytest.raises(ValueError, match="Grid \\(first number in waste_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(68, 1),
-                cleaner_location=(52, 0),
+                waste_location=(68, 2),
+                cleaner_location=(52, 1),
             )
         with pytest.raises(ValueError, match="Grid \\(first number in waste_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(0, 1),
-                cleaner_location=(52, 0),
+                waste_location=(0, 2),
+                cleaner_location=(52, 1),
             )
         with pytest.raises(ValueError, match="Grid \\(first number in waste_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(1.7, 1),
-                cleaner_location=(52, 0),
+                waste_location=(1.7, 2),
+                cleaner_location=(52, 1),
             )
         with pytest.raises(ValueError, match="Site \\(second number in waste_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, -1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 0),
+                cleaner_location=(52, 1),
             )
         with pytest.raises(ValueError, match="Site \\(second number in waste_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 128),
-                cleaner_location=(52, 0),
+                waste_location=(52, 129),
+                cleaner_location=(52, 1),
             )
         with pytest.raises(ValueError, match="Site \\(second number in waste_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
                 waste_location=(52, 1.7),
-                cleaner_location=(52, 0),
+                cleaner_location=(52, 1),
             )
 
         # test cleaner_location argument checks
         with pytest.raises(ValueError, match="Grid \\(first number in cleaner_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
                 waste_location=(52, 1),
@@ -281,236 +281,236 @@
                 waste_location=(52, 1),
                 cleaner_location=(1.7, 1),
             )
         with pytest.raises(ValueError, match="Site \\(second number in cleaner_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
                 waste_location=(52, 1),
-                cleaner_location=(52, -1),
+                cleaner_location=(52, 0),
             )
         with pytest.raises(ValueError, match="Site \\(second number in cleaner_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
                 waste_location=(52, 1),
-                cleaner_location=(52, 128),
+                cleaner_location=(52, 129),
             )
         with pytest.raises(ValueError, match="Site \\(second number in cleaner_location tuple\\)"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
                 waste_location=(52, 1),
                 cleaner_location=(52, 1.7),
             )
 
         # test arm argument check
         with pytest.raises(ValueError, match="Parameter arm"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 arm=2,
             )
 
         # test waste_vol argument check
         with pytest.raises(ValueError, match="waste_vol has to be a float"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 waste_vol=-1.0,
             )
         with pytest.raises(ValueError, match="waste_vol has to be a float"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 waste_vol=101.0,
             )
         with pytest.raises(ValueError, match="waste_vol has to be a float"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 waste_vol=1,
             )
 
         # test waste_delay argument check
         with pytest.raises(ValueError, match="waste_delay has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 waste_delay=-1,
             )
         with pytest.raises(ValueError, match="waste_delay has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 waste_delay=1001,
             )
         with pytest.raises(ValueError, match="waste_delay has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 waste_delay=10.0,
             )
 
         # test cleaner_vol argument check
         with pytest.raises(ValueError, match="cleaner_vol has to be a float"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 cleaner_vol=-1.0,
             )
         with pytest.raises(ValueError, match="cleaner_vol has to be a float"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 cleaner_vol=101.0,
             )
         with pytest.raises(ValueError, match="cleaner_vol has to be a float"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 cleaner_vol=1,
             )
 
         # test cleaner_delay argument check
         with pytest.raises(ValueError, match="cleaner_delay has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 cleaner_delay=-1,
             )
         with pytest.raises(ValueError, match="cleaner_delay has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 cleaner_delay=1001,
             )
         with pytest.raises(ValueError, match="cleaner_delay has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 cleaner_delay=10.0,
             )
 
         # test airgap argument check
         with pytest.raises(ValueError, match="airgap has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 airgap=-1,
             )
         with pytest.raises(ValueError, match="airgap has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 airgap=101,
             )
         with pytest.raises(ValueError, match="airgap has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 airgap=10.0,
             )
 
         # test airgap_speed argument check
         with pytest.raises(ValueError, match="airgap_speed has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 airgap_speed=0,
             )
         with pytest.raises(ValueError, match="airgap_speed has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 airgap_speed=1001,
             )
         with pytest.raises(ValueError, match="airgap_speed has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 airgap_speed=10.0,
             )
 
         # test retract_speed argument check
         with pytest.raises(ValueError, match="retract_speed has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 retract_speed=0,
             )
         with pytest.raises(ValueError, match="retract_speed has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 retract_speed=101,
             )
         with pytest.raises(ValueError, match="retract_speed has to be an int"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 retract_speed=10.0,
             )
 
         # test fastwash argument check
         with pytest.raises(ValueError, match="Parameter fastwash"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 fastwash=2,
             )
         with pytest.raises(ValueError, match="Parameter fastwash"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 fastwash=1.0,
             )
 
         # test low_volume argument check
         with pytest.raises(ValueError, match="Parameter low_volume"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 low_volume=2,
             )
         with pytest.raises(ValueError, match="Parameter low_volume"):
             prepare_evo_wash_parameters(
                 tips=[1, 2],
-                waste_location=(52, 1),
-                cleaner_location=(52, 0),
+                waste_location=(52, 2),
+                cleaner_location=(52, 1),
                 low_volume=1.0,
             )
 
         # test complete prepare_evo_wash_parameters() command
         actual = prepare_evo_wash_parameters(
             tips=[1, 2, 3, 4, 5, 6, 7, 8],
-            waste_location=(52, 1),
-            cleaner_location=(52, 0),
+            waste_location=(52, 2),
+            cleaner_location=(52, 1),
         )
         expected = (
             [
                 Tip.T1,
                 Tip.T2,
                 Tip.T3,
                 Tip.T4,
@@ -534,12 +534,12 @@
         )
         assert actual == expected
         return
 
     def test_evo_wash(self) -> None:
         cmd = evo_wash(
             tips=[1, 2, 3, 4, 5, 6, 7, 8],
-            waste_location=(52, 1),
-            cleaner_location=(52, 0),
+            waste_location=(52, 2),
+            cleaner_location=(52, 1),
         )
         assert cmd == 'B;Wash(255,52,1,52,0,"3.0",500,"4.0",500,10,70,30,1,0,1000,0);'
         return
```

### Comparing `robotools-1.6.1/robotools/evotools/test_worklist.py` & `robotools-1.7.0/robotools/evotools/test_worklist.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/evotools/types.py` & `robotools-1.7.0/robotools/evotools/types.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/evotools/worklist.py` & `robotools-1.7.0/robotools/evotools/worklist.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/liquidhandling/__pycache__/composition.cpython-311.pyc` & `robotools-1.7.0/robotools/liquidhandling/__pycache__/composition.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 5455
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 14
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/liquidhandling/__pycache__/exceptions.cpython-311.pyc` & `robotools-1.7.0/robotools/liquidhandling/__pycache__/exceptions.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 1355
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/liquidhandling/__pycache__/labware.cpython-311.pyc` & `robotools-1.7.0/robotools/liquidhandling/__pycache__/labware.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 14683
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/liquidhandling/__pycache__/test_composition.cpython-311-pytest-7.3.1.pyc` & `robotools-1.7.0/robotools/liquidhandling/__pycache__/test_composition.cpython-311-pytest-7.3.2.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 14399
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/liquidhandling/__pycache__/test_labware.cpython-311-pytest-7.3.1.pyc` & `robotools-1.7.0/robotools/liquidhandling/__pycache__/test_labware.cpython-311-pytest-7.3.2.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb67d8064 (Wed Jun  7 12:53:10 2023 UTC)
+moddate:  0x57f29264 (Wed Jun 21 12:51:35 2023 UTC)
 files sz: 10190
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `robotools-1.6.1/robotools/liquidhandling/composition.py` & `robotools-1.7.0/robotools/liquidhandling/composition.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/liquidhandling/exceptions.py` & `robotools-1.7.0/robotools/liquidhandling/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/liquidhandling/labware.py` & `robotools-1.7.0/robotools/liquidhandling/labware.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/liquidhandling/test_composition.py` & `robotools-1.7.0/robotools/liquidhandling/test_composition.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/liquidhandling/test_labware.py` & `robotools-1.7.0/robotools/liquidhandling/test_labware.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/test_transform.py` & `robotools-1.7.0/robotools/test_transform.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/test_utils.py` & `robotools-1.7.0/robotools/test_utils.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/transform.py` & `robotools-1.7.0/robotools/transform.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools/utils.py` & `robotools-1.7.0/robotools/utils.py`

 * *Files identical despite different names*

### Comparing `robotools-1.6.1/robotools.egg-info/PKG-INFO` & `robotools-1.7.0/robotools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotools
-Version: 1.6.1
+Version: 1.7.0
 Summary: Pythonic in-silico liquid handling and creation of Tecan FreedomEVO worklists.
 Home-page: https://github.com/jubiotech/robotools
-Download-URL: https://github.com/jubiotech/robotools/tarball/1.6.1
+Download-URL: https://github.com/jubiotech/robotools/tarball/1.7.0
 Author: Michael Osthege
 Author-email: m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `robotools-1.6.1/robotools.egg-info/SOURCES.txt` & `robotools-1.7.0/robotools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 robotools/utils.py
 robotools.egg-info/PKG-INFO
 robotools.egg-info/SOURCES.txt
 robotools.egg-info/dependency_links.txt
 robotools.egg-info/requires.txt
 robotools.egg-info/top_level.txt
 robotools/__pycache__/__init__.cpython-311.pyc
-robotools/__pycache__/test_transform.cpython-311-pytest-7.3.1.pyc
-robotools/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+robotools/__pycache__/test_transform.cpython-311-pytest-7.3.2.pyc
+robotools/__pycache__/test_utils.cpython-311-pytest-7.3.2.pyc
 robotools/__pycache__/transform.cpython-311.pyc
 robotools/__pycache__/utils.cpython-311.pyc
 robotools/evotools/__init__.py
 robotools/evotools/commands.py
 robotools/evotools/exceptions.py
 robotools/evotools/test_commands.py
 robotools/evotools/test_worklist.py
 robotools/evotools/types.py
 robotools/evotools/utils.py
 robotools/evotools/worklist.py
 robotools/evotools/__pycache__/__init__.cpython-311.pyc
 robotools/evotools/__pycache__/commands.cpython-311.pyc
 robotools/evotools/__pycache__/exceptions.cpython-311.pyc
-robotools/evotools/__pycache__/test_commands.cpython-311-pytest-7.3.1.pyc
-robotools/evotools/__pycache__/test_worklist.cpython-311-pytest-7.3.1.pyc
+robotools/evotools/__pycache__/test_commands.cpython-311-pytest-7.3.2.pyc
+robotools/evotools/__pycache__/test_worklist.cpython-311-pytest-7.3.2.pyc
 robotools/evotools/__pycache__/types.cpython-311.pyc
 robotools/evotools/__pycache__/utils.cpython-311.pyc
 robotools/evotools/__pycache__/worklist.cpython-311.pyc
 robotools/liquidhandling/__init__.py
 robotools/liquidhandling/composition.py
 robotools/liquidhandling/exceptions.py
 robotools/liquidhandling/labware.py
 robotools/liquidhandling/test_composition.py
 robotools/liquidhandling/test_labware.py
 robotools/liquidhandling/__pycache__/__init__.cpython-311.pyc
 robotools/liquidhandling/__pycache__/composition.cpython-311.pyc
 robotools/liquidhandling/__pycache__/exceptions.cpython-311.pyc
 robotools/liquidhandling/__pycache__/labware.cpython-311.pyc
-robotools/liquidhandling/__pycache__/test_composition.cpython-311-pytest-7.3.1.pyc
-robotools/liquidhandling/__pycache__/test_labware.cpython-311-pytest-7.3.1.pyc
+robotools/liquidhandling/__pycache__/test_composition.cpython-311-pytest-7.3.2.pyc
+robotools/liquidhandling/__pycache__/test_labware.cpython-311-pytest-7.3.2.pyc
```

### Comparing `robotools-1.6.1/setup.py` & `robotools-1.7.0/setup.py`

 * *Files identical despite different names*

