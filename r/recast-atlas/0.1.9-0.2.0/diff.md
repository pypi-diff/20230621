# Comparing `tmp/recast_atlas-0.1.9.tar.gz` & `tmp/recast_atlas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recast_atlas-0.1.9.tar", last modified: Tue Dec 21 18:13:40 2021, max compression
+gzip compressed data, was "recast_atlas-0.2.0.tar", last modified: Tue Jun 20 22:48:25 2023, max compression
```

## Comparing `recast_atlas-0.1.9.tar` & `recast_atlas-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.674192 recast_atlas-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    10759 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2021-12-21 18:13:40.674192 recast_atlas-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      365 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2021-12-21 18:13:40.674192 recast_atlas-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.666191 recast_atlas-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.670192 recast_atlas-0.1.9/src/recast_atlas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2021-12-21 18:13:40.000000 recast_atlas-0.1.9/src/recast_atlas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-12-21 18:13:40.000000 recast_atlas-0.1.9/src/recast_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-21 18:13:40.000000 recast_atlas-0.1.9/src/recast_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-12-21 18:13:40.000000 recast_atlas-0.1.9/src/recast_atlas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-12-21 18:13:40.000000 recast_atlas-0.1.9/src/recast_atlas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-21 18:13:40.000000 recast_atlas-0.1.9/src/recast_atlas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.670192 recast_atlas-0.1.9/src/recastatlas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.670192 recast_atlas-0.1.9/src/recastatlas/backends/
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/backends/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/backends/reana.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4715 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.670192 recast_atlas-0.1.9/src/recastatlas/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.670192 recast_atlas-0.1.9/src/recastatlas/data/catalogue/
--rw-r--r--   0 runner    (1001) docker     (121)      710 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/catalogue/busyboxtest.yml
--rw-r--r--   0 runner    (1001) docker     (121)      422 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/catalogue/examples_checkmate1.yml
--rw-r--r--   0 runner    (1001) docker     (121)      438 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/catalogue/examples_checkmate2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      891 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/catalogue/examples_rome.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)      562 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/expect_script.sh
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/getkrb_reana.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.666191 recast_atlas-0.1.9/src/recastatlas/data/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.670192 recast_atlas-0.1.9/src/recastatlas/data/templates/helloworld/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/templates/helloworld/recast.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.670192 recast_atlas-0.1.9/src/recastatlas/data/templates/helloworld/specs/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/templates/helloworld/specs/steps.yml
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/data/templates/helloworld/specs/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/resultsextraction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.674192 recast_atlas-0.1.9/src/recastatlas/subcommands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10094 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     3780 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     6010 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/software.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/subcommands/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.674192 recast_atlas-0.1.9/src/recastatlas/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/test/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/src/recastatlas/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-21 18:13:40.674192 recast_atlas-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      781 2021-12-21 18:13:21.000000 recast_atlas-0.1.9/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.992233 recast_atlas-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recast_atlas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/reana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/data/catalogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/busyboxtest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_checkmate1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_checkmate2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_rome.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/expect_script.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/getkrb_reana.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.992233 recast_atlas-0.2.0/src/recastatlas/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/recast.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/specs/steps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/specs/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/resultsextraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/software.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/test/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/tests/test_cli.py
```

### Comparing `recast_atlas-0.1.9/LICENSE` & `recast_atlas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/PKG-INFO` & `recast_atlas-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: recast_atlas
-Version: 0.1.9
+Version: 0.2.0
 Summary: RECAST for ATLAS at the LHC
 Home-page: https://github.com/recast-hep/recast-atlas
 Author: Lukas Heinrich
 Author-email: lukas.heinrich@cern.ch
 License: Apache
 Project-URL: Documentation, https://github.com/recast-hep/recast-atlas
 Project-URL: Source Code, https://github.com/recast-hep/recast-atlas
 Project-URL: Issue Tracker, https://github.com/recast-hep/recast-atlas/issues
 Keywords: physics recast atlas
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: local
 Provides-Extra: kubernetes
 Provides-Extra: reana
 License-File: LICENSE
 
 # RECAST for ATLAS
 
+[![DOI](https://zenodo.org/badge/142000927.svg)](https://doi.org/10.5281/zenodo.5854896)
+
 [![CI](https://github.com/recast-hep/recast-atlas/actions/workflows/ci.yml/badge.svg)](https://github.com/recast-hep/recast-atlas/actions/workflows/ci.yml?query=branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/recast-hep/recast-atlas/main.svg)](https://results.pre-commit.ci/latest/github/recast-hep/recast-atlas/main)
 [![PyPI version](https://badge.fury.io/py/recast-atlas.svg)](https://badge.fury.io/py/recast-atlas)
 
 ATLAS tools to facilitate integration of ATLAS analyses into RECAST
 
 ## Getting Started
@@ -101,9 +101,7 @@
 
 ```console
 ssh lxplus8.cern.ch
 source ~recast/public/setup.sh
 recast catalogue ls
 recast run examples/rome
 ```
-
-
```

### Comparing `recast_atlas-0.1.9/README.md` & `recast_atlas-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # RECAST for ATLAS
 
+[![DOI](https://zenodo.org/badge/142000927.svg)](https://doi.org/10.5281/zenodo.5854896)
+
 [![CI](https://github.com/recast-hep/recast-atlas/actions/workflows/ci.yml/badge.svg)](https://github.com/recast-hep/recast-atlas/actions/workflows/ci.yml?query=branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/recast-hep/recast-atlas/main.svg)](https://results.pre-commit.ci/latest/github/recast-hep/recast-atlas/main)
 [![PyPI version](https://badge.fury.io/py/recast-atlas.svg)](https://badge.fury.io/py/recast-atlas)
 
 ATLAS tools to facilitate integration of ATLAS analyses into RECAST
 
 ## Getting Started
```

### Comparing `recast_atlas-0.1.9/setup.cfg` & `recast_atlas-0.2.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [metadata]
 name = recast_atlas
-version = 0.1.9
+version = 0.2.0
 description = RECAST for ATLAS at the LHC
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/recast-hep/recast-atlas
 author = Lukas Heinrich
 author_email = lukas.heinrich@cern.ch
 license = Apache
 license_file = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Physics
@@ -32,15 +31,15 @@
 [options]
 packages = find:
 install_requires = 
 	click>=7.0  # for console scripts
 	jsonschema>=3.0.0
 	pyyaml>=5.1  # for parsing CLI options
 	yadage-schemas>=0.10.7  # c.f. https://github.com/yadage/yadage-schemas/issues/35
-python_requires = >=3.6
+python_requires = >=3.7
 include_package_data = True
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
```

### Comparing `recast_atlas-0.1.9/src/recast_atlas.egg-info/PKG-INFO` & `recast_atlas-0.2.0/src/recast_atlas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: recast-atlas
-Version: 0.1.9
+Version: 0.2.0
 Summary: RECAST for ATLAS at the LHC
 Home-page: https://github.com/recast-hep/recast-atlas
 Author: Lukas Heinrich
 Author-email: lukas.heinrich@cern.ch
 License: Apache
 Project-URL: Documentation, https://github.com/recast-hep/recast-atlas
 Project-URL: Source Code, https://github.com/recast-hep/recast-atlas
 Project-URL: Issue Tracker, https://github.com/recast-hep/recast-atlas/issues
 Keywords: physics recast atlas
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: local
 Provides-Extra: kubernetes
 Provides-Extra: reana
 License-File: LICENSE
 
 # RECAST for ATLAS
 
+[![DOI](https://zenodo.org/badge/142000927.svg)](https://doi.org/10.5281/zenodo.5854896)
+
 [![CI](https://github.com/recast-hep/recast-atlas/actions/workflows/ci.yml/badge.svg)](https://github.com/recast-hep/recast-atlas/actions/workflows/ci.yml?query=branch%3Amain)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/recast-hep/recast-atlas/main.svg)](https://results.pre-commit.ci/latest/github/recast-hep/recast-atlas/main)
 [![PyPI version](https://badge.fury.io/py/recast-atlas.svg)](https://badge.fury.io/py/recast-atlas)
 
 ATLAS tools to facilitate integration of ATLAS analyses into RECAST
 
 ## Getting Started
@@ -101,9 +101,7 @@
 
 ```console
 ssh lxplus8.cern.ch
 source ~recast/public/setup.sh
 recast catalogue ls
 recast run examples/rome
 ```
-
-
```

### Comparing `recast_atlas-0.1.9/src/recast_atlas.egg-info/SOURCES.txt` & `recast_atlas-0.2.0/src/recast_atlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/backends/__init__.py` & `recast_atlas-0.2.0/src/recastatlas/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/backends/docker.py` & `recast_atlas-0.2.0/src/recastatlas/backends/docker.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/backends/kubernetes.py` & `recast_atlas-0.2.0/src/recastatlas/backends/kubernetes.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/backends/local.py` & `recast_atlas-0.2.0/src/recastatlas/backends/local.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/backends/reana.py` & `recast_atlas-0.2.0/src/recastatlas/backends/reana.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/cli.py` & `recast_atlas-0.2.0/src/recastatlas/cli.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/config.py` & `recast_atlas-0.2.0/src/recastatlas/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             },
             "docker": {
                 "metadata": {"short_description": "runs with containerized tools"},
                 "fromstring": conf_from_env(
                     "RECAST_DOCKER_BACKENDSTRING", "multiproc:auto"
                 ),
                 "image": conf_from_env(
-                    "RECAST_DOCKER_IMAGE", "recast/recastatlas:v0.1.9"
+                    "RECAST_DOCKER_IMAGE", "recast/recastatlas:v0.2.0"
                 ),
                 "cvmfs": {"location": "/cvmfs", "propagation": "rprivate"},
                 "reg": {
                     "user": conf_from_env("RECAST_REGISTRY_USERNAME"),
                     "pass": conf_from_env("RECAST_REGISTRY_PASSWORD"),
                     "host": conf_from_env("RECAST_REGISTRY_HOST"),
                 },
```

### Comparing `recast_atlas-0.1.9/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml` & `recast_atlas-0.2.0/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/data/catalogue/examples_rome.yml` & `recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_rome.yml`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/data/expect_script.sh` & `recast_atlas-0.2.0/src/recastatlas/data/expect_script.sh`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/data/templates/helloworld/recast.yml` & `recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/recast.yml`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/resultsextraction.py` & `recast_atlas-0.2.0/src/recastatlas/resultsextraction.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/subcommands/auth.py` & `recast_atlas-0.2.0/src/recastatlas/subcommands/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,14 @@
 )
 @click.option(
     "--backend",
     type=click.Choice(["local", "docker"]),
     default=config.default_run_backend,
 )
 def check_access_xrootd(image, location, backend):
-
     image = image.split(":", 1)
     if len(image) > 1:
         image, tag = image
     else:
         image = image[0]
         tag = "latest"
```

### Comparing `recast_atlas-0.1.9/src/recastatlas/subcommands/backends.py` & `recast_atlas-0.2.0/src/recastatlas/subcommands/backends.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/subcommands/catalogue.py` & `recast_atlas-0.2.0/src/recastatlas/subcommands/catalogue.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/subcommands/run.py` & `recast_atlas-0.2.0/src/recastatlas/subcommands/run.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/subcommands/software.py` & `recast_atlas-0.2.0/src/recastatlas/subcommands/software.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/subcommands/testing.py` & `recast_atlas-0.2.0/src/recastatlas/subcommands/testing.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/src/recastatlas/testing.py` & `recast_atlas-0.2.0/src/recastatlas/testing.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.1.9/tests/test_cli.py` & `recast_atlas-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

