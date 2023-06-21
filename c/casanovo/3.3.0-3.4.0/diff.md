# Comparing `tmp/casanovo-3.3.0.tar.gz` & `tmp/casanovo-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casanovo-3.3.0.tar", last modified: Tue Apr  4 16:40:58 2023, max compression
+gzip compressed data, was "casanovo-3.4.0.tar", last modified: Wed Jun 21 06:33:14 2023, max compression
```

## Comparing `casanovo-3.3.0.tar` & `casanovo-3.4.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.742132 casanovo-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.734132 casanovo-3.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.738132 casanovo-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-04 16:40:39.000000 casanovo-3.3.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-04 16:40:39.000000 casanovo-3.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-04 16:40:39.000000 casanovo-3.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-04 16:40:39.000000 casanovo-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-04 16:40:39.000000 casanovo-3.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-04 16:40:39.000000 casanovo-3.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-04 16:40:39.000000 casanovo-3.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-04 16:40:39.000000 casanovo-3.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-04 16:40:39.000000 casanovo-3.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-04 16:40:39.000000 casanovo-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-04 16:40:39.000000 casanovo-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-04 16:40:58.742132 casanovo-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-04 16:40:39.000000 casanovo-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.738132 casanovo-3.3.0/casanovo/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/casanovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.738132 casanovo-3.3.0/casanovo/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/data/ms_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.738132 casanovo-3.3.0/casanovo/denovo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/denovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/denovo/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/denovo/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    40899 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/denovo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/denovo/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-04 16:40:39.000000 casanovo-3.3.0/casanovo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.738132 casanovo-3.3.0/casanovo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-04 16:40:58.000000 casanovo-3.3.0/casanovo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-04 16:40:58.000000 casanovo-3.3.0/casanovo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:40:58.000000 casanovo-3.3.0/casanovo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 16:40:58.000000 casanovo-3.3.0/casanovo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-04 16:40:58.000000 casanovo-3.3.0/casanovo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 16:40:58.000000 casanovo-3.3.0/casanovo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-04 16:40:39.000000 casanovo-3.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.742132 casanovo-3.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-04 16:40:39.000000 casanovo-3.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-04 16:40:39.000000 casanovo-3.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.742132 casanovo-3.3.0/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)   283201 2023-04-04 16:40:39.000000 casanovo-3.3.0/sample_data/sample_preprocessed_spectra.mgf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 16:40:58.742132 casanovo-3.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.742132 casanovo-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-04 16:40:39.000000 casanovo-3.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-04 16:40:39.000000 casanovo-3.3.0/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:40:58.742132 casanovo-3.3.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-04 16:40:39.000000 casanovo-3.3.0/tests/unit_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-04-04 16:40:39.000000 casanovo-3.3.0/tests/unit_tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.114443 casanovo-3.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.114443 casanovo-3.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-21 06:32:53.000000 casanovo-3.4.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-21 06:32:53.000000 casanovo-3.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-21 06:32:53.000000 casanovo-3.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-21 06:32:53.000000 casanovo-3.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-21 06:32:53.000000 casanovo-3.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 06:32:53.000000 casanovo-3.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-21 06:32:53.000000 casanovo-3.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-21 06:32:53.000000 casanovo-3.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-21 06:32:53.000000 casanovo-3.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-21 06:32:53.000000 casanovo-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 06:32:53.000000 casanovo-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-21 06:33:14.118443 casanovo-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 06:32:53.000000 casanovo-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.114443 casanovo-3.4.0/casanovo/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/casanovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/casanovo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/data/ms_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/casanovo/denovo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/denovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/denovo/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/denovo/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40338 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/denovo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/denovo/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 06:32:53.000000 casanovo-3.4.0/casanovo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/casanovo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-21 06:33:14.000000 casanovo-3.4.0/casanovo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-21 06:33:14.000000 casanovo-3.4.0/casanovo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:33:14.000000 casanovo-3.4.0/casanovo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 06:33:14.000000 casanovo-3.4.0/casanovo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 06:33:14.000000 casanovo-3.4.0/casanovo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 06:33:14.000000 casanovo-3.4.0/casanovo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-21 06:32:53.000000 casanovo-3.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-21 06:32:53.000000 casanovo-3.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-21 06:32:53.000000 casanovo-3.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   283201 2023-06-21 06:32:53.000000 casanovo-3.4.0/sample_data/sample_preprocessed_spectra.mgf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:33:14.118443 casanovo-3.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-21 06:32:53.000000 casanovo-3.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 06:32:53.000000 casanovo-3.4.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:33:14.118443 casanovo-3.4.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-21 06:32:53.000000 casanovo-3.4.0/tests/unit_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18207 2023-06-21 06:32:53.000000 casanovo-3.4.0/tests/unit_tests/test_unit.py
```

### Comparing `casanovo-3.3.0/.github/workflows/black.yml` & `casanovo-3.4.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/.github/workflows/publish.yml` & `casanovo-3.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/.github/workflows/tests.yml` & `casanovo-3.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/.gitignore` & `casanovo-3.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/CHANGELOG.md` & `casanovo-3.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.4.0] - 2023-06-19
+
+### Added
+
+- `every_n_train_steps` parameter now controls the frequency of both validation epochs and model checkpointing during training.
+
+### Changed
+
+- We now log steps rather than epochs as units of progress during training.
+- Validation performance metrics are logged (and added to tensorboard) at the validation epoch, and training loss is logged at the end of training epoch, i.e. training and validation metrics are logged asynchronously.
+
+### Fixed
+
+- Correctly refer to input peak files by their full file path.
+
 ## [3.3.0] - 2023-04-04
 
 ### Added
 
 - Included the `min_peptide_len` parameter in the configuration file to restrict predictions to peptide with a minimum length.
 - Export multiple PSMs per spectrum using the `top_match` parameter in the configuration file.
 
@@ -155,16 +170,17 @@
 
 ## [1.0.0] - 2022-01-28
 
 ### Added
 
 - Initial Casanovo version.
 
-[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v3.3.0...HEAD
-[3.2.0]: https://github.com/Noble-Lab/casanovo/compare/v3.2.0...v3.3.0
+[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v3.4.0...HEAD
+[3.4.0]: https://github.com/Noble-Lab/casanovo/compare/v3.3.0...v3.4.0
+[3.3.0]: https://github.com/Noble-Lab/casanovo/compare/v3.2.0...v3.3.0
 [3.2.0]: https://github.com/Noble-Lab/casanovo/compare/v3.1.0...v3.2.0
 [3.1.0]: https://github.com/Noble-Lab/casanovo/compare/v3.0.0...v3.1.0
 [3.0.0]: https://github.com/Noble-Lab/casanovo/compare/v2.1.1...v3.0.0
 [2.1.1]: https://github.com/Noble-Lab/casanovo/compare/v2.1.0...v2.1.1
 [2.1.0]: https://github.com/Noble-Lab/casanovo/compare/v2.0.1...v2.1.0
 [2.0.1]: https://github.com/Noble-Lab/casanovo/compare/v2.0.0...v2.0.1
 [2.0.0]: https://github.com/Noble-Lab/casanovo/compare/v1.2.0...v2.0.0
```

### Comparing `casanovo-3.3.0/CODE_OF_CONDUCT.md` & `casanovo-3.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/CONTRIBUTING.md` & `casanovo-3.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/LICENSE` & `casanovo-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/PKG-INFO` & `casanovo-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanovo
-Version: 3.3.0
+Version: 3.4.0
 Summary: De novo mass spectrometry peptide sequencing with a transformer model
 Author-email: Melih Yilmaz <melih@cs.washington.edu>, "William E. Fondrie" <fondriew@gmail.com>, Wout Bittremieux <wout.bittremieux@uantwerpen.be>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Noble-Lab/casanovo
 Project-URL: Documentation, https://casanovo.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Noble-Lab/casanovo/issues
 Project-URL: Discussion Board, https://github.com/Noble-Lab/casanovo/discussions
```

### Comparing `casanovo-3.3.0/README.md` & `casanovo-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/casanovo/casanovo.py` & `casanovo-3.4.0/casanovo/casanovo.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     help="The file name of the configuration file with custom options. If not "
     "specified, a default configuration will be used.",
     type=click.Path(exists=True, dir_okay=False),
 )
 @click.option(
     "--output",
     help="The base output file name to store logging (extension: .log) and "
-    "(optionally) prediction results (extension: .csv).",
+    "(optionally) prediction results (extension: .mztab).",
     type=click.Path(dir_okay=False),
 )
 def main(
     mode: str,
     model: Optional[str],
     peak_path: str,
     peak_path_val: Optional[str],
@@ -92,15 +92,16 @@
     """
     if output is None:
         output = os.path.join(
             os.getcwd(),
             f"casanovo_{datetime.datetime.now().strftime('%Y%m%d%H%M%S')}",
         )
     else:
-        output = os.path.splitext(os.path.abspath(output))[0]
+        basename, ext = os.path.splitext(os.path.abspath(output))
+        output = basename if ext.lower() in (".log", ".mztab") else output
 
     # Configure logging.
     logging.captureWarnings(True)
     root = logging.getLogger()
     root.setLevel(logging.DEBUG)
     log_formatter = logging.Formatter(
         "{asctime} {levelname} [{name}/{processName}] {module}.{funcName} : "
```

### Comparing `casanovo-3.3.0/casanovo/config.py` & `casanovo-3.4.0/casanovo/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         n_head=int,
         dim_feedforward=int,
         n_layers=int,
         dropout=float,
         dim_intensity=int,
         max_length=int,
         n_log=int,
+        tb_summarywriter=str,
         warmup_iters=int,
         max_iters=int,
         learning_rate=float,
         weight_decay=float,
         train_batch_size=int,
         predict_batch_size=int,
         n_beams=int,
```

### Comparing `casanovo-3.3.0/casanovo/config.yaml` & `casanovo-3.4.0/casanovo/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -113,11 +113,11 @@
 train_from_scratch: True
 # Save model checkpoints during training
 save_model: True
 # Path to saved checkpoints
 model_save_folder_path: ""
 # Set to "False" to save the PyTorch model instance
 save_weights_only: True
-# Model checkpointing frequency in training steps
+# Model validation and checkpointing frequency in training steps
 every_n_train_steps: 50_000
 # Disable usage of a GPU (including Apple MPS):
 no_gpu: False
```

### Comparing `casanovo-3.3.0/casanovo/data/datasets.py` & `casanovo-3.4.0/casanovo/data/datasets.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/casanovo/data/ms_io.py` & `casanovo-3.4.0/casanovo/data/ms_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,17 @@
 
         Parameters
         ----------
         peak_filenames : List[str]
             The input peak file name(s).
         """
         for i, filename in enumerate(natsort.natsorted(peak_filenames), 1):
+            filename = os.path.abspath(filename)
             self.metadata.append(
-                (
-                    f"ms_run[{i}]-location",
-                    Path(os.path.abspath(filename)).as_uri(),
-                ),
+                (f"ms_run[{i}]-location", Path(filename).as_uri()),
             )
             self._run_map[filename] = i
 
     def save(self) -> None:
         """
         Export the spectrum identifications to the mzTab file.
         """
@@ -176,14 +174,15 @@
                     "end",
                     "opt_ms_run[1]_aa_scores",
                 ]
             )
             for i, psm in enumerate(
                 natsort.natsorted(self.psms, key=operator.itemgetter(1)), 1
             ):
+                filename, idx = os.path.abspath(psm[1][0]), psm[1][1]
                 writer.writerow(
                     [
                         "PSM",
                         psm[0],  # sequence
                         i,  # PSM_ID
                         "null",  # accession
                         "null",  # unique
@@ -196,15 +195,15 @@
                         "null",  # modifications
                         # FIXME: Can we get the retention time from the data
                         #  loader?
                         "null",  # retention_time
                         psm[3],  # charge
                         psm[4],  # exp_mass_to_charge
                         psm[5],  # calc_mass_to_charge
-                        f"ms_run[{self._run_map[psm[1][0]]}]:{psm[1][1]}",
+                        f"ms_run[{self._run_map[filename]}]:{idx}",
                         "null",  # pre
                         "null",  # post
                         "null",  # start
                         "null",  # end
                         psm[6],  # opt_ms_run[1]_aa_scores
                     ]
                 )
```

### Comparing `casanovo-3.3.0/casanovo/denovo/dataloaders.py` & `casanovo-3.4.0/casanovo/denovo/dataloaders.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/casanovo/denovo/evaluate.py` & `casanovo-3.4.0/casanovo/denovo/evaluate.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/casanovo/denovo/model.py` & `casanovo-3.4.0/casanovo/denovo/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -750,24 +750,18 @@
             The loss of the validation step.
         """
         # Record the loss.
         loss = self.training_step(batch, mode="valid")
 
         # Calculate and log amino acid and peptide match evaluation metrics from
         # the predicted peptides.
-        peptides_pred_raw, _ = self.forward(batch[0], batch[1])
-        # FIXME: Temporary fix to skip predictions with multiple stop tokens.
-        peptides_pred, peptides_true = [], []
-        for peptide_pred, peptide_true in zip(peptides_pred_raw, batch[2]):
-            if len(peptide_pred) > 0:
-                if peptide_pred[0] == "$":
-                    peptide_pred = peptide_pred[1:]  # Remove stop token.
-                if "$" not in peptide_pred and len(peptide_pred) > 0:
-                    peptides_pred.append(peptide_pred)
-                    peptides_true.append(peptide_true)
+        peptides_pred, peptides_true = [], batch[2]
+        for spectrum_preds in self.forward(batch[0], batch[1]):
+            for _, _, pred in spectrum_preds:
+                peptides_pred.append(pred)
         aa_precision, _, pep_precision = evaluate.aa_match_metrics(
             *evaluate.aa_match_batch(
                 peptides_pred, peptides_true, self.decoder._peptide_mass.masses
             )
         )
         log_args = dict(on_step=False, on_epoch=True, sync_dist=True)
         self.log(
@@ -827,32 +821,35 @@
         return predictions
 
     def on_train_epoch_end(self) -> None:
         """
         Log the training loss at the end of each epoch.
         """
         train_loss = self.trainer.callback_metrics["CELoss"]["train"].detach()
-        self._history[-1]["train"] = train_loss
+        metrics = {
+            "step": self.trainer.global_step,
+            "train": train_loss,
+        }
+        self._history.append(metrics)
         self._log_history()
 
     def on_validation_epoch_end(self) -> None:
         """
         Log the validation metrics at the end of each epoch.
         """
         callback_metrics = self.trainer.callback_metrics
         metrics = {
-            "epoch": self.trainer.current_epoch,
+            "step": self.trainer.global_step,
             "valid": callback_metrics["CELoss"]["valid"].detach(),
-            "valid_aa_precision": callback_metrics["aa_precision"][
-                "valid"
-            ].detach(),
-            "valid_aa_recall": callback_metrics["aa_recall"]["valid"].detach(),
-            "valid_pep_recall": callback_metrics["pep_recall"][
-                "valid"
-            ].detach(),
+            "valid_aa_precision": callback_metrics[
+                "AA precision at coverage=1"
+            ]["valid"].detach(),
+            "valid_pep_precision": callback_metrics[
+                "Peptide precision at coverage=1"
+            ]["valid"].detach(),
         }
         self._history.append(metrics)
         self._log_history()
 
     def on_predict_epoch_end(
         self, results: List[List[Tuple[np.ndarray, List[str], torch.Tensor]]]
     ) -> None:
@@ -888,43 +885,41 @@
             )
 
     def _log_history(self) -> None:
         """
         Write log to console, if requested.
         """
         # Log only if all output for the current epoch is recorded.
-        if len(self._history) > 0 and len(self._history[-1]) == 6:
-            if len(self._history) == 1:
-                logger.info(
-                    "Epoch\tTrain loss\tValid loss\tAA precision\tAA recall\t"
-                    "Peptide recall"
-                )
-            metrics = self._history[-1]
-            if metrics["epoch"] % self.n_log == 0:
-                logger.info(
-                    "%i\t%.6f\t%.6f\t%.6f\t%.6f\t%.6f",
-                    metrics["epoch"] + 1,
-                    metrics.get("train", np.nan),
-                    metrics.get("valid", np.nan),
-                    metrics.get("valid_aa_precision", np.nan),
-                    metrics.get("valid_aa_recall", np.nan),
-                    metrics.get("valid_pep_recall", np.nan),
-                )
-                if self.tb_summarywriter is not None:
-                    for descr, key in [
-                        ("loss/train_crossentropy_loss", "train"),
-                        ("loss/dev_crossentropy_loss", "valid"),
-                        ("eval/dev_aa_precision", "valid_aa_precision"),
-                        ("eval/dev_aa_recall", "valid_aa_recall"),
-                        ("eval/dev_pep_recall", "valid_pep_recall"),
-                    ]:
+        if len(self._history) == 0:
+            return
+        if len(self._history) == 1:
+            logger.info(
+                "Step\tTrain loss\tValid loss\tPeptide precision\tAA precision"
+            )
+        metrics = self._history[-1]
+        if metrics["step"] % self.n_log == 0:
+            logger.info(
+                "%i\t%.6f\t%.6f\t%.6f\t%.6f",
+                metrics["step"],
+                metrics.get("train", np.nan),
+                metrics.get("valid", np.nan),
+                metrics.get("valid_pep_precision", np.nan),
+                metrics.get("valid_aa_precision", np.nan),
+            )
+            if self.tb_summarywriter is not None:
+                for descr, key in [
+                    ("loss/train_crossentropy_loss", "train"),
+                    ("loss/val_crossentropy_loss", "valid"),
+                    ("eval/val_pep_precision", "valid_pep_precision"),
+                    ("eval/val_aa_precision", "valid_aa_precision"),
+                ]:
+                    metric_value = metrics.get(key, np.nan)
+                    if not np.isnan(metric_value):
                         self.tb_summarywriter.add_scalar(
-                            descr,
-                            metrics.get(key, np.nan),
-                            metrics["epoch"] + 1,
+                            descr, metric_value, metrics["step"]
                         )
 
     def configure_optimizers(
         self,
     ) -> Tuple[torch.optim.Optimizer, Dict[str, Any]]:
         """
         Initialize the optimizer.
```

### Comparing `casanovo-3.3.0/casanovo/denovo/model_runner.py` & `casanovo-3.4.0/casanovo/denovo/model_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,18 +303,20 @@
         callbacks = None
 
     trainer = pl.Trainer(
         accelerator="auto",
         auto_select_gpus=True,
         callbacks=callbacks,
         devices=_get_devices(config["no_gpu"]),
+        enable_checkpointing=config["save_model"],
         logger=config["logger"],
         max_epochs=config["max_epochs"],
         num_sanity_val_steps=config["num_sanity_val_steps"],
         strategy=_get_strategy(),
+        val_check_interval=config["every_n_train_steps"],
     )
     # Train the model.
     trainer.fit(
         model, train_loader.train_dataloader(), val_loader.val_dataloader()
     )
     # Clean up temporary files.
     tmp_dir.cleanup()
@@ -340,15 +342,15 @@
     -------
     List[str]
         The peak file names matching the path pattern.
     """
     path = os.path.expanduser(path)
     path = os.path.expandvars(path)
     return [
-        fn
+        os.path.abspath(fn)
         for fn in glob.glob(path, recursive=True)
         if os.path.splitext(fn.lower())[1] in supported_ext
     ]
 
 
 def _get_strategy() -> Optional[DDPStrategy]:
     """
```

### Comparing `casanovo-3.3.0/casanovo/utils.py` & `casanovo-3.4.0/casanovo/utils.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/casanovo/version.py` & `casanovo-3.4.0/casanovo/version.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/casanovo.egg-info/PKG-INFO` & `casanovo-3.4.0/casanovo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanovo
-Version: 3.3.0
+Version: 3.4.0
 Summary: De novo mass spectrometry peptide sequencing with a transformer model
 Author-email: Melih Yilmaz <melih@cs.washington.edu>, "William E. Fondrie" <fondriew@gmail.com>, Wout Bittremieux <wout.bittremieux@uantwerpen.be>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Noble-Lab/casanovo
 Project-URL: Documentation, https://casanovo.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Noble-Lab/casanovo/issues
 Project-URL: Discussion Board, https://github.com/Noble-Lab/casanovo/discussions
```

### Comparing `casanovo-3.3.0/casanovo.egg-info/SOURCES.txt` & `casanovo-3.4.0/casanovo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/docs/CHANGELOG.md` & `casanovo-3.4.0/docs/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.4.0] - 2023-06-19
+
+### Added
+
+- `every_n_train_steps` parameter now controls the frequency of both validation epochs and model checkpointing during training.
+
+### Changed
+
+- We now log steps rather than epochs as units of progress during training.
+- Validation performance metrics are logged (and added to tensorboard) at the validation epoch, and training loss is logged at the end of training epoch, i.e. training and validation metrics are logged asynchronously.
+
+### Fixed
+
+- Correctly refer to input peak files by their full file path.
+
 ## [3.3.0] - 2023-04-04
 
 ### Added
 
 - Included the `min_peptide_len` parameter in the configuration file to restrict predictions to peptide with a minimum length.
 - Export multiple PSMs per spectrum using the `top_match` parameter in the configuration file.
 
@@ -155,16 +170,17 @@
 
 ## [1.0.0] - 2022-01-28
 
 ### Added
 
 - Initial Casanovo version.
 
-[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v3.3.0...HEAD
-[3.2.0]: https://github.com/Noble-Lab/casanovo/compare/v3.2.0...v3.3.0
+[Unreleased]: https://github.com/Noble-Lab/casanovo/compare/v3.4.0...HEAD
+[3.4.0]: https://github.com/Noble-Lab/casanovo/compare/v3.3.0...v3.4.0
+[3.3.0]: https://github.com/Noble-Lab/casanovo/compare/v3.2.0...v3.3.0
 [3.2.0]: https://github.com/Noble-Lab/casanovo/compare/v3.1.0...v3.2.0
 [3.1.0]: https://github.com/Noble-Lab/casanovo/compare/v3.0.0...v3.1.0
 [3.0.0]: https://github.com/Noble-Lab/casanovo/compare/v2.1.1...v3.0.0
 [2.1.1]: https://github.com/Noble-Lab/casanovo/compare/v2.1.0...v2.1.1
 [2.1.0]: https://github.com/Noble-Lab/casanovo/compare/v2.0.1...v2.1.0
 [2.0.1]: https://github.com/Noble-Lab/casanovo/compare/v2.0.0...v2.0.1
 [2.0.0]: https://github.com/Noble-Lab/casanovo/compare/v1.2.0...v2.0.0
```

### Comparing `casanovo-3.3.0/docs/CODE_OF_CONDUCT.md` & `casanovo-3.4.0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/docs/CONTRIBUTING.md` & `casanovo-3.4.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/docs/Makefile` & `casanovo-3.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/docs/conf.py` & `casanovo-3.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/docs/faq.md` & `casanovo-3.4.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/docs/getting_started.md` & `casanovo-3.4.0/docs/getting_started.md`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 Training and validation MS/MS data need to be provided as annotated MGF files, where the peptide sequence is denoted in the `SEQ` field.
 
 If a training is continued for a previously trained model, specify the starting model weights using `--model`.
 
 ## Try Casanovo on a small example
 
 Here, we demonstrate how to use Casanovo using a small collection of mass spectra in an MGF file (~100 MS/MS spectra).
-The example MGF file is available at [`sample_data/sample_preprocessed_spectra.mgf`](https://github.com/Noble-Lab/casanovo/blob/main/sample_data/sample_preprocessed_spectra.mgf`).
+The example MGF file is available at [`sample_data/sample_preprocessed_spectra.mgf`](https://github.com/Noble-Lab/casanovo/blob/main/sample_data/sample_preprocessed_spectra.mgf).
 
 To obtain *de novo* sequencing predictions for these spectra:
 1. Download the example MGF above.
 2. [Install Casanovo](#installation).
 3. Ensure your Casanovo conda environment is activated by typing `conda activate casanovo_env`. (If you named your environment differently, type in that name instead.)
 4. Sequence the mass spectra with Casanovo, replacing `[PATH_TO]` with the path to the example MGF file that you downloaded:
 ```sh
```

### Comparing `casanovo-3.3.0/docs/index.md` & `casanovo-3.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/docs/make.bat` & `casanovo-3.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/pyproject.toml` & `casanovo-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/sample_data/sample_preprocessed_spectra.mgf` & `casanovo-3.4.0/sample_data/sample_preprocessed_spectra.mgf`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/tests/conftest.py` & `casanovo-3.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/tests/test_integration.py` & `casanovo-3.4.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/tests/unit_tests/test_config.py` & `casanovo-3.4.0/tests/unit_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `casanovo-3.3.0/tests/unit_tests/test_unit.py` & `casanovo-3.4.0/tests/unit_tests/test_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import github
 import numpy as np
 import pytest
 import torch
 
 from casanovo import casanovo
 from casanovo import utils
+from casanovo.data import ms_io
 from casanovo.data.datasets import SpectrumDataset, AnnotatedSpectrumDataset
 from casanovo.denovo.evaluate import aa_match_batch, aa_match_metrics
 from casanovo.denovo.model import Spec2Pep, _aa_pep_score
 from depthcharge.data import SpectrumIndex, AnnotatedSpectrumIndex
 
 
 def test_version():
@@ -476,7 +477,32 @@
             (mzml_small, 111),
             (mzml_small2, 17),
             (mzml_small2, 111),
         ]
     ):
         spectrum_id = str(filename), f"scan={scan_nr}"
         assert dataset.get_spectrum_id(i) == spectrum_id
+
+
+def test_train_val_step_functions():
+    """Test train and validation step functions operating on batches."""
+    model = Spec2Pep(n_beams=1, residues="massivekb", min_peptide_len=4)
+    spectra = torch.zeros(1, 5, 2)
+    precursors = torch.tensor([[469.25364, 2.0, 235.63410]])
+    peptides = ["PEPK"]
+    batch = (spectra, precursors, peptides)
+
+    # Check if valid loss value returned
+    assert model.training_step(batch) > 0
+    assert model.validation_step(batch) > 0
+
+
+def test_run_map(mgf_small):
+    out_writer = ms_io.MztabWriter("dummy.mztab")
+    # Set peak file by base file name only.
+    out_writer.set_ms_run([os.path.basename(mgf_small.name)])
+    assert os.path.basename(mgf_small.name) not in out_writer._run_map
+    assert os.path.abspath(mgf_small.name) in out_writer._run_map
+    # Set peak file by full path.
+    out_writer.set_ms_run([os.path.abspath(mgf_small.name)])
+    assert os.path.basename(mgf_small.name) not in out_writer._run_map
+    assert os.path.abspath(mgf_small.name) in out_writer._run_map
```

