# Comparing `tmp/brainglobe-0.0.1a0.tar.gz` & `tmp/brainglobe-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brainglobe-0.0.1a0.tar", last modified: Thu Apr 30 12:36:50 2020, max compression
+gzip compressed data, was "brainglobe-0.1.0.tar", last modified: Wed Jun 21 12:08:17 2023, max compression
```

## Comparing `brainglobe-0.0.1a0.tar` & `brainglobe-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,28 @@
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/
--rw-rw-r--   0 adam      (1000) adam      (1000)      311 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)       65 2020-04-30 11:12:32.000000 brainglobe-0.0.1a0/README.md
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/brainglobe/
--rw-rw-r--   0 adam      (1000) adam      (1000)        0 2020-04-30 11:14:43.000000 brainglobe-0.0.1a0/brainglobe/__init__.py
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/brainglobe.egg-info/
--rw-rw-r--   0 adam      (1000) adam      (1000)      311 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/brainglobe.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1000) adam      (1000)      243 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/brainglobe.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)        1 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/brainglobe.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)        1 2020-04-30 11:18:53.000000 brainglobe-0.0.1a0/brainglobe.egg-info/not-zip-safe
--rw-rw-r--   0 adam      (1000) adam      (1000)      119 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/brainglobe.egg-info/requires.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)       18 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/brainglobe.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1000) adam      (1000)       38 2020-04-30 12:36:50.000000 brainglobe-0.0.1a0/setup.cfg
--rw-rw-r--   0 adam      (1000) adam      (1000)      815 2020-04-30 12:36:34.000000 brainglobe-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.910550 brainglobe-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.906550 brainglobe-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.906550 brainglobe-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-21 12:08:08.000000 brainglobe-0.1.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 12:08:08.000000 brainglobe-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-21 12:08:08.000000 brainglobe-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 12:08:08.000000 brainglobe-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-21 12:08:17.910550 brainglobe-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-21 12:08:08.000000 brainglobe-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.906550 brainglobe-0.1.0/brainglobe/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 12:08:08.000000 brainglobe-0.1.0/brainglobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.910550 brainglobe-0.1.0/brainglobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-21 12:08:17.000000 brainglobe-0.1.0/brainglobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-21 12:08:17.000000 brainglobe-0.1.0/brainglobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:08:17.000000 brainglobe-0.1.0/brainglobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 12:08:17.000000 brainglobe-0.1.0/brainglobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 12:08:17.000000 brainglobe-0.1.0/brainglobe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-21 12:08:08.000000 brainglobe-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:08:17.910550 brainglobe-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.910550 brainglobe-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:08.000000 brainglobe-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.910550 brainglobe-0.1.0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:08.000000 brainglobe-0.1.0/tests/test_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:17.910550 brainglobe-0.1.0/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:08:08.000000 brainglobe-0.1.0/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 12:08:08.000000 brainglobe-0.1.0/tests/test_unit/test__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-21 12:08:08.000000 brainglobe-0.1.0/tests/test_unit/test_tool_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 12:08:08.000000 brainglobe-0.1.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

