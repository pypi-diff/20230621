# Comparing `tmp/piel-0.0.26.tar.gz` & `tmp/piel-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.26.tar", last modified: Mon Jun 19 09:42:09 2023, max compression
+gzip compressed data, was "piel-0.0.29.tar", last modified: Wed Jun 21 15:17:29 2023, max compression
```

## Comparing `piel-0.0.26.tar` & `piel-0.0.29.tar`

### file list

```diff
@@ -1,72 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-19 09:41:52.000000 piel-0.0.26/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-19 09:41:52.000000 piel-0.0.26/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 09:41:52.000000 piel-0.0.26/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-19 09:41:52.000000 piel-0.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-19 09:41:52.000000 piel-0.0.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-19 09:42:09.537931 piel-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-19 09:41:52.000000 piel-0.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-19 09:41:52.000000 piel-0.0.26/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 09:41:52.000000 piel-0.0.26/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/file_system/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/gdsfactory/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/openlane_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/openlane_v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/openlane_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/openlane_v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/autoapi/piel/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-19 09:41:52.000000 piel-0.0.26/docs/autoapi/piel/simulation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-19 09:41:52.000000 piel-0.0.26/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-19 09:41:52.000000 piel-0.0.26/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.529931 piel-0.0.26/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.529931 piel-0.0.26/docs/examples/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/examples/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-19 09:41:52.000000 piel-0.0.26/docs/examples/simple_design/tb/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 09:41:52.000000 piel-0.0.26/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 09:41:52.000000 piel-0.0.26/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 09:41:52.000000 piel-0.0.26/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 09:41:52.000000 piel-0.0.26/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 09:41:52.000000 piel-0.0.26/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.529931 piel-0.0.26/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.533931 piel-0.0.26/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-19 09:41:52.000000 piel-0.0.26/docs/sections/environment/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 09:41:52.000000 piel-0.0.26/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-19 09:41:52.000000 piel-0.0.26/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 09:41:52.000000 piel-0.0.26/piel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-19 09:41:52.000000 piel-0.0.26/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-19 09:41:52.000000 piel-0.0.26/piel/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-19 09:41:52.000000 piel-0.0.26/piel/gdsfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-19 09:41:52.000000 piel-0.0.26/piel/openlane_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-19 09:41:52.000000 piel-0.0.26/piel/openlane_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-19 09:41:52.000000 piel-0.0.26/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 09:41:52.000000 piel-0.0.26/piel/piel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-19 09:41:52.000000 piel-0.0.26/piel/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 09:42:09.000000 piel-0.0.26/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 09:42:09.537931 piel-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-19 09:41:52.000000 piel-0.0.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:42:09.537931 piel-0.0.26/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 09:41:52.000000 piel-0.0.26/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-19 09:41:52.000000 piel-0.0.26/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.394924 piel-0.0.29/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 15:17:08.000000 piel-0.0.29/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-21 15:17:08.000000 piel-0.0.29/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 15:17:08.000000 piel-0.0.29/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 15:17:08.000000 piel-0.0.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 15:17:08.000000 piel-0.0.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-21 15:17:29.394924 piel-0.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-21 15:17:08.000000 piel-0.0.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 15:17:08.000000 piel-0.0.29/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 15:17:08.000000 piel-0.0.29/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/file_system/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/gdsfactory/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/parse_results_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/parse_results_v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/openlane/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/openlane/v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.386924 piel-0.0.29/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/autoapi/piel/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 15:17:08.000000 piel-0.0.29/docs/autoapi/piel/piel/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-21 15:17:08.000000 piel-0.0.29/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 15:17:08.000000 piel-0.0.29/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.378924 piel-0.0.29/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.378924 piel-0.0.29/docs/examples/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.378924 piel-0.0.29/docs/examples/simple_design/tb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/examples/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-21 15:17:08.000000 piel-0.0.29/docs/examples/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 15:17:08.000000 piel-0.0.29/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 15:17:08.000000 piel-0.0.29/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 15:17:08.000000 piel-0.0.29/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-21 15:17:08.000000 piel-0.0.29/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 15:17:08.000000 piel-0.0.29/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.382924 piel-0.0.29/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 15:17:08.000000 piel-0.0.29/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-21 15:17:08.000000 piel-0.0.29/docs/sections/environment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 15:17:08.000000 piel-0.0.29/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 15:17:08.000000 piel-0.0.29/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-21 15:17:08.000000 piel-0.0.29/piel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-21 15:17:08.000000 piel-0.0.29/piel/cocotb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-21 15:17:08.000000 piel-0.0.29/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-06-21 15:17:08.000000 piel-0.0.29/piel/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 15:17:08.000000 piel-0.0.29/piel/gdsfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.394924 piel-0.0.29/piel/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/parse_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-21 15:17:08.000000 piel-0.0.29/piel/openlane/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-21 15:17:08.000000 piel-0.0.29/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 15:17:08.000000 piel-0.0.29/piel/piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.390924 piel-0.0.29/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 15:17:29.000000 piel-0.0.29/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-21 15:17:29.394924 piel-0.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-21 15:17:08.000000 piel-0.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:17:29.394924 piel-0.0.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 15:17:08.000000 piel-0.0.29/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-21 15:17:08.000000 piel-0.0.29/tests/test_piel.py
```

### Comparing `piel-0.0.26/CONTRIBUTING.rst` & `piel-0.0.29/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.26/LICENSE` & `piel-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.26/PKG-INFO` & `piel-0.0.29/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.26
+Version: 0.0.29
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,19 +12,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-# `piel` - Photonic-Electronic Simulation and System Design
+# `piel` - Photonic and Integrated ELectronic system design
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
 Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 
@@ -32,21 +33,25 @@
 - Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
 
 ## Target functionality
 * Co-simulation and optimisation between integrated photonic and electronic chip design.
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
 
+`piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
+
 ## Dependency Toolset
-* `gdsfactory` for the photonic design
-* `OpenROAD OpenLane` for the micro-electronic layout design
-* `verilator` for the digital HDL simulations
-* `cocotb` for python-based testbench modelling
-* `porf` my custom package for `OpenROAD` data extraction.
-* [Future] FPGA modelling and integration
+This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+
+Some individual tools already integrated are:
+* [cocotb](https://github.com/cocotb/cocotb) - implements the methods that allow the testbenching configuration of signal stimulus to the electronic logic directly from Python.
+* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - implements the RTL-to-GDSII flow for the
+  electronic logic and outputs performance parameters of the implemented circuitry.
+
+Coming next GDSFactory netlisting and layout integration.
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
```

### Comparing `piel-0.0.26/README.md` & `piel-0.0.29/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `piel` - Photonic-Electronic Simulation and System Design
+# `piel` - Photonic and Integrated ELectronic system design
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
 Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 
@@ -10,21 +10,25 @@
 - Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
 
 ## Target functionality
 * Co-simulation and optimisation between integrated photonic and electronic chip design.
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
 
+`piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
+
 ## Dependency Toolset
-* `gdsfactory` for the photonic design
-* `OpenROAD OpenLane` for the micro-electronic layout design
-* `verilator` for the digital HDL simulations
-* `cocotb` for python-based testbench modelling
-* `porf` my custom package for `OpenROAD` data extraction.
-* [Future] FPGA modelling and integration
+This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+
+Some individual tools already integrated are:
+* [cocotb](https://github.com/cocotb/cocotb) - implements the methods that allow the testbenching configuration of signal stimulus to the electronic logic directly from Python.
+* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - implements the RTL-to-GDSII flow for the
+  electronic logic and outputs performance parameters of the implemented circuitry.
+
+Coming next GDSFactory netlisting and layout integration.
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
```

### Comparing `piel-0.0.26/docs/Makefile` & `piel-0.0.29/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.26/docs/autoapi/piel/openlane_v2/index.rst` & `piel-0.0.29/docs/autoapi/piel/openlane/v2/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-:py:mod:`piel.openlane_v2`
+:py:mod:`piel.openlane.v2`
 ==========================
 
-.. py:module:: piel.openlane_v2
+.. py:module:: piel.openlane.v2
 
 
 Module Contents
 ---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.openlane_v2.run_openlane_flow
+   piel.openlane.v2.run_openlane_flow
 
 
 
 .. py:function:: run_openlane_flow(configuration: dict | None = test_spm_open_lane_configuration, design_directory: str = '/foss/designs/spm') -> None
 
    Runs the OpenLane flow.
 
    :param configuration: OpenLane configuration dictionary. If none is present it will default to the config.json file on the design_directory.
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
-
-
```

### Comparing `piel-0.0.26/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.29/docs/autoapi/piel/parametric/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -16,16 +16,28 @@
    piel.parametric.single_parameter_sweep
    piel.parametric.multi_parameter_sweep
 
 
 
 .. py:function:: single_parameter_sweep(base_design_configuration: dict, parameter_name: str, parameter_sweep_values: list)
 
+   This function takes a base_design_configuration dictionary and sweeps a single parameter over a list of values. It returns a list of dictionaries that correspond to the parameter sweep.
 
-.. py:function:: multi_parameter_sweep(base_design_configuration: dict, parameter_sweep_dictionary: dict)
+   :param base_design_configuration: Base design configuration dictionary.
+   :type base_design_configuration: dict
+   :param parameter_name: Name of parameter to sweep.
+   :type parameter_name: str
+   :param parameter_sweep_values: List of values to sweep.
+   :type parameter_sweep_values: list
+
+   :returns: List of dictionaries that correspond to the parameter sweep.
+   :rtype: parameter_sweep_design_dictionary_array(list)
+
+
+.. py:function:: multi_parameter_sweep(base_design_configuration: dict, parameter_sweep_dictionary: dict) -> list
 
    This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping `parameter_1 = np.arange(0, 2) = array([0, 1])`, and `parameter_2 = np.arange(2, 4) = array([2, 3])`, then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
 
    For the example above, there arould be 4 combinations [(0, 2), (0, 3), (1, 2), (1, 3)].
 
    If you were instead sweeping for `parameter_1 = np.arange(0, 5)` and `parameter_2 = np.arange(0, 5)`, the dictionary generated would correspond to these parameter combinations of::
        [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
@@ -38,11 +50,17 @@
            "parameter_1": np.arange(1, -40, 1),
            "parameter_2": np.arange(1, -40, 1),
        }
 
        example_base_design_configuration = {
            "parameter_1": 10.0,
            "parameter_2": 40.0,
-           "parameter_3": 0
+           "parameter_3": 0,
        }
 
+   :param base_design_configuration: Dictionary of the default design configuration.
+   :type base_design_configuration: dict
+   :param parameter_sweep_dictionary: Dictionary of the parameter sweep. The keys should be the same as the keys in the base_design_configuration dictionary.
+   :type parameter_sweep_dictionary: dict
 
+   :returns: List of dictionaries that comprise of all the possible combinations of your parameter sweeps.
+   :rtype: parameter_sweep_design_dictionary_array(list)
```

### Comparing `piel-0.0.26/docs/conf.py` & `piel-0.0.29/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.26/docs/examples/simple_design/tb/Makefile` & `piel-0.0.29/docs/examples/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.26/docs/make.bat` & `piel-0.0.29/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.26/piel/defaults.py` & `piel-0.0.29/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.26/piel/openlane_v2.py` & `piel-0.0.29/piel/openlane/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import openlane
-from .defaults import test_spm_open_lane_configuration
+from piel.defaults import test_spm_open_lane_configuration
 
 
 def run_openlane_flow(
     configuration: dict | None = test_spm_open_lane_configuration,
     design_directory: str = "/foss/designs/spm",
 ) -> None:
     """
```

### Comparing `piel-0.0.26/piel/parametric.py` & `piel-0.0.29/piel/parametric.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,37 @@
+import itertools
+
+
 def single_parameter_sweep(
     base_design_configuration: dict,
     parameter_name: str,
     parameter_sweep_values: list,
 ):
+    """
+    This function takes a base_design_configuration dictionary and sweeps a single parameter over a list of values. It returns a list of dictionaries that correspond to the parameter sweep.
+
+    Args:
+        base_design_configuration(dict): Base design configuration dictionary.
+        parameter_name(str): Name of parameter to sweep.
+        parameter_sweep_values(list): List of values to sweep.
+
+    Returns:
+        parameter_sweep_design_dictionary_array(list): List of dictionaries that correspond to the parameter sweep.
+    """
     parameter_sweep_design_dictionary_array = []
     for parameter in parameter_sweep_values:
         design = base_design_configuration.copy()
         design[parameter_name] = parameter
         parameter_sweep_design_dictionary_array.extend([design])
     return parameter_sweep_design_dictionary_array
 
 
 def multi_parameter_sweep(
     base_design_configuration: dict, parameter_sweep_dictionary: dict
-):
+) -> list:
     """
     This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping `parameter_1 = np.arange(0, 2) = array([0, 1])`, and `parameter_2 = np.arange(2, 4) = array([2, 3])`, then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
 
     For the example above, there arould be 4 combinations [(0, 2), (0, 3), (1, 2), (1, 3)].
 
     If you were instead sweeping for `parameter_1 = np.arange(0, 5)` and `parameter_2 = np.arange(0, 5)`, the dictionary generated would correspond to these parameter combinations of::
         [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
@@ -30,16 +44,23 @@
             "parameter_1": np.arange(1, -40, 1),
             "parameter_2": np.arange(1, -40, 1),
         }
 
         example_base_design_configuration = {
             "parameter_1": 10.0,
             "parameter_2": 40.0,
-            "parameter_3": 0
+            "parameter_3": 0,
         }
+
+    Args:
+        base_design_configuration(dict): Dictionary of the default design configuration.
+        parameter_sweep_dictionary(dict): Dictionary of the parameter sweep. The keys should be the same as the keys in the base_design_configuration dictionary.
+
+    Returns:
+        parameter_sweep_design_dictionary_array(list): List of dictionaries that comprise of all the possible combinations of your parameter sweeps.
     """
     parameter_names_sweep_list = []
     parameter_sweep_values_list = []
     parameter_sweep_design_dictionary_array = []
 
     for parameter_sweep_name in parameter_sweep_dictionary.keys():
         parameter_names_sweep_list.extend([parameter_sweep_name])
```

### Comparing `piel-0.0.26/piel.egg-info/PKG-INFO` & `piel-0.0.29/piel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.26
+Version: 0.0.29
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,19 +12,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-# `piel` - Photonic-Electronic Simulation and System Design
+# `piel` - Photonic and Integrated ELectronic system design
 [![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
 [![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
 [![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
 [![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
 
 Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 
@@ -32,21 +33,25 @@
 - Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
 
 ## Target functionality
 * Co-simulation and optimisation between integrated photonic and electronic chip design.
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
 
+`piel` aims to provide an integrated workflow to co-design photonics and electronics. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
+
 ## Dependency Toolset
-* `gdsfactory` for the photonic design
-* `OpenROAD OpenLane` for the micro-electronic layout design
-* `verilator` for the digital HDL simulations
-* `cocotb` for python-based testbench modelling
-* `porf` my custom package for `OpenROAD` data extraction.
-* [Future] FPGA modelling and integration
+This package provides a wrapper to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+
+Some individual tools already integrated are:
+* [cocotb](https://github.com/cocotb/cocotb) - implements the methods that allow the testbenching configuration of signal stimulus to the electronic logic directly from Python.
+* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - implements the RTL-to-GDSII flow for the
+  electronic logic and outputs performance parameters of the implemented circuitry.
+
+Coming next GDSFactory netlisting and layout integration.
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
 
 ## Credits
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template.
```

### Comparing `piel-0.0.26/piel.egg-info/SOURCES.txt` & `piel-0.0.29/piel.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,36 +15,43 @@
 docs/index.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 docs/autoapi/index.rst
 docs/autoapi/piel/index.rst
 docs/autoapi/piel/cli/index.rst
+docs/autoapi/piel/cocotb/index.rst
 docs/autoapi/piel/defaults/index.rst
 docs/autoapi/piel/file_system/index.rst
 docs/autoapi/piel/gdsfactory/index.rst
-docs/autoapi/piel/openlane_v1/index.rst
-docs/autoapi/piel/openlane_v2/index.rst
+docs/autoapi/piel/openlane/index.rst
+docs/autoapi/piel/openlane/parse_results_v1/index.rst
+docs/autoapi/piel/openlane/utils/index.rst
+docs/autoapi/piel/openlane/v1/index.rst
+docs/autoapi/piel/openlane/v2/index.rst
 docs/autoapi/piel/parametric/index.rst
 docs/autoapi/piel/piel/index.rst
-docs/autoapi/piel/simulation/index.rst
-docs/examples/simple_design/tb/Makefile
+docs/examples/simple_design/tb/default/Makefile
+docs/sections/codesign/index.rst
 docs/sections/environment/index.rst
 piel/__init__.py
 piel/cli.py
+piel/cocotb.py
 piel/defaults.py
 piel/file_system.py
 piel/gdsfactory.py
-piel/openlane_v1.py
-piel/openlane_v2.py
 piel/parametric.py
 piel/piel.py
-piel/simulation.py
 piel.egg-info/PKG-INFO
 piel.egg-info/SOURCES.txt
 piel.egg-info/dependency_links.txt
 piel.egg-info/entry_points.txt
 piel.egg-info/not-zip-safe
 piel.egg-info/requires.txt
 piel.egg-info/top_level.txt
+piel/openlane/__init__.py
+piel/openlane/parse_results_v1.py
+piel/openlane/utils.py
+piel/openlane/v1.py
+piel/openlane/v2.py
 tests/__init__.py
 tests/test_piel.py
```

### Comparing `piel-0.0.26/setup.py` & `piel-0.0.29/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,18 +54,19 @@
             "myst_parser",
             "pandoc",
             "flake8",
         ]
     },
     install_requires=requirements,
     license="MIT license",
+    long_description_content_type="text/markdown",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
-    url='https://github.com/daquintero/piel',
-    version="0.0.26",
+    url="https://github.com/daquintero/piel",
+    version="0.0.29",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.26/tests/test_piel.py` & `piel-0.0.29/tests/test_piel.py`

 * *Files identical despite different names*

