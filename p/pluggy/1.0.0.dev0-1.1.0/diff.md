# Comparing `tmp/pluggy-1.0.0.dev0.tar.gz` & `tmp/pluggy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pluggy-1.0.0.dev0.tar", last modified: Thu Jun  4 19:37:24 2020, max compression
+gzip compressed data, was "pluggy-1.1.0.tar", last modified: Mon Jun 19 11:28:20 2023, max compression
```

## Comparing `pluggy-1.0.0.dev0.tar` & `pluggy-1.1.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11287 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/changelog.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/docs/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)      911 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/toy-example.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/docs/examples/eggsample/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/docs/examples/eggsample/eggsample/
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/eggsample/eggsample/lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1557 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/eggsample/eggsample/host.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      512 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/eggsample/eggsample/hookspecs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/eggsample/eggsample/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      220 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/eggsample/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/docs/examples/eggsample-spam/
--rw-rw-r--   0 travis    (2000) travis    (2000)      616 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/eggsample-spam/eggsample_spam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      194 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/examples/eggsample-spam/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/api_reference.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    29173 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/docs/_static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/docs/_static/img/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9350 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/docs/_static/img/plug.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    19225 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/codecov.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/changelog/
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/changelog/_template.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/changelog/59.removal.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1662 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/changelog/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4026 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/src/pluggy/callers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12060 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/src/pluggy/hooks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15582 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/src/pluggy/manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      486 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/src/pluggy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1561 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/src/pluggy/_tracing.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19225 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1249 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/src/pluggy.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1180 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      802 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/.gitignore
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1958 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/scripts/release.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1872 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)     3026 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      885 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/appveyor.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      925 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/.pre-commit-config.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/HOWTORELEASE.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 19:37:23.000000 pluggy-1.0.0.dev0/testing/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5109 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_invocations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1825 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2978 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_multicall.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/benchmark.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6193 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_hookcaller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_tracer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1058 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_deprecations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14289 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_pluginmanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3588 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/test_details.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      505 2020-06-04 19:37:06.000000 pluggy-1.0.0.dev0/testing/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.887653 pluggy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-19 11:28:07.000000 pluggy-1.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.879653 pluggy-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-19 11:28:07.000000 pluggy-1.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-19 11:28:07.000000 pluggy-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-19 11:28:07.000000 pluggy-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16644 2023-06-19 11:28:07.000000 pluggy-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-19 11:28:07.000000 pluggy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 11:28:07.000000 pluggy-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-19 11:28:20.887653 pluggy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-19 11:28:07.000000 pluggy-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-19 11:28:07.000000 pluggy-1.1.0/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-19 11:28:07.000000 pluggy-1.1.0/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-19 11:28:07.000000 pluggy-1.1.0/changelog/_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-19 11:28:07.000000 pluggy-1.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.879653 pluggy-1.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/docs/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/_static/img/plug.png
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/docs/examples/eggsample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/docs/examples/eggsample/eggsample/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/eggsample/eggsample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/eggsample/eggsample/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/eggsample/eggsample/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/eggsample/eggsample/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/eggsample/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/docs/examples/eggsample-spam/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/eggsample-spam/eggsample_spam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/eggsample-spam/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/examples/toy-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-06-19 11:28:07.000000 pluggy-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-19 11:28:07.000000 pluggy-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.883653 pluggy-1.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-19 11:28:07.000000 pluggy-1.1.0/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-19 11:28:07.000000 pluggy-1.1.0/scripts/towncrier-draft-to-file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-19 11:28:07.000000 pluggy-1.1.0/scripts/upload-coverage.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-19 11:28:20.887653 pluggy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-19 11:28:07.000000 pluggy-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.879653 pluggy-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.887653 pluggy-1.1.0/src/pluggy/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-19 11:28:07.000000 pluggy-1.1.0/src/pluggy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-19 11:28:07.000000 pluggy-1.1.0/src/pluggy/_callers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-06-19 11:28:07.000000 pluggy-1.1.0/src/pluggy/_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17702 2023-06-19 11:28:07.000000 pluggy-1.1.0/src/pluggy/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-19 11:28:07.000000 pluggy-1.1.0/src/pluggy/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-19 11:28:07.000000 pluggy-1.1.0/src/pluggy/_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 11:28:20.000000 pluggy-1.1.0/src/pluggy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.887653 pluggy-1.1.0/src/pluggy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-19 11:28:20.000000 pluggy-1.1.0/src/pluggy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-19 11:28:20.000000 pluggy-1.1.0/src/pluggy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:28:20.000000 pluggy-1.1.0/src/pluggy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-19 11:28:20.000000 pluggy-1.1.0/src/pluggy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 11:28:20.000000 pluggy-1.1.0/src/pluggy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:28:20.887653 pluggy-1.1.0/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/test_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/test_hookcaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/test_invocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/test_pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-19 11:28:07.000000 pluggy-1.1.0/testing/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-19 11:28:07.000000 pluggy-1.1.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pluggy-1.0.0.dev0/CHANGELOG.rst` & `pluggy-1.1.0/CHANGELOG.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,145 @@
 =========
 Changelog
 =========
 
+Versions follow `Semantic Versioning <https://semver.org/>`_ (``<major>.<minor>.<patch>``).
+
+..
+    You should *NOT* be adding new change log entries to this file, this
+    file is managed by towncrier. You *may* edit previous change logs to
+    fix problems like typo corrections or such.
+    To add a new change log entry, please see
+    https://pip.pypa.io/en/latest/development/contributing/#news-entries
+    we named the news folder changelog
+
+.. only:: changelog_towncrier_draft
+
+    .. The 'changelog_towncrier_draft' tag is included by our 'tox -e docs',
+       but not on readthedocs.
+
+    .. include:: _changelog_towncrier_draft.rst
+
 .. towncrier release notes start
 
+pluggy 1.1.0 (2023-06-19)
+=========================
+
+Deprecations and Removals
+-------------------------
+
+- `#364 <https://github.com/pytest-dev/pluggy/issues/364>`_: Python 3.6 is no longer supported.
+
+
+
+Features
+--------
+
+- `#260 <https://github.com/pytest-dev/pluggy/issues/260>`_: Added "new-style" hook wrappers, a simpler but equally powerful alternative to the existing ``hookwrapper=True`` wrappers.
+
+  New-style wrappers are generator functions, similarly to ``hookwrapper``, but do away with the :class:`result <pluggy._callers._Result>` object.
+  Instead, the return value is sent directly to the ``yield`` statement, or, if inner calls raised an exception, it is raised from the ``yield``.
+  The wrapper is expected to return a value or raise an exception, which will become the result of the hook call.
+
+  New-style wrappers are fully interoperable with old-style wrappers.
+  We encourage users to use the new style, however we do not intend to deprecate the old style any time soon.
+
+  See :ref:`hookwrappers` for the full documentation.
+
+
+- `#364 <https://github.com/pytest-dev/pluggy/issues/364>`_: Python 3.11 and 3.12 are now officially supported.
+
+
+- `#394 <https://github.com/pytest-dev/pluggy/issues/394>`_: Added the :meth:`~pluggy._callers._Result.force_exception` method to ``_Result``.
+
+  ``force_exception`` allows (old-style) hookwrappers to force an exception or override/adjust an existing exception of a hook invocation,
+  in a properly behaving manner. Using ``force_exception`` is preferred over raising an exception from the hookwrapper,
+  because raising an exception causes other hookwrappers to be skipped.
+
+
+pluggy 1.0.0 (2021-08-25)
+=========================
+
+Deprecations and Removals
+-------------------------
+
+- `#116 <https://github.com/pytest-dev/pluggy/issues/116>`_: Remove deprecated ``implprefix`` support.
+  Decorate hook implementations using an instance of HookimplMarker instead.
+  The deprecation was announced in release ``0.7.0``.
+
+
+- `#120 <https://github.com/pytest-dev/pluggy/issues/120>`_: Remove the deprecated ``proc`` argument to ``call_historic``.
+  Use ``result_callback`` instead, which has the same behavior.
+  The deprecation was announced in release ``0.7.0``.
+
+
+- `#265 <https://github.com/pytest-dev/pluggy/issues/265>`_: Remove the ``_Result.result`` property. Use ``_Result.get_result()`` instead.
+  Note that unlike ``result``, ``get_result()`` raises the exception if the hook raised.
+  The deprecation was announced in release ``0.6.0``.
+
+
+- `#267 <https://github.com/pytest-dev/pluggy/issues/267>`_: Remove official support for Python 3.4.
+
+
+- `#272 <https://github.com/pytest-dev/pluggy/issues/272>`_: Dropped support for Python 2.
+  Continue to use pluggy 0.13.x for Python 2 support.
+
+
+- `#308 <https://github.com/pytest-dev/pluggy/issues/308>`_: Remove official support for Python 3.5.
+
+
+- `#313 <https://github.com/pytest-dev/pluggy/issues/313>`_: The internal ``pluggy.callers``, ``pluggy.manager`` and ``pluggy.hooks`` are now explicitly marked private by a ``_`` prefix (e.g. ``pluggy._callers``).
+  Only API exported by the top-level ``pluggy`` module is considered public.
+
+
+- `#59 <https://github.com/pytest-dev/pluggy/issues/59>`_: Remove legacy ``__multicall__`` recursive hook calling system.
+  The deprecation was announced in release ``0.5.0``.
+
+
+
+Features
+--------
+
+- `#282 <https://github.com/pytest-dev/pluggy/issues/282>`_: When registering a hookimpl which is declared as ``hookwrapper=True`` but whose
+  function is not a generator function, a ``PluggyValidationError`` exception is
+  now raised.
+
+  Previously this problem would cause an error only later, when calling the hook.
+
+  In the unlikely case that you have a hookwrapper that *returns* a generator
+  instead of yielding directly, for example:
+
+  .. code-block:: python
+
+      def my_hook_real_implementation(arg):
+          print("before")
+          yield
+          print("after")
+
+
+      @hookimpl(hookwrapper=True)
+      def my_hook(arg):
+          return my_hook_implementation(arg)
+
+  change it to use ``yield from`` instead:
+
+  .. code-block:: python
+
+      @hookimpl(hookwrapper=True)
+      def my_hook(arg):
+          yield from my_hook_implementation(arg)
+
+
+- `#309 <https://github.com/pytest-dev/pluggy/issues/309>`_: Add official support for Python 3.9.
+
+- `#251 <https://github.com/pytest-dev/pluggy/issues/251>`_: Add ``specname`` option to ``@hookimpl``. If ``specname`` is provided, it will be used
+  instead of the function name when matching this hook implementation to a hook specification during registration (allowing a plugin to register
+  a hook implementation that was not named the same thing as the corresponding ``@hookspec``).
+
+
 pluggy 0.13.1 (2019-11-21)
 ==========================
 
 Trivial/Internal Changes
 ------------------------
 
 - `#236 <https://github.com/pytest-dev/pluggy/pull/236>`_: Improved documentation, especially with regard to references.
```

### Comparing `pluggy-1.0.0.dev0/docs/examples/toy-example.py` & `pluggy-1.1.0/docs/examples/toy-example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import pluggy
 
 hookspec = pluggy.HookspecMarker("myproject")
 hookimpl = pluggy.HookimplMarker("myproject")
 
 
-class MySpec(object):
+class MySpec:
     """A hook specification namespace."""
 
     @hookspec
     def myhook(self, arg1, arg2):
         """My special little hook that you can customize."""
 
 
-class Plugin_1(object):
+class Plugin_1:
     """A hook implementation namespace."""
 
     @hookimpl
     def myhook(self, arg1, arg2):
         print("inside Plugin_1.myhook()")
         return arg1 + arg2
 
 
-class Plugin_2(object):
+class Plugin_2:
     """A 2nd hook implementation namespace."""
 
     @hookimpl
     def myhook(self, arg1, arg2):
         print("inside Plugin_2.myhook()")
         return arg1 - arg2
```

### Comparing `pluggy-1.0.0.dev0/docs/examples/eggsample/eggsample/host.py` & `pluggy-1.1.0/docs/examples/eggsample/eggsample/host.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import itertools
 import random
 
-import pluggy
+from eggsample import hookspecs
+from eggsample import lib
 
-from eggsample import hookspecs, lib
+import pluggy
 
 condiments_tray = {"pickled walnuts": 13, "steak sauce": 4, "mushy peas": 2}
 
 
 def main():
     pm = get_plugin_manager()
     cook = EggsellentCook(pm.hook)
```

### Comparing `pluggy-1.0.0.dev0/docs/examples/eggsample/eggsample/hookspecs.py` & `pluggy-1.1.0/docs/examples/eggsample/eggsample/hookspecs.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.0.0.dev0/docs/examples/eggsample-spam/eggsample_spam.py` & `pluggy-1.1.0/docs/examples/eggsample-spam/eggsample_spam.py`

 * *Files identical despite different names*

### Comparing `pluggy-1.0.0.dev0/docs/conf.py` & `pluggy-1.1.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-# -*- coding: utf-8 -*-
 import sys
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    import sphinx.application
 
 if sys.version_info >= (3, 8):
     from importlib import metadata
 else:
     import importlib_metadata as metadata
 
 
@@ -22,68 +25,96 @@
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 
 project = "pluggy"
-copyright = u"2016, Holger Krekel"
+copyright = "2016, Holger Krekel"
 author = "Holger Krekel"
 
 release = metadata.version(project)
 # The short X.Y version.
-version = u".".join(release.split(".")[:2])
+version = ".".join(release.split(".")[:2])
 
 
-language = None
+language = "en"
 
 pygments_style = "sphinx"
 # html_logo = "_static/img/plug.png"
 html_theme = "alabaster"
 html_theme_options = {
     "logo": "img/plug.png",
     "description": "The pytest plugin system",
     "github_user": "pytest-dev",
     "github_repo": "pluggy",
     "github_button": "true",
     "github_banner": "true",
     "github_type": "star",
-    "travis_button": "true",
     "badge_branch": "master",
     "page_width": "1080px",
     "fixed_sidebar": "false",
 }
 html_sidebars = {
     "**": ["about.html", "localtoc.html", "relations.html", "searchbox.html"]
 }
 html_static_path = ["_static"]
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "pluggy", u"pluggy Documentation", [author], 1)]
+man_pages = [(master_doc, "pluggy", "pluggy Documentation", [author], 1)]
 
+autodoc_typehints = "none"
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
         "pluggy",
-        u"pluggy Documentation",
+        "pluggy Documentation",
         author,
         "pluggy",
         "One line description of project.",
         "Miscellaneous",
     )
 ]
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "pytest": ("https://docs.pytest.org/en/latest", None),
     "setuptools": ("https://setuptools.readthedocs.io/en/latest", None),
     "tox": ("https://tox.readthedocs.io/en/latest", None),
     "devpi": ("https://devpi.net/docs/devpi/devpi/stable/+doc/", None),
+    "kedro": ("https://kedro.readthedocs.io/en/latest/", None),
 }
+
+
+def configure_logging(app: "sphinx.application.Sphinx") -> None:
+    """Configure Sphinx's WarningHandler to handle (expected) missing include."""
+    import sphinx.util.logging
+    import logging
+
+    class WarnLogFilter(logging.Filter):
+        def filter(self, record: logging.LogRecord) -> bool:
+            """Ignore warnings about missing include with "only" directive.
+
+            Ref: https://github.com/sphinx-doc/sphinx/issues/2150."""
+            if (
+                record.msg.startswith('Problems with "include" directive path:')
+                and "_changelog_towncrier_draft.rst" in record.msg
+            ):
+                return False
+            return True
+
+    logger = logging.getLogger(sphinx.util.logging.NAMESPACE)
+    warn_handler = [x for x in logger.handlers if x.level == logging.WARNING]
+    assert len(warn_handler) == 1, warn_handler
+    warn_handler[0].filters.insert(0, WarnLogFilter())
+
+
+def setup(app: "sphinx.application.Sphinx") -> None:
+    configure_logging(app)
```

### Comparing `pluggy-1.0.0.dev0/docs/index.rst` & `pluggy-1.1.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -64,1761 +64,1973 @@
 000003f0: 6b65 7920 7061 7463 6869 6e67 203c 6874  key patching <ht
 00000400: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
 00000410: 6961 2e6f 7267 2f77 696b 692f 4d6f 6e6b  ia.org/wiki/Monk
 00000420: 6579 5f70 6174 6368 3e60 5f20 2865 2e67  ey_patch>`_ (e.g
 00000430: 2e20 6765 7665 6e74 0a6f 7220 666f 7220  . gevent.or for 
 00000440: 3a73 7464 3a64 6f63 3a60 7772 6974 696e  :std:doc:`writin
 00000450: 6720 7465 7374 7320 3c70 7974 6573 743a  g tests <pytest:
-00000460: 6d6f 6e6b 6579 7061 7463 683e 6029 2e0a  monkeypatch>`)..
-00000470: 5468 6573 6520 7374 7261 7465 6769 6573  These strategies
-00000480: 2062 6563 6f6d 6520 7072 6f62 6c65 6d61   become problema
-00000490: 7469 6320 7468 6f75 6768 2077 6865 6e20  tic though when 
-000004a0: 7365 7665 7261 6c20 7061 7274 6965 7320  several parties 
-000004b0: 7761 6e74 2074 6f0a 7061 7274 6963 6970  want to.particip
-000004c0: 6174 6520 696e 2074 6865 206d 6f64 6966  ate in the modif
-000004d0: 6963 6174 696f 6e20 6f66 2074 6865 2073  ication of the s
-000004e0: 616d 6520 7072 6f67 7261 6d2e 2054 6865  ame program. The
-000004f0: 7265 666f 7265 2060 6070 6c75 6767 7960  refore ``pluggy`
-00000500: 600a 646f 6573 206e 6f74 2072 656c 7920  `.does not rely 
-00000510: 6f6e 2074 6865 7365 206d 6563 6861 6e69  on these mechani
-00000520: 736d 7320 746f 2065 6e61 626c 6520 6120  sms to enable a 
-00000530: 6d6f 7265 2073 7472 7563 7475 7265 6420  more structured 
-00000540: 6170 7072 6f61 6368 2061 6e64 0a61 766f  approach and.avo
-00000550: 6964 2075 6e6e 6563 6573 7361 7279 2065  id unnecessary e
-00000560: 7870 6f73 7572 6520 6f66 2073 7461 7465  xposure of state
-00000570: 2061 6e64 2062 6568 6176 696f 7572 2e20   and behaviour. 
-00000580: 5468 6973 206c 6561 6473 2074 6f20 6120  This leads to a 
-00000590: 6d6f 7265 0a60 6c6f 6f73 656c 7920 636f  more.`loosely co
-000005a0: 7570 6c65 6420 3c68 7474 7073 3a2f 2f65  upled <https://e
-000005b0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-000005c0: 7769 6b69 2f4c 6f6f 7365 5f63 6f75 706c  wiki/Loose_coupl
-000005d0: 696e 673e 605f 2072 656c 6174 696f 6e73  ing>`_ relations
-000005e0: 6869 700a 6265 7477 6565 6e20 6060 686f  hip.between ``ho
-000005f0: 7374 6060 2061 6e64 2060 6070 6c75 6769  st`` and ``plugi
-00000600: 6e73 6060 2e0a 0a54 6865 2060 6070 6c75  ns``...The ``plu
-00000610: 6767 7960 6020 6170 7072 6f61 6368 2070  ggy`` approach p
-00000620: 7574 7320 7468 6520 6275 7264 656e 206f  uts the burden o
-00000630: 6e20 7468 6520 6465 7369 676e 6572 206f  n the designer o
-00000640: 6620 7468 650a 6060 686f 7374 2070 726f  f the.``host pro
-00000650: 6772 616d 6060 2074 6f20 7468 696e 6b20  gram`` to think 
-00000660: 6361 7265 6675 6c6c 7920 6162 6f75 7420  carefully about 
-00000670: 7768 6963 6820 6f62 6a65 6374 7320 6172  which objects ar
-00000680: 6520 7265 616c 6c79 0a6e 6565 6465 6420  e really.needed 
-00000690: 696e 2061 2068 6f6f 6b20 696d 706c 656d  in a hook implem
-000006a0: 656e 7461 7469 6f6e 2e20 5468 6973 2067  entation. This g
-000006b0: 6976 6573 2060 6070 6c75 6769 6e60 6020  ives ``plugin`` 
-000006c0: 6372 6561 746f 7273 2061 2063 6c65 6172  creators a clear
-000006d0: 0a66 7261 6d65 776f 726b 2066 6f72 2068  .framework for h
-000006e0: 6f77 2074 6f20 6578 7465 6e64 2074 6865  ow to extend the
-000006f0: 2060 6068 6f73 7460 6020 7669 6120 6120   ``host`` via a 
-00000700: 7765 6c6c 2064 6566 696e 6564 2073 6574  well defined set
-00000710: 206f 6620 6675 6e63 7469 6f6e 730a 616e   of functions.an
-00000720: 6420 6f62 6a65 6374 7320 746f 2077 6f72  d objects to wor
-00000730: 6b20 7769 7468 2e0a 0a48 6f77 2064 6f65  k with...How doe
-00000740: 7320 6974 2077 6f72 6b3f 0a2a 2a2a 2a2a  s it work?.*****
-00000750: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a4c 6574  ************.Let
-00000760: 2075 7320 7374 6172 7420 7769 7468 2061   us start with a
-00000770: 2073 686f 7274 206f 7665 7276 6965 7720   short overview 
-00000780: 6f66 2077 6861 7420 6973 2069 6e76 6f6c  of what is invol
-00000790: 7665 643a 0a0a 2a20 6060 686f 7374 6060  ved:..* ``host``
-000007a0: 206f 7220 6060 686f 7374 2070 726f 6772   or ``host progr
-000007b0: 616d 6060 3a20 7468 6520 7072 6f67 7261  am``: the progra
-000007c0: 6d20 6f66 6665 7269 6e67 2065 7874 656e  m offering exten
-000007d0: 7369 6269 6c69 7479 0a20 2062 7920 7370  sibility.  by sp
-000007e0: 6563 6966 7969 6e67 2060 6068 6f6f 6b20  ecifying ``hook 
-000007f0: 6675 6e63 7469 6f6e 7360 6020 616e 6420  functions`` and 
-00000800: 696e 766f 6b69 6e67 2074 6865 6972 2069  invoking their i
-00000810: 6d70 6c65 6d65 6e74 6174 696f 6e28 7329  mplementation(s)
-00000820: 2061 730a 2020 7061 7274 206f 6620 7072   as.  part of pr
-00000830: 6f67 7261 6d20 6578 6563 7574 696f 6e0a  ogram execution.
-00000840: 2a20 6060 706c 7567 696e 6060 3a20 7468  * ``plugin``: th
-00000850: 6520 7072 6f67 7261 6d20 696d 706c 656d  e program implem
-00000860: 656e 7469 6e67 2028 6120 7375 6273 6574  enting (a subset
-00000870: 206f 6629 2074 6865 2073 7065 6369 6669   of) the specifi
-00000880: 6564 2068 6f6f 6b73 2061 6e64 0a20 2070  ed hooks and.  p
-00000890: 6172 7469 6369 7061 7469 6e67 2069 6e20  articipating in 
-000008a0: 7072 6f67 7261 6d20 6578 6563 7574 696f  program executio
-000008b0: 6e20 7768 656e 2074 6865 2069 6d70 6c65  n when the imple
-000008c0: 6d65 6e74 6174 696f 6e73 2061 7265 2069  mentations are i
-000008d0: 6e76 6f6b 6564 0a20 2062 7920 7468 6520  nvoked.  by the 
-000008e0: 6060 686f 7374 6060 0a2a 2060 6070 6c75  ``host``.* ``plu
-000008f0: 6767 7960 603a 2063 6f6e 6e65 6374 7320  ggy``: connects 
-00000900: 6060 686f 7374 6060 2061 6e64 2060 6070  ``host`` and ``p
-00000910: 6c75 6769 6e73 6060 2062 7920 7573 696e  lugins`` by usin
-00000920: 6720 2e2e 2e0a 0a20 2020 202d 2074 6865  g .....    - the
-00000930: 2068 6f6f 6b20 3a72 6566 3a60 7370 6563   hook :ref:`spec
-00000940: 6966 6963 6174 696f 6e73 203c 7370 6563  ifications <spec
-00000950: 733e 6020 6465 6669 6e69 6e67 2063 616c  s>` defining cal
-00000960: 6c20 7369 676e 6174 7572 6573 0a20 2020  l signatures.   
-00000970: 2020 2070 726f 7669 6465 6420 6279 2074     provided by t
-00000980: 6865 2060 6068 6f73 7460 6020 2861 2e6b  he ``host`` (a.k
-00000990: 2e61 2060 6068 6f6f 6b73 7065 6373 6060  .a ``hookspecs``
-000009a0: 202d 2073 6565 203a 7265 663a 606d 6172   - see :ref:`mar
-000009b0: 6b69 6e67 5f68 6f6f 6b73 6029 0a20 2020  king_hooks`).   
-000009c0: 202d 2074 6865 2068 6f6f 6b20 3a72 6566   - the hook :ref
-000009d0: 3a60 696d 706c 656d 656e 7461 7469 6f6e  :`implementation
-000009e0: 7320 3c69 6d70 6c73 3e60 2070 726f 7669  s <impls>` provi
-000009f0: 6465 6420 6279 2072 6567 6973 7465 7265  ded by registere
-00000a00: 640a 2020 2020 2020 6060 706c 7567 696e  d.      ``plugin
-00000a10: 7360 6020 2861 2e6b 2e61 2060 6068 6f6f  s`` (a.k.a ``hoo
-00000a20: 6b69 6d70 6c60 6020 2d20 7365 6520 6063  kimpl`` - see `c
-00000a30: 616c 6c62 6163 6b73 605f 290a 2020 2020  allbacks`_).    
-00000a40: 2d20 7468 6520 686f 6f6b 203a 7265 663a  - the hook :ref:
-00000a50: 6063 616c 6c65 7220 3c63 616c 6c69 6e67  `caller <calling
-00000a60: 3e60 202d 2061 2063 616c 6c20 6c6f 6f70  >` - a call loop
-00000a70: 2074 7269 6767 6572 6564 2061 7420 6170   triggered at ap
-00000a80: 7072 6f70 7269 6174 650a 2020 2020 2020  propriate.      
-00000a90: 7072 6f67 7261 6d20 706f 7369 7469 6f6e  program position
-00000aa0: 7320 696e 2074 6865 2060 6068 6f73 7460  s in the ``host`
-00000ab0: 6020 696e 766f 6b69 6e67 2074 6865 2069  ` invoking the i
-00000ac0: 6d70 6c65 6d65 6e74 6174 696f 6e73 2061  mplementations a
-00000ad0: 6e64 0a20 2020 2020 2063 6f6c 6c65 6374  nd.      collect
-00000ae0: 696e 6720 7468 6520 7265 7375 6c74 730a  ing the results.
-00000af0: 0a20 2020 202e 2e2e 2077 6865 7265 2066  .    ... where f
-00000b00: 6f72 2065 6163 6820 7265 6769 7374 6572  or each register
-00000b10: 6564 2068 6f6f 6b20 2a73 7065 6369 6669  ed hook *specifi
-00000b20: 6361 7469 6f6e 2a2c 2061 2068 6f6f 6b20  cation*, a hook 
-00000b30: 2a63 616c 6c2a 2077 696c 6c0a 2020 2020  *call* will.    
-00000b40: 696e 766f 6b65 2075 7020 746f 2060 604e  invoke up to ``N
-00000b50: 6060 2072 6567 6973 7465 7265 6420 686f  `` registered ho
-00000b60: 6f6b 202a 696d 706c 656d 656e 7461 7469  ok *implementati
-00000b70: 6f6e 732a 2e0a 2a20 6060 7573 6572 6060  ons*..* ``user``
-00000b80: 3a20 7468 6520 7065 7273 6f6e 2077 686f  : the person who
-00000b90: 2069 6e73 7461 6c6c 6564 2074 6865 2060   installed the `
-00000ba0: 6068 6f73 7420 7072 6f67 7261 6d60 6020  `host program`` 
-00000bb0: 616e 6420 7761 6e74 7320 746f 0a20 2065  and wants to.  e
-00000bc0: 7874 656e 6420 6974 7320 6675 6e63 7469  xtend its functi
-00000bd0: 6f6e 616c 6974 7920 7769 7468 2060 6070  onality with ``p
-00000be0: 6c75 6769 6e73 6060 2e20 496e 2074 6865  lugins``. In the
-00000bf0: 2073 696d 706c 6573 7420 6361 7365 2074   simplest case t
-00000c00: 6865 7920 696e 7374 616c 6c0a 2020 7468  hey install.  th
-00000c10: 6520 6060 706c 7567 696e 6060 2069 6e20  e ``plugin`` in 
-00000c20: 7468 6520 7361 6d65 2065 6e76 6972 6f6e  the same environ
-00000c30: 6d65 6e74 2061 7320 7468 6520 6060 686f  ment as the ``ho
-00000c40: 7374 6060 2061 6e64 2074 6865 206d 6167  st`` and the mag
-00000c50: 6963 2077 696c 6c0a 2020 6861 7070 656e  ic will.  happen
-00000c60: 2077 6865 6e20 7468 6520 6060 686f 7374   when the ``host
-00000c70: 2070 726f 6772 616d 6060 2069 7320 7275   program`` is ru
-00000c80: 6e20 7468 6520 6e65 7874 2074 696d 652e  n the next time.
-00000c90: 2044 6570 656e 6469 6e67 206f 6e0a 2020   Depending on.  
-00000ca0: 7468 6520 6060 706c 7567 696e 6060 2c20  the ``plugin``, 
-00000cb0: 7468 6572 6520 6d69 6768 7420 6265 206f  there might be o
-00000cc0: 7468 6572 2074 6869 6e67 7320 7468 6579  ther things they
-00000cd0: 206e 6565 6420 746f 2064 6f2e 2046 6f72   need to do. For
-00000ce0: 2065 7861 6d70 6c65 2c0a 2020 7468 6579   example,.  they
-00000cf0: 206d 6967 6874 2068 6176 6520 746f 2063   might have to c
-00000d00: 616c 6c20 7468 6520 686f 7374 2077 6974  all the host wit
-00000d10: 6820 616e 2061 6464 6974 696f 6e61 6c20  h an additional 
-00000d20: 636f 6d6d 616e 646c 696e 6520 7061 7261  commandline para
-00000d30: 6d65 7465 720a 2020 746f 2074 6865 2068  meter.  to the h
-00000d40: 6f73 7420 7468 6174 2074 6865 2060 6070  ost that the ``p
-00000d50: 6c75 6769 6e60 6020 6164 6465 642e 0a0a  lugin`` added...
-00000d60: 4120 746f 7920 6578 616d 706c 650a 2d2d  A toy example.--
-00000d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4c65 7420  -----------.Let 
-00000d80: 7573 2064 656d 6f6e 7374 7261 7465 2074  us demonstrate t
-00000d90: 6865 2063 6f72 6520 6675 6e63 7469 6f6e  he core function
-00000da0: 616c 6974 7920 696e 206f 6e65 206d 6f64  ality in one mod
-00000db0: 756c 6520 616e 6420 7368 6f77 2068 6f77  ule and show how
-00000dc0: 2079 6f75 2063 616e 0a73 7461 7274 2065   you can.start e
-00000dd0: 7870 6572 696d 656e 7469 6e67 2077 6974  xperimenting wit
-00000de0: 6820 706c 7567 6779 2066 756e 6374 696f  h pluggy functio
-00000df0: 6e61 6c69 7479 2e0a 0a2e 2e20 6c69 7465  nality..... lite
-00000e00: 7261 6c69 6e63 6c75 6465 3a3a 2065 7861  ralinclude:: exa
-00000e10: 6d70 6c65 732f 746f 792d 6578 616d 706c  mples/toy-exampl
-00000e20: 652e 7079 0a0a 5275 6e6e 696e 6720 7468  e.py..Running th
-00000e30: 6973 2064 6972 6563 746c 7920 6765 7473  is directly gets
-00000e40: 2075 733a 3a0a 0a20 2020 2024 2070 7974   us::..    $ pyt
-00000e50: 686f 6e20 646f 6373 2f65 7861 6d70 6c65  hon docs/example
-00000e60: 732f 746f 792d 6578 616d 706c 652e 7079  s/toy-example.py
-00000e70: 0a0a 2020 2020 696e 7369 6465 2050 6c75  ..    inside Plu
-00000e80: 6769 6e5f 322e 6d79 686f 6f6b 2829 0a20  gin_2.myhook(). 
-00000e90: 2020 2069 6e73 6964 6520 506c 7567 696e     inside Plugin
-00000ea0: 5f31 2e6d 7968 6f6f 6b28 290a 2020 2020  _1.myhook().    
-00000eb0: 5b2d 312c 2033 5d0a 0a41 2063 6f6d 706c  [-1, 3]..A compl
-00000ec0: 6574 6520 6578 616d 706c 650a 2d2d 2d2d  ete example.----
-00000ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a4e  --------------.N
-00000ee0: 6f77 206c 6574 2075 7320 6465 6d6f 6e73  ow let us demons
-00000ef0: 7472 6174 6520 686f 7720 7468 6973 2070  trate how this p
-00000f00: 6c61 7973 2074 6f67 6574 6865 7220 696e  lays together in
-00000f10: 2061 2076 6167 7565 6c79 2072 6561 6c20   a vaguely real 
-00000f20: 776f 726c 6420 7363 656e 6172 696f 2e0a  world scenario..
-00000f30: 0a4c 6574 2773 2061 7373 756d 6520 6f75  .Let's assume ou
-00000f40: 7220 6060 686f 7374 2070 726f 6772 616d  r ``host program
-00000f50: 6060 2069 7320 6361 6c6c 6564 202a 2a65  `` is called **e
-00000f60: 6767 7361 6d70 6c65 2a2a 2077 6865 7265  ggsample** where
-00000f70: 2073 6f6d 6520 6567 6773 2077 696c 6c0a   some eggs will.
-00000f80: 6265 2070 7265 7061 7265 6420 616e 6420  be prepared and 
-00000f90: 7365 7276 6564 2077 6974 6820 6120 7472  served with a tr
-00000fa0: 6179 2063 6f6e 7461 696e 696e 6720 636f  ay containing co
-00000fb0: 6e64 696d 656e 7473 2e20 4173 2065 7665  ndiments. As eve
-00000fc0: 7279 626f 6479 206b 6e6f 7773 3a0a 7468  rybody knows:.th
-00000fd0: 6520 6d6f 7265 2063 6f6f 6b73 2061 7265  e more cooks are
-00000fe0: 2069 6e76 6f6c 7665 6420 7468 6520 6265   involved the be
-00000ff0: 7474 6572 2074 6865 2066 6f6f 642c 2073  tter the food, s
-00001000: 6f20 6c65 7420 7573 206d 616b 6520 7468  o let us make th
-00001010: 6520 7072 6f63 6573 730a 706c 7567 6761  e process.plugga
-00001020: 626c 6520 616e 6420 7772 6974 6520 6120  ble and write a 
-00001030: 706c 7567 696e 2074 6861 7420 696d 7072  plugin that impr
-00001040: 6f76 6573 2074 6865 206d 6561 6c20 7769  oves the meal wi
-00001050: 7468 2073 6f6d 6520 7370 616d 2061 6e64  th some spam and
-00001060: 2072 6570 6c61 6365 730a 7468 6520 7374   replaces.the st
-00001070: 6561 6b20 7361 7563 6520 286e 6f62 6f64  eak sauce (nobod
-00001080: 7920 6c69 6b65 7320 7468 6174 2061 6e79  y likes that any
-00001090: 7761 7929 2077 6974 6820 7370 616d 2073  way) with spam s
-000010a0: 6175 6365 2028 6974 2773 2061 2074 6869  auce (it's a thi
-000010b0: 6e67 202d 2074 7275 7374 206d 6529 2e0a  ng - trust me)..
-000010c0: 0a2e 2e20 6e6f 7465 3a3a 0a0a 2020 2020  ... note::..    
-000010d0: 2a2a 6e61 6d69 6e67 206d 6172 6b65 7273  **naming markers
-000010e0: 2a2a 3a20 6060 486f 6f6b 5370 6563 4d61  **: ``HookSpecMa
-000010f0: 726b 6572 6060 2061 6e64 2060 6048 6f6f  rker`` and ``Hoo
-00001100: 6b49 6d70 6c4d 6172 6b65 7260 6020 6d75  kImplMarker`` mu
-00001110: 7374 2062 650a 2020 2020 696e 6974 6961  st be.    initia
-00001120: 6c69 7a65 6420 7769 7468 2074 6865 206e  lized with the n
-00001130: 616d 6520 6f66 2074 6865 2060 6068 6f73  ame of the ``hos
-00001140: 7460 6020 7072 6f6a 6563 7420 2874 6865  t`` project (the
-00001150: 2060 606e 616d 6560 600a 2020 2020 7061   ``name``.    pa
-00001160: 7261 6d65 7465 7220 696e 2060 6073 6574  rameter in ``set
-00001170: 7570 2829 6060 2920 2d20 736f 202a 2a65  up()``) - so **e
-00001180: 6767 7361 6d70 6c65 2a2a 2069 6e20 6f75  ggsample** in ou
-00001190: 7220 6361 7365 2e0a 0a20 2020 202a 2a6e  r case...    **n
-000011a0: 616d 696e 6720 706c 7567 696e 2070 726f  aming plugin pro
-000011b0: 6a65 6374 732a 2a3a 2074 6865 7920 7368  jects**: they sh
-000011c0: 6f75 6c64 2062 6520 6e61 6d65 6420 696e  ould be named in
-000011d0: 2074 6865 2066 6f72 6d20 6f66 0a20 2020   the form of.   
-000011e0: 2060 603c 686f 7374 3e2d 3c70 6c75 6769   ``<host>-<plugi
-000011f0: 6e3e 6060 2028 652e 672e 2060 6070 7974  n>`` (e.g. ``pyt
-00001200: 6573 742d 7864 6973 7460 6029 2c20 7468  est-xdist``), th
-00001210: 6572 6566 6f72 6520 7765 2063 616c 6c20  erefore we call 
-00001220: 6f75 720a 2020 2020 706c 7567 696e 202a  our.    plugin *
-00001230: 6567 6773 616d 706c 652d 7370 616d 2a2e  eggsample-spam*.
-00001240: 0a0a 5468 6520 686f 7374 0a5e 5e5e 5e5e  ..The host.^^^^^
-00001250: 5e5e 5e0a 6060 6567 6773 616d 706c 652f  ^^^.``eggsample/
-00001260: 6567 6773 616d 706c 652f 5f5f 696e 6974  eggsample/__init
-00001270: 5f5f 2e70 7960 600a 0a2e 2e20 6c69 7465  __.py``.... lite
-00001280: 7261 6c69 6e63 6c75 6465 3a3a 2065 7861  ralinclude:: exa
-00001290: 6d70 6c65 732f 6567 6773 616d 706c 652f  mples/eggsample/
-000012a0: 6567 6773 616d 706c 652f 5f5f 696e 6974  eggsample/__init
-000012b0: 5f5f 2e70 790a 0a60 6065 6767 7361 6d70  __.py..``eggsamp
-000012c0: 6c65 2f65 6767 7361 6d70 6c65 2f68 6f6f  le/eggsample/hoo
-000012d0: 6b73 7065 6373 2e70 7960 600a 0a2e 2e20  kspecs.py``.... 
-000012e0: 6c69 7465 7261 6c69 6e63 6c75 6465 3a3a  literalinclude::
-000012f0: 2065 7861 6d70 6c65 732f 6567 6773 616d   examples/eggsam
-00001300: 706c 652f 6567 6773 616d 706c 652f 686f  ple/eggsample/ho
-00001310: 6f6b 7370 6563 732e 7079 0a0a 6060 6567  okspecs.py..``eg
-00001320: 6773 616d 706c 652f 6567 6773 616d 706c  gsample/eggsampl
-00001330: 652f 6c69 622e 7079 6060 0a0a 2e2e 206c  e/lib.py``.... l
-00001340: 6974 6572 616c 696e 636c 7564 653a 3a20  iteralinclude:: 
-00001350: 6578 616d 706c 6573 2f65 6767 7361 6d70  examples/eggsamp
-00001360: 6c65 2f65 6767 7361 6d70 6c65 2f6c 6962  le/eggsample/lib
-00001370: 2e70 790a 0a60 6065 6767 7361 6d70 6c65  .py..``eggsample
-00001380: 2f65 6767 7361 6d70 6c65 2f68 6f73 742e  /eggsample/host.
-00001390: 7079 6060 0a0a 2e2e 206c 6974 6572 616c  py``.... literal
-000013a0: 696e 636c 7564 653a 3a20 6578 616d 706c  include:: exampl
-000013b0: 6573 2f65 6767 7361 6d70 6c65 2f65 6767  es/eggsample/egg
-000013c0: 7361 6d70 6c65 2f68 6f73 742e 7079 0a0a  sample/host.py..
-000013d0: 6060 6567 6773 616d 706c 652f 7365 7475  ``eggsample/setu
-000013e0: 702e 7079 6060 0a0a 2e2e 206c 6974 6572  p.py``.... liter
-000013f0: 616c 696e 636c 7564 653a 3a20 6578 616d  alinclude:: exam
-00001400: 706c 6573 2f65 6767 7361 6d70 6c65 2f73  ples/eggsample/s
-00001410: 6574 7570 2e70 790a 0a4c 6574 2773 2067  etup.py..Let's g
-00001420: 6574 2063 6f6f 6b69 6e67 202d 2077 6520  et cooking - we 
-00001430: 696e 7374 616c 6c20 7468 6520 686f 7374  install the host
-00001440: 2061 6e64 2073 6565 2077 6861 7420 6120   and see what a 
-00001450: 7072 6f67 7261 6d20 7275 6e20 6c6f 6f6b  program run look
-00001460: 7320 6c69 6b65 3a3a 0a0a 2020 2020 2420  s like::..    $ 
-00001470: 7069 7020 696e 7374 616c 6c20 2d2d 6564  pip install --ed
-00001480: 6974 6162 6c65 2070 6c75 6767 792f 646f  itable pluggy/do
-00001490: 6373 2f65 7861 6d70 6c65 732f 6567 6773  cs/examples/eggs
-000014a0: 616d 706c 650a 2020 2020 2420 6567 6773  ample.    $ eggs
-000014b0: 616d 706c 650a 0a20 2020 2059 6f75 7220  ample..    Your 
-000014c0: 666f 6f64 2e20 456e 6a6f 7920 736f 6d65  food. Enjoy some
-000014d0: 2065 6767 2c20 6567 672c 2073 616c 742c   egg, egg, salt,
-000014e0: 2065 6767 2c20 6567 672c 2070 6570 7065   egg, egg, peppe
-000014f0: 722c 2065 6767 0a20 2020 2053 6f6d 6520  r, egg.    Some 
-00001500: 636f 6e64 696d 656e 7473 3f20 5765 2068  condiments? We h
-00001510: 6176 6520 7069 636b 6c65 6420 7761 6c6e  ave pickled waln
-00001520: 7574 732c 2073 7465 616b 2073 6175 6365  uts, steak sauce
-00001530: 2c20 6d75 7368 7920 7065 6173 2c20 6d69  , mushy peas, mi
-00001540: 6e74 2073 6175 6365 0a0a 5468 6520 706c  nt sauce..The pl
-00001550: 7567 696e 0a5e 5e5e 5e5e 5e5e 5e5e 5e0a  ugin.^^^^^^^^^^.
-00001560: 6060 6567 6773 616d 706c 652d 7370 616d  ``eggsample-spam
-00001570: 2f65 6767 7361 6d70 6c65 5f73 7061 6d2e  /eggsample_spam.
-00001580: 7079 6060 0a0a 2e2e 206c 6974 6572 616c  py``.... literal
-00001590: 696e 636c 7564 653a 3a20 6578 616d 706c  include:: exampl
-000015a0: 6573 2f65 6767 7361 6d70 6c65 2d73 7061  es/eggsample-spa
-000015b0: 6d2f 6567 6773 616d 706c 655f 7370 616d  m/eggsample_spam
-000015c0: 2e70 790a 0a60 6065 6767 7361 6d70 6c65  .py..``eggsample
-000015d0: 2d73 7061 6d2f 7365 7475 702e 7079 6060  -spam/setup.py``
-000015e0: 0a0a 2e2e 206c 6974 6572 616c 696e 636c  .... literalincl
-000015f0: 7564 653a 3a20 6578 616d 706c 6573 2f65  ude:: examples/e
-00001600: 6767 7361 6d70 6c65 2d73 7061 6d2f 7365  ggsample-spam/se
-00001610: 7475 702e 7079 0a0a 4c65 7427 7320 6765  tup.py..Let's ge
-00001620: 7420 636f 6f6b 696e 6720 7769 7468 206d  t cooking with m
-00001630: 6f72 6520 636f 6f6b 7320 2d20 7765 2069  ore cooks - we i
-00001640: 6e73 7461 6c6c 2074 6865 2070 6c75 6769  nstall the plugi
-00001650: 6e20 616e 6420 616e 6420 7365 6520 7768  n and and see wh
-00001660: 6174 0a77 6520 6765 743a 3a0a 0a20 2020  at.we get::..   
-00001670: 2024 2070 6970 2069 6e73 7461 6c6c 202d   $ pip install -
-00001680: 2d65 6469 7461 626c 6520 706c 7567 6779  -editable pluggy
-00001690: 2f64 6f63 732f 6578 616d 706c 6573 2f65  /docs/examples/e
-000016a0: 6767 7361 6d70 6c65 2d73 7061 6d0a 2020  ggsample-spam.  
-000016b0: 2020 2420 6567 6773 616d 706c 650a 0a20    $ eggsample.. 
-000016c0: 2020 2059 6f75 7220 666f 6f64 2e20 456e     Your food. En
-000016d0: 6a6f 7920 736f 6d65 2065 6767 2c20 6c6f  joy some egg, lo
-000016e0: 7665 6c79 2073 7061 6d2c 2073 616c 742c  vely spam, salt,
-000016f0: 2065 6767 2c20 6567 672c 2065 6767 2c20   egg, egg, egg, 
-00001700: 776f 6e64 6572 6f75 7320 7370 616d 2c20  wonderous spam, 
-00001710: 6567 672c 2070 6570 7065 720a 2020 2020  egg, pepper.    
-00001720: 536f 6d65 2063 6f6e 6469 6d65 6e74 733f  Some condiments?
-00001730: 2057 6520 6861 7665 2070 6963 6b6c 6564   We have pickled
-00001740: 2077 616c 6e75 7473 2c20 6d75 7368 7920   walnuts, mushy 
-00001750: 7065 6173 2c20 6d69 6e74 2073 6175 6365  peas, mint sauce
-00001760: 2c20 7370 616d 2073 6175 6365 0a20 2020  , spam sauce.   
-00001770: 204e 6f77 2074 6869 7320 6973 2077 6861   Now this is wha
-00001780: 7420 4920 6361 6c6c 2061 2063 6f6e 6469  t I call a condi
-00001790: 6d65 6e74 7320 7472 6179 210a 0a4d 6f72  ments tray!..Mor
-000017a0: 6520 7265 616c 2077 6f72 6c64 2065 7861  e real world exa
-000017b0: 6d70 6c65 730a 2d2d 2d2d 2d2d 2d2d 2d2d  mples.----------
-000017c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a54  --------------.T
-000017d0: 6f20 7365 6520 686f 7720 6060 706c 7567  o see how ``plug
-000017e0: 6779 6060 2069 7320 7573 6564 2069 6e20  gy`` is used in 
-000017f0: 7468 6520 7265 616c 2077 6f72 6c64 2c20  the real world, 
-00001800: 6861 7665 2061 206c 6f6f 6b20 6174 2074  have a look at t
-00001810: 6865 7365 2070 726f 6a65 6374 730a 646f  hese projects.do
-00001820: 6375 6d65 6e74 6174 696f 6e20 616e 6420  cumentation and 
-00001830: 736f 7572 6365 2063 6f64 653a 0a0a 2a20  source code:..* 
-00001840: 3a72 6566 3a60 7079 7465 7374 203c 7079  :ref:`pytest <py
-00001850: 7465 7374 3a77 7269 7469 6e67 2d70 6c75  test:writing-plu
-00001860: 6769 6e73 3e60 0a2a 203a 7374 643a 646f  gins>`.* :std:do
-00001870: 633a 6074 6f78 203c 746f 783a 706c 7567  c:`tox <tox:plug
-00001880: 696e 733e 600a 2a20 3a73 7464 3a64 6f63  ins>`.* :std:doc
-00001890: 3a60 6465 7670 6920 3c64 6576 7069 3a64  :`devpi <devpi:d
-000018a0: 6576 6775 6964 652f 696e 6465 783e 600a  evguide/index>`.
-000018b0: 0a46 6f72 206d 6f72 6520 6465 7461 696c  .For more detail
-000018c0: 7320 616e 6420 6164 7661 6e63 6564 2075  s and advanced u
-000018d0: 7361 6765 2070 6c65 6173 6520 7265 6164  sage please read
-000018e0: 206f 6e2e 0a0a 2e2e 205f 6465 6669 6e65   on..... _define
-000018f0: 3a0a 0a44 6566 696e 6520 616e 6420 636f  :..Define and co
-00001900: 6c6c 6563 7420 686f 6f6b 730a 2a2a 2a2a  llect hooks.****
-00001910: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00001920: 2a2a 2a2a 0a41 202a 706c 7567 696e 2a20  ****.A *plugin* 
-00001930: 6973 2061 203a 7265 663a 606e 616d 6573  is a :ref:`names
-00001940: 7061 6365 203c 7079 7468 6f6e 3a74 7574  pace <python:tut
-00001950: 2d73 636f 7065 733e 6020 7479 7065 2028  -scopes>` type (
-00001960: 6375 7272 656e 746c 7920 6f6e 6520 6f66  currently one of
-00001970: 2061 0a60 6063 6c61 7373 6060 206f 7220   a.``class`` or 
-00001980: 6d6f 6475 6c65 2920 7768 6963 6820 6465  module) which de
-00001990: 6669 6e65 7320 6120 7365 7420 6f66 202a  fines a set of *
-000019a0: 686f 6f6b 2a20 6675 6e63 7469 6f6e 732e  hook* functions.
-000019b0: 0a0a 4173 206d 656e 7469 6f6e 6564 2069  ..As mentioned i
-000019c0: 6e20 3a72 6566 3a60 6d61 6e61 6765 602c  n :ref:`manage`,
-000019d0: 2061 6c6c 202a 706c 7567 696e 732a 2077   all *plugins* w
-000019e0: 6869 6368 2073 7065 6369 6679 202a 686f  hich specify *ho
-000019f0: 6f6b 732a 0a61 7265 206d 616e 6167 6564  oks*.are managed
-00001a00: 2062 7920 616e 2069 6e73 7461 6e63 6520   by an instance 
-00001a10: 6f66 2061 203a 7079 3a63 6c61 7373 3a60  of a :py:class:`
-00001a20: 706c 7567 6779 2e50 6c75 6769 6e4d 616e  pluggy.PluginMan
-00001a30: 6167 6572 6020 7768 6963 680a 6465 6669  ager` which.defi
-00001a40: 6e65 7320 7468 6520 7072 696d 6172 7920  nes the primary 
-00001a50: 6060 706c 7567 6779 6060 2041 5049 2e0a  ``pluggy`` API..
-00001a60: 0a49 6e20 6f72 6465 7220 666f 7220 6120  .In order for a 
-00001a70: 3a70 793a 636c 6173 733a 607e 706c 7567  :py:class:`~plug
-00001a80: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
-00001a90: 6020 746f 2064 6574 6563 7420 6675 6e63  ` to detect func
-00001aa0: 7469 6f6e 7320 696e 2061 206e 616d 6573  tions in a names
-00001ab0: 7061 6365 0a69 6e74 656e 6465 6420 746f  pace.intended to
-00001ac0: 2062 6520 2a68 6f6f 6b73 2a2c 2074 6865   be *hooks*, the
-00001ad0: 7920 6d75 7374 2062 6520 6465 636f 7261  y must be decora
-00001ae0: 7465 6420 7573 696e 6720 7370 6563 6961  ted using specia
-00001af0: 6c20 6060 706c 7567 6779 6060 202a 6d61  l ``pluggy`` *ma
-00001b00: 726b 732a 2e0a 0a2e 2e20 5f6d 6172 6b69  rks*..... _marki
-00001b10: 6e67 5f68 6f6f 6b73 3a0a 0a4d 6172 6b69  ng_hooks:..Marki
-00001b20: 6e67 2068 6f6f 6b73 0a2d 2d2d 2d2d 2d2d  ng hooks.-------
-00001b30: 2d2d 2d2d 2d2d 0a54 6865 203a 7079 3a63  ------.The :py:c
-00001b40: 6c61 7373 3a60 7e70 6c75 6767 792e 486f  lass:`~pluggy.Ho
-00001b50: 6f6b 7370 6563 4d61 726b 6572 6020 616e  okspecMarker` an
-00001b60: 6420 3a70 793a 636c 6173 733a 607e 706c  d :py:class:`~pl
-00001b70: 7567 6779 2e48 6f6f 6b69 6d70 6c4d 6172  uggy.HookimplMar
-00001b80: 6b65 7260 0a64 6563 6f72 6174 6f72 7320  ker`.decorators 
-00001b90: 6172 6520 7573 6564 2074 6f20 2a6d 6172  are used to *mar
-00001ba0: 6b2a 2066 756e 6374 696f 6e73 2066 6f72  k* functions for
-00001bb0: 2064 6574 6563 7469 6f6e 2062 7920 610a   detection by a.
-00001bc0: 3a70 793a 636c 6173 733a 607e 706c 7567  :py:class:`~plug
-00001bd0: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
-00001be0: 603a 0a0a 2e2e 2063 6f64 652d 626c 6f63  `:.... code-bloc
-00001bf0: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
-00001c00: 6672 6f6d 2070 6c75 6767 7920 696d 706f  from pluggy impo
-00001c10: 7274 2048 6f6f 6b73 7065 634d 6172 6b65  rt HookspecMarke
-00001c20: 722c 2048 6f6f 6b69 6d70 6c4d 6172 6b65  r, HookimplMarke
-00001c30: 720a 0a20 2020 2068 6f6f 6b73 7065 6320  r..    hookspec 
-00001c40: 3d20 486f 6f6b 7370 6563 4d61 726b 6572  = HookspecMarker
-00001c50: 2822 7072 6f6a 6563 745f 6e61 6d65 2229  ("project_name")
-00001c60: 0a20 2020 2068 6f6f 6b69 6d70 6c20 3d20  .    hookimpl = 
-00001c70: 486f 6f6b 696d 706c 4d61 726b 6572 2822  HookimplMarker("
-00001c80: 7072 6f6a 6563 745f 6e61 6d65 2229 0a0a  project_name")..
-00001c90: 0a45 6163 6820 6465 636f 7261 746f 7220  .Each decorator 
-00001ca0: 7479 7065 2074 616b 6573 2061 2073 696e  type takes a sin
-00001cb0: 676c 6520 6060 7072 6f6a 6563 745f 6e61  gle ``project_na
-00001cc0: 6d65 6060 2073 7472 696e 6720 6173 2069  me`` string as i
-00001cd0: 7473 0a6c 6f6e 6520 6172 6775 6d65 6e74  ts.lone argument
-00001ce0: 2074 6865 2076 616c 7565 206f 6620 7768   the value of wh
-00001cf0: 6963 6820 6973 2075 7365 6420 746f 206d  ich is used to m
-00001d00: 6172 6b20 686f 6f6b 7320 666f 7220 6465  ark hooks for de
-00001d10: 7465 6374 696f 6e20 6279 0a61 2073 696d  tection by.a sim
-00001d20: 696c 6172 6c79 2063 6f6e 6669 6775 7265  ilarly configure
-00001d30: 6420 3a70 793a 636c 6173 733a 607e 706c  d :py:class:`~pl
-00001d40: 7567 6779 2e50 6c75 6769 6e4d 616e 6167  uggy.PluginManag
-00001d50: 6572 6020 696e 7374 616e 6365 2e0a 0a54  er` instance...T
-00001d60: 6861 7420 6973 2c20 6120 2a6d 6172 6b2a  hat is, a *mark*
-00001d70: 2074 7970 6520 6361 6c6c 6564 2077 6974   type called wit
-00001d80: 6820 6060 7072 6f6a 6563 745f 6e61 6d65  h ``project_name
-00001d90: 6060 2072 6574 7572 6e73 2061 6e20 6f62  `` returns an ob
-00001da0: 6a65 6374 2077 6869 6368 0a63 616e 2062  ject which.can b
-00001db0: 6520 7573 6564 2074 6f20 6465 636f 7261  e used to decora
-00001dc0: 7465 2066 756e 6374 696f 6e73 2077 6869  te functions whi
-00001dd0: 6368 2077 696c 6c20 7468 656e 2062 6520  ch will then be 
-00001de0: 6465 7465 6374 6564 2062 7920 610a 3a70  detected by a.:p
-00001df0: 793a 636c 6173 733a 607e 706c 7567 6779  y:class:`~pluggy
-00001e00: 2e50 6c75 6769 6e4d 616e 6167 6572 6020  .PluginManager` 
-00001e10: 7768 6963 6820 7761 7320 696e 7374 616e  which was instan
-00001e20: 7469 6174 6564 2077 6974 6820 7468 6520  tiated with the 
-00001e30: 7361 6d65 0a60 6070 726f 6a65 6374 5f6e  same.``project_n
-00001e40: 616d 6560 6020 7661 6c75 652e 0a0a 4675  ame`` value...Fu
-00001e50: 7274 6865 726d 6f72 652c 2065 6163 6820  rthermore, each 
-00001e60: 2a68 6f6f 6b69 6d70 6c2a 206f 7220 2a68  *hookimpl* or *h
-00001e70: 6f6f 6b73 7065 632a 2064 6563 6f72 6174  ookspec* decorat
-00001e80: 6f72 2063 616e 2063 6f6e 6669 6775 7265  or can configure
-00001e90: 2074 6865 0a75 6e64 6572 6c79 696e 6720   the.underlying 
-00001ea0: 6361 6c6c 2d74 696d 6520 6265 6861 7669  call-time behavi
-00001eb0: 6f72 206f 6620 6561 6368 202a 686f 6f6b  or of each *hook
-00001ec0: 2a20 6f62 6a65 6374 2062 7920 7072 6f76  * object by prov
-00001ed0: 6964 696e 6720 7370 6563 6961 6c0a 2a6f  iding special.*o
-00001ee0: 7074 696f 6e73 2a20 7061 7373 6564 2061  ptions* passed a
-00001ef0: 7320 6b65 7977 6f72 6420 6172 6775 6d65  s keyword argume
-00001f00: 6e74 732e 0a0a 0a2e 2e20 6e6f 7465 3a3a  nts...... note::
-00001f10: 0a20 2020 2054 6865 2066 6f6c 6c6f 7769  .    The followi
-00001f20: 6e67 2073 6563 7469 6f6e 7320 636f 7272  ng sections corr
-00001f30: 6573 706f 6e64 2074 6f20 7369 6d69 6c61  espond to simila
-00001f40: 7220 646f 6375 6d65 6e74 6174 696f 6e20  r documentation 
-00001f50: 696e 0a20 2020 2060 6070 7974 6573 7460  in.    ``pytest`
-00001f60: 6020 666f 7220 3a72 6566 3a60 7079 7465  ` for :ref:`pyte
-00001f70: 7374 3a77 7269 7469 6e67 686f 6f6b 7360  st:writinghooks`
-00001f80: 2061 6e64 2063 616e 2062 6520 7573 6564   and can be used
-00001f90: 2061 730a 2020 2020 6120 7375 7070 6c65   as.    a supple
-00001fa0: 6d65 6e74 6172 7920 7265 736f 7572 6365  mentary resource
-00001fb0: 2e0a 0a2e 2e20 5f69 6d70 6c73 3a0a 0a49  ..... _impls:..I
-00001fc0: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a2d  mplementations.-
-00001fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a41  --------------.A
-00001fe0: 2068 6f6f 6b20 2a69 6d70 6c65 6d65 6e74   hook *implement
-00001ff0: 6174 696f 6e2a 2028 2a68 6f6f 6b69 6d70  ation* (*hookimp
-00002000: 6c2a 2920 6973 206a 7573 7420 6120 2863  l*) is just a (c
-00002010: 616c 6c62 6163 6b29 2066 756e 6374 696f  allback) functio
-00002020: 6e0a 7768 6963 6820 6861 7320 6265 656e  n.which has been
-00002030: 2061 7070 726f 7072 6961 7465 6c79 206d   appropriately m
-00002040: 6172 6b65 642e 0a0a 2a68 6f6f 6b69 6d70  arked...*hookimp
-00002050: 6c73 2a20 6172 6520 6c6f 6164 6564 2066  ls* are loaded f
-00002060: 726f 6d20 6120 706c 7567 696e 2075 7369  rom a plugin usi
-00002070: 6e67 2074 6865 0a3a 7079 3a6d 6574 683a  ng the.:py:meth:
-00002080: 607e 706c 7567 6779 2e50 6c75 6769 6e4d  `~pluggy.PluginM
-00002090: 616e 6167 6572 2e72 6567 6973 7465 7228  anager.register(
-000020a0: 2960 206d 6574 686f 643a 0a0a 2e2e 2063  )` method:.... c
-000020b0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-000020c0: 6f6e 0a0a 2020 2020 696d 706f 7274 2073  on..    import s
-000020d0: 7973 0a20 2020 2066 726f 6d20 706c 7567  ys.    from plug
-000020e0: 6779 2069 6d70 6f72 7420 506c 7567 696e  gy import Plugin
-000020f0: 4d61 6e61 6765 722c 2048 6f6f 6b69 6d70  Manager, Hookimp
-00002100: 6c4d 6172 6b65 720a 0a20 2020 2068 6f6f  lMarker..    hoo
-00002110: 6b69 6d70 6c20 3d20 486f 6f6b 696d 706c  kimpl = Hookimpl
-00002120: 4d61 726b 6572 2822 6d79 7072 6f6a 6563  Marker("myprojec
-00002130: 7422 290a 0a0a 2020 2020 4068 6f6f 6b69  t")...    @hooki
-00002140: 6d70 6c0a 2020 2020 6465 6620 7365 7475  mpl.    def setu
-00002150: 705f 7072 6f6a 6563 7428 636f 6e66 6967  p_project(config
-00002160: 2c20 6172 6773 293a 0a20 2020 2020 2020  , args):.       
-00002170: 2022 2222 5468 6973 2068 6f6f 6b20 6973   """This hook is
-00002180: 2075 7365 6420 746f 2070 726f 6365 7373   used to process
-00002190: 2074 6865 2069 6e69 7469 616c 2063 6f6e   the initial con
-000021a0: 6669 670a 2020 2020 2020 2020 616e 6420  fig.        and 
-000021b0: 706f 7373 6962 6c79 2069 6e70 7574 2061  possibly input a
-000021c0: 7267 756d 656e 7473 2e0a 2020 2020 2020  rguments..      
-000021d0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000021e0: 2061 7267 733a 0a20 2020 2020 2020 2020   args:.         
-000021f0: 2020 2063 6f6e 6669 672e 7072 6f63 6573     config.proces
-00002200: 735f 6172 6773 2861 7267 7329 0a0a 2020  s_args(args)..  
-00002210: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
-00002220: 6669 670a 0a0a 2020 2020 706d 203d 2050  fig...    pm = P
-00002230: 6c75 6769 6e4d 616e 6167 6572 2822 6d79  luginManager("my
-00002240: 7072 6f6a 6563 7422 290a 0a20 2020 2023  project")..    #
-00002250: 206c 6f61 6420 616c 6c20 686f 6f6b 696d   load all hookim
-00002260: 706c 7320 6672 6f6d 2074 6865 206c 6f63  pls from the loc
-00002270: 616c 206d 6f64 756c 6527 7320 6e61 6d65  al module's name
-00002280: 7370 6163 650a 2020 2020 706c 7567 696e  space.    plugin
-00002290: 5f6e 616d 6520 3d20 706d 2e72 6567 6973  _name = pm.regis
-000022a0: 7465 7228 7379 732e 6d6f 6475 6c65 735b  ter(sys.modules[
-000022b0: 5f5f 6e61 6d65 5f5f 5d29 0a0a 2e2e 205f  __name__]).... _
-000022c0: 6f70 7469 6f6e 616c 686f 6f6b 3a0a 0a4f  optionalhook:..O
-000022d0: 7074 696f 6e61 6c20 7661 6c69 6461 7469  ptional validati
-000022e0: 6f6e 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  on.^^^^^^^^^^^^^
-000022f0: 5e5e 5e5e 5e5e 0a4e 6f72 6d61 6c6c 7920  ^^^^^^.Normally 
-00002300: 6561 6368 202a 686f 6f6b 696d 706c 2a20  each *hookimpl* 
-00002310: 7368 6f75 6c64 2062 6520 7661 6c69 6461  should be valida
-00002320: 7465 6420 6167 6169 6e73 7420 6120 636f  ted against a co
-00002330: 7272 6573 706f 6e64 696e 670a 686f 6f6b  rresponding.hook
-00002340: 203a 7265 663a 6073 7065 6369 6669 6361   :ref:`specifica
-00002350: 7469 6f6e 203c 7370 6563 733e 602e 2049  tion <specs>`. I
-00002360: 6620 796f 7520 7761 6e74 2074 6f20 6d61  f you want to ma
-00002370: 6b65 2061 6e20 6578 6365 7074 696f 6e0a  ke an exception.
-00002380: 7468 656e 2074 6865 202a 686f 6f6b 696d  then the *hookim
-00002390: 706c 2a20 7368 6f75 6c64 2062 6520 6d61  pl* should be ma
-000023a0: 726b 6564 2077 6974 6820 7468 6520 6060  rked with the ``
-000023b0: 226f 7074 696f 6e61 6c68 6f6f 6b22 6060  "optionalhook"``
-000023c0: 206f 7074 696f 6e3a 0a0a 2e2e 2063 6f64   option:.... cod
-000023d0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-000023e0: 0a0a 2020 2020 4068 6f6f 6b69 6d70 6c28  ..    @hookimpl(
-000023f0: 6f70 7469 6f6e 616c 686f 6f6b 3d54 7275  optionalhook=Tru
-00002400: 6529 0a20 2020 2064 6566 2073 6574 7570  e).    def setup
-00002410: 5f70 726f 6a65 6374 2863 6f6e 6669 672c  _project(config,
-00002420: 2061 7267 7329 3a0a 2020 2020 2020 2020   args):.        
-00002430: 2222 2254 6869 7320 686f 6f6b 2069 7320  """This hook is 
-00002440: 7573 6564 2074 6f20 7072 6f63 6573 7320  used to process 
-00002450: 7468 6520 696e 6974 6961 6c20 636f 6e66  the initial conf
-00002460: 6967 0a20 2020 2020 2020 2061 6e64 2070  ig.        and p
-00002470: 6f73 7369 626c 7920 696e 7075 7420 6172  ossibly input ar
-00002480: 6775 6d65 6e74 732e 0a20 2020 2020 2020  guments..       
-00002490: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-000024a0: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
-000024b0: 2020 636f 6e66 6967 2e70 726f 6365 7373    config.process
-000024c0: 5f61 7267 7328 6172 6773 290a 0a20 2020  _args(args)..   
-000024d0: 2020 2020 2072 6574 7572 6e20 636f 6e66       return conf
-000024e0: 6967 0a0a 4361 6c6c 2074 696d 6520 6f72  ig..Call time or
-000024f0: 6465 720a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  der.^^^^^^^^^^^^
-00002500: 5e5e 5e0a 4279 2064 6566 6175 6c74 2068  ^^^.By default h
-00002510: 6f6f 6b73 2061 7265 203a 7265 663a 6063  ooks are :ref:`c
-00002520: 616c 6c65 6420 3c63 616c 6c69 6e67 3e60  alled <calling>`
-00002530: 2069 6e20 4c49 464f 2072 6567 6973 7465   in LIFO registe
-00002540: 7265 6420 6f72 6465 722c 2068 6f77 6576  red order, howev
-00002550: 6572 2c0a 6120 2a68 6f6f 6b69 6d70 6c2a  er,.a *hookimpl*
-00002560: 2063 616e 2069 6e66 6c75 656e 6365 2069   can influence i
-00002570: 7473 2063 616c 6c2d 7469 6d65 2069 6e76  ts call-time inv
-00002580: 6f63 6174 696f 6e20 706f 7369 7469 6f6e  ocation position
-00002590: 2075 7369 6e67 2073 7065 6369 616c 0a61   using special.a
-000025a0: 7474 7269 6275 7465 732e 2049 6620 6d61  ttributes. If ma
-000025b0: 726b 6564 2077 6974 6820 6120 6060 2274  rked with a ``"t
-000025c0: 7279 6669 7273 7422 6060 206f 7220 6060  ryfirst"`` or ``
-000025d0: 2274 7279 6c61 7374 2260 6020 6f70 7469  "trylast"`` opti
-000025e0: 6f6e 2069 740a 7769 6c6c 2062 6520 6578  on it.will be ex
-000025f0: 6563 7574 6564 202a 6669 7273 742a 206f  ecuted *first* o
-00002600: 7220 2a6c 6173 742a 2072 6573 7065 6374  r *last* respect
-00002610: 6976 656c 7920 696e 2074 6865 2068 6f6f  ively in the hoo
-00002620: 6b20 6361 6c6c 206c 6f6f 703a 0a0a 2e2e  k call loop:....
-00002630: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00002640: 7468 6f6e 0a0a 2020 2020 696d 706f 7274  thon..    import
-00002650: 2073 7973 0a20 2020 2066 726f 6d20 706c   sys.    from pl
-00002660: 7567 6779 2069 6d70 6f72 7420 506c 7567  uggy import Plug
-00002670: 696e 4d61 6e61 6765 722c 2048 6f6f 6b69  inManager, Hooki
-00002680: 6d70 6c4d 6172 6b65 720a 0a20 2020 2068  mplMarker..    h
-00002690: 6f6f 6b69 6d70 6c20 3d20 486f 6f6b 696d  ookimpl = Hookim
-000026a0: 706c 4d61 726b 6572 2822 6d79 7072 6f6a  plMarker("myproj
-000026b0: 6563 7422 290a 0a0a 2020 2020 4068 6f6f  ect")...    @hoo
-000026c0: 6b69 6d70 6c28 7472 796c 6173 743d 5472  kimpl(trylast=Tr
-000026d0: 7565 290a 2020 2020 6465 6620 7365 7475  ue).    def setu
-000026e0: 705f 7072 6f6a 6563 7428 636f 6e66 6967  p_project(config
-000026f0: 2c20 6172 6773 293a 0a20 2020 2020 2020  , args):.       
-00002700: 2022 2222 4465 6661 756c 7420 696d 706c   """Default impl
-00002710: 656d 656e 7461 7469 6f6e 2e0a 2020 2020  ementation..    
-00002720: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002730: 6966 2061 7267 733a 0a20 2020 2020 2020  if args:.       
-00002740: 2020 2020 2063 6f6e 6669 672e 7072 6f63       config.proc
-00002750: 6573 735f 6172 6773 2861 7267 7329 0a0a  ess_args(args)..
-00002760: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00002770: 6f6e 6669 670a 0a0a 2020 2020 636c 6173  onfig...    clas
-00002780: 7320 536f 6d65 4f74 6865 7250 6c75 6769  s SomeOtherPlugi
-00002790: 6e28 6f62 6a65 6374 293a 0a20 2020 2020  n(object):.     
-000027a0: 2020 2022 2222 536f 6d65 206f 7468 6572     """Some other
-000027b0: 2070 6c75 6769 6e20 6465 6669 6e69 6e67   plugin defining
-000027c0: 2074 6865 2073 616d 6520 686f 6f6b 2e0a   the same hook..
-000027d0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-000027e0: 2020 2020 2040 686f 6f6b 696d 706c 2874       @hookimpl(t
-000027f0: 7279 6669 7273 743d 5472 7565 290a 2020  ryfirst=True).  
-00002800: 2020 2020 2020 6465 6620 7365 7475 705f        def setup_
-00002810: 7072 6f6a 6563 7428 7365 6c66 2c20 636f  project(self, co
-00002820: 6e66 6967 2c20 6172 6773 293a 0a20 2020  nfig, args):.   
-00002830: 2020 2020 2020 2020 2022 2222 5265 706f           """Repo
-00002840: 7274 2077 6861 7420 6172 6773 2077 6572  rt what args wer
-00002850: 6520 7061 7373 6564 2062 6566 6f72 6520  e passed before 
-00002860: 6361 6c6c 696e 670a 2020 2020 2020 2020  calling.        
-00002870: 2020 2020 646f 776e 7374 7265 616d 2068      downstream h
-00002880: 6f6f 6b73 2e0a 2020 2020 2020 2020 2020  ooks..          
-00002890: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
-000028a0: 2020 6966 2061 7267 733a 0a20 2020 2020    if args:.     
-000028b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000028c0: 2822 476f 7420 6172 6773 3a20 7b7d 222e  ("Got args: {}".
-000028d0: 666f 726d 6174 2861 7267 7329 290a 0a20  format(args)).. 
-000028e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000028f0: 6e20 636f 6e66 6967 0a0a 0a20 2020 2070  n config...    p
-00002900: 6d20 3d20 506c 7567 696e 4d61 6e61 6765  m = PluginManage
-00002910: 7228 226d 7970 726f 6a65 6374 2229 0a0a  r("myproject")..
-00002920: 2020 2020 2320 6c6f 6164 2066 726f 6d20      # load from 
-00002930: 7468 6520 6c6f 6361 6c20 6d6f 6475 6c65  the local module
-00002940: 2773 206e 616d 6573 7061 6365 0a20 2020  's namespace.   
-00002950: 2070 6d2e 7265 6769 7374 6572 2873 7973   pm.register(sys
-00002960: 2e6d 6f64 756c 6573 5b5f 5f6e 616d 655f  .modules[__name_
-00002970: 5f5d 290a 2020 2020 2320 6c6f 6164 2061  _]).    # load a
-00002980: 2070 6c75 6769 6e20 6465 6669 6e65 6420   plugin defined 
-00002990: 6f6e 2061 2063 6c61 7373 0a20 2020 2070  on a class.    p
-000029a0: 6d2e 7265 6769 7374 6572 2853 6f6d 654f  m.register(SomeO
-000029b0: 7468 6572 506c 7567 696e 2829 290a 0a46  therPlugin())..F
-000029c0: 6f72 2061 6e6f 7468 6572 2065 7861 6d70  or another examp
-000029d0: 6c65 2073 6565 2074 6865 2060 686f 6f6b  le see the `hook
-000029e0: 2066 756e 6374 696f 6e20 6f72 6465 7269   function orderi
-000029f0: 6e67 605f 2073 6563 7469 6f6e 206f 6620  ng`_ section of 
-00002a00: 7468 650a 6060 7079 7465 7374 6060 2064  the.``pytest`` d
-00002a10: 6f63 732e 0a0a 2e2e 206e 6f74 653a 3a0a  ocs..... note::.
-00002a20: 2020 2020 6060 7472 7966 6972 7374 6060      ``tryfirst``
-00002a30: 2061 6e64 2060 6074 7279 6c61 7374 6060   and ``trylast``
-00002a40: 2068 6f6f 6b73 2061 7265 2073 7469 6c6c   hooks are still
-00002a50: 2069 6e76 6f6b 6564 2069 6e20 4c49 464f   invoked in LIFO
-00002a60: 206f 7264 6572 2077 6974 6869 6e0a 2020   order within.  
-00002a70: 2020 6561 6368 2063 6174 6567 6f72 792e    each category.
-00002a80: 0a0a 0a2e 2e20 5f68 6f6f 6b77 7261 7070  ..... _hookwrapp
-00002a90: 6572 733a 0a0a 5772 6170 7065 7273 0a5e  ers:..Wrappers.^
-00002aa0: 5e5e 5e5e 5e5e 5e0a 4120 2a68 6f6f 6b69  ^^^^^^^.A *hooki
-00002ab0: 6d70 6c2a 2063 616e 2062 6520 6d61 726b  mpl* can be mark
-00002ac0: 6564 2077 6974 6820 6120 6060 2268 6f6f  ed with a ``"hoo
-00002ad0: 6b77 7261 7070 6572 2260 6020 6f70 7469  kwrapper"`` opti
-00002ae0: 6f6e 2077 6869 6368 2069 6e64 6963 6174  on which indicat
-00002af0: 6573 2074 6861 740a 7468 6520 6675 6e63  es that.the func
-00002b00: 7469 6f6e 2077 696c 6c20 6265 2063 616c  tion will be cal
-00002b10: 6c65 6420 746f 202a 7772 6170 2a20 286f  led to *wrap* (o
-00002b20: 7220 7375 7272 6f75 6e64 2920 616c 6c20  r surround) all 
-00002b30: 6f74 6865 7220 6e6f 726d 616c 202a 686f  other normal *ho
-00002b40: 6f6b 696d 706c 2a0a 6361 6c6c 732e 2041  okimpl*.calls. A
-00002b50: 202a 686f 6f6b 7772 6170 7065 722a 2063   *hookwrapper* c
-00002b60: 616e 2074 6875 7320 6578 6563 7574 6520  an thus execute 
-00002b70: 736f 6d65 2063 6f64 6520 6168 6561 6420  some code ahead 
-00002b80: 616e 6420 6166 7465 7220 7468 6520 6578  and after the ex
-00002b90: 6563 7574 696f 6e0a 6f66 2061 6c6c 2063  ecution.of all c
-00002ba0: 6f72 7265 7370 6f6e 6469 6e67 206e 6f6e  orresponding non
-00002bb0: 2d77 7261 7070 7065 7220 2a68 6f6f 6b69  -wrappper *hooki
-00002bc0: 6d70 6c73 2a2e 0a0a 4d75 6368 2069 6e20  mpls*...Much in 
-00002bd0: 7468 6520 7361 6d65 2077 6179 2061 7320  the same way as 
-00002be0: 6120 3a70 793a 6675 6e63 3a60 4063 6f6e  a :py:func:`@con
-00002bf0: 7465 7874 6c69 622e 636f 6e74 6578 746d  textlib.contextm
-00002c00: 616e 6167 6572 203c 7079 7468 6f6e 3a63  anager <python:c
-00002c10: 6f6e 7465 7874 6c69 622e 636f 6e74 6578  ontextlib.contex
-00002c20: 746d 616e 6167 6572 3e60 2c20 2a68 6f6f  tmanager>`, *hoo
-00002c30: 6b77 7261 7070 6572 732a 206d 7573 740a  kwrappers* must.
-00002c40: 6265 2069 6d70 6c65 6d65 6e74 6564 2061  be implemented a
-00002c50: 7320 6765 6e65 7261 746f 7220 6675 6e63  s generator func
-00002c60: 7469 6f6e 2077 6974 6820 6120 7369 6e67  tion with a sing
-00002c70: 6c65 2060 6079 6965 6c64 6060 2069 6e20  le ``yield`` in 
-00002c80: 6974 7320 626f 6479 3a0a 0a0a 2e2e 2063  its body:..... c
-00002c90: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00002ca0: 6f6e 0a0a 2020 2020 4068 6f6f 6b69 6d70  on..    @hookimp
-00002cb0: 6c28 686f 6f6b 7772 6170 7065 723d 5472  l(hookwrapper=Tr
-00002cc0: 7565 290a 2020 2020 6465 6620 7365 7475  ue).    def setu
-00002cd0: 705f 7072 6f6a 6563 7428 636f 6e66 6967  p_project(config
-00002ce0: 2c20 6172 6773 293a 0a20 2020 2020 2020  , args):.       
-00002cf0: 2022 2222 5772 6170 2063 616c 6c73 2074   """Wrap calls t
-00002d00: 6f20 6060 7365 7475 705f 7072 6f6a 6563  o ``setup_projec
-00002d10: 7428 2960 6020 696d 706c 656d 656e 7461  t()`` implementa
-00002d20: 7469 6f6e 7320 7768 6963 680a 2020 2020  tions which.    
-00002d30: 2020 2020 7368 6f75 6c64 2072 6574 7572      should retur
-00002d40: 6e20 6a73 6f6e 2065 6e63 6f64 6564 2063  n json encoded c
-00002d50: 6f6e 6669 6720 6f70 7469 6f6e 732e 0a20  onfig options.. 
-00002d60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00002d70: 2020 2069 6620 636f 6e66 6967 2e64 6562     if config.deb
-00002d80: 7567 3a0a 2020 2020 2020 2020 2020 2020  ug:.            
-00002d90: 7072 696e 7428 2250 7265 2d68 6f6f 6b20  print("Pre-hook 
-00002da0: 636f 6e66 6967 2069 7320 7b7d 222e 666f  config is {}".fo
-00002db0: 726d 6174 2863 6f6e 6669 672e 746f 6a73  rmat(config.tojs
-00002dc0: 6f6e 2829 2929 0a0a 2020 2020 2020 2020  on()))..        
-00002dd0: 2320 6765 7420 696e 6974 6961 6c20 6465  # get initial de
-00002de0: 6661 756c 7420 636f 6e66 6967 0a20 2020  fault config.   
-00002df0: 2020 2020 2064 6566 6175 6c74 7320 3d20       defaults = 
-00002e00: 636f 6e66 6967 2e74 6f6a 736f 6e28 290a  config.tojson().
-00002e10: 0a20 2020 2020 2020 2023 2061 6c6c 2063  .        # all c
-00002e20: 6f72 7265 7370 6f6e 6469 6e67 2068 6f6f  orresponding hoo
-00002e30: 6b69 6d70 6c73 2061 7265 2069 6e76 6f6b  kimpls are invok
-00002e40: 6564 2068 6572 650a 2020 2020 2020 2020  ed here.        
-00002e50: 6f75 7463 6f6d 6520 3d20 7969 656c 640a  outcome = yield.
-00002e60: 0a20 2020 2020 2020 2066 6f72 2069 7465  .        for ite
-00002e70: 6d20 696e 206f 7574 636f 6d65 2e67 6574  m in outcome.get
-00002e80: 5f72 6573 756c 7428 293a 0a20 2020 2020  _result():.     
-00002e90: 2020 2020 2020 2070 7269 6e74 2822 4a53         print("JS
-00002ea0: 4f4e 2063 6f6e 6669 6720 6f76 6572 7269  ON config overri
-00002eb0: 6465 2069 7320 7b7d 222e 666f 726d 6174  de is {}".format
-00002ec0: 2869 7465 6d29 290a 0a20 2020 2020 2020  (item))..       
-00002ed0: 2069 6620 636f 6e66 6967 2e64 6562 7567   if config.debug
-00002ee0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00002ef0: 696e 7428 2250 6f73 742d 686f 6f6b 2063  int("Post-hook c
-00002f00: 6f6e 6669 6720 6973 207b 7d22 2e66 6f72  onfig is {}".for
-00002f10: 6d61 7428 636f 6e66 6967 2e74 6f6a 736f  mat(config.tojso
-00002f20: 6e28 2929 290a 0a20 2020 2020 2020 2069  n()))..        i
-00002f30: 6620 636f 6e66 6967 2e75 7365 5f64 6566  f config.use_def
-00002f40: 6175 6c74 733a 0a20 2020 2020 2020 2020  aults:.         
-00002f50: 2020 206f 7574 636f 6d65 2e66 6f72 6365     outcome.force
-00002f60: 5f72 6573 756c 7428 6465 6661 756c 7473  _result(defaults
-00002f70: 290a 0a54 6865 2067 656e 6572 6174 6f72  )..The generator
-00002f80: 2069 7320 3a70 793a 6d65 7468 3a60 7365   is :py:meth:`se
-00002f90: 6e74 203c 7079 7468 6f6e 3a67 656e 6572  nt <python:gener
-00002fa0: 6174 6f72 2e73 656e 643e 6020 6120 3a70  ator.send>` a :p
-00002fb0: 793a 636c 6173 733a 6070 6c75 6767 792e  y:class:`pluggy.
-00002fc0: 6361 6c6c 6572 732e 5f52 6573 756c 7460  callers._Result`
-00002fd0: 206f 626a 6563 7420 7768 6963 6820 6361   object which ca
-00002fe0: 6e0a 6265 2061 7373 6967 6e65 6420 696e  n.be assigned in
-00002ff0: 2074 6865 2060 6079 6965 6c64 6060 2065   the ``yield`` e
-00003000: 7870 7265 7373 696f 6e20 616e 6420 7573  xpression and us
-00003010: 6564 2074 6f20 6f76 6572 7269 6465 206f  ed to override o
-00003020: 7220 696e 7370 6563 740a 7468 6520 6669  r inspect.the fi
-00003030: 6e61 6c20 7265 7375 6c74 2873 2920 7265  nal result(s) re
-00003040: 7475 726e 6564 2062 6163 6b20 746f 2074  turned back to t
-00003050: 6865 2063 616c 6c65 7220 7573 696e 6720  he caller using 
-00003060: 7468 650a 3a70 793a 6d65 7468 3a60 7e70  the.:py:meth:`~p
-00003070: 6c75 6767 792e 6361 6c6c 6572 732e 5f52  luggy.callers._R
-00003080: 6573 756c 742e 666f 7263 655f 7265 7375  esult.force_resu
-00003090: 6c74 6020 6f72 0a3a 7079 3a6d 6574 683a  lt` or.:py:meth:
-000030a0: 607e 706c 7567 6779 2e63 616c 6c65 7273  `~pluggy.callers
-000030b0: 2e5f 5265 7375 6c74 2e67 6574 5f72 6573  ._Result.get_res
-000030c0: 756c 7460 206d 6574 686f 6473 2e0a 0a2e  ult` methods....
-000030d0: 2e20 6e6f 7465 3a3a 0a20 2020 2048 6f6f  . note::.    Hoo
-000030e0: 6b20 7772 6170 7065 7273 2063 616e 202a  k wrappers can *
-000030f0: 2a6e 6f74 2a2a 2072 6574 7572 6e20 7265  *not** return re
-00003100: 7375 6c74 7320 2861 7320 7065 7220 6765  sults (as per ge
-00003110: 6e65 7261 746f 7220 6675 6e63 7469 6f6e  nerator function
-00003120: 0a20 2020 2073 656d 616e 7469 6373 293b  .    semantics);
-00003130: 2074 6865 7920 6361 6e20 6f6e 6c79 206d   they can only m
-00003140: 6f64 6966 7920 7468 656d 2075 7369 6e67  odify them using
-00003150: 2074 6865 2060 605f 5265 7375 6c74 6060   the ``_Result``
-00003160: 2041 5049 2e0a 0a41 6c73 6f20 7365 6520   API...Also see 
-00003170: 7468 6520 6068 6f6f 6b77 7261 7070 6572  the `hookwrapper
-00003180: 605f 2073 6563 7469 6f6e 2069 6e20 7468  `_ section in th
-00003190: 6520 6060 7079 7465 7374 6060 2064 6f63  e ``pytest`` doc
-000031a0: 732e 0a0a 2e2e 205f 7370 6563 733a 0a0a  s..... _specs:..
-000031b0: 5370 6563 6966 6963 6174 696f 6e73 0a2d  Specifications.-
-000031c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4120  -------------.A 
-000031d0: 686f 6f6b 202a 7370 6563 6966 6963 6174  hook *specificat
-000031e0: 696f 6e2a 2028 2a68 6f6f 6b73 7065 632a  ion* (*hookspec*
-000031f0: 2920 6973 2061 2064 6566 696e 6974 696f  ) is a definitio
-00003200: 6e20 7573 6564 2074 6f20 7661 6c69 6461  n used to valida
-00003210: 7465 2065 6163 680a 2a68 6f6f 6b69 6d70  te each.*hookimp
-00003220: 6c2a 2065 6e73 7572 696e 6720 7468 6174  l* ensuring that
-00003230: 2061 6e20 6578 7465 6e73 696f 6e20 7772   an extension wr
-00003240: 6974 6572 2068 6173 2063 6f72 7265 6374  iter has correct
-00003250: 6c79 2064 6566 696e 6564 2074 6865 6972  ly defined their
-00003260: 0a63 616c 6c62 6163 6b20 6675 6e63 7469  .callback functi
-00003270: 6f6e 202a 696d 706c 656d 656e 7461 7469  on *implementati
-00003280: 6f6e 2a20 2e0a 0a2a 686f 6f6b 7370 6563  on* ...*hookspec
-00003290: 732a 2061 7265 2064 6566 696e 6564 2075  s* are defined u
-000032a0: 7369 6e67 2073 696d 696c 6172 6c79 206d  sing similarly m
-000032b0: 6172 6b65 6420 6675 6e63 7469 6f6e 7320  arked functions 
-000032c0: 686f 7765 7665 7220 6f6e 6c79 2074 6865  however only the
-000032d0: 0a66 756e 6374 696f 6e20 2a73 6967 6e61  .function *signa
-000032e0: 7475 7265 2a20 2869 7473 206e 616d 6520  ture* (its name 
-000032f0: 616e 6420 6e61 6d65 7320 6f66 2061 6c6c  and names of all
-00003300: 2069 7473 2061 7267 756d 656e 7473 2920   its arguments) 
-00003310: 6973 2061 6e61 6c79 7a65 640a 616e 6420  is analyzed.and 
-00003320: 7374 6f72 6564 2e20 4173 2073 7563 682c  stored. As such,
-00003330: 206f 6674 656e 2079 6f75 2077 696c 6c20   often you will 
-00003340: 7365 6520 6120 2a68 6f6f 6b73 7065 632a  see a *hookspec*
-00003350: 2064 6566 696e 6564 2077 6974 6820 6f6e   defined with on
-00003360: 6c79 0a61 2064 6f63 7374 7269 6e67 2069  ly.a docstring i
-00003370: 6e20 6974 7320 626f 6479 2e0a 0a2a 686f  n its body...*ho
-00003380: 6f6b 7370 6563 732a 2061 7265 206c 6f61  okspecs* are loa
-00003390: 6465 6420 7573 696e 6720 7468 650a 3a70  ded using the.:p
-000033a0: 793a 6d65 7468 3a60 7e70 6c75 6767 792e  y:meth:`~pluggy.
-000033b0: 506c 7567 696e 4d61 6e61 6765 722e 6164  PluginManager.ad
-000033c0: 645f 686f 6f6b 7370 6563 7328 2960 206d  d_hookspecs()` m
-000033d0: 6574 686f 6420 616e 6420 6e6f 726d 616c  ethod and normal
-000033e0: 6c79 0a73 686f 756c 6420 6265 2061 6464  ly.should be add
-000033f0: 6564 2062 6566 6f72 6520 7265 6769 7374  ed before regist
-00003400: 6572 696e 6720 636f 7272 6573 706f 6e64  ering correspond
-00003410: 696e 6720 2a68 6f6f 6b69 6d70 6c73 2a3a  ing *hookimpls*:
-00003420: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
-00003430: 3a20 7079 7468 6f6e 0a0a 2020 2020 696d  : python..    im
-00003440: 706f 7274 2073 7973 0a20 2020 2066 726f  port sys.    fro
-00003450: 6d20 706c 7567 6779 2069 6d70 6f72 7420  m pluggy import 
-00003460: 506c 7567 696e 4d61 6e61 6765 722c 2048  PluginManager, H
-00003470: 6f6f 6b73 7065 634d 6172 6b65 720a 0a20  ookspecMarker.. 
-00003480: 2020 2068 6f6f 6b73 7065 6320 3d20 486f     hookspec = Ho
-00003490: 6f6b 7370 6563 4d61 726b 6572 2822 6d79  okspecMarker("my
-000034a0: 7072 6f6a 6563 7422 290a 0a0a 2020 2020  project")...    
-000034b0: 4068 6f6f 6b73 7065 630a 2020 2020 6465  @hookspec.    de
-000034c0: 6620 7365 7475 705f 7072 6f6a 6563 7428  f setup_project(
-000034d0: 636f 6e66 6967 2c20 6172 6773 293a 0a20  config, args):. 
-000034e0: 2020 2020 2020 2022 2222 5468 6973 2068         """This h
-000034f0: 6f6f 6b20 6973 2075 7365 6420 746f 2070  ook is used to p
-00003500: 726f 6365 7373 2074 6865 2069 6e69 7469  rocess the initi
-00003510: 616c 2063 6f6e 6669 6720 616e 6420 696e  al config and in
-00003520: 7075 740a 2020 2020 2020 2020 6172 6775  put.        argu
-00003530: 6d65 6e74 732e 0a20 2020 2020 2020 2022  ments..        "
-00003540: 2222 0a0a 0a20 2020 2070 6d20 3d20 506c  ""...    pm = Pl
-00003550: 7567 696e 4d61 6e61 6765 7228 226d 7970  uginManager("myp
-00003560: 726f 6a65 6374 2229 0a0a 2020 2020 2320  roject")..    # 
-00003570: 6c6f 6164 2066 726f 6d20 7468 6520 6c6f  load from the lo
-00003580: 6361 6c20 6d6f 6475 6c65 2773 206e 616d  cal module's nam
-00003590: 6573 7061 6365 0a20 2020 2070 6d2e 6164  espace.    pm.ad
-000035a0: 645f 686f 6f6b 7370 6563 7328 7379 732e  d_hookspecs(sys.
-000035b0: 6d6f 6475 6c65 735b 5f5f 6e61 6d65 5f5f  modules[__name__
-000035c0: 5d29 0a0a 0a52 6567 6973 7465 7269 6e67  ])...Registering
-000035d0: 2061 202a 686f 6f6b 696d 706c 2a20 7768   a *hookimpl* wh
-000035e0: 6963 6820 646f 6573 206e 6f74 206d 6565  ich does not mee
-000035f0: 7420 7468 6520 636f 6e73 7472 6169 6e74  t the constraint
-00003600: 7320 6f66 2069 7473 0a63 6f72 7265 7370  s of its.corresp
-00003610: 6f6e 6469 6e67 202a 686f 6f6b 7370 6563  onding *hookspec
-00003620: 2a20 7769 6c6c 2072 6573 756c 7420 696e  * will result in
-00003630: 2061 6e20 6572 726f 722e 0a0a 4120 2a68   an error...A *h
-00003640: 6f6f 6b73 7065 632a 2063 616e 2061 6c73  ookspec* can als
-00003650: 6f20 6265 2061 6464 6564 202a 2a61 6674  o be added **aft
-00003660: 6572 2a2a 2073 6f6d 6520 2a68 6f6f 6b69  er** some *hooki
-00003670: 6d70 6c73 2a20 6861 7665 2062 6565 6e0a  mpls* have been.
-00003680: 7265 6769 7374 6572 6564 2068 6f77 6576  registered howev
-00003690: 6572 2074 6869 7320 6973 206e 6f74 206e  er this is not n
-000036a0: 6f72 6d61 6c6c 7920 7265 636f 6d6d 656e  ormally recommen
-000036b0: 6465 6420 6173 2069 7420 7265 7375 6c74  ded as it result
-000036c0: 7320 696e 0a64 656c 6179 6564 2068 6f6f  s in.delayed hoo
-000036d0: 6b20 7661 6c69 6461 7469 6f6e 2e0a 0a2e  k validation....
-000036e0: 2e20 6e6f 7465 3a3a 0a20 2020 2054 6865  . note::.    The
-000036f0: 2074 6572 6d20 2a68 6f6f 6b73 7065 632a   term *hookspec*
-00003700: 2063 616e 2073 6f6d 6574 696d 6573 2072   can sometimes r
-00003710: 6566 6572 2074 6f20 7468 6520 706c 7567  efer to the plug
-00003720: 696e 2d6e 616d 6573 7061 6365 0a20 2020  in-namespace.   
-00003730: 2077 6869 6368 2064 6566 696e 6573 2060   which defines `
-00003740: 6068 6f6f 6b73 7065 6360 6020 6465 636f  `hookspec`` deco
-00003750: 7261 7465 6420 6675 6e63 7469 6f6e 7320  rated functions 
-00003760: 6173 2069 6e20 7468 6520 6361 7365 206f  as in the case o
-00003770: 660a 2020 2020 6060 7079 7465 7374 6060  f.    ``pytest``
-00003780: 2773 2060 686f 6f6b 7370 6563 206d 6f64  's `hookspec mod
-00003790: 756c 6560 5f0a 0a45 6e66 6f72 6369 6e67  ule`_..Enforcing
-000037a0: 2073 7065 6320 7661 6c69 6461 7469 6f6e   spec validation
-000037b0: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  .^^^^^^^^^^^^^^^
-000037c0: 5e5e 5e5e 5e5e 5e5e 5e5e 0a42 7920 6465  ^^^^^^^^^^.By de
-000037d0: 6661 756c 7420 7468 6572 6520 6973 206e  fault there is n
-000037e0: 6f20 7374 7269 6374 2072 6571 7569 7265  o strict require
-000037f0: 6d65 6e74 2074 6861 7420 6561 6368 202a  ment that each *
-00003800: 686f 6f6b 696d 706c 2a20 6861 730a 6120  hookimpl* has.a 
-00003810: 636f 7272 6573 706f 6e64 696e 6720 2a68  corresponding *h
-00003820: 6f6f 6b73 7065 632a 2e20 486f 7765 7665  ookspec*. Howeve
-00003830: 722c 2069 6620 796f 7527 6420 6c69 6b65  r, if you'd like
-00003840: 2079 6f75 2065 6e66 6f72 6365 2074 6869   you enforce thi
-00003850: 730a 6265 6861 7669 6f72 2079 6f75 2063  s.behavior you c
-00003860: 616e 2072 756e 2061 2063 6865 636b 2077  an run a check w
-00003870: 6974 6820 7468 650a 3a70 793a 6d65 7468  ith the.:py:meth
-00003880: 3a60 7e70 6c75 6767 792e 506c 7567 696e  :`~pluggy.Plugin
-00003890: 4d61 6e61 6765 722e 6368 6563 6b5f 7065  Manager.check_pe
-000038a0: 6e64 696e 6728 2960 206d 6574 686f 642e  nding()` method.
-000038b0: 2049 6620 796f 7527 6420 6c69 6b65 0a74   If you'd like.t
-000038c0: 6f20 656e 666f 7263 6520 7265 7175 6973  o enforce requis
-000038d0: 6974 6520 2a68 6f6f 6b73 7065 6373 2a20  ite *hookspecs* 
-000038e0: 6275 7420 7769 7468 2063 6572 7461 696e  but with certain
-000038f0: 2065 7863 6570 7469 6f6e 7320 666f 7220   exceptions for 
-00003900: 736f 6d65 2068 6f6f 6b73 0a74 6865 6e20  some hooks.then 
-00003910: 6d61 6b65 2073 7572 6520 746f 206d 6172  make sure to mar
-00003920: 6b20 7468 6f73 6520 686f 6f6b 7320 6173  k those hooks as
-00003930: 203a 7265 663a 606f 7074 696f 6e61 6c20   :ref:`optional 
-00003940: 3c6f 7074 696f 6e61 6c68 6f6f 6b3e 602e  <optionalhook>`.
-00003950: 0a0a 4f70 742d 696e 2061 7267 756d 656e  ..Opt-in argumen
-00003960: 7473 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ts.^^^^^^^^^^^^^
-00003970: 5e5e 5e0a 546f 2061 6c6c 6f77 2066 6f72  ^^^.To allow for
-00003980: 202a 686f 6f6b 7370 6563 732a 2074 6f20   *hookspecs* to 
-00003990: 6576 6f6c 7665 206f 7665 7220 7468 6520  evolve over the 
-000039a0: 6c69 6665 7469 6d65 206f 6620 6120 7072  lifetime of a pr
-000039b0: 6f6a 6563 742c 0a2a 686f 6f6b 696d 706c  oject,.*hookimpl
-000039c0: 732a 2063 616e 2061 6363 6570 7420 2a2a  s* can accept **
-000039d0: 6c65 7373 2a2a 2061 7267 756d 656e 7473  less** arguments
-000039e0: 2074 6865 6e20 6465 6669 6e65 6420 696e   then defined in
-000039f0: 2074 6865 2073 7065 632e 0a54 6869 7320   the spec..This 
-00003a00: 616c 6c6f 7773 2066 6f72 2065 7874 656e  allows for exten
-00003a10: 6469 6e67 2068 6f6f 6b20 6172 6775 6d65  ding hook argume
-00003a20: 6e74 7320 2861 6e64 2074 6875 7320 7365  nts (and thus se
-00003a30: 6d61 6e74 6963 7329 2077 6974 686f 7574  mantics) without
-00003a40: 0a62 7265 616b 696e 6720 6578 6973 7469  .breaking existi
-00003a50: 6e67 202a 686f 6f6b 696d 706c 732a 2e0a  ng *hookimpls*..
-00003a60: 0a49 6e20 6f74 6865 7220 776f 7264 7320  .In other words 
-00003a70: 7468 6973 2069 7320 6f6b 3a0a 0a2e 2e20  this is ok:.... 
-00003a80: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-00003a90: 686f 6e0a 0a20 2020 2040 686f 6f6b 7370  hon..    @hooksp
-00003aa0: 6563 0a20 2020 2064 6566 206d 7968 6f6f  ec.    def myhoo
-00003ab0: 6b28 636f 6e66 6967 2c20 6172 6773 293a  k(config, args):
-00003ac0: 0a20 2020 2020 2020 2070 6173 730a 0a0a  .        pass...
-00003ad0: 2020 2020 4068 6f6f 6b69 6d70 6c0a 2020      @hookimpl.  
-00003ae0: 2020 6465 6620 6d79 686f 6f6b 2861 7267    def myhook(arg
-00003af0: 7329 3a0a 2020 2020 2020 2020 7072 696e  s):.        prin
-00003b00: 7428 6172 6773 290a 0a0a 7768 6572 6561  t(args)...wherea
-00003b10: 7320 7468 6973 2069 7320 6e6f 743a 0a0a  s this is not:..
-00003b20: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00003b30: 7079 7468 6f6e 0a0a 2020 2020 4068 6f6f  python..    @hoo
-00003b40: 6b73 7065 630a 2020 2020 6465 6620 6d79  kspec.    def my
-00003b50: 686f 6f6b 2863 6f6e 6669 672c 2061 7267  hook(config, arg
-00003b60: 7329 3a0a 2020 2020 2020 2020 7061 7373  s):.        pass
-00003b70: 0a0a 0a20 2020 2040 686f 6f6b 696d 706c  ...    @hookimpl
-00003b80: 0a20 2020 2064 6566 206d 7968 6f6f 6b28  .    def myhook(
-00003b90: 636f 6e66 6967 2c20 6172 6773 2c20 6578  config, args, ex
-00003ba0: 7472 615f 6172 6729 3a0a 2020 2020 2020  tra_arg):.      
-00003bb0: 2020 7072 696e 7428 6172 6773 290a 0a2e    print(args)...
-00003bc0: 2e20 6e6f 7465 3a3a 0a20 2020 2054 6865  . note::.    The
-00003bd0: 206f 6e65 2065 7863 6570 7469 6f6e 2074   one exception t
-00003be0: 6f20 7468 6973 2072 756c 6520 2874 6861  o this rule (tha
-00003bf0: 7420 6120 2a68 6f6f 6b73 7065 632a 206d  t a *hookspec* m
-00003c00: 7573 7420 6861 7665 2061 7320 6c65 6173  ust have as leas
-00003c10: 7420 6173 0a20 2020 206d 616e 7920 6172  t as.    many ar
-00003c20: 6775 6d65 6e74 7320 6173 2069 7473 202a  guments as its *
-00003c30: 686f 6f6b 696d 706c 732a 2920 6973 2074  hookimpls*) is t
-00003c40: 6865 2063 6f6e 7665 6e74 696f 6e61 6c20  he conventional 
-00003c50: 3a72 6566 3a60 7365 6c66 203c 7079 7468  :ref:`self <pyth
-00003c60: 6f6e 3a74 7574 2d72 656d 6172 6b73 3e60  on:tut-remarks>`
-00003c70: 2061 7267 3b20 7468 6973 0a20 2020 2069   arg; this.    i
-00003c80: 7320 616c 7761 7973 2069 676e 6f72 6564  s always ignored
-00003c90: 2077 6865 6e20 2a68 6f6f 6b69 6d70 6c73   when *hookimpls
-00003ca0: 2a20 6172 6520 6465 6669 6e65 6420 6173  * are defined as
-00003cb0: 203a 7265 663a 606d 6574 686f 6473 203c   :ref:`methods <
-00003cc0: 7079 7468 6f6e 3a74 7574 2d6d 6574 686f  python:tut-metho
-00003cd0: 646f 626a 6563 7473 3e60 2e0a 0a2e 2e20  dobjects>`..... 
-00003ce0: 5f66 6972 7374 7265 7375 6c74 3a0a 0a46  _firstresult:..F
-00003cf0: 6972 7374 2072 6573 756c 7420 6f6e 6c79  irst result only
-00003d00: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  .^^^^^^^^^^^^^^^
-00003d10: 5e5e 0a41 202a 686f 6f6b 7370 6563 2a20  ^^.A *hookspec* 
-00003d20: 6361 6e20 6265 206d 6172 6b65 6420 7375  can be marked su
-00003d30: 6368 2074 6861 7420 7768 656e 2074 6865  ch that when the
-00003d40: 202a 686f 6f6b 2a20 6973 2063 616c 6c65   *hook* is calle
-00003d50: 6420 7468 6520 6361 6c6c 206c 6f6f 700a  d the call loop.
-00003d60: 7769 6c6c 206f 6e6c 7920 696e 766f 6b65  will only invoke
-00003d70: 2075 7020 746f 2074 6865 2066 6972 7374   up to the first
-00003d80: 202a 686f 6f6b 696d 706c 2a20 7768 6963   *hookimpl* whic
-00003d90: 6820 7265 7475 726e 7320 6120 7265 7375  h returns a resu
-00003da0: 6c74 206f 7468 6572 0a74 6865 6e20 6060  lt other.then ``
-00003db0: 4e6f 6e65 6060 2e0a 0a2e 2e20 636f 6465  None``..... code
-00003dc0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00003dd0: 0a20 2020 2040 686f 6f6b 7370 6563 2866  .    @hookspec(f
-00003de0: 6972 7374 7265 7375 6c74 3d54 7275 6529  irstresult=True)
-00003df0: 0a20 2020 2064 6566 206d 7968 6f6f 6b28  .    def myhook(
-00003e00: 636f 6e66 6967 2c20 6172 6773 293a 0a20  config, args):. 
-00003e10: 2020 2020 2020 2070 6173 730a 0a54 6869         pass..Thi
-00003e20: 7320 6361 6e20 6265 2075 7365 6675 6c20  s can be useful 
-00003e30: 666f 7220 6f70 7469 6d69 7a69 6e67 2061  for optimizing a
-00003e40: 2063 616c 6c20 6c6f 6f70 2066 6f72 2077   call loop for w
-00003e50: 6869 6368 2079 6f75 2061 7265 206f 6e6c  hich you are onl
-00003e60: 790a 696e 7465 7265 7374 6564 2069 6e20  y.interested in 
-00003e70: 6120 7369 6e67 6c65 2063 6f72 6520 2a68  a single core *h
-00003e80: 6f6f 6b69 6d70 6c2a 2e20 416e 2065 7861  ookimpl*. An exa
-00003e90: 6d70 6c65 2069 7320 7468 650a 6070 7974  mple is the.`pyt
-00003ea0: 6573 745f 636d 646c 696e 655f 6d61 696e  est_cmdline_main
-00003eb0: 605f 2063 656e 7472 616c 2072 6f75 7469  `_ central routi
-00003ec0: 6e65 206f 6620 6060 7079 7465 7374 6060  ne of ``pytest``
-00003ed0: 2e0a 4e6f 7465 2074 6861 7420 616c 6c20  ..Note that all 
-00003ee0: 6060 686f 6f6b 7772 6170 7065 7273 6060  ``hookwrappers``
-00003ef0: 2061 7265 2073 7469 6c6c 2069 6e76 6f6b   are still invok
-00003f00: 6564 2077 6974 6820 7468 6520 6669 7273  ed with the firs
-00003f10: 7420 7265 7375 6c74 2e0a 0a41 6c73 6f20  t result...Also 
-00003f20: 7365 6520 7468 6520 3a72 6566 3a60 7079  see the :ref:`py
-00003f30: 7465 7374 3a66 6972 7374 7265 7375 6c74  test:firstresult
-00003f40: 6020 7365 6374 696f 6e20 696e 2074 6865  ` section in the
-00003f50: 2060 6070 7974 6573 7460 6020 646f 6373   ``pytest`` docs
-00003f60: 2e0a 0a2e 2e20 5f68 6973 746f 7269 633a  ..... _historic:
-00003f70: 0a0a 4869 7374 6f72 6963 2068 6f6f 6b73  ..Historic hooks
-00003f80: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  .^^^^^^^^^^^^^^.
-00003f90: 596f 7520 6361 6e20 6d61 726b 2061 202a  You can mark a *
-00003fa0: 686f 6f6b 7370 6563 2a20 6173 2062 6569  hookspec* as bei
-00003fb0: 6e67 202a 6869 7374 6f72 6963 2a20 6d65  ng *historic* me
-00003fc0: 616e 696e 6720 7468 6174 2074 6865 2068  aning that the h
-00003fd0: 6f6f 6b0a 6361 6e20 6265 2063 616c 6c65  ook.can be calle
-00003fe0: 6420 7769 7468 203a 7079 3a6d 6574 683a  d with :py:meth:
-00003ff0: 607e 706c 7567 6779 2e68 6f6f 6b73 2e5f  `~pluggy.hooks._
-00004000: 486f 6f6b 4361 6c6c 6572 2e63 616c 6c5f  HookCaller.call_
-00004010: 6869 7374 6f72 6963 2829 6020 2a2a 6265  historic()` **be
-00004020: 666f 7265 2a2a 0a68 6176 696e 6720 6265  fore**.having be
-00004030: 656e 2072 6567 6973 7465 7265 643a 0a0a  en registered:..
-00004040: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00004050: 7079 7468 6f6e 0a0a 2020 2020 4068 6f6f  python..    @hoo
-00004060: 6b73 7065 6328 6869 7374 6f72 6963 3d54  kspec(historic=T
-00004070: 7275 6529 0a20 2020 2064 6566 206d 7968  rue).    def myh
-00004080: 6f6f 6b28 636f 6e66 6967 2c20 6172 6773  ook(config, args
-00004090: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000040a0: 0a54 6865 2069 6d70 6c69 6361 7469 6f6e  .The implication
-000040b0: 2069 7320 7468 6174 206c 6174 6520 7265   is that late re
-000040c0: 6769 7374 6572 6564 202a 686f 6f6b 696d  gistered *hookim
-000040d0: 706c 732a 2077 696c 6c20 6265 2063 616c  pls* will be cal
-000040e0: 6c65 6420 6261 636b 0a69 6d6d 6564 6961  led back.immedia
-000040f0: 7465 6c79 2061 7420 7265 6769 7374 6572  tely at register
-00004100: 2074 696d 6520 616e 6420 2a2a 6361 6e20   time and **can 
-00004110: 6e6f 742a 2a20 7265 7475 726e 2061 2072  not** return a r
-00004120: 6573 756c 7420 746f 2074 6865 2063 616c  esult to the cal
-00004130: 6c65 722e 0a0a 5468 6973 2074 7572 6e73  ler...This turns
-00004140: 206f 7574 2074 6f20 6265 2070 6172 7469   out to be parti
-00004150: 6375 6c61 726c 7920 7573 6566 756c 2077  cularly useful w
-00004160: 6865 6e20 6465 616c 696e 6720 7769 7468  hen dealing with
-00004170: 206c 617a 7920 6f72 0a64 796e 616d 6963   lazy or.dynamic
-00004180: 616c 6c79 206c 6f61 6465 6420 706c 7567  ally loaded plug
-00004190: 696e 732e 0a0a 466f 7220 6d6f 7265 2069  ins...For more i
-000041a0: 6e66 6f20 7365 6520 3a72 6566 3a60 6361  nfo see :ref:`ca
-000041b0: 6c6c 5f68 6973 746f 7269 6360 2e0a 0a0a  ll_historic`....
-000041c0: 5761 726e 696e 6773 206f 6e20 686f 6f6b  Warnings on hook
-000041d0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e0a   implementation.
-000041e0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-000041f0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  ^^^^^^^^^^^^^^^.
-00004200: 0a41 7320 7072 6f6a 6563 7473 2065 766f  .As projects evo
-00004210: 6c76 6520 6e65 7720 686f 6f6b 7320 6d61  lve new hooks ma
-00004220: 7920 6265 2069 6e74 726f 6475 6365 6420  y be introduced 
-00004230: 616e 642f 6f72 2064 6570 7265 6361 7465  and/or deprecate
-00004240: 642e 0a0a 6966 2061 2068 6f6f 6b73 7065  d...if a hookspe
-00004250: 6320 7370 6563 6966 6965 7320 6120 6060  c specifies a ``
-00004260: 7761 726e 5f6f 6e5f 696d 706c 6060 2c20  warn_on_impl``, 
-00004270: 706c 7567 6779 2077 696c 6c20 7472 6967  pluggy will trig
-00004280: 6765 7220 6974 2066 6f72 2061 6e79 2070  ger it for any p
-00004290: 6c75 6769 6e20 696d 706c 656d 656e 7469  lugin implementi
-000042a0: 6e67 2074 6865 2068 6f6f 6b2e 0a0a 0a2e  ng the hook.....
-000042b0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-000042c0: 7974 686f 6e0a 0a20 2020 2040 686f 6f6b  ython..    @hook
-000042d0: 7370 6563 280a 2020 2020 2020 2020 7761  spec(.        wa
-000042e0: 726e 5f6f 6e5f 696d 706c 3d44 6570 7265  rn_on_impl=Depre
-000042f0: 6361 7469 6f6e 5761 726e 696e 6728 226f  cationWarning("o
-00004300: 6c64 686f 6f6b 2069 7320 6465 7072 6563  ldhook is deprec
-00004310: 6174 6564 2061 6e64 2077 696c 6c20 6265  ated and will be
-00004320: 2072 656d 6f76 6564 2073 6f6f 6e22 290a   removed soon").
-00004330: 2020 2020 290a 2020 2020 6465 6620 6f6c      ).    def ol
-00004340: 6468 6f6f 6b28 293a 0a20 2020 2020 2020  dhook():.       
-00004350: 2070 6173 730a 0a2e 2e20 5f6d 616e 6167   pass.... _manag
-00004360: 653a 0a0a 5468 6520 506c 7567 696e 2072  e:..The Plugin r
-00004370: 6567 6973 7472 790a 2a2a 2a2a 2a2a 2a2a  egistry.********
-00004380: 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a 6060 706c  ***********.``pl
-00004390: 7567 6779 6060 206d 616e 6167 6573 2070  uggy`` manages p
-000043a0: 6c75 6769 6e73 2075 7369 6e67 2069 6e73  lugins using ins
-000043b0: 7461 6e63 6573 206f 6620 7468 650a 3a70  tances of the.:p
-000043c0: 793a 636c 6173 733a 6070 6c75 6767 792e  y:class:`pluggy.
-000043d0: 506c 7567 696e 4d61 6e61 6765 7260 2e0a  PluginManager`..
-000043e0: 0a41 203a 7079 3a63 6c61 7373 3a60 7e70  .A :py:class:`~p
-000043f0: 6c75 6767 792e 506c 7567 696e 4d61 6e61  luggy.PluginMana
-00004400: 6765 7260 2069 7320 696e 7374 616e 7469  ger` is instanti
-00004410: 6174 6564 2077 6974 6820 6120 7369 6e67  ated with a sing
-00004420: 6c65 0a60 6073 7472 6060 2061 7267 756d  le.``str`` argum
-00004430: 656e 742c 2074 6865 2060 6070 726f 6a65  ent, the ``proje
-00004440: 6374 5f6e 616d 6560 603a 0a0a 2e2e 2063  ct_name``:.... c
-00004450: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00004460: 6f6e 0a0a 2020 2020 696d 706f 7274 2070  on..    import p
-00004470: 6c75 6767 790a 0a20 2020 2070 6d20 3d20  luggy..    pm = 
-00004480: 706c 7567 6779 2e50 6c75 6769 6e4d 616e  pluggy.PluginMan
-00004490: 6167 6572 2822 6d79 5f70 726f 6a65 6374  ager("my_project
-000044a0: 5f6e 616d 6522 290a 0a0a 5468 6520 6060  _name")...The ``
-000044b0: 7072 6f6a 6563 745f 6e61 6d65 6060 2076  project_name`` v
-000044c0: 616c 7565 2069 7320 7573 6564 2077 6865  alue is used whe
-000044d0: 6e20 6120 3a70 793a 636c 6173 733a 607e  n a :py:class:`~
-000044e0: 706c 7567 6779 2e50 6c75 6769 6e4d 616e  pluggy.PluginMan
-000044f0: 6167 6572 600a 7363 616e 7320 666f 7220  ager`.scans for 
-00004500: 2a68 6f6f 6b2a 2066 756e 6374 696f 6e73  *hook* functions
-00004510: 203a 7265 663a 6064 6566 696e 6564 206f   :ref:`defined o
-00004520: 6e20 6120 706c 7567 696e 203c 6465 6669  n a plugin <defi
-00004530: 6e65 3e60 2e0a 5468 6973 2061 6c6c 6f77  ne>`..This allow
-00004540: 7320 666f 7220 6d75 6c74 6970 6c65 2070  s for multiple p
-00004550: 6c75 6769 6e20 6d61 6e61 6765 7273 2066  lugin managers f
-00004560: 726f 6d20 6d75 6c74 6970 6c65 2070 726f  rom multiple pro
-00004570: 6a65 6374 730a 746f 2064 6566 696e 6520  jects.to define 
-00004580: 686f 6f6b 7320 616c 6f6e 6773 6964 6520  hooks alongside 
-00004590: 6561 6368 206f 7468 6572 2e0a 0a0a 5265  each other....Re
-000045a0: 6769 7374 7261 7469 6f6e 0a2d 2d2d 2d2d  gistration.-----
-000045b0: 2d2d 2d2d 2d2d 2d0a 4561 6368 203a 7079  -------.Each :py
-000045c0: 3a63 6c61 7373 3a60 7e70 6c75 6767 792e  :class:`~pluggy.
-000045d0: 506c 7567 696e 4d61 6e61 6765 7260 206d  PluginManager` m
-000045e0: 6169 6e74 6169 6e73 2061 202a 706c 7567  aintains a *plug
-000045f0: 696e 2a20 7265 6769 7374 7279 2077 6865  in* registry whe
-00004600: 7265 2065 6163 6820 2a70 6c75 6769 6e2a  re each *plugin*
-00004610: 0a63 6f6e 7461 696e 7320 6120 7365 7420  .contains a set 
-00004620: 6f66 202a 686f 6f6b 696d 706c 2a20 6465  of *hookimpl* de
-00004630: 6669 6e69 7469 6f6e 732e 204c 6f61 6469  finitions. Loadi
-00004640: 6e67 202a 686f 6f6b 696d 706c 2a20 616e  ng *hookimpl* an
-00004650: 6420 2a68 6f6f 6b73 7065 632a 0a64 6566  d *hookspec*.def
-00004660: 696e 6974 696f 6e73 2074 6f20 706f 7075  initions to popu
-00004670: 6c61 7465 2074 6865 2072 6567 6973 7472  late the registr
-00004680: 7920 6973 2064 6573 6372 6962 6564 2069  y is described i
-00004690: 6e20 6465 7461 696c 2069 6e20 7468 6520  n detail in the 
-000046a0: 7365 6374 696f 6e20 6f6e 0a3a 7265 663a  section on.:ref:
-000046b0: 6064 6566 696e 6560 2e0a 0a49 6e20 7375  `define`...In su
-000046c0: 6d6d 6172 792c 2079 6f75 2070 6173 7320  mmary, you pass 
-000046d0: 6120 706c 7567 696e 206e 616d 6573 7061  a plugin namespa
-000046e0: 6365 206f 626a 6563 7420 746f 2074 6865  ce object to the
-000046f0: 0a3a 7079 3a6d 6574 683a 607e 706c 7567  .:py:meth:`~plug
-00004700: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
-00004710: 2e72 6567 6973 7465 7228 2960 2061 6e64  .register()` and
-00004720: 0a3a 7079 3a6d 6574 683a 607e 706c 7567  .:py:meth:`~plug
-00004730: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
-00004740: 2e61 6464 5f68 6f6f 6b73 7065 6373 2829  .add_hookspecs()
-00004750: 6020 6d65 7468 6f64 7320 746f 2063 6f6c  ` methods to col
-00004760: 6c65 6374 0a68 6f6f 6b20 2a69 6d70 6c65  lect.hook *imple
-00004770: 6d65 6e74 6174 696f 6e73 2a20 616e 6420  mentations* and 
-00004780: 2a73 7065 6369 6669 6361 7469 6f6e 732a  *specifications*
-00004790: 2066 726f 6d20 2a70 6c75 6769 6e2a 206e   from *plugin* n
-000047a0: 616d 6573 7061 6365 7320 7265 7370 6563  amespaces respec
-000047b0: 7469 7665 6c79 2e0a 0a59 6f75 2063 616e  tively...You can
-000047c0: 2075 6e72 6567 6973 7465 7220 616e 7920   unregister any 
-000047d0: 2a70 6c75 6769 6e2a 2773 2068 6f6f 6b73  *plugin*'s hooks
-000047e0: 2075 7369 6e67 0a3a 7079 3a6d 6574 683a   using.:py:meth:
-000047f0: 607e 706c 7567 6779 2e50 6c75 6769 6e4d  `~pluggy.PluginM
-00004800: 616e 6167 6572 2e75 6e72 6567 6973 7465  anager.unregiste
-00004810: 7228 2960 2061 6e64 2063 6865 636b 2069  r()` and check i
-00004820: 6620 6120 706c 7567 696e 2069 730a 7265  f a plugin is.re
-00004830: 6769 7374 6572 6564 2062 7920 7061 7373  gistered by pass
-00004840: 696e 6720 6974 7320 6e61 6d65 2074 6f20  ing its name to 
-00004850: 7468 650a 3a70 793a 6d65 7468 3a60 7e70  the.:py:meth:`~p
-00004860: 6c75 6767 792e 506c 7567 696e 4d61 6e61  luggy.PluginMana
-00004870: 6765 722e 6973 5f72 6567 6973 7465 7265  ger.is_registere
-00004880: 6428 2960 206d 6574 686f 642e 0a0a 4c6f  d()` method...Lo
-00004890: 6164 696e 6720 6060 7365 7475 7074 6f6f  ading ``setuptoo
-000048a0: 6c73 6060 2065 6e74 7279 2070 6f69 6e74  ls`` entry point
-000048b0: 730a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  s.^^^^^^^^^^^^^^
-000048c0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-000048d0: 5e5e 5e5e 5e0a 596f 7520 6361 6e20 6175  ^^^^^.You can au
-000048e0: 746f 6d61 7469 6361 6c6c 7920 6c6f 6164  tomatically load
-000048f0: 2070 6c75 6769 6e73 2072 6567 6973 7465   plugins registe
-00004900: 7265 6420 7468 726f 7567 680a 3a72 6566  red through.:ref
-00004910: 3a60 7365 7475 7074 6f6f 6c73 2065 6e74  :`setuptools ent
-00004920: 7279 2070 6f69 6e74 7320 3c73 6574 7570  ry points <setup
-00004930: 746f 6f6c 733a 656e 7472 7920 706f 696e  tools:entry poin
-00004940: 7473 3e60 0a77 6974 6820 7468 6520 3a70  ts>`.with the :p
-00004950: 793a 6d65 7468 3a60 7e70 6c75 6767 792e  y:meth:`~pluggy.
-00004960: 506c 7567 696e 4d61 6e61 6765 722e 6c6f  PluginManager.lo
-00004970: 6164 5f73 6574 7570 746f 6f6c 735f 656e  ad_setuptools_en
-00004980: 7472 7970 6f69 6e74 7328 2960 0a6d 6574  trypoints()`.met
-00004990: 686f 642e 0a0a 416e 2065 7861 6d70 6c65  hod...An example
-000049a0: 2075 7365 206f 6620 7468 6973 2069 7320   use of this is 
-000049b0: 7468 6520 3a72 6566 3a60 7079 7465 7374  the :ref:`pytest
-000049c0: 2065 6e74 7279 2070 6f69 6e74 203c 7079   entry point <py
-000049d0: 7465 7374 3a70 6970 2d69 6e73 7461 6c6c  test:pip-install
-000049e0: 6162 6c65 2070 6c75 6769 6e73 3e60 2e0a  able plugins>`..
-000049f0: 0a0a 426c 6f63 6b69 6e67 0a2d 2d2d 2d2d  ..Blocking.-----
-00004a00: 2d2d 2d0a 596f 7520 6361 6e20 626c 6f63  ---.You can bloc
-00004a10: 6b20 616e 7920 706c 7567 696e 2066 726f  k any plugin fro
-00004a20: 6d20 6265 696e 6720 7265 6769 7374 6572  m being register
-00004a30: 6564 2075 7369 6e67 0a3a 7079 3a6d 6574  ed using.:py:met
-00004a40: 683a 607e 706c 7567 6779 2e50 6c75 6769  h:`~pluggy.Plugi
-00004a50: 6e4d 616e 6167 6572 2e73 6574 5f62 6c6f  nManager.set_blo
-00004a60: 636b 6564 2829 6020 616e 6420 6368 6563  cked()` and chec
-00004a70: 6b20 6966 2061 2067 6976 656e 0a2a 706c  k if a given.*pl
-00004a80: 7567 696e 2a20 6973 2062 6c6f 636b 6564  ugin* is blocked
-00004a90: 2062 7920 6e61 6d65 2075 7369 6e67 203a   by name using :
-00004aa0: 7079 3a6d 6574 683a 607e 706c 7567 6779  py:meth:`~pluggy
-00004ab0: 2e50 6c75 6769 6e4d 616e 6167 6572 2e69  .PluginManager.i
-00004ac0: 735f 626c 6f63 6b65 6428 2960 2e0a 0a0a  s_blocked()`....
-00004ad0: 496e 7370 6563 7469 6f6e 0a2d 2d2d 2d2d  Inspection.-----
-00004ae0: 2d2d 2d2d 2d0a 596f 7520 6361 6e20 7573  -----.You can us
-00004af0: 6520 6120 7661 7269 6574 7920 6f66 206d  e a variety of m
-00004b00: 6574 686f 6473 2074 6f20 696e 7370 6563  ethods to inspec
-00004b10: 7420 626f 7468 2074 6865 2072 6567 6973  t both the regis
-00004b20: 7472 790a 616e 6420 7061 7274 6963 756c  try.and particul
-00004b30: 6172 2070 6c75 6769 6e73 2069 6e20 6974  ar plugins in it
-00004b40: 3a0a 0a2d 203a 7079 3a6d 6574 683a 607e  :..- :py:meth:`~
-00004b50: 706c 7567 6779 2e50 6c75 6769 6e4d 616e  pluggy.PluginMan
-00004b60: 6167 6572 2e6c 6973 745f 6e61 6d65 5f70  ager.list_name_p
-00004b70: 6c75 6769 6e28 2960 202d 0a20 2072 6574  lugin()` -.  ret
-00004b80: 7572 6e20 6120 6c69 7374 206f 6620 6e61  urn a list of na
-00004b90: 6d65 2d70 6c75 6769 6e20 7061 6972 730a  me-plugin pairs.
-00004ba0: 2d20 3a70 793a 6d65 7468 3a60 7e70 6c75  - :py:meth:`~plu
-00004bb0: 6767 792e 506c 7567 696e 4d61 6e61 6765  ggy.PluginManage
-00004bc0: 722e 6765 745f 706c 7567 696e 7328 2960  r.get_plugins()`
-00004bd0: 202d 2072 6574 7269 6576 6520 616c 6c20   - retrieve all 
-00004be0: 706c 7567 696e 730a 2d20 3a70 793a 6d65  plugins.- :py:me
-00004bf0: 7468 3a60 7e70 6c75 6767 792e 506c 7567  th:`~pluggy.Plug
-00004c00: 696e 4d61 6e61 6765 722e 6765 745f 6361  inManager.get_ca
-00004c10: 6e6f 6e69 6361 6c5f 6e61 6d65 2829 602d  nonical_name()`-
-00004c20: 2067 6574 2061 202a 706c 7567 696e 2a27   get a *plugin*'
-00004c30: 730a 2020 6361 6e6f 6e69 6361 6c20 6e61  s.  canonical na
-00004c40: 6d65 2028 7468 6520 6e61 6d65 2069 7420  me (the name it 
-00004c50: 7761 7320 7265 6769 7374 6572 6564 2077  was registered w
-00004c60: 6974 6829 0a2d 203a 7079 3a6d 6574 683a  ith).- :py:meth:
-00004c70: 607e 706c 7567 6779 2e50 6c75 6769 6e4d  `~pluggy.PluginM
-00004c80: 616e 6167 6572 2e67 6574 5f70 6c75 6769  anager.get_plugi
-00004c90: 6e28 2960 202d 2072 6574 7269 6576 6520  n()` - retrieve 
-00004ca0: 6120 706c 7567 696e 2062 7920 6974 730a  a plugin by its.
-00004cb0: 2020 6361 6e6f 6e69 6361 6c20 6e61 6d65    canonical name
-00004cc0: 0a0a 0a50 6172 7369 6e67 206d 6172 6b20  ...Parsing mark 
-00004cd0: 6f70 7469 6f6e 730a 5e5e 5e5e 5e5e 5e5e  options.^^^^^^^^
-00004ce0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a59 6f75  ^^^^^^^^^^^^.You
-00004cf0: 2063 616e 2072 6574 7269 6576 6520 7468   can retrieve th
-00004d00: 6520 2a6f 7074 696f 6e73 2a20 6170 706c  e *options* appl
-00004d10: 6965 6420 746f 2061 2070 6172 7469 6375  ied to a particu
-00004d20: 6c61 720a 2a68 6f6f 6b73 7065 632a 206f  lar.*hookspec* o
-00004d30: 7220 2a68 6f6f 6b69 6d70 6c2a 2061 7320  r *hookimpl* as 
-00004d40: 7065 7220 3a72 6566 3a60 6d61 726b 696e  per :ref:`markin
-00004d50: 675f 686f 6f6b 7360 2075 7369 6e67 2074  g_hooks` using t
-00004d60: 6865 0a3a 7079 3a6d 6574 683a 607e 706c  he.:py:meth:`~pl
-00004d70: 7567 6779 2e50 6c75 6769 6e4d 616e 6167  uggy.PluginManag
-00004d80: 6572 2e70 6172 7365 5f68 6f6f 6b73 7065  er.parse_hookspe
-00004d90: 635f 6f70 7473 2829 6020 616e 640a 3a70  c_opts()` and.:p
-00004da0: 793a 6d65 7468 3a60 7e70 6c75 6767 792e  y:meth:`~pluggy.
-00004db0: 506c 7567 696e 4d61 6e61 6765 722e 7061  PluginManager.pa
-00004dc0: 7273 655f 686f 6f6b 696d 706c 5f6f 7074  rse_hookimpl_opt
-00004dd0: 7328 2960 2072 6573 7065 6374 6976 656c  s()` respectivel
-00004de0: 792e 0a0a 0a2e 2e20 5f63 616c 6c69 6e67  y...... _calling
-00004df0: 3a0a 0a43 616c 6c69 6e67 2068 6f6f 6b73  :..Calling hooks
-00004e00: 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a54  .*************.T
-00004e10: 6865 2063 6f72 6520 6675 6e63 7469 6f6e  he core function
-00004e20: 616c 6974 7920 6f66 2060 6070 6c75 6767  ality of ``plugg
-00004e30: 7960 6020 656e 6162 6c65 7320 616e 2065  y`` enables an e
-00004e40: 7874 656e 7369 6f6e 2070 726f 7669 6465  xtension provide
-00004e50: 720a 746f 206f 7665 7272 6964 6520 6675  r.to override fu
-00004e60: 6e63 7469 6f6e 2063 616c 6c73 206d 6164  nction calls mad
-00004e70: 6520 6174 2063 6572 7461 696e 2070 6f69  e at certain poi
-00004e80: 6e74 7320 7468 726f 7567 686f 7574 2061  nts throughout a
-00004e90: 2070 726f 6772 616d 2e0a 0a41 2070 6172   program...A par
-00004ea0: 7469 6375 6c61 7220 2a68 6f6f 6b2a 2069  ticular *hook* i
-00004eb0: 7320 696e 766f 6b65 6420 6279 2063 616c  s invoked by cal
-00004ec0: 6c69 6e67 2061 6e20 696e 7374 616e 6365  ling an instance
-00004ed0: 206f 660a 6120 3a70 793a 636c 6173 733a   of.a :py:class:
-00004ee0: 6070 6c75 6767 792e 686f 6f6b 732e 5f48  `pluggy.hooks._H
-00004ef0: 6f6f 6b43 616c 6c65 7260 2077 6869 6368  ookCaller` which
-00004f00: 2069 6e20 7475 726e 202a 6c6f 6f70 732a   in turn *loops*
-00004f10: 2074 6872 6f75 6768 2074 6865 0a60 6031   through the.``1
-00004f20: 3a4e 6060 2072 6567 6973 7465 7265 6420  :N`` registered 
-00004f30: 2a68 6f6f 6b69 6d70 6c73 2a20 616e 6420  *hookimpls* and 
-00004f40: 6361 6c6c 7320 7468 656d 2069 6e20 7365  calls them in se
-00004f50: 7175 656e 6365 2e0a 0a45 7665 7279 203a  quence...Every :
-00004f60: 7079 3a63 6c61 7373 3a60 7e70 6c75 6767  py:class:`~plugg
-00004f70: 792e 506c 7567 696e 4d61 6e61 6765 7260  y.PluginManager`
-00004f80: 2068 6173 2061 2060 6068 6f6f 6b60 6020   has a ``hook`` 
-00004f90: 6174 7472 6962 7574 650a 7768 6963 6820  attribute.which 
-00004fa0: 6973 2061 6e20 696e 7374 616e 6365 206f  is an instance o
-00004fb0: 6620 7468 6973 203a 7079 3a63 6c61 7373  f this :py:class
-00004fc0: 3a60 706c 7567 6779 2e68 6f6f 6b73 2e5f  :`pluggy.hooks._
-00004fd0: 486f 6f6b 5265 6c61 7960 2e0a 5468 6520  HookRelay`..The 
-00004fe0: 3a70 793a 636c 6173 733a 607e 706c 7567  :py:class:`~plug
-00004ff0: 6779 2e68 6f6f 6b73 2e5f 486f 6f6b 5265  gy.hooks._HookRe
-00005000: 6c61 7960 2069 7473 656c 6620 636f 6e74  lay` itself cont
-00005010: 6169 6e73 2072 6566 6572 656e 6365 730a  ains references.
-00005020: 2862 7920 686f 6f6b 206e 616d 6529 2074  (by hook name) t
-00005030: 6f20 6561 6368 2072 6567 6973 7465 7265  o each registere
-00005040: 6420 2a68 6f6f 6b69 6d70 6c2a 2773 203a  d *hookimpl*'s :
-00005050: 7079 3a63 6c61 7373 3a60 7e70 6c75 6767  py:class:`~plugg
-00005060: 792e 686f 6f6b 732e 5f48 6f6f 6b43 616c  y.hooks._HookCal
-00005070: 6c65 7260 2069 6e73 7461 6e63 652e 0a0a  ler` instance...
-00005080: 4d6f 7265 2070 7261 6374 6963 616c 6c79  More practically
-00005090: 2079 6f75 2063 616c 6c20 6120 2a68 6f6f   you call a *hoo
-000050a0: 6b2a 206c 696b 6520 736f 3a0a 0a2e 2e20  k* like so:.... 
-000050b0: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-000050c0: 686f 6e0a 0a20 2020 2069 6d70 6f72 7420  hon..    import 
-000050d0: 7379 730a 2020 2020 696d 706f 7274 2070  sys.    import p
-000050e0: 6c75 6767 790a 2020 2020 696d 706f 7274  luggy.    import
-000050f0: 206d 7970 6c75 6769 6e73 7065 630a 2020   mypluginspec.  
-00005100: 2020 696d 706f 7274 206d 7970 6c75 6769    import myplugi
-00005110: 6e0a 2020 2020 6672 6f6d 2063 6f6e 6669  n.    from confi
-00005120: 6775 7261 7469 6f6e 2069 6d70 6f72 7420  guration import 
-00005130: 636f 6e66 6967 0a0a 2020 2020 706d 203d  config..    pm =
-00005140: 2070 6c75 6767 792e 506c 7567 696e 4d61   pluggy.PluginMa
-00005150: 6e61 6765 7228 226d 7970 726f 6a65 6374  nager("myproject
-00005160: 2229 0a20 2020 2070 6d2e 6164 645f 686f  ").    pm.add_ho
-00005170: 6f6b 7370 6563 7328 6d79 706c 7567 696e  okspecs(myplugin
-00005180: 7370 6563 290a 2020 2020 706d 2e72 6567  spec).    pm.reg
-00005190: 6973 7465 7228 6d79 706c 7567 696e 290a  ister(myplugin).
-000051a0: 0a20 2020 2023 2077 6520 696e 766f 6b65  .    # we invoke
-000051b0: 2074 6865 205f 486f 6f6b 4361 6c6c 6572   the _HookCaller
-000051c0: 2061 6e64 2074 6875 7320 616c 6c20 756e   and thus all un
-000051d0: 6465 726c 7969 6e67 2068 6f6f 6b69 6d70  derlying hookimp
-000051e0: 6c73 0a20 2020 2072 6573 756c 745f 6c69  ls.    result_li
-000051f0: 7374 203d 2070 6d2e 686f 6f6b 2e6d 7968  st = pm.hook.myh
-00005200: 6f6f 6b28 636f 6e66 6967 3d63 6f6e 6669  ook(config=confi
-00005210: 672c 2061 7267 733d 7379 732e 6172 6776  g, args=sys.argv
-00005220: 290a 0a4e 6f74 6520 7468 6174 2079 6f75  )..Note that you
-00005230: 202a 2a6d 7573 742a 2a20 6361 6c6c 2068   **must** call h
-00005240: 6f6f 6b73 2075 7369 6e67 206b 6579 776f  ooks using keywo
-00005250: 7264 203a 7374 643a 7465 726d 3a60 7079  rd :std:term:`py
-00005260: 7468 6f6e 3a61 7267 756d 656e 7460 2073  thon:argument` s
-00005270: 796e 7461 7821 0a0a 486f 6f6b 2069 6d70  yntax!..Hook imp
-00005280: 6c65 6d65 6e74 6174 696f 6e73 2061 7265  lementations are
-00005290: 2063 616c 6c65 6420 696e 204c 4946 4f20   called in LIFO 
-000052a0: 7265 6769 7374 6572 6564 206f 7264 6572  registered order
-000052b0: 3a20 2a74 6865 206c 6173 740a 7265 6769  : *the last.regi
-000052c0: 7374 6572 6564 2070 6c75 6769 6e27 7320  stered plugin's 
-000052d0: 686f 6f6b 7320 6172 6520 6361 6c6c 6564  hooks are called
-000052e0: 2066 6972 7374 2a2e 2041 7320 616e 2065   first*. As an e
-000052f0: 7861 6d70 6c65 2c20 7468 6520 6265 6c6f  xample, the belo
-00005300: 770a 6173 7365 7274 696f 6e20 7368 6f75  w.assertion shou
-00005310: 6c64 206e 6f74 2065 7272 6f72 3a0a 0a2e  ld not error:...
-00005320: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00005330: 7974 686f 6e0a 0a20 2020 2066 726f 6d20  ython..    from 
-00005340: 706c 7567 6779 2069 6d70 6f72 7420 506c  pluggy import Pl
-00005350: 7567 696e 4d61 6e61 6765 722c 2048 6f6f  uginManager, Hoo
-00005360: 6b69 6d70 6c4d 6172 6b65 720a 0a20 2020  kimplMarker..   
-00005370: 2068 6f6f 6b69 6d70 6c20 3d20 486f 6f6b   hookimpl = Hook
-00005380: 696d 706c 4d61 726b 6572 2822 6d79 7072  implMarker("mypr
-00005390: 6f6a 6563 7422 290a 0a0a 2020 2020 636c  oject")...    cl
-000053a0: 6173 7320 506c 7567 696e 3128 6f62 6a65  ass Plugin1(obje
-000053b0: 6374 293a 0a20 2020 2020 2020 2040 686f  ct):.        @ho
-000053c0: 6f6b 696d 706c 0a20 2020 2020 2020 2064  okimpl.        d
-000053d0: 6566 206d 7968 6f6f 6b28 7365 6c66 2c20  ef myhook(self, 
-000053e0: 6172 6773 293a 0a20 2020 2020 2020 2020  args):.         
-000053f0: 2020 2022 2222 4465 6661 756c 7420 696d     """Default im
-00005400: 706c 656d 656e 7461 7469 6f6e 2e0a 2020  plementation..  
-00005410: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-00005420: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005430: 2031 0a0a 0a20 2020 2063 6c61 7373 2050   1...    class P
-00005440: 6c75 6769 6e32 286f 626a 6563 7429 3a0a  lugin2(object):.
-00005450: 2020 2020 2020 2020 4068 6f6f 6b69 6d70          @hookimp
-00005460: 6c0a 2020 2020 2020 2020 6465 6620 6d79  l.        def my
-00005470: 686f 6f6b 2873 656c 662c 2061 7267 7329  hook(self, args)
-00005480: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
-00005490: 2244 6566 6175 6c74 2069 6d70 6c65 6d65  "Default impleme
-000054a0: 6e74 6174 696f 6e2e 0a20 2020 2020 2020  ntation..       
-000054b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000054c0: 2020 2020 2072 6574 7572 6e20 320a 0a0a       return 2...
-000054d0: 2020 2020 636c 6173 7320 506c 7567 696e      class Plugin
-000054e0: 3328 6f62 6a65 6374 293a 0a20 2020 2020  3(object):.     
-000054f0: 2020 2040 686f 6f6b 696d 706c 0a20 2020     @hookimpl.   
-00005500: 2020 2020 2064 6566 206d 7968 6f6f 6b28       def myhook(
-00005510: 7365 6c66 2c20 6172 6773 293a 0a20 2020  self, args):.   
-00005520: 2020 2020 2020 2020 2022 2222 4465 6661           """Defa
-00005530: 756c 7420 696d 706c 656d 656e 7461 7469  ult implementati
-00005540: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00005550: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
-00005560: 7265 7475 726e 2033 0a0a 0a20 2020 2070  return 3...    p
-00005570: 6d20 3d20 506c 7567 696e 4d61 6e61 6765  m = PluginManage
-00005580: 7228 226d 7970 726f 6a65 6374 2229 0a20  r("myproject"). 
-00005590: 2020 2070 6d2e 7265 6769 7374 6572 2850     pm.register(P
-000055a0: 6c75 6769 6e31 2829 290a 2020 2020 706d  lugin1()).    pm
-000055b0: 2e72 6567 6973 7465 7228 506c 7567 696e  .register(Plugin
-000055c0: 3228 2929 0a20 2020 2070 6d2e 7265 6769  2()).    pm.regi
-000055d0: 7374 6572 2850 6c75 6769 6e33 2829 290a  ster(Plugin3()).
-000055e0: 0a20 2020 2061 7373 6572 7420 706d 2e68  .    assert pm.h
-000055f0: 6f6f 6b2e 6d79 686f 6f6b 2861 7267 733d  ook.myhook(args=
-00005600: 2829 2920 3d3d 205b 332c 2032 2c20 315d  ()) == [3, 2, 1]
-00005610: 0a0a 436f 6c6c 6563 7469 6e67 2072 6573  ..Collecting res
-00005620: 756c 7473 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ults.-----------
-00005630: 2d2d 2d2d 2d2d 2d0a 4279 2064 6566 6175  -------.By defau
-00005640: 6c74 2063 616c 6c69 6e67 2061 2068 6f6f  lt calling a hoo
-00005650: 6b20 7265 7375 6c74 7320 696e 2061 6c6c  k results in all
-00005660: 2075 6e64 6572 6c79 696e 6720 3a72 6566   underlying :ref
-00005670: 3a60 686f 6f6b 696d 706c 730a 3c69 6d70  :`hookimpls.<imp
-00005680: 6c73 3e60 2066 756e 6374 696f 6e73 2074  ls>` functions t
-00005690: 6f20 6265 2069 6e76 6f6b 6564 2069 6e20  o be invoked in 
-000056a0: 7365 7175 656e 6365 2076 6961 2061 206c  sequence via a l
-000056b0: 6f6f 702e 2041 6e79 2066 756e 6374 696f  oop. Any functio
-000056c0: 6e0a 7768 6963 6820 7265 7475 726e 7320  n.which returns 
-000056d0: 6120 7661 6c75 6520 6f74 6865 7220 7468  a value other th
-000056e0: 656e 2061 2060 604e 6f6e 6560 6020 7265  en a ``None`` re
-000056f0: 7375 6c74 2077 696c 6c20 6861 7665 2074  sult will have t
-00005700: 6861 7420 7265 7375 6c74 0a61 7070 656e  hat result.appen
-00005710: 6465 6420 746f 2061 203a 7079 3a63 6c61  ded to a :py:cla
-00005720: 7373 3a60 6c69 7374 6020 7768 6963 6820  ss:`list` which 
-00005730: 6973 2072 6574 7572 6e65 6420 6279 2074  is returned by t
-00005740: 6865 2063 616c 6c2e 0a0a 5468 6520 6f6e  he call...The on
-00005750: 6c79 2065 7863 6570 7469 6f6e 2074 6f20  ly exception to 
-00005760: 7468 6973 2062 6568 6176 696f 7572 2069  this behaviour i
-00005770: 7320 6966 2074 6865 2068 6f6f 6b20 6861  s if the hook ha
-00005780: 7320 6265 656e 206d 6172 6b65 6420 746f  s been marked to
-00005790: 2072 6574 7572 6e0a 6974 7320 3a72 6566   return.its :ref
-000057a0: 3a60 6669 7273 7420 7265 7375 6c74 206f  :`first result o
-000057b0: 6e6c 7920 3c66 6972 7374 7265 7375 6c74  nly <firstresult
-000057c0: 3e60 2069 6e20 7768 6963 6820 6361 7365  >` in which case
-000057d0: 206f 6e6c 7920 7468 6520 6669 7273 740a   only the first.
-000057e0: 7369 6e67 6c65 2076 616c 7565 2028 7768  single value (wh
-000057f0: 6963 6820 6973 206e 6f74 2060 604e 6f6e  ich is not ``Non
-00005800: 6560 6029 2077 696c 6c20 6265 2072 6574  e``) will be ret
-00005810: 7572 6e65 642e 0a0a 2e2e 205f 6361 6c6c  urned..... _call
-00005820: 5f68 6973 746f 7269 633a 0a0a 4578 6365  _historic:..Exce
-00005830: 7074 696f 6e20 6861 6e64 6c69 6e67 0a2d  ption handling.-
-00005840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005850: 2d0a 4966 2061 6e79 202a 686f 6f6b 696d  -.If any *hookim
-00005860: 706c 2a20 6572 726f 7273 2077 6974 6820  pl* errors with 
-00005870: 616e 2065 7863 6570 7469 6f6e 206e 6f20  an exception no 
-00005880: 6675 7274 6865 7220 6361 6c6c 6261 636b  further callback
-00005890: 730a 6172 6520 696e 766f 6b65 6420 616e  s.are invoked an
-000058a0: 6420 7468 6520 6578 6365 7074 696f 6e20  d the exception 
-000058b0: 6973 2070 6163 6b61 6765 6420 7570 2061  is packaged up a
-000058c0: 6e64 2064 656c 6976 6572 6564 2074 6f0a  nd delivered to.
-000058d0: 616e 7920 3a72 6566 3a60 7772 6170 7065  any :ref:`wrappe
-000058e0: 7273 203c 686f 6f6b 7772 6170 7065 7273  rs <hookwrappers
-000058f0: 3e60 2062 6566 6f72 6520 6265 696e 6720  >` before being 
-00005900: 7265 2d72 6169 7365 6420 6174 2074 6865  re-raised at the
-00005910: 0a68 6f6f 6b20 696e 766f 6361 7469 6f6e  .hook invocation
-00005920: 2070 6f69 6e74 3a0a 0a2e 2e20 636f 6465   point:.... code
-00005930: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00005940: 0a20 2020 2066 726f 6d20 706c 7567 6779  .    from pluggy
-00005950: 2069 6d70 6f72 7420 506c 7567 696e 4d61   import PluginMa
-00005960: 6e61 6765 722c 2048 6f6f 6b69 6d70 6c4d  nager, HookimplM
-00005970: 6172 6b65 720a 0a20 2020 2068 6f6f 6b69  arker..    hooki
-00005980: 6d70 6c20 3d20 486f 6f6b 696d 706c 4d61  mpl = HookimplMa
-00005990: 726b 6572 2822 6d79 7072 6f6a 6563 7422  rker("myproject"
-000059a0: 290a 0a0a 2020 2020 636c 6173 7320 506c  )...    class Pl
-000059b0: 7567 696e 3128 6f62 6a65 6374 293a 0a20  ugin1(object):. 
-000059c0: 2020 2020 2020 2040 686f 6f6b 696d 706c         @hookimpl
-000059d0: 0a20 2020 2020 2020 2064 6566 206d 7968  .        def myh
-000059e0: 6f6f 6b28 7365 6c66 2c20 6172 6773 293a  ook(self, args):
-000059f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00005a00: 7572 6e20 310a 0a0a 2020 2020 636c 6173  urn 1...    clas
-00005a10: 7320 506c 7567 696e 3228 6f62 6a65 6374  s Plugin2(object
-00005a20: 293a 0a20 2020 2020 2020 2040 686f 6f6b  ):.        @hook
-00005a30: 696d 706c 0a20 2020 2020 2020 2064 6566  impl.        def
-00005a40: 206d 7968 6f6f 6b28 7365 6c66 2c20 6172   myhook(self, ar
-00005a50: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
-00005a60: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
-00005a70: 726f 720a 0a0a 2020 2020 636c 6173 7320  ror...    class 
-00005a80: 506c 7567 696e 3328 6f62 6a65 6374 293a  Plugin3(object):
-00005a90: 0a20 2020 2020 2020 2040 686f 6f6b 696d  .        @hookim
-00005aa0: 706c 0a20 2020 2020 2020 2064 6566 206d  pl.        def m
-00005ab0: 7968 6f6f 6b28 7365 6c66 2c20 6172 6773  yhook(self, args
-00005ac0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00005ad0: 6574 7572 6e20 330a 0a0a 2020 2020 4068  eturn 3...    @h
-00005ae0: 6f6f 6b69 6d70 6c28 686f 6f6b 7772 6170  ookimpl(hookwrap
-00005af0: 7065 723d 5472 7565 290a 2020 2020 6465  per=True).    de
-00005b00: 6620 6d79 686f 6f6b 2873 656c 662c 2061  f myhook(self, a
-00005b10: 7267 7329 3a0a 2020 2020 2020 2020 6f75  rgs):.        ou
-00005b20: 7463 6f6d 6520 3d20 7969 656c 640a 0a20  tcome = yield.. 
-00005b30: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00005b40: 2020 2020 2020 2020 6f75 7463 6f6d 652e          outcome.
-00005b50: 6765 745f 7265 7375 6c74 2829 0a20 2020  get_result().   
-00005b60: 2020 2020 2065 7863 6570 7420 5275 6e74       except Runt
-00005b70: 696d 6545 7272 6f72 3a0a 2020 2020 2020  imeError:.      
-00005b80: 2020 2020 2020 2320 6c6f 6720 7468 6520        # log the 
-00005b90: 6572 726f 7220 6465 7461 696c 730a 2020  error details.  
-00005ba0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00005bb0: 6f75 7463 6f6d 652e 6578 6369 6e66 6f29  outcome.excinfo)
-00005bc0: 0a0a 0a20 2020 2070 6d20 3d20 506c 7567  ...    pm = Plug
-00005bd0: 696e 4d61 6e61 6765 7228 226d 7970 726f  inManager("mypro
-00005be0: 6a65 6374 2229 0a0a 2020 2020 2320 7265  ject")..    # re
-00005bf0: 6769 7374 6572 2070 6c75 6769 6e73 0a20  gister plugins. 
-00005c00: 2020 2070 6d2e 7265 6769 7374 6572 2850     pm.register(P
-00005c10: 6c75 6769 6e31 2829 290a 2020 2020 706d  lugin1()).    pm
-00005c20: 2e72 6567 6973 7465 7228 506c 7567 696e  .register(Plugin
-00005c30: 3228 2929 0a20 2020 2070 6d2e 7265 6769  2()).    pm.regi
-00005c40: 7374 6572 2850 6c75 6769 6e33 2829 290a  ster(Plugin3()).
-00005c50: 0a20 2020 2023 2072 6567 6973 7465 7220  .    # register 
-00005c60: 7772 6170 7065 720a 2020 2020 706d 2e72  wrapper.    pm.r
-00005c70: 6567 6973 7465 7228 7379 732e 6d6f 6475  egister(sys.modu
-00005c80: 6c65 735b 5f5f 6e61 6d65 5f5f 5d29 0a0a  les[__name__])..
-00005c90: 2020 2020 2320 7468 6973 2072 6169 7365      # this raise
-00005ca0: 7320 5275 6e74 696d 6545 7272 6f72 2064  s RuntimeError d
-00005cb0: 7565 2074 6f20 506c 7567 696e 320a 2020  ue to Plugin2.  
-00005cc0: 2020 706d 2e68 6f6f 6b2e 6d79 686f 6f6b    pm.hook.myhook
-00005cd0: 2861 7267 733d 2829 290a 0a48 6973 746f  (args=())..Histo
-00005ce0: 7269 6320 6361 6c6c 730a 2d2d 2d2d 2d2d  ric calls.------
-00005cf0: 2d2d 2d2d 2d2d 2d2d 0a41 202a 6869 7374  --------.A *hist
-00005d00: 6f72 6963 2063 616c 6c2a 2061 6c6c 6f77  oric call* allow
-00005d10: 7320 666f 7220 616c 6c20 6e65 776c 7920  s for all newly 
-00005d20: 7265 6769 7374 6572 6564 2066 756e 6374  registered funct
-00005d30: 696f 6e73 2074 6f20 7265 6365 6976 6520  ions to receive 
-00005d40: 616c 6c20 686f 6f6b 0a63 616c 6c73 2074  all hook.calls t
-00005d50: 6861 7420 6861 7070 656e 6564 2062 6566  hat happened bef
-00005d60: 6f72 6520 7468 6569 7220 7265 6769 7374  ore their regist
-00005d70: 7261 7469 6f6e 2e20 5468 6520 696d 706c  ration. The impl
-00005d80: 6963 6174 696f 6e20 6973 2074 6861 7420  ication is that 
-00005d90: 7468 6973 2069 730a 6f6e 6c79 2075 7365  this is.only use
-00005da0: 6675 6c20 6966 2079 6f75 2065 7870 6563  ful if you expec
-00005db0: 7420 7468 6174 2073 6f6d 6520 2a68 6f6f  t that some *hoo
-00005dc0: 6b69 6d70 6c73 2a20 6d61 7920 6265 2072  kimpls* may be r
-00005dd0: 6567 6973 7465 7265 6420 2a2a 6166 7465  egistered **afte
-00005de0: 722a 2a20 7468 650a 686f 6f6b 2069 7320  r** the.hook is 
-00005df0: 696e 6974 6961 6c6c 7920 696e 766f 6b65  initially invoke
-00005e00: 642e 0a0a 4869 7374 6f72 6963 2068 6f6f  d...Historic hoo
-00005e10: 6b73 206d 7573 7420 6265 203a 7265 663a  ks must be :ref:
-00005e20: 6073 7065 6369 616c 6c79 206d 6172 6b65  `specially marke
-00005e30: 6420 3c68 6973 746f 7269 633e 6020 616e  d <historic>` an
-00005e40: 6420 6361 6c6c 6564 0a75 7369 6e67 2074  d called.using t
-00005e50: 6865 203a 7079 3a6d 6574 683a 607e 706c  he :py:meth:`~pl
-00005e60: 7567 6779 2e68 6f6f 6b73 2e5f 486f 6f6b  uggy.hooks._Hook
-00005e70: 4361 6c6c 6572 2e63 616c 6c5f 6869 7374  Caller.call_hist
-00005e80: 6f72 6963 2829 6020 6d65 7468 6f64 3a0a  oric()` method:.
-00005e90: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00005ea0: 2070 7974 686f 6e0a 0a20 2020 2064 6566   python..    def
-00005eb0: 2063 616c 6c62 6163 6b28 7265 7375 6c74   callback(result
-00005ec0: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
-00005ed0: 2822 6869 7374 6f72 6963 2063 616c 6c20  ("historic call 
-00005ee0: 7265 7375 6c74 2069 7320 7b72 6573 756c  result is {resul
-00005ef0: 747d 222e 666f 726d 6174 2872 6573 756c  t}".format(resul
-00005f00: 743d 7265 7375 6c74 2929 0a0a 0a20 2020  t=result))...   
-00005f10: 2023 2063 616c 6c20 7769 7468 2068 6973   # call with his
-00005f20: 746f 7279 3b20 6e6f 2072 6573 756c 7473  tory; no results
-00005f30: 2072 6574 7572 6e65 640a 2020 2020 706d   returned.    pm
-00005f40: 2e68 6f6f 6b2e 6d79 686f 6f6b 2e63 616c  .hook.myhook.cal
-00005f50: 6c5f 6869 7374 6f72 6963 280a 2020 2020  l_historic(.    
-00005f60: 2020 2020 6b77 6172 6773 3d7b 2263 6f6e      kwargs={"con
-00005f70: 6669 6722 3a20 636f 6e66 6967 2c20 2261  fig": config, "a
-00005f80: 7267 7322 3a20 7379 732e 6172 6776 7d2c  rgs": sys.argv},
-00005f90: 2072 6573 756c 745f 6361 6c6c 6261 636b   result_callback
-00005fa0: 3d63 616c 6c62 6163 6b0a 2020 2020 290a  =callback.    ).
-00005fb0: 0a20 2020 2023 202e 2e2e 206d 6f72 6520  .    # ... more 
-00005fc0: 6f66 206f 7572 2070 726f 6772 616d 202e  of our program .
-00005fd0: 2e2e 0a0a 2020 2020 2320 6c61 7465 206c  ....    # late l
-00005fe0: 6f61 6469 6e67 206f 6620 736f 6d65 2070  oading of some p
-00005ff0: 6c75 6769 6e0a 2020 2020 696d 706f 7274  lugin.    import
-00006000: 206d 796c 6174 6570 6c75 6769 6e0a 0a20   mylateplugin.. 
-00006010: 2020 2023 2068 6973 746f 7269 6320 6361     # historic ca
-00006020: 6c6c 6261 636b 2069 7320 696e 766f 6b65  llback is invoke
-00006030: 6420 6865 7265 0a20 2020 2070 6d2e 7265  d here.    pm.re
-00006040: 6769 7374 6572 286d 796c 6174 6570 6c75  gister(mylateplu
-00006050: 6769 6e29 0a0a 4e6f 7465 2074 6861 7420  gin)..Note that 
-00006060: 6966 2079 6f75 203a 7079 3a6d 6574 683a  if you :py:meth:
-00006070: 607e 706c 7567 6779 2e68 6f6f 6b73 2e5f  `~pluggy.hooks._
-00006080: 486f 6f6b 4361 6c6c 6572 2e63 616c 6c5f  HookCaller.call_
-00006090: 6869 7374 6f72 6963 2829 600a 7468 6520  historic()`.the 
-000060a0: 3a70 793a 636c 6173 733a 607e 706c 7567  :py:class:`~plug
-000060b0: 6779 2e68 6f6f 6b73 2e5f 486f 6f6b 4361  gy.hooks._HookCa
-000060c0: 6c6c 6572 6020 2861 6e64 2074 6875 7320  ller` (and thus 
-000060d0: 796f 7572 2063 616c 6c69 6e67 2063 6f64  your calling cod
-000060e0: 6529 0a63 616e 206e 6f74 2072 6563 6569  e).can not recei
-000060f0: 7665 2072 6573 756c 7473 2062 6163 6b20  ve results back 
-00006100: 6672 6f6d 2074 6865 2075 6e64 6572 6c79  from the underly
-00006110: 696e 6720 2a68 6f6f 6b69 6d70 6c2a 2066  ing *hookimpl* f
-00006120: 756e 6374 696f 6e73 2e0a 496e 7374 6561  unctions..Instea
-00006130: 6420 796f 7520 6361 6e20 7072 6f76 6964  d you can provid
-00006140: 6520 6120 2a63 616c 6c62 6163 6b2a 2066  e a *callback* f
-00006150: 6f72 2070 726f 6365 7373 696e 6720 7265  or processing re
-00006160: 7375 6c74 7320 286c 696b 6520 7468 650a  sults (like the.
-00006170: 6060 6361 6c6c 6261 636b 6060 2066 756e  ``callback`` fun
-00006180: 6374 696f 6e20 6162 6f76 6529 2077 6869  ction above) whi
-00006190: 6368 2077 696c 6c20 6265 2063 616c 6c65  ch will be calle
-000061a0: 6420 6173 2065 6163 6820 6e65 7720 706c  d as each new pl
-000061b0: 7567 696e 0a69 7320 7265 6769 7374 6572  ugin.is register
-000061c0: 6564 2e0a 0a2e 2e20 6e6f 7465 3a3a 0a20  ed..... note::. 
-000061d0: 2020 202a 6869 7374 6f72 6963 2a20 6361     *historic* ca
-000061e0: 6c6c 7320 6172 6520 696e 636f 6d70 6174  lls are incompat
-000061f0: 6962 6c65 2077 6974 6820 3a72 6566 3a60  ible with :ref:`
-00006200: 6669 7273 7472 6573 756c 7460 206d 6172  firstresult` mar
-00006210: 6b65 640a 2020 2020 686f 6f6b 7320 7369  ked.    hooks si
-00006220: 6e63 6520 6f6e 6c79 2074 6865 2066 6972  nce only the fir
-00006230: 7374 2072 6567 6973 7465 7265 6420 706c  st registered pl
-00006240: 7567 696e 2773 2068 6f6f 6b28 7329 2077  ugin's hook(s) w
-00006250: 6f75 6c64 0a20 2020 2065 7665 7220 6265  ould.    ever be
-00006260: 2063 616c 6c65 642e 0a0a 4361 6c6c 696e   called...Callin
-00006270: 6720 7769 7468 2065 7874 7261 730a 2d2d  g with extras.--
-00006280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006290: 2d0a 596f 7520 6361 6e20 6361 6c6c 2061  -.You can call a
-000062a0: 2068 6f6f 6b20 7769 7468 2074 656d 706f   hook with tempo
-000062b0: 7261 7269 6c79 2070 6172 7469 6369 7061  rarily participa
-000062c0: 7469 6e67 202a 696d 706c 656d 656e 7461  ting *implementa
-000062d0: 7469 6f6e 2a20 6675 6e63 7469 6f6e 730a  tion* functions.
-000062e0: 2874 6861 7420 6172 656e 2774 2069 6e20  (that aren't in 
-000062f0: 7468 6520 7265 6769 7374 7279 2920 7573  the registry) us
-00006300: 696e 6720 7468 650a 3a70 793a 6d65 7468  ing the.:py:meth
-00006310: 3a60 706c 7567 6779 2e68 6f6f 6b73 2e5f  :`pluggy.hooks._
-00006320: 486f 6f6b 4361 6c6c 6572 2e63 616c 6c5f  HookCaller.call_
-00006330: 6578 7472 6128 2960 206d 6574 686f 642e  extra()` method.
-00006340: 0a0a 0a43 616c 6c69 6e67 2077 6974 6820  ...Calling with 
-00006350: 6120 7375 6273 6574 206f 6620 7265 6769  a subset of regi
-00006360: 7374 6572 6564 2070 6c75 6769 6e73 0a2d  stered plugins.-
-00006370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006390: 2d2d 2d2d 2d2d 2d2d 2d2d 0a59 6f75 2063  ----------.You c
-000063a0: 616e 206d 616b 6520 6120 6361 6c6c 2075  an make a call u
-000063b0: 7369 6e67 2061 2073 7562 7365 7420 6f66  sing a subset of
-000063c0: 2070 6c75 6769 6e73 2062 7920 6173 6b69   plugins by aski
-000063d0: 6e67 2074 6865 0a3a 7079 3a63 6c61 7373  ng the.:py:class
-000063e0: 3a60 7e70 6c75 6767 792e 506c 7567 696e  :`~pluggy.Plugin
-000063f0: 4d61 6e61 6765 7260 2066 6972 7374 2066  Manager` first f
-00006400: 6f72 2061 0a3a 7079 3a63 6c61 7373 3a60  or a.:py:class:`
-00006410: 7e70 6c75 6767 792e 686f 6f6b 732e 5f48  ~pluggy.hooks._H
-00006420: 6f6f 6b43 616c 6c65 7260 2077 6974 6820  ookCaller` with 
-00006430: 7468 6f73 6520 706c 7567 696e 7320 7265  those plugins re
-00006440: 6d6f 7665 640a 7573 696e 6720 7468 6520  moved.using the 
-00006450: 3a70 793a 6d65 7468 3a60 706c 7567 6779  :py:meth:`pluggy
-00006460: 2e50 6c75 6769 6e4d 616e 6167 6572 2e73  .PluginManager.s
-00006470: 7562 7365 745f 686f 6f6b 5f63 616c 6c65  ubset_hook_calle
-00006480: 7228 2960 206d 6574 686f 642e 0a0a 596f  r()` method...Yo
-00006490: 7520 7468 656e 2063 616e 2075 7365 2074  u then can use t
-000064a0: 6861 7420 3a70 793a 636c 6173 733a 605f  hat :py:class:`_
-000064b0: 486f 6f6b 4361 6c6c 6572 203c 706c 7567  HookCaller <plug
-000064c0: 6779 2e68 6f6f 6b73 2e5f 486f 6f6b 4361  gy.hooks._HookCa
-000064d0: 6c6c 6572 3e60 0a74 6f20 6d61 6b65 206e  ller>`.to make n
-000064e0: 6f72 6d61 6c2c 203a 7079 3a6d 6574 683a  ormal, :py:meth:
-000064f0: 607e 706c 7567 6779 2e68 6f6f 6b73 2e5f  `~pluggy.hooks._
-00006500: 486f 6f6b 4361 6c6c 6572 2e63 616c 6c5f  HookCaller.call_
-00006510: 6869 7374 6f72 6963 602c 206f 720a 3a70  historic`, or.:p
-00006520: 793a 6d65 7468 3a60 7e70 6c75 6767 792e  y:meth:`~pluggy.
-00006530: 686f 6f6b 732e 5f48 6f6f 6b43 616c 6c65  hooks._HookCalle
-00006540: 722e 6361 6c6c 5f65 7874 7261 6020 6361  r.call_extra` ca
-00006550: 6c6c 7320 6173 206e 6563 6573 7361 7279  lls as necessary
-00006560: 2e0a 0a42 7569 6c74 2d69 6e20 7472 6163  ...Built-in trac
-00006570: 696e 670a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ing.************
-00006580: 2a2a 2a2a 0a60 6070 6c75 6767 7960 6020  ****.``pluggy`` 
-00006590: 636f 6d65 7320 7769 7468 2073 6f6d 6520  comes with some 
-000065a0: 6261 7474 6572 6965 7320 696e 636c 7564  batteries includ
-000065b0: 6564 2068 6f6f 6b20 7472 6163 696e 6720  ed hook tracing 
-000065c0: 666f 7220 796f 7572 0a64 6562 7567 6769  for your.debuggi
-000065d0: 6e67 206e 6565 6473 2e0a 0a0a 4361 6c6c  ng needs....Call
-000065e0: 2074 7261 6369 6e67 0a2d 2d2d 2d2d 2d2d   tracing.-------
-000065f0: 2d2d 2d2d 2d0a 546f 2065 6e61 626c 6520  -----.To enable 
-00006600: 7472 6163 696e 6720 7573 6520 7468 650a  tracing use the.
-00006610: 3a70 793a 6d65 7468 3a60 706c 7567 6779  :py:meth:`pluggy
-00006620: 2e50 6c75 6769 6e4d 616e 6167 6572 2e65  .PluginManager.e
-00006630: 6e61 626c 655f 7472 6163 696e 6728 2960  nable_tracing()`
-00006640: 206d 6574 686f 6420 7768 6963 6820 7265   method which re
-00006650: 7475 726e 7320 616e 0a75 6e64 6f20 6675  turns an.undo fu
-00006660: 6e63 7469 6f6e 2074 6f20 6469 7361 626c  nction to disabl
-00006670: 6520 7468 6520 6265 6861 7669 6f75 722e  e the behaviour.
-00006680: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
-00006690: 3a20 7079 7468 6f6e 0a0a 2020 2020 706d  : python..    pm
-000066a0: 203d 2050 6c75 6769 6e4d 616e 6167 6572   = PluginManager
-000066b0: 2822 6d79 7072 6f6a 6563 7422 290a 2020  ("myproject").  
-000066c0: 2020 2320 6d61 6769 6320 6c69 6e65 2074    # magic line t
-000066d0: 6f20 7365 7420 6120 7772 6974 6572 2066  o set a writer f
-000066e0: 756e 6374 696f 6e0a 2020 2020 706d 2e74  unction.    pm.t
-000066f0: 7261 6365 2e72 6f6f 742e 7365 7477 7269  race.root.setwri
-00006700: 7465 7228 7072 696e 7429 0a20 2020 2075  ter(print).    u
-00006710: 6e64 6f20 3d20 706d 2e65 6e61 626c 655f  ndo = pm.enable_
-00006720: 7472 6163 696e 6728 290a 0a0a 4361 6c6c  tracing()...Call
-00006730: 206d 6f6e 6974 6f72 696e 670a 2d2d 2d2d   monitoring.----
-00006740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 496e 7374  -----------.Inst
-00006750: 6561 6420 6f66 2075 7369 6e67 2074 6865  ead of using the
-00006760: 2062 7569 6c74 2d69 6e20 7472 6163 696e   built-in tracin
-00006770: 6720 6d65 6368 616e 6973 6d20 796f 7520  g mechanism you 
-00006780: 6361 6e20 616c 736f 2061 6464 2079 6f75  can also add you
-00006790: 720a 6f77 6e20 6060 6265 666f 7265 6060  r.own ``before``
-000067a0: 2061 6e64 2060 6061 6674 6572 6060 206d   and ``after`` m
-000067b0: 6f6e 6974 6f72 696e 6720 6675 6e63 7469  onitoring functi
-000067c0: 6f6e 7320 7573 696e 670a 3a70 793a 636c  ons using.:py:cl
-000067d0: 6173 733a 6070 6c75 6767 792e 506c 7567  ass:`pluggy.Plug
-000067e0: 696e 4d61 6e61 6765 722e 6164 645f 686f  inManager.add_ho
-000067f0: 6f6b 6361 6c6c 5f6d 6f6e 6974 6f72 696e  okcall_monitorin
-00006800: 6728 2960 2e0a 0a54 6865 2065 7870 6563  g()`...The expec
-00006810: 7465 6420 7369 676e 6174 7572 6520 616e  ted signature an
-00006820: 6420 6465 6661 756c 7420 696d 706c 656d  d default implem
-00006830: 656e 7461 7469 6f6e 7320 666f 7220 7468  entations for th
-00006840: 6573 6520 6675 6e63 7469 6f6e 7320 6973  ese functions is
-00006850: 3a0a 0a2e 2e20 636f 6465 2d62 6c6f 636b  :.... code-block
-00006860: 3a3a 2070 7974 686f 6e0a 0a20 2020 2064  :: python..    d
-00006870: 6566 2062 6566 6f72 6528 686f 6f6b 5f6e  ef before(hook_n
-00006880: 616d 652c 206d 6574 686f 6473 2c20 6b77  ame, methods, kw
-00006890: 6172 6773 293a 0a20 2020 2020 2020 2070  args):.        p
-000068a0: 6173 730a 0a0a 2020 2020 6465 6620 6166  ass...    def af
-000068b0: 7465 7228 6f75 7463 6f6d 652c 2068 6f6f  ter(outcome, hoo
-000068c0: 6b5f 6e61 6d65 2c20 6d65 7468 6f64 732c  k_name, methods,
-000068d0: 206b 7761 7267 7329 3a0a 2020 2020 2020   kwargs):.      
-000068e0: 2020 7061 7373 0a0a 5075 626c 6963 2041    pass..Public A
-000068f0: 5049 0a2a 2a2a 2a2a 2a2a 2a2a 2a0a 506c  PI.**********.Pl
-00006900: 6561 7365 2073 6565 2074 6865 203a 646f  ease see the :do
-00006910: 633a 6061 7069 5f72 6566 6572 656e 6365  c:`api_reference
-00006920: 602e 0a0a 4465 7665 6c6f 706d 656e 740a  `...Development.
-00006930: 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a 4772 6561  ***********.Grea
-00006940: 7420 6361 7265 206d 7573 7420 7461 6b65  t care must take
-00006950: 6e20 7768 656e 2068 6163 6b69 6e67 206f  n when hacking o
-00006960: 6e20 6060 706c 7567 6779 6060 2073 696e  n ``pluggy`` sin
-00006970: 6365 206d 756c 7469 706c 6520 6d61 7475  ce multiple matu
-00006980: 7265 0a70 726f 6a65 6374 7320 7265 6c79  re.projects rely
-00006990: 206f 6e20 6974 2e20 4f75 7220 4769 7468   on it. Our Gith
-000069a0: 7562 2069 6e74 6567 7261 7465 6420 4349  ub integrated CI
-000069b0: 2070 726f 6365 7373 2072 756e 7320 7468   process runs th
-000069c0: 6520 6675 6c6c 0a60 746f 7820 7465 7374  e full.`tox test
-000069d0: 2073 7569 7465 605f 206f 6e20 6561 6368   suite`_ on each
-000069e0: 2063 6f6d 6d69 7420 736f 2062 6520 7375   commit so be su
-000069f0: 7265 2079 6f75 7220 6368 616e 6765 7320  re your changes 
-00006a00: 6361 6e20 7275 6e20 6f6e 0a61 6c6c 2072  can run on.all r
-00006a10: 6571 7569 7265 6420 6050 7974 686f 6e20  equired `Python 
-00006a20: 696e 7465 7270 7265 7465 7273 605f 2061  interpreters`_ a
-00006a30: 6e64 2060 6070 7974 6573 7460 6020 7665  nd ``pytest`` ve
-00006a40: 7273 696f 6e73 2e0a 0a46 6f72 2064 6576  rsions...For dev
-00006a50: 656c 6f70 6d65 6e74 2c20 7765 2073 7567  elopment, we sug
-00006a60: 6765 7374 2074 6f20 6372 6561 7465 2061  gest to create a
-00006a70: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
-00006a80: 6d65 6e74 2061 6e64 2069 6e73 7461 6c6c  ment and install
-00006a90: 2060 6070 6c75 6767 7960 6020 696e 0a65   ``pluggy`` in.e
-00006aa0: 6469 7461 626c 6520 6d6f 6465 2061 6e64  ditable mode and
-00006ab0: 2060 6064 6576 6060 2064 6570 656e 6465   ``dev`` depende
-00006ac0: 6e63 6965 733a 3a0a 0a20 2020 2024 2070  ncies::..    $ p
-00006ad0: 7974 686f 6e33 202d 6d20 7665 6e76 202e  ython3 -m venv .
-00006ae0: 656e 760a 2020 2020 2420 736f 7572 6365  env.    $ source
-00006af0: 202e 656e 762f 6269 6e2f 6163 7469 7661   .env/bin/activa
-00006b00: 7465 0a20 2020 2024 2070 6970 2069 6e73  te.    $ pip ins
-00006b10: 7461 6c6c 202d 6520 2e5b 6465 765d 0a0a  tall -e .[dev]..
-00006b20: 546f 206d 616b 6520 7375 7265 2079 6f75  To make sure you
-00006b30: 2066 6f6c 6c6f 7720 7468 6520 636f 6465   follow the code
-00006b40: 2073 7479 6c65 2075 7365 6420 696e 2074   style used in t
-00006b50: 6865 2070 726f 6a65 6374 2c20 696e 7374  he project, inst
-00006b60: 616c 6c20 7072 652d 636f 6d6d 6974 5f20  all pre-commit_ 
-00006b70: 7768 6963 680a 7769 6c6c 2072 756e 2073  which.will run s
-00006b80: 7479 6c65 2063 6865 636b 7320 6265 666f  tyle checks befo
-00006b90: 7265 2065 6163 6820 636f 6d6d 6974 3a3a  re each commit::
-00006ba0: 0a0a 2020 2020 2420 7072 652d 636f 6d6d  ..    $ pre-comm
-00006bb0: 6974 2069 6e73 7461 6c6c 0a0a 0a52 656c  it install...Rel
-00006bc0: 6561 7365 2050 6f6c 6963 790a 2a2a 2a2a  ease Policy.****
-00006bd0: 2a2a 2a2a 2a2a 2a2a 2a2a 0a50 6c75 6767  **********.Plugg
-00006be0: 7920 7573 6573 2060 5365 6d61 6e74 6963  y uses `Semantic
-00006bf0: 2056 6572 7369 6f6e 696e 6760 5f2e 2042   Versioning`_. B
-00006c00: 7265 616b 696e 6720 6368 616e 6765 7320  reaking changes 
-00006c10: 6172 6520 6f6e 6c79 2066 6f72 6573 6565  are only foresee
-00006c20: 6e20 666f 720a 4d61 6a6f 7220 7265 6c65  n for.Major rele
-00006c30: 6173 6573 2028 696e 6372 656d 656e 7465  ases (incremente
-00006c40: 6420 5820 696e 2022 582e 592e 5a22 292e  d X in "X.Y.Z").
-00006c50: 2020 4966 2079 6f75 2077 616e 7420 746f    If you want to
-00006c60: 2075 7365 2060 6070 6c75 6767 7960 600a   use ``pluggy``.
-00006c70: 696e 2079 6f75 7220 7072 6f6a 6563 7420  in your project 
-00006c80: 796f 7520 7368 6f75 6c64 2074 6875 7320  you should thus 
-00006c90: 7573 6520 6120 6465 7065 6e64 656e 6379  use a dependency
-00006ca0: 2072 6573 7472 6963 7469 6f6e 206c 696b   restriction lik
-00006cb0: 650a 6060 2270 6c75 6767 793e 3d30 2e31  e.``"pluggy>=0.1
-00006cc0: 2e30 2c3c 312e 3022 6060 2074 6f20 6176  .0,<1.0"`` to av
-00006cd0: 6f69 6420 7375 7270 7269 7365 732e 0a0a  oid surprises...
-00006ce0: 0a54 6162 6c65 206f 6620 636f 6e74 656e  .Table of conten
-00006cf0: 7473 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ts.*************
-00006d00: 2a2a 2a2a 0a0a 2e2e 2074 6f63 7472 6565  ****.... toctree
-00006d10: 3a3a 0a20 2020 203a 6d61 7864 6570 7468  ::.    :maxdepth
-00006d20: 3a20 320a 0a20 2020 2061 7069 5f72 6566  : 2..    api_ref
-00006d30: 6572 656e 6365 0a20 2020 2063 6861 6e67  erence.    chang
-00006d40: 656c 6f67 0a0a 0a0a 2e2e 2068 7970 6572  elog...... hyper
-00006d50: 6c69 6e6b 730a 2e2e 205f 7079 7465 7374  links... _pytest
-00006d60: 5f63 6d64 6c69 6e65 5f6d 6169 6e3a 0a20  _cmdline_main:. 
-00006d70: 2020 2068 7474 7073 3a2f 2f64 6f63 732e     https://docs.
-00006d80: 7079 7465 7374 2e6f 7267 2f65 6e2f 6c61  pytest.org/en/la
-00006d90: 7465 7374 2f5f 6d6f 6475 6c65 732f 5f70  test/_modules/_p
-00006da0: 7974 6573 742f 686f 6f6b 7370 6563 2e68  ytest/hookspec.h
-00006db0: 746d 6c23 7079 7465 7374 5f63 6d64 6c69  tml#pytest_cmdli
-00006dc0: 6e65 5f6d 6169 6e0a 2e2e 205f 686f 6f6b  ne_main... _hook
-00006dd0: 7370 6563 206d 6f64 756c 653a 0a20 2020  spec module:.   
-00006de0: 2068 7474 7073 3a2f 2f64 6f63 732e 7079   https://docs.py
-00006df0: 7465 7374 2e6f 7267 2f65 6e2f 6c61 7465  test.org/en/late
-00006e00: 7374 2f5f 6d6f 6475 6c65 732f 5f70 7974  st/_modules/_pyt
-00006e10: 6573 742f 686f 6f6b 7370 6563 2e68 746d  est/hookspec.htm
-00006e20: 6c0a 2e2e 205f 686f 6f6b 7772 6170 7065  l... _hookwrappe
-00006e30: 723a 0a20 2020 2068 7474 703a 2f2f 646f  r:.    http://do
-00006e40: 632e 7079 7465 7374 2e6f 7267 2f65 6e2f  c.pytest.org/en/
-00006e50: 6c61 7465 7374 2f77 7269 7469 6e67 5f70  latest/writing_p
-00006e60: 6c75 6769 6e73 2e68 746d 6c23 686f 6f6b  lugins.html#hook
-00006e70: 7772 6170 7065 722d 6578 6563 7574 696e  wrapper-executin
-00006e80: 672d 6172 6f75 6e64 2d6f 7468 6572 2d68  g-around-other-h
-00006e90: 6f6f 6b73 0a2e 2e20 5f68 6f6f 6b20 6675  ooks... _hook fu
-00006ea0: 6e63 7469 6f6e 206f 7264 6572 696e 673a  nction ordering:
-00006eb0: 0a20 2020 2068 7474 703a 2f2f 646f 632e  .    http://doc.
-00006ec0: 7079 7465 7374 2e6f 7267 2f65 6e2f 6c61  pytest.org/en/la
-00006ed0: 7465 7374 2f77 7269 7469 6e67 5f70 6c75  test/writing_plu
-00006ee0: 6769 6e73 2e68 746d 6c23 686f 6f6b 2d66  gins.html#hook-f
-00006ef0: 756e 6374 696f 6e2d 6f72 6465 7269 6e67  unction-ordering
-00006f00: 2d63 616c 6c2d 6578 616d 706c 650a 2e2e  -call-example...
-00006f10: 205f 7265 7175 6573 742d 7265 7370 6f6e   _request-respon
-00006f20: 7365 2070 6174 7465 726e 3a0a 2020 2020  se pattern:.    
-00006f30: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00006f40: 6564 6961 2e6f 7267 2f77 696b 692f 5265  edia.org/wiki/Re
-00006f50: 7175 6573 7425 4532 2538 3025 3933 7265  quest%E2%80%93re
-00006f60: 7370 6f6e 7365 0a2e 2e20 5f70 7562 6c69  sponse... _publi
-00006f70: 7368 2d73 7562 7363 7269 6265 3a0a 2020  sh-subscribe:.  
-00006f80: 2020 6874 7470 733a 2f2f 656e 2e77 696b    https://en.wik
-00006f90: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00006fa0: 5075 626c 6973 6825 4532 2538 3025 3933  Publish%E2%80%93
-00006fb0: 7375 6273 6372 6962 655f 7061 7474 6572  subscribe_patter
-00006fc0: 6e0a 2e2e 205f 686f 6f6b 696e 673a 0a20  n... _hooking:. 
-00006fd0: 2020 2068 7474 7073 3a2f 2f65 6e2e 7769     https://en.wi
-00006fe0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00006ff0: 2f48 6f6f 6b69 6e67 0a2e 2e20 5f63 616c  /Hooking... _cal
-00007000: 6c62 6163 6b73 3a0a 2020 2020 6874 7470  lbacks:.    http
-00007010: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-00007020: 2e6f 7267 2f77 696b 692f 4361 6c6c 6261  .org/wiki/Callba
-00007030: 636b 5f28 636f 6d70 7574 6572 5f70 726f  ck_(computer_pro
-00007040: 6772 616d 6d69 6e67 290a 2e2e 205f 746f  gramming)... _to
-00007050: 7820 7465 7374 2073 7569 7465 3a0a 2020  x test suite:.  
-00007060: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
-00007070: 2e63 6f6d 2f70 7974 6573 742d 6465 762f  .com/pytest-dev/
-00007080: 706c 7567 6779 2f62 6c6f 622f 6d61 7374  pluggy/blob/mast
-00007090: 6572 2f74 6f78 2e69 6e69 0a2e 2e20 5f53  er/tox.ini... _S
-000070a0: 656d 616e 7469 6320 5665 7273 696f 6e69  emantic Versioni
-000070b0: 6e67 3a0a 2020 2020 6874 7470 733a 2f2f  ng:.    https://
-000070c0: 7365 6d76 6572 2e6f 7267 2f0a 2e2e 205f  semver.org/... _
-000070d0: 5079 7468 6f6e 2069 6e74 6572 7072 6574  Python interpret
-000070e0: 6572 733a 0a20 2020 2068 7474 7073 3a2f  ers:.    https:/
-000070f0: 2f67 6974 6875 622e 636f 6d2f 7079 7465  /github.com/pyte
-00007100: 7374 2d64 6576 2f70 6c75 6767 792f 626c  st-dev/pluggy/bl
-00007110: 6f62 2f6d 6173 7465 722f 746f 782e 696e  ob/master/tox.in
-00007120: 6923 4c32 0a2e 2e20 5f35 3030 2b20 706c  i#L2... _500+ pl
-00007130: 7567 696e 733a 0a20 2020 2068 7474 703a  ugins:.    http:
-00007140: 2f2f 706c 7567 696e 636f 6d70 6174 2e68  //plugincompat.h
-00007150: 6572 6f6b 7561 7070 2e63 6f6d 2f0a 2e2e  erokuapp.com/...
-00007160: 205f 7072 652d 636f 6d6d 6974 3a0a 2020   _pre-commit:.  
-00007170: 2020 6874 7470 733a 2f2f 7072 652d 636f    https://pre-co
-00007180: 6d6d 6974 2e63 6f6d 2f0a 0a0a 2e2e 2049  mmit.com/..... I
-00007190: 6e64 6963 6573 2061 6e64 2074 6162 6c65  ndices and table
-000071a0: 730a 2e2e 203d 3d3d 3d3d 3d3d 3d3d 3d3d  s... ===========
-000071b0: 3d3d 3d3d 3d3d 3d0a 2e2e 202a 203a 7265  =======... * :re
-000071c0: 663a 6067 656e 696e 6465 7860 0a2e 2e20  f:`genindex`... 
-000071d0: 2a20 3a72 6566 3a60 6d6f 6469 6e64 6578  * :ref:`modindex
-000071e0: 600a 2e2e 202a 203a 7265 663a 6073 6561  `... * :ref:`sea
-000071f0: 7263 6860 0a                             rch`.
+00000460: 686f 772d 746f 2f6d 6f6e 6b65 7970 6174  how-to/monkeypat
+00000470: 6368 3e60 292e 0a54 6865 7365 2073 7472  ch>`)..These str
+00000480: 6174 6567 6965 7320 6265 636f 6d65 2070  ategies become p
+00000490: 726f 626c 656d 6174 6963 2074 686f 7567  roblematic thoug
+000004a0: 6820 7768 656e 2073 6576 6572 616c 2070  h when several p
+000004b0: 6172 7469 6573 2077 616e 7420 746f 0a70  arties want to.p
+000004c0: 6172 7469 6369 7061 7465 2069 6e20 7468  articipate in th
+000004d0: 6520 6d6f 6469 6669 6361 7469 6f6e 206f  e modification o
+000004e0: 6620 7468 6520 7361 6d65 2070 726f 6772  f the same progr
+000004f0: 616d 2e20 5468 6572 6566 6f72 6520 6060  am. Therefore ``
+00000500: 706c 7567 6779 6060 0a64 6f65 7320 6e6f  pluggy``.does no
+00000510: 7420 7265 6c79 206f 6e20 7468 6573 6520  t rely on these 
+00000520: 6d65 6368 616e 6973 6d73 2074 6f20 656e  mechanisms to en
+00000530: 6162 6c65 2061 206d 6f72 6520 7374 7275  able a more stru
+00000540: 6374 7572 6564 2061 7070 726f 6163 6820  ctured approach 
+00000550: 616e 640a 6176 6f69 6420 756e 6e65 6365  and.avoid unnece
+00000560: 7373 6172 7920 6578 706f 7375 7265 206f  ssary exposure o
+00000570: 6620 7374 6174 6520 616e 6420 6265 6861  f state and beha
+00000580: 7669 6f75 722e 2054 6869 7320 6c65 6164  viour. This lead
+00000590: 7320 746f 2061 206d 6f72 650a 606c 6f6f  s to a more.`loo
+000005a0: 7365 6c79 2063 6f75 706c 6564 203c 6874  sely coupled <ht
+000005b0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000005c0: 6961 2e6f 7267 2f77 696b 692f 4c6f 6f73  ia.org/wiki/Loos
+000005d0: 655f 636f 7570 6c69 6e67 3e60 5f20 7265  e_coupling>`_ re
+000005e0: 6c61 7469 6f6e 7368 6970 0a62 6574 7765  lationship.betwe
+000005f0: 656e 2060 6068 6f73 7460 6020 616e 6420  en ``host`` and 
+00000600: 6060 706c 7567 696e 7360 602e 0a0a 5468  ``plugins``...Th
+00000610: 6520 6060 706c 7567 6779 6060 2061 7070  e ``pluggy`` app
+00000620: 726f 6163 6820 7075 7473 2074 6865 2062  roach puts the b
+00000630: 7572 6465 6e20 6f6e 2074 6865 2064 6573  urden on the des
+00000640: 6967 6e65 7220 6f66 2074 6865 0a60 6068  igner of the.``h
+00000650: 6f73 7420 7072 6f67 7261 6d60 6020 746f  ost program`` to
+00000660: 2074 6869 6e6b 2063 6172 6566 756c 6c79   think carefully
+00000670: 2061 626f 7574 2077 6869 6368 206f 626a   about which obj
+00000680: 6563 7473 2061 7265 2072 6561 6c6c 790a  ects are really.
+00000690: 6e65 6564 6564 2069 6e20 6120 686f 6f6b  needed in a hook
+000006a0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2e   implementation.
+000006b0: 2054 6869 7320 6769 7665 7320 6060 706c   This gives ``pl
+000006c0: 7567 696e 6060 2063 7265 6174 6f72 7320  ugin`` creators 
+000006d0: 6120 636c 6561 720a 6672 616d 6577 6f72  a clear.framewor
+000006e0: 6b20 666f 7220 686f 7720 746f 2065 7874  k for how to ext
+000006f0: 656e 6420 7468 6520 6060 686f 7374 6060  end the ``host``
+00000700: 2076 6961 2061 2077 656c 6c20 6465 6669   via a well defi
+00000710: 6e65 6420 7365 7420 6f66 2066 756e 6374  ned set of funct
+00000720: 696f 6e73 0a61 6e64 206f 626a 6563 7473  ions.and objects
+00000730: 2074 6f20 776f 726b 2077 6974 682e 0a0a   to work with...
+00000740: 486f 7720 646f 6573 2069 7420 776f 726b  How does it work
+00000750: 3f0a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ?.**************
+00000760: 2a2a 2a0a 4c65 7420 7573 2073 7461 7274  ***.Let us start
+00000770: 2077 6974 6820 6120 7368 6f72 7420 6f76   with a short ov
+00000780: 6572 7669 6577 206f 6620 7768 6174 2069  erview of what i
+00000790: 7320 696e 766f 6c76 6564 3a0a 0a2a 2060  s involved:..* `
+000007a0: 6068 6f73 7460 6020 6f72 2060 6068 6f73  `host`` or ``hos
+000007b0: 7420 7072 6f67 7261 6d60 603a 2074 6865  t program``: the
+000007c0: 2070 726f 6772 616d 206f 6666 6572 696e   program offerin
+000007d0: 6720 6578 7465 6e73 6962 696c 6974 790a  g extensibility.
+000007e0: 2020 6279 2073 7065 6369 6679 696e 6720    by specifying 
+000007f0: 6060 686f 6f6b 2066 756e 6374 696f 6e73  ``hook functions
+00000800: 6060 2061 6e64 2069 6e76 6f6b 696e 6720  `` and invoking 
+00000810: 7468 6569 7220 696d 706c 656d 656e 7461  their implementa
+00000820: 7469 6f6e 2873 2920 6173 0a20 2070 6172  tion(s) as.  par
+00000830: 7420 6f66 2070 726f 6772 616d 2065 7865  t of program exe
+00000840: 6375 7469 6f6e 0a2a 2060 6070 6c75 6769  cution.* ``plugi
+00000850: 6e60 603a 2074 6865 2070 726f 6772 616d  n``: the program
+00000860: 2069 6d70 6c65 6d65 6e74 696e 6720 2861   implementing (a
+00000870: 2073 7562 7365 7420 6f66 2920 7468 6520   subset of) the 
+00000880: 7370 6563 6966 6965 6420 686f 6f6b 7320  specified hooks 
+00000890: 616e 640a 2020 7061 7274 6963 6970 6174  and.  participat
+000008a0: 696e 6720 696e 2070 726f 6772 616d 2065  ing in program e
+000008b0: 7865 6375 7469 6f6e 2077 6865 6e20 7468  xecution when th
+000008c0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+000008d0: 7320 6172 6520 696e 766f 6b65 640a 2020  s are invoked.  
+000008e0: 6279 2074 6865 2060 6068 6f73 7460 600a  by the ``host``.
+000008f0: 2a20 6060 706c 7567 6779 6060 3a20 636f  * ``pluggy``: co
+00000900: 6e6e 6563 7473 2060 6068 6f73 7460 6020  nnects ``host`` 
+00000910: 616e 6420 6060 706c 7567 696e 7360 6020  and ``plugins`` 
+00000920: 6279 2075 7369 6e67 202e 2e2e 0a0a 2020  by using .....  
+00000930: 2020 2d20 7468 6520 686f 6f6b 203a 7265    - the hook :re
+00000940: 663a 6073 7065 6369 6669 6361 7469 6f6e  f:`specification
+00000950: 7320 3c73 7065 6373 3e60 2064 6566 696e  s <specs>` defin
+00000960: 696e 6720 6361 6c6c 2073 6967 6e61 7475  ing call signatu
+00000970: 7265 730a 2020 2020 2020 7072 6f76 6964  res.      provid
+00000980: 6564 2062 7920 7468 6520 6060 686f 7374  ed by the ``host
+00000990: 6060 2028 612e 6b2e 6120 6060 686f 6f6b  `` (a.k.a ``hook
+000009a0: 7370 6563 7360 6020 2d20 7365 6520 3a72  specs`` - see :r
+000009b0: 6566 3a60 6d61 726b 696e 675f 686f 6f6b  ef:`marking_hook
+000009c0: 7360 290a 2020 2020 2d20 7468 6520 686f  s`).    - the ho
+000009d0: 6f6b 203a 7265 663a 6069 6d70 6c65 6d65  ok :ref:`impleme
+000009e0: 6e74 6174 696f 6e73 203c 696d 706c 733e  ntations <impls>
+000009f0: 6020 7072 6f76 6964 6564 2062 7920 7265  ` provided by re
+00000a00: 6769 7374 6572 6564 0a20 2020 2020 2060  gistered.      `
+00000a10: 6070 6c75 6769 6e73 6060 2028 612e 6b2e  `plugins`` (a.k.
+00000a20: 6120 6060 686f 6f6b 696d 706c 6060 202d  a ``hookimpl`` -
+00000a30: 2073 6565 2060 6361 6c6c 6261 636b 7360   see `callbacks`
+00000a40: 5f29 0a20 2020 202d 2074 6865 2068 6f6f  _).    - the hoo
+00000a50: 6b20 3a72 6566 3a60 6361 6c6c 6572 203c  k :ref:`caller <
+00000a60: 6361 6c6c 696e 673e 6020 2d20 6120 6361  calling>` - a ca
+00000a70: 6c6c 206c 6f6f 7020 7472 6967 6765 7265  ll loop triggere
+00000a80: 6420 6174 2061 7070 726f 7072 6961 7465  d at appropriate
+00000a90: 0a20 2020 2020 2070 726f 6772 616d 2070  .      program p
+00000aa0: 6f73 6974 696f 6e73 2069 6e20 7468 6520  ositions in the 
+00000ab0: 6060 686f 7374 6060 2069 6e76 6f6b 696e  ``host`` invokin
+00000ac0: 6720 7468 6520 696d 706c 656d 656e 7461  g the implementa
+00000ad0: 7469 6f6e 7320 616e 640a 2020 2020 2020  tions and.      
+00000ae0: 636f 6c6c 6563 7469 6e67 2074 6865 2072  collecting the r
+00000af0: 6573 756c 7473 0a0a 2020 2020 2e2e 2e20  esults..    ... 
+00000b00: 7768 6572 6520 666f 7220 6561 6368 2072  where for each r
+00000b10: 6567 6973 7465 7265 6420 686f 6f6b 202a  egistered hook *
+00000b20: 7370 6563 6966 6963 6174 696f 6e2a 2c20  specification*, 
+00000b30: 6120 686f 6f6b 202a 6361 6c6c 2a20 7769  a hook *call* wi
+00000b40: 6c6c 0a20 2020 2069 6e76 6f6b 6520 7570  ll.    invoke up
+00000b50: 2074 6f20 6060 4e60 6020 7265 6769 7374   to ``N`` regist
+00000b60: 6572 6564 2068 6f6f 6b20 2a69 6d70 6c65  ered hook *imple
+00000b70: 6d65 6e74 6174 696f 6e73 2a2e 0a2a 2060  mentations*..* `
+00000b80: 6075 7365 7260 603a 2074 6865 2070 6572  `user``: the per
+00000b90: 736f 6e20 7768 6f20 696e 7374 616c 6c65  son who installe
+00000ba0: 6420 7468 6520 6060 686f 7374 2070 726f  d the ``host pro
+00000bb0: 6772 616d 6060 2061 6e64 2077 616e 7473  gram`` and wants
+00000bc0: 2074 6f0a 2020 6578 7465 6e64 2069 7473   to.  extend its
+00000bd0: 2066 756e 6374 696f 6e61 6c69 7479 2077   functionality w
+00000be0: 6974 6820 6060 706c 7567 696e 7360 602e  ith ``plugins``.
+00000bf0: 2049 6e20 7468 6520 7369 6d70 6c65 7374   In the simplest
+00000c00: 2063 6173 6520 7468 6579 2069 6e73 7461   case they insta
+00000c10: 6c6c 0a20 2074 6865 2060 6070 6c75 6769  ll.  the ``plugi
+00000c20: 6e60 6020 696e 2074 6865 2073 616d 6520  n`` in the same 
+00000c30: 656e 7669 726f 6e6d 656e 7420 6173 2074  environment as t
+00000c40: 6865 2060 6068 6f73 7460 6020 616e 6420  he ``host`` and 
+00000c50: 7468 6520 6d61 6769 6320 7769 6c6c 0a20  the magic will. 
+00000c60: 2068 6170 7065 6e20 7768 656e 2074 6865   happen when the
+00000c70: 2060 6068 6f73 7420 7072 6f67 7261 6d60   ``host program`
+00000c80: 6020 6973 2072 756e 2074 6865 206e 6578  ` is run the nex
+00000c90: 7420 7469 6d65 2e20 4465 7065 6e64 696e  t time. Dependin
+00000ca0: 6720 6f6e 0a20 2074 6865 2060 6070 6c75  g on.  the ``plu
+00000cb0: 6769 6e60 602c 2074 6865 7265 206d 6967  gin``, there mig
+00000cc0: 6874 2062 6520 6f74 6865 7220 7468 696e  ht be other thin
+00000cd0: 6773 2074 6865 7920 6e65 6564 2074 6f20  gs they need to 
+00000ce0: 646f 2e20 466f 7220 6578 616d 706c 652c  do. For example,
+00000cf0: 0a20 2074 6865 7920 6d69 6768 7420 6861  .  they might ha
+00000d00: 7665 2074 6f20 6361 6c6c 2074 6865 2068  ve to call the h
+00000d10: 6f73 7420 7769 7468 2061 6e20 6164 6469  ost with an addi
+00000d20: 7469 6f6e 616c 2063 6f6d 6d61 6e64 6c69  tional commandli
+00000d30: 6e65 2070 6172 616d 6574 6572 0a20 2074  ne parameter.  t
+00000d40: 6f20 7468 6520 686f 7374 2074 6861 7420  o the host that 
+00000d50: 7468 6520 6060 706c 7567 696e 6060 2061  the ``plugin`` a
+00000d60: 6464 6564 2e0a 0a41 2074 6f79 2065 7861  dded...A toy exa
+00000d70: 6d70 6c65 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  mple.-----------
+00000d80: 2d2d 0a4c 6574 2075 7320 6465 6d6f 6e73  --.Let us demons
+00000d90: 7472 6174 6520 7468 6520 636f 7265 2066  trate the core f
+00000da0: 756e 6374 696f 6e61 6c69 7479 2069 6e20  unctionality in 
+00000db0: 6f6e 6520 6d6f 6475 6c65 2061 6e64 2073  one module and s
+00000dc0: 686f 7720 686f 7720 796f 7520 6361 6e0a  how how you can.
+00000dd0: 7374 6172 7420 6578 7065 7269 6d65 6e74  start experiment
+00000de0: 696e 6720 7769 7468 2070 6c75 6767 7920  ing with pluggy 
+00000df0: 6675 6e63 7469 6f6e 616c 6974 792e 0a0a  functionality...
+00000e00: 2e2e 206c 6974 6572 616c 696e 636c 7564  .. literalinclud
+00000e10: 653a 3a20 6578 616d 706c 6573 2f74 6f79  e:: examples/toy
+00000e20: 2d65 7861 6d70 6c65 2e70 790a 0a52 756e  -example.py..Run
+00000e30: 6e69 6e67 2074 6869 7320 6469 7265 6374  ning this direct
+00000e40: 6c79 2067 6574 7320 7573 3a3a 0a0a 2020  ly gets us::..  
+00000e50: 2020 2420 7079 7468 6f6e 2064 6f63 732f    $ python docs/
+00000e60: 6578 616d 706c 6573 2f74 6f79 2d65 7861  examples/toy-exa
+00000e70: 6d70 6c65 2e70 790a 0a20 2020 2069 6e73  mple.py..    ins
+00000e80: 6964 6520 506c 7567 696e 5f32 2e6d 7968  ide Plugin_2.myh
+00000e90: 6f6f 6b28 290a 2020 2020 696e 7369 6465  ook().    inside
+00000ea0: 2050 6c75 6769 6e5f 312e 6d79 686f 6f6b   Plugin_1.myhook
+00000eb0: 2829 0a20 2020 205b 2d31 2c20 335d 0a0a  ().    [-1, 3]..
+00000ec0: 4120 636f 6d70 6c65 7465 2065 7861 6d70  A complete examp
+00000ed0: 6c65 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  le.-------------
+00000ee0: 2d2d 2d2d 2d0a 4e6f 7720 6c65 7420 7573  -----.Now let us
+00000ef0: 2064 656d 6f6e 7374 7261 7465 2068 6f77   demonstrate how
+00000f00: 2074 6869 7320 706c 6179 7320 746f 6765   this plays toge
+00000f10: 7468 6572 2069 6e20 6120 7661 6775 656c  ther in a vaguel
+00000f20: 7920 7265 616c 2077 6f72 6c64 2073 6365  y real world sce
+00000f30: 6e61 7269 6f2e 0a0a 4c65 7427 7320 6173  nario...Let's as
+00000f40: 7375 6d65 206f 7572 2060 6068 6f73 7420  sume our ``host 
+00000f50: 7072 6f67 7261 6d60 6020 6973 2063 616c  program`` is cal
+00000f60: 6c65 6420 2a2a 6567 6773 616d 706c 652a  led **eggsample*
+00000f70: 2a20 7768 6572 6520 736f 6d65 2065 6767  * where some egg
+00000f80: 7320 7769 6c6c 0a62 6520 7072 6570 6172  s will.be prepar
+00000f90: 6564 2061 6e64 2073 6572 7665 6420 7769  ed and served wi
+00000fa0: 7468 2061 2074 7261 7920 636f 6e74 6169  th a tray contai
+00000fb0: 6e69 6e67 2063 6f6e 6469 6d65 6e74 732e  ning condiments.
+00000fc0: 2041 7320 6576 6572 7962 6f64 7920 6b6e   As everybody kn
+00000fd0: 6f77 733a 0a74 6865 206d 6f72 6520 636f  ows:.the more co
+00000fe0: 6f6b 7320 6172 6520 696e 766f 6c76 6564  oks are involved
+00000ff0: 2074 6865 2062 6574 7465 7220 7468 6520   the better the 
+00001000: 666f 6f64 2c20 736f 206c 6574 2075 7320  food, so let us 
+00001010: 6d61 6b65 2074 6865 2070 726f 6365 7373  make the process
+00001020: 0a70 6c75 6767 6162 6c65 2061 6e64 2077  .pluggable and w
+00001030: 7269 7465 2061 2070 6c75 6769 6e20 7468  rite a plugin th
+00001040: 6174 2069 6d70 726f 7665 7320 7468 6520  at improves the 
+00001050: 6d65 616c 2077 6974 6820 736f 6d65 2073  meal with some s
+00001060: 7061 6d20 616e 6420 7265 706c 6163 6573  pam and replaces
+00001070: 0a74 6865 2073 7465 616b 2073 6175 6365  .the steak sauce
+00001080: 2028 6e6f 626f 6479 206c 696b 6573 2074   (nobody likes t
+00001090: 6861 7420 616e 7977 6179 2920 7769 7468  hat anyway) with
+000010a0: 2073 7061 6d20 7361 7563 6520 2869 7427   spam sauce (it'
+000010b0: 7320 6120 7468 696e 6720 2d20 7472 7573  s a thing - trus
+000010c0: 7420 6d65 292e 0a0a 2e2e 206e 6f74 653a  t me)..... note:
+000010d0: 3a0a 0a20 2020 202a 2a6e 616d 696e 6720  :..    **naming 
+000010e0: 6d61 726b 6572 732a 2a3a 2060 6048 6f6f  markers**: ``Hoo
+000010f0: 6b53 7065 634d 6172 6b65 7260 6020 616e  kSpecMarker`` an
+00001100: 6420 6060 486f 6f6b 496d 706c 4d61 726b  d ``HookImplMark
+00001110: 6572 6060 206d 7573 7420 6265 0a20 2020  er`` must be.   
+00001120: 2069 6e69 7469 616c 697a 6564 2077 6974   initialized wit
+00001130: 6820 7468 6520 6e61 6d65 206f 6620 7468  h the name of th
+00001140: 6520 6060 686f 7374 6060 2070 726f 6a65  e ``host`` proje
+00001150: 6374 2028 7468 6520 6060 6e61 6d65 6060  ct (the ``name``
+00001160: 0a20 2020 2070 6172 616d 6574 6572 2069  .    parameter i
+00001170: 6e20 6060 7365 7475 7028 2960 6029 202d  n ``setup()``) -
+00001180: 2073 6f20 2a2a 6567 6773 616d 706c 652a   so **eggsample*
+00001190: 2a20 696e 206f 7572 2063 6173 652e 0a0a  * in our case...
+000011a0: 2020 2020 2a2a 6e61 6d69 6e67 2070 6c75      **naming plu
+000011b0: 6769 6e20 7072 6f6a 6563 7473 2a2a 3a20  gin projects**: 
+000011c0: 7468 6579 2073 686f 756c 6420 6265 206e  they should be n
+000011d0: 616d 6564 2069 6e20 7468 6520 666f 726d  amed in the form
+000011e0: 206f 660a 2020 2020 6060 3c68 6f73 743e   of.    ``<host>
+000011f0: 2d3c 706c 7567 696e 3e60 6020 2865 2e67  -<plugin>`` (e.g
+00001200: 2e20 6060 7079 7465 7374 2d78 6469 7374  . ``pytest-xdist
+00001210: 6060 292c 2074 6865 7265 666f 7265 2077  ``), therefore w
+00001220: 6520 6361 6c6c 206f 7572 0a20 2020 2070  e call our.    p
+00001230: 6c75 6769 6e20 2a65 6767 7361 6d70 6c65  lugin *eggsample
+00001240: 2d73 7061 6d2a 2e0a 0a54 6865 2068 6f73  -spam*...The hos
+00001250: 740a 5e5e 5e5e 5e5e 5e5e 0a60 6065 6767  t.^^^^^^^^.``egg
+00001260: 7361 6d70 6c65 2f65 6767 7361 6d70 6c65  sample/eggsample
+00001270: 2f5f 5f69 6e69 745f 5f2e 7079 6060 0a0a  /__init__.py``..
+00001280: 2e2e 206c 6974 6572 616c 696e 636c 7564  .. literalinclud
+00001290: 653a 3a20 6578 616d 706c 6573 2f65 6767  e:: examples/egg
+000012a0: 7361 6d70 6c65 2f65 6767 7361 6d70 6c65  sample/eggsample
+000012b0: 2f5f 5f69 6e69 745f 5f2e 7079 0a0a 6060  /__init__.py..``
+000012c0: 6567 6773 616d 706c 652f 6567 6773 616d  eggsample/eggsam
+000012d0: 706c 652f 686f 6f6b 7370 6563 732e 7079  ple/hookspecs.py
+000012e0: 6060 0a0a 2e2e 206c 6974 6572 616c 696e  ``.... literalin
+000012f0: 636c 7564 653a 3a20 6578 616d 706c 6573  clude:: examples
+00001300: 2f65 6767 7361 6d70 6c65 2f65 6767 7361  /eggsample/eggsa
+00001310: 6d70 6c65 2f68 6f6f 6b73 7065 6373 2e70  mple/hookspecs.p
+00001320: 790a 0a60 6065 6767 7361 6d70 6c65 2f65  y..``eggsample/e
+00001330: 6767 7361 6d70 6c65 2f6c 6962 2e70 7960  ggsample/lib.py`
+00001340: 600a 0a2e 2e20 6c69 7465 7261 6c69 6e63  `.... literalinc
+00001350: 6c75 6465 3a3a 2065 7861 6d70 6c65 732f  lude:: examples/
+00001360: 6567 6773 616d 706c 652f 6567 6773 616d  eggsample/eggsam
+00001370: 706c 652f 6c69 622e 7079 0a0a 6060 6567  ple/lib.py..``eg
+00001380: 6773 616d 706c 652f 6567 6773 616d 706c  gsample/eggsampl
+00001390: 652f 686f 7374 2e70 7960 600a 0a2e 2e20  e/host.py``.... 
+000013a0: 6c69 7465 7261 6c69 6e63 6c75 6465 3a3a  literalinclude::
+000013b0: 2065 7861 6d70 6c65 732f 6567 6773 616d   examples/eggsam
+000013c0: 706c 652f 6567 6773 616d 706c 652f 686f  ple/eggsample/ho
+000013d0: 7374 2e70 790a 0a60 6065 6767 7361 6d70  st.py..``eggsamp
+000013e0: 6c65 2f73 6574 7570 2e70 7960 600a 0a2e  le/setup.py``...
+000013f0: 2e20 6c69 7465 7261 6c69 6e63 6c75 6465  . literalinclude
+00001400: 3a3a 2065 7861 6d70 6c65 732f 6567 6773  :: examples/eggs
+00001410: 616d 706c 652f 7365 7475 702e 7079 0a0a  ample/setup.py..
+00001420: 4c65 7427 7320 6765 7420 636f 6f6b 696e  Let's get cookin
+00001430: 6720 2d20 7765 2069 6e73 7461 6c6c 2074  g - we install t
+00001440: 6865 2068 6f73 7420 616e 6420 7365 6520  he host and see 
+00001450: 7768 6174 2061 2070 726f 6772 616d 2072  what a program r
+00001460: 756e 206c 6f6f 6b73 206c 696b 653a 3a0a  un looks like::.
+00001470: 0a20 2020 2024 2070 6970 2069 6e73 7461  .    $ pip insta
+00001480: 6c6c 202d 2d65 6469 7461 626c 6520 706c  ll --editable pl
+00001490: 7567 6779 2f64 6f63 732f 6578 616d 706c  uggy/docs/exampl
+000014a0: 6573 2f65 6767 7361 6d70 6c65 0a20 2020  es/eggsample.   
+000014b0: 2024 2065 6767 7361 6d70 6c65 0a0a 2020   $ eggsample..  
+000014c0: 2020 596f 7572 2066 6f6f 642e 2045 6e6a    Your food. Enj
+000014d0: 6f79 2073 6f6d 6520 6567 672c 2065 6767  oy some egg, egg
+000014e0: 2c20 7361 6c74 2c20 6567 672c 2065 6767  , salt, egg, egg
+000014f0: 2c20 7065 7070 6572 2c20 6567 670a 2020  , pepper, egg.  
+00001500: 2020 536f 6d65 2063 6f6e 6469 6d65 6e74    Some condiment
+00001510: 733f 2057 6520 6861 7665 2070 6963 6b6c  s? We have pickl
+00001520: 6564 2077 616c 6e75 7473 2c20 7374 6561  ed walnuts, stea
+00001530: 6b20 7361 7563 652c 206d 7573 6879 2070  k sauce, mushy p
+00001540: 6561 732c 206d 696e 7420 7361 7563 650a  eas, mint sauce.
+00001550: 0a54 6865 2070 6c75 6769 6e0a 5e5e 5e5e  .The plugin.^^^^
+00001560: 5e5e 5e5e 5e5e 0a60 6065 6767 7361 6d70  ^^^^^^.``eggsamp
+00001570: 6c65 2d73 7061 6d2f 6567 6773 616d 706c  le-spam/eggsampl
+00001580: 655f 7370 616d 2e70 7960 600a 0a2e 2e20  e_spam.py``.... 
+00001590: 6c69 7465 7261 6c69 6e63 6c75 6465 3a3a  literalinclude::
+000015a0: 2065 7861 6d70 6c65 732f 6567 6773 616d   examples/eggsam
+000015b0: 706c 652d 7370 616d 2f65 6767 7361 6d70  ple-spam/eggsamp
+000015c0: 6c65 5f73 7061 6d2e 7079 0a0a 6060 6567  le_spam.py..``eg
+000015d0: 6773 616d 706c 652d 7370 616d 2f73 6574  gsample-spam/set
+000015e0: 7570 2e70 7960 600a 0a2e 2e20 6c69 7465  up.py``.... lite
+000015f0: 7261 6c69 6e63 6c75 6465 3a3a 2065 7861  ralinclude:: exa
+00001600: 6d70 6c65 732f 6567 6773 616d 706c 652d  mples/eggsample-
+00001610: 7370 616d 2f73 6574 7570 2e70 790a 0a4c  spam/setup.py..L
+00001620: 6574 2773 2067 6574 2063 6f6f 6b69 6e67  et's get cooking
+00001630: 2077 6974 6820 6d6f 7265 2063 6f6f 6b73   with more cooks
+00001640: 202d 2077 6520 696e 7374 616c 6c20 7468   - we install th
+00001650: 6520 706c 7567 696e 2061 6e64 2061 6e64  e plugin and and
+00001660: 2073 6565 2077 6861 740a 7765 2067 6574   see what.we get
+00001670: 3a3a 0a0a 2020 2020 2420 7069 7020 696e  ::..    $ pip in
+00001680: 7374 616c 6c20 2d2d 6564 6974 6162 6c65  stall --editable
+00001690: 2070 6c75 6767 792f 646f 6373 2f65 7861   pluggy/docs/exa
+000016a0: 6d70 6c65 732f 6567 6773 616d 706c 652d  mples/eggsample-
+000016b0: 7370 616d 0a20 2020 2024 2065 6767 7361  spam.    $ eggsa
+000016c0: 6d70 6c65 0a0a 2020 2020 596f 7572 2066  mple..    Your f
+000016d0: 6f6f 642e 2045 6e6a 6f79 2073 6f6d 6520  ood. Enjoy some 
+000016e0: 6567 672c 206c 6f76 656c 7920 7370 616d  egg, lovely spam
+000016f0: 2c20 7361 6c74 2c20 6567 672c 2065 6767  , salt, egg, egg
+00001700: 2c20 6567 672c 2077 6f6e 6465 726f 7573  , egg, wonderous
+00001710: 2073 7061 6d2c 2065 6767 2c20 7065 7070   spam, egg, pepp
+00001720: 6572 0a20 2020 2053 6f6d 6520 636f 6e64  er.    Some cond
+00001730: 696d 656e 7473 3f20 5765 2068 6176 6520  iments? We have 
+00001740: 7069 636b 6c65 6420 7761 6c6e 7574 732c  pickled walnuts,
+00001750: 206d 7573 6879 2070 6561 732c 206d 696e   mushy peas, min
+00001760: 7420 7361 7563 652c 2073 7061 6d20 7361  t sauce, spam sa
+00001770: 7563 650a 2020 2020 4e6f 7720 7468 6973  uce.    Now this
+00001780: 2069 7320 7768 6174 2049 2063 616c 6c20   is what I call 
+00001790: 6120 636f 6e64 696d 656e 7473 2074 7261  a condiments tra
+000017a0: 7921 0a0a 4d6f 7265 2072 6561 6c20 776f  y!..More real wo
+000017b0: 726c 6420 6578 616d 706c 6573 0a2d 2d2d  rld examples.---
+000017c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017d0: 2d2d 2d2d 2d0a 546f 2073 6565 2068 6f77  -----.To see how
+000017e0: 2060 6070 6c75 6767 7960 6020 6973 2075   ``pluggy`` is u
+000017f0: 7365 6420 696e 2074 6865 2072 6561 6c20  sed in the real 
+00001800: 776f 726c 642c 2068 6176 6520 6120 6c6f  world, have a lo
+00001810: 6f6b 2061 7420 7468 6573 6520 7072 6f6a  ok at these proj
+00001820: 6563 7473 0a64 6f63 756d 656e 7461 7469  ects.documentati
+00001830: 6f6e 2061 6e64 2073 6f75 7263 6520 636f  on and source co
+00001840: 6465 3a0a 0a2a 203a 7265 663a 6070 7974  de:..* :ref:`pyt
+00001850: 6573 7420 3c70 7974 6573 743a 7772 6974  est <pytest:writ
+00001860: 696e 672d 706c 7567 696e 733e 600a 2a20  ing-plugins>`.* 
+00001870: 3a73 7464 3a64 6f63 3a60 746f 7820 3c74  :std:doc:`tox <t
+00001880: 6f78 3a70 6c75 6769 6e73 3e60 0a2a 203a  ox:plugins>`.* :
+00001890: 7374 643a 646f 633a 6064 6576 7069 203c  std:doc:`devpi <
+000018a0: 6465 7670 693a 6465 7667 7569 6465 2f69  devpi:devguide/i
+000018b0: 6e64 6578 3e60 0a2a 203a 7374 643a 646f  ndex>`.* :std:do
+000018c0: 633a 606b 6564 726f 203c 6b65 6472 6f3a  c:`kedro <kedro:
+000018d0: 6b65 6472 6f2e 6672 616d 6577 6f72 6b2e  kedro.framework.
+000018e0: 686f 6f6b 732e 7370 6563 733e 600a 0a46  hooks.specs>`..F
+000018f0: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
+00001900: 616e 6420 6164 7661 6e63 6564 2075 7361  and advanced usa
+00001910: 6765 2070 6c65 6173 6520 7265 6164 206f  ge please read o
+00001920: 6e2e 0a0a 2e2e 205f 6465 6669 6e65 3a0a  n..... _define:.
+00001930: 0a44 6566 696e 6520 616e 6420 636f 6c6c  .Define and coll
+00001940: 6563 7420 686f 6f6b 730a 2a2a 2a2a 2a2a  ect hooks.******
+00001950: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00001960: 2a2a 0a41 202a 706c 7567 696e 2a20 6973  **.A *plugin* is
+00001970: 2061 203a 7265 663a 606e 616d 6573 7061   a :ref:`namespa
+00001980: 6365 203c 7079 7468 6f6e 3a74 7574 2d73  ce <python:tut-s
+00001990: 636f 7065 733e 6020 7479 7065 2028 6375  copes>` type (cu
+000019a0: 7272 656e 746c 7920 6f6e 6520 6f66 2061  rrently one of a
+000019b0: 0a60 6063 6c61 7373 6060 206f 7220 6d6f  .``class`` or mo
+000019c0: 6475 6c65 2920 7768 6963 6820 6465 6669  dule) which defi
+000019d0: 6e65 7320 6120 7365 7420 6f66 202a 686f  nes a set of *ho
+000019e0: 6f6b 2a20 6675 6e63 7469 6f6e 732e 0a0a  ok* functions...
+000019f0: 4173 206d 656e 7469 6f6e 6564 2069 6e20  As mentioned in 
+00001a00: 3a72 6566 3a60 6d61 6e61 6765 602c 2061  :ref:`manage`, a
+00001a10: 6c6c 202a 706c 7567 696e 732a 2077 6869  ll *plugins* whi
+00001a20: 6368 2073 7065 6369 6679 202a 686f 6f6b  ch specify *hook
+00001a30: 732a 0a61 7265 206d 616e 6167 6564 2062  s*.are managed b
+00001a40: 7920 616e 2069 6e73 7461 6e63 6520 6f66  y an instance of
+00001a50: 2061 203a 7079 3a63 6c61 7373 3a60 706c   a :py:class:`pl
+00001a60: 7567 6779 2e50 6c75 6769 6e4d 616e 6167  uggy.PluginManag
+00001a70: 6572 6020 7768 6963 680a 6465 6669 6e65  er` which.define
+00001a80: 7320 7468 6520 7072 696d 6172 7920 6060  s the primary ``
+00001a90: 706c 7567 6779 6060 2041 5049 2e0a 0a49  pluggy`` API...I
+00001aa0: 6e20 6f72 6465 7220 666f 7220 6120 3a70  n order for a :p
+00001ab0: 793a 636c 6173 733a 607e 706c 7567 6779  y:class:`~pluggy
+00001ac0: 2e50 6c75 6769 6e4d 616e 6167 6572 6020  .PluginManager` 
+00001ad0: 746f 2064 6574 6563 7420 6675 6e63 7469  to detect functi
+00001ae0: 6f6e 7320 696e 2061 206e 616d 6573 7061  ons in a namespa
+00001af0: 6365 0a69 6e74 656e 6465 6420 746f 2062  ce.intended to b
+00001b00: 6520 2a68 6f6f 6b73 2a2c 2074 6865 7920  e *hooks*, they 
+00001b10: 6d75 7374 2062 6520 6465 636f 7261 7465  must be decorate
+00001b20: 6420 7573 696e 6720 7370 6563 6961 6c20  d using special 
+00001b30: 6060 706c 7567 6779 6060 202a 6d61 726b  ``pluggy`` *mark
+00001b40: 732a 2e0a 0a2e 2e20 5f6d 6172 6b69 6e67  s*..... _marking
+00001b50: 5f68 6f6f 6b73 3a0a 0a4d 6172 6b69 6e67  _hooks:..Marking
+00001b60: 2068 6f6f 6b73 0a2d 2d2d 2d2d 2d2d 2d2d   hooks.---------
+00001b70: 2d2d 2d2d 0a54 6865 203a 7079 3a63 6c61  ----.The :py:cla
+00001b80: 7373 3a60 7e70 6c75 6767 792e 486f 6f6b  ss:`~pluggy.Hook
+00001b90: 7370 6563 4d61 726b 6572 6020 616e 6420  specMarker` and 
+00001ba0: 3a70 793a 636c 6173 733a 607e 706c 7567  :py:class:`~plug
+00001bb0: 6779 2e48 6f6f 6b69 6d70 6c4d 6172 6b65  gy.HookimplMarke
+00001bc0: 7260 0a64 6563 6f72 6174 6f72 7320 6172  r`.decorators ar
+00001bd0: 6520 7573 6564 2074 6f20 2a6d 6172 6b2a  e used to *mark*
+00001be0: 2066 756e 6374 696f 6e73 2066 6f72 2064   functions for d
+00001bf0: 6574 6563 7469 6f6e 2062 7920 610a 3a70  etection by a.:p
+00001c00: 793a 636c 6173 733a 607e 706c 7567 6779  y:class:`~pluggy
+00001c10: 2e50 6c75 6769 6e4d 616e 6167 6572 603a  .PluginManager`:
+00001c20: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+00001c30: 3a20 7079 7468 6f6e 0a0a 2020 2020 6672  : python..    fr
+00001c40: 6f6d 2070 6c75 6767 7920 696d 706f 7274  om pluggy import
+00001c50: 2048 6f6f 6b73 7065 634d 6172 6b65 722c   HookspecMarker,
+00001c60: 2048 6f6f 6b69 6d70 6c4d 6172 6b65 720a   HookimplMarker.
+00001c70: 0a20 2020 2068 6f6f 6b73 7065 6320 3d20  .    hookspec = 
+00001c80: 486f 6f6b 7370 6563 4d61 726b 6572 2822  HookspecMarker("
+00001c90: 7072 6f6a 6563 745f 6e61 6d65 2229 0a20  project_name"). 
+00001ca0: 2020 2068 6f6f 6b69 6d70 6c20 3d20 486f     hookimpl = Ho
+00001cb0: 6f6b 696d 706c 4d61 726b 6572 2822 7072  okimplMarker("pr
+00001cc0: 6f6a 6563 745f 6e61 6d65 2229 0a0a 0a45  oject_name")...E
+00001cd0: 6163 6820 6465 636f 7261 746f 7220 7479  ach decorator ty
+00001ce0: 7065 2074 616b 6573 2061 2073 696e 676c  pe takes a singl
+00001cf0: 6520 6060 7072 6f6a 6563 745f 6e61 6d65  e ``project_name
+00001d00: 6060 2073 7472 696e 6720 6173 2069 7473  `` string as its
+00001d10: 0a6c 6f6e 6520 6172 6775 6d65 6e74 2074  .lone argument t
+00001d20: 6865 2076 616c 7565 206f 6620 7768 6963  he value of whic
+00001d30: 6820 6973 2075 7365 6420 746f 206d 6172  h is used to mar
+00001d40: 6b20 686f 6f6b 7320 666f 7220 6465 7465  k hooks for dete
+00001d50: 6374 696f 6e20 6279 0a61 2073 696d 696c  ction by.a simil
+00001d60: 6172 6c79 2063 6f6e 6669 6775 7265 6420  arly configured 
+00001d70: 3a70 793a 636c 6173 733a 607e 706c 7567  :py:class:`~plug
+00001d80: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
+00001d90: 6020 696e 7374 616e 6365 2e0a 0a54 6861  ` instance...Tha
+00001da0: 7420 6973 2c20 6120 2a6d 6172 6b2a 2074  t is, a *mark* t
+00001db0: 7970 6520 6361 6c6c 6564 2077 6974 6820  ype called with 
+00001dc0: 6060 7072 6f6a 6563 745f 6e61 6d65 6060  ``project_name``
+00001dd0: 2072 6574 7572 6e73 2061 6e20 6f62 6a65   returns an obje
+00001de0: 6374 2077 6869 6368 0a63 616e 2062 6520  ct which.can be 
+00001df0: 7573 6564 2074 6f20 6465 636f 7261 7465  used to decorate
+00001e00: 2066 756e 6374 696f 6e73 2077 6869 6368   functions which
+00001e10: 2077 696c 6c20 7468 656e 2062 6520 6465   will then be de
+00001e20: 7465 6374 6564 2062 7920 610a 3a70 793a  tected by a.:py:
+00001e30: 636c 6173 733a 607e 706c 7567 6779 2e50  class:`~pluggy.P
+00001e40: 6c75 6769 6e4d 616e 6167 6572 6020 7768  luginManager` wh
+00001e50: 6963 6820 7761 7320 696e 7374 616e 7469  ich was instanti
+00001e60: 6174 6564 2077 6974 6820 7468 6520 7361  ated with the sa
+00001e70: 6d65 0a60 6070 726f 6a65 6374 5f6e 616d  me.``project_nam
+00001e80: 6560 6020 7661 6c75 652e 0a0a 4675 7274  e`` value...Furt
+00001e90: 6865 726d 6f72 652c 2065 6163 6820 2a68  hermore, each *h
+00001ea0: 6f6f 6b69 6d70 6c2a 206f 7220 2a68 6f6f  ookimpl* or *hoo
+00001eb0: 6b73 7065 632a 2064 6563 6f72 6174 6f72  kspec* decorator
+00001ec0: 2063 616e 2063 6f6e 6669 6775 7265 2074   can configure t
+00001ed0: 6865 0a75 6e64 6572 6c79 696e 6720 6361  he.underlying ca
+00001ee0: 6c6c 2d74 696d 6520 6265 6861 7669 6f72  ll-time behavior
+00001ef0: 206f 6620 6561 6368 202a 686f 6f6b 2a20   of each *hook* 
+00001f00: 6f62 6a65 6374 2062 7920 7072 6f76 6964  object by provid
+00001f10: 696e 6720 7370 6563 6961 6c0a 2a6f 7074  ing special.*opt
+00001f20: 696f 6e73 2a20 7061 7373 6564 2061 7320  ions* passed as 
+00001f30: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00001f40: 732e 0a0a 0a2e 2e20 6e6f 7465 3a3a 0a20  s...... note::. 
+00001f50: 2020 2054 6865 2066 6f6c 6c6f 7769 6e67     The following
+00001f60: 2073 6563 7469 6f6e 7320 636f 7272 6573   sections corres
+00001f70: 706f 6e64 2074 6f20 7369 6d69 6c61 7220  pond to similar 
+00001f80: 646f 6375 6d65 6e74 6174 696f 6e20 696e  documentation in
+00001f90: 0a20 2020 2060 6070 7974 6573 7460 6020  .    ``pytest`` 
+00001fa0: 666f 7220 3a72 6566 3a60 7079 7465 7374  for :ref:`pytest
+00001fb0: 3a77 7269 7469 6e67 686f 6f6b 7360 2061  :writinghooks` a
+00001fc0: 6e64 2063 616e 2062 6520 7573 6564 2061  nd can be used a
+00001fd0: 730a 2020 2020 6120 7375 7070 6c65 6d65  s.    a suppleme
+00001fe0: 6e74 6172 7920 7265 736f 7572 6365 2e0a  ntary resource..
+00001ff0: 0a2e 2e20 5f69 6d70 6c73 3a0a 0a49 6d70  ... _impls:..Imp
+00002000: 6c65 6d65 6e74 6174 696f 6e73 0a2d 2d2d  lementations.---
+00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a41 2068  ------------.A h
+00002020: 6f6f 6b20 2a69 6d70 6c65 6d65 6e74 6174  ook *implementat
+00002030: 696f 6e2a 2028 2a68 6f6f 6b69 6d70 6c2a  ion* (*hookimpl*
+00002040: 2920 6973 206a 7573 7420 6120 2863 616c  ) is just a (cal
+00002050: 6c62 6163 6b29 2066 756e 6374 696f 6e0a  lback) function.
+00002060: 7768 6963 6820 6861 7320 6265 656e 2061  which has been a
+00002070: 7070 726f 7072 6961 7465 6c79 206d 6172  ppropriately mar
+00002080: 6b65 642e 0a0a 2a68 6f6f 6b69 6d70 6c73  ked...*hookimpls
+00002090: 2a20 6172 6520 6c6f 6164 6564 2066 726f  * are loaded fro
+000020a0: 6d20 6120 706c 7567 696e 2075 7369 6e67  m a plugin using
+000020b0: 2074 6865 0a3a 7079 3a6d 6574 683a 607e   the.:py:meth:`~
+000020c0: 706c 7567 6779 2e50 6c75 6769 6e4d 616e  pluggy.PluginMan
+000020d0: 6167 6572 2e72 6567 6973 7465 7228 2960  ager.register()`
+000020e0: 206d 6574 686f 643a 0a0a 2a68 6f6f 6b69   method:..*hooki
+000020f0: 6d70 6c73 2a20 6d75 7374 2062 6520 6861  mpls* must be ha
+00002100: 7368 6162 6c65 2e0a 0a2e 2e20 636f 6465  shable..... code
+00002110: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00002120: 0a20 2020 2069 6d70 6f72 7420 7379 730a  .    import sys.
+00002130: 2020 2020 6672 6f6d 2070 6c75 6767 7920      from pluggy 
+00002140: 696d 706f 7274 2050 6c75 6769 6e4d 616e  import PluginMan
+00002150: 6167 6572 2c20 486f 6f6b 696d 706c 4d61  ager, HookimplMa
+00002160: 726b 6572 0a0a 2020 2020 686f 6f6b 696d  rker..    hookim
+00002170: 706c 203d 2048 6f6f 6b69 6d70 6c4d 6172  pl = HookimplMar
+00002180: 6b65 7228 226d 7970 726f 6a65 6374 2229  ker("myproject")
+00002190: 0a0a 0a20 2020 2040 686f 6f6b 696d 706c  ...    @hookimpl
+000021a0: 0a20 2020 2064 6566 2073 6574 7570 5f70  .    def setup_p
+000021b0: 726f 6a65 6374 2863 6f6e 6669 672c 2061  roject(config, a
+000021c0: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
+000021d0: 2254 6869 7320 686f 6f6b 2069 7320 7573  "This hook is us
+000021e0: 6564 2074 6f20 7072 6f63 6573 7320 7468  ed to process th
+000021f0: 6520 696e 6974 6961 6c20 636f 6e66 6967  e initial config
+00002200: 0a20 2020 2020 2020 2061 6e64 2070 6f73  .        and pos
+00002210: 7369 626c 7920 696e 7075 7420 6172 6775  sibly input argu
+00002220: 6d65 6e74 732e 0a20 2020 2020 2020 2022  ments..        "
+00002230: 2222 0a20 2020 2020 2020 2069 6620 6172  "".        if ar
+00002240: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00002250: 636f 6e66 6967 2e70 726f 6365 7373 5f61  config.process_a
+00002260: 7267 7328 6172 6773 290a 0a20 2020 2020  rgs(args)..     
+00002270: 2020 2072 6574 7572 6e20 636f 6e66 6967     return config
+00002280: 0a0a 0a20 2020 2070 6d20 3d20 506c 7567  ...    pm = Plug
+00002290: 696e 4d61 6e61 6765 7228 226d 7970 726f  inManager("mypro
+000022a0: 6a65 6374 2229 0a0a 2020 2020 2320 6c6f  ject")..    # lo
+000022b0: 6164 2061 6c6c 2068 6f6f 6b69 6d70 6c73  ad all hookimpls
+000022c0: 2066 726f 6d20 7468 6520 6c6f 6361 6c20   from the local 
+000022d0: 6d6f 6475 6c65 2773 206e 616d 6573 7061  module's namespa
+000022e0: 6365 0a20 2020 2070 6c75 6769 6e5f 6e61  ce.    plugin_na
+000022f0: 6d65 203d 2070 6d2e 7265 6769 7374 6572  me = pm.register
+00002300: 2873 7973 2e6d 6f64 756c 6573 5b5f 5f6e  (sys.modules[__n
+00002310: 616d 655f 5f5d 290a 0a2e 2e20 5f6f 7074  ame__]).... _opt
+00002320: 696f 6e61 6c68 6f6f 6b3a 0a0a 4f70 7469  ionalhook:..Opti
+00002330: 6f6e 616c 2076 616c 6964 6174 696f 6e0a  onal validation.
+00002340: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+00002350: 5e5e 5e0a 4e6f 726d 616c 6c79 2065 6163  ^^^.Normally eac
+00002360: 6820 2a68 6f6f 6b69 6d70 6c2a 2073 686f  h *hookimpl* sho
+00002370: 756c 6420 6265 2076 616c 6964 6174 6564  uld be validated
+00002380: 2061 6761 696e 7374 2061 2063 6f72 7265   against a corre
+00002390: 7370 6f6e 6469 6e67 0a68 6f6f 6b20 3a72  sponding.hook :r
+000023a0: 6566 3a60 7370 6563 6966 6963 6174 696f  ef:`specificatio
+000023b0: 6e20 3c73 7065 6373 3e60 2e20 4966 2079  n <specs>`. If y
+000023c0: 6f75 2077 616e 7420 746f 206d 616b 6520  ou want to make 
+000023d0: 616e 2065 7863 6570 7469 6f6e 0a74 6865  an exception.the
+000023e0: 6e20 7468 6520 2a68 6f6f 6b69 6d70 6c2a  n the *hookimpl*
+000023f0: 2073 686f 756c 6420 6265 206d 6172 6b65   should be marke
+00002400: 6420 7769 7468 2074 6865 2060 6022 6f70  d with the ``"op
+00002410: 7469 6f6e 616c 686f 6f6b 2260 6020 6f70  tionalhook"`` op
+00002420: 7469 6f6e 3a0a 0a2e 2e20 636f 6465 2d62  tion:.... code-b
+00002430: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+00002440: 2020 2040 686f 6f6b 696d 706c 286f 7074     @hookimpl(opt
+00002450: 696f 6e61 6c68 6f6f 6b3d 5472 7565 290a  ionalhook=True).
+00002460: 2020 2020 6465 6620 7365 7475 705f 7072      def setup_pr
+00002470: 6f6a 6563 7428 636f 6e66 6967 2c20 6172  oject(config, ar
+00002480: 6773 293a 0a20 2020 2020 2020 2022 2222  gs):.        """
+00002490: 5468 6973 2068 6f6f 6b20 6973 2075 7365  This hook is use
+000024a0: 6420 746f 2070 726f 6365 7373 2074 6865  d to process the
+000024b0: 2069 6e69 7469 616c 2063 6f6e 6669 670a   initial config.
+000024c0: 2020 2020 2020 2020 616e 6420 706f 7373          and poss
+000024d0: 6962 6c79 2069 6e70 7574 2061 7267 756d  ibly input argum
+000024e0: 656e 7473 2e0a 2020 2020 2020 2020 2222  ents..        ""
+000024f0: 220a 2020 2020 2020 2020 6966 2061 7267  ".        if arg
+00002500: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00002510: 6f6e 6669 672e 7072 6f63 6573 735f 6172  onfig.process_ar
+00002520: 6773 2861 7267 7329 0a0a 2020 2020 2020  gs(args)..      
+00002530: 2020 7265 7475 726e 2063 6f6e 6669 670a    return config.
+00002540: 0a2e 2e20 5f73 7065 636e 616d 653a 0a0a  ... _specname:..
+00002550: 486f 6f6b 7370 6563 206e 616d 6520 6d61  Hookspec name ma
+00002560: 7463 6869 6e67 0a5e 5e5e 5e5e 5e5e 5e5e  tching.^^^^^^^^^
+00002570: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 0a44  ^^^^^^^^^^^^^..D
+00002580: 7572 696e 6720 706c 7567 696e 203a 7265  uring plugin :re
+00002590: 663a 6072 6567 6973 7472 6174 696f 6e20  f:`registration 
+000025a0: 3c72 6567 6973 7472 6174 696f 6e3e 602c  <registration>`,
+000025b0: 2070 6c75 6767 7920 6174 7465 6d70 7473   pluggy attempts
+000025c0: 2074 6f20 6d61 7463 6820 6561 6368 0a68   to match each.h
+000025d0: 6f6f 6b20 696d 706c 656d 656e 7461 7469  ook implementati
+000025e0: 6f6e 2064 6563 6c61 7265 6420 6279 2074  on declared by t
+000025f0: 6865 202a 706c 7567 696e 2a20 746f 2061  he *plugin* to a
+00002600: 2068 6f6f 6b0a 3a72 6566 3a60 7370 6563   hook.:ref:`spec
+00002610: 6966 6963 6174 696f 6e20 3c73 7065 6373  ification <specs
+00002620: 3e60 2069 6e20 7468 6520 2a68 6f73 742a  >` in the *host*
+00002630: 2070 726f 6772 616d 2077 6974 6820 7468   program with th
+00002640: 6520 2a2a 7361 6d65 206e 616d 652a 2a20  e **same name** 
+00002650: 6173 0a74 6865 2066 756e 6374 696f 6e20  as.the function 
+00002660: 6265 696e 6720 6465 636f 7261 7465 6420  being decorated 
+00002670: 6279 2060 6040 686f 6f6b 696d 706c 6060  by ``@hookimpl``
+00002680: 2028 652e 672e 2060 6073 6574 7570 5f70   (e.g. ``setup_p
+00002690: 726f 6a65 6374 6060 2069 6e20 7468 650a  roject`` in the.
+000026a0: 6578 616d 706c 6520 6162 6f76 6529 2e20  example above). 
+000026b0: 204e 6f74 653a 2074 6865 7265 2069 7320   Note: there is 
+000026c0: 2a6e 6f2a 2073 7472 6963 7420 7265 7175  *no* strict requ
+000026d0: 6972 656d 656e 7420 7468 6174 2065 6163  irement that eac
+000026e0: 6820 2a68 6f6f 6b69 6d70 6c2a 0a68 6173  h *hookimpl*.has
+000026f0: 2061 2063 6f72 7265 7370 6f6e 6469 6e67   a corresponding
+00002700: 202a 686f 6f6b 7370 6563 2a20 2873 6565   *hookspec* (see
+00002710: 0a3a 7265 663a 6065 6e66 6f72 6369 6e67  .:ref:`enforcing
+00002720: 2073 7065 6320 7661 6c69 6461 7469 6f6e   spec validation
+00002730: 203c 656e 666f 7263 696e 673e 6029 2e0a   <enforcing>`)..
+00002740: 0a2a 6e65 7720 696e 2076 6572 7369 6f6e  .*new in version
+00002750: 2031 2e30 2e30 3a2a 0a0a 546f 206f 7665   1.0.0:*..To ove
+00002760: 7272 6964 6520 7468 6520 6465 6661 756c  rride the defaul
+00002770: 7420 6265 6861 7669 6f72 2c20 6120 2a68  t behavior, a *h
+00002780: 6f6f 6b69 6d70 6c2a 206d 6179 2061 6c73  ookimpl* may als
+00002790: 6f20 6265 206d 6174 6368 6564 2074 6f20  o be matched to 
+000027a0: 610a 2a68 6f6f 6b73 7065 632a 2069 6e20  a.*hookspec* in 
+000027b0: 7468 6520 2a68 6f73 742a 2070 726f 6772  the *host* progr
+000027c0: 616d 2077 6974 6820 6120 6e6f 6e2d 6d61  am with a non-ma
+000027d0: 7463 6869 6e67 2066 756e 6374 696f 6e20  tching function 
+000027e0: 6e61 6d65 2062 7920 7573 696e 670a 7468  name by using.th
+000027f0: 6520 6060 7370 6563 6e61 6d65 6060 206f  e ``specname`` o
+00002800: 7074 696f 6e2e 2020 436f 6e74 696e 7569  ption.  Continui
+00002810: 6e67 2074 6865 2065 7861 6d70 6c65 2061  ng the example a
+00002820: 626f 7665 2c20 7468 6520 2a68 6f6f 6b69  bove, the *hooki
+00002830: 6d70 6c2a 2066 756e 6374 696f 6e0a 646f  mpl* function.do
+00002840: 6573 206e 6f74 206e 6565 6420 746f 2062  es not need to b
+00002850: 6520 6e61 6d65 6420 6060 7365 7475 705f  e named ``setup_
+00002860: 7072 6f6a 6563 7460 602c 2062 7574 2069  project``, but i
+00002870: 6620 7468 6520 6172 6775 6d65 6e74 0a60  f the argument.`
+00002880: 6073 7065 636e 616d 653d 2273 6574 7570  `specname="setup
+00002890: 5f70 726f 6a65 6374 2260 6020 6973 2070  _project"`` is p
+000028a0: 726f 7669 6465 6420 746f 2074 6865 2060  rovided to the `
+000028b0: 6068 6f6f 6b69 6d70 6c60 6020 6465 636f  `hookimpl`` deco
+000028c0: 7261 746f 722c 2069 7420 7769 6c6c 0a62  rator, it will.b
+000028d0: 6520 6d61 7463 6865 6420 616e 6420 6368  e matched and ch
+000028e0: 6563 6b65 6420 6167 6169 6e73 7420 7468  ecked against th
+000028f0: 6520 6060 7365 7475 705f 7072 6f6a 6563  e ``setup_projec
+00002900: 7460 6020 686f 6f6b 7370 6563 3a0a 0a2e  t`` hookspec:...
+00002910: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+00002920: 7974 686f 6e0a 0a20 2020 2040 686f 6f6b  ython..    @hook
+00002930: 696d 706c 2873 7065 636e 616d 653d 2273  impl(specname="s
+00002940: 6574 7570 5f70 726f 6a65 6374 2229 0a20  etup_project"). 
+00002950: 2020 2064 6566 2061 6e79 5f70 6c75 6769     def any_plugi
+00002960: 6e5f 6675 6e63 7469 6f6e 2863 6f6e 6669  n_function(confi
+00002970: 672c 2061 7267 7329 3a0a 2020 2020 2020  g, args):.      
+00002980: 2020 2222 2254 6869 7320 686f 6f6b 2069    """This hook i
+00002990: 7320 7573 6564 2074 6f20 7072 6f63 6573  s used to proces
+000029a0: 7320 7468 6520 696e 6974 6961 6c20 636f  s the initial co
+000029b0: 6e66 6967 0a20 2020 2020 2020 2061 6e64  nfig.        and
+000029c0: 2070 6f73 7369 626c 7920 696e 7075 7420   possibly input 
+000029d0: 6172 6775 6d65 6e74 732e 0a20 2020 2020  arguments..     
+000029e0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000029f0: 6620 6172 6773 3a0a 2020 2020 2020 2020  f args:.        
+00002a00: 2020 2020 636f 6e66 6967 2e70 726f 6365      config.proce
+00002a10: 7373 5f61 7267 7328 6172 6773 290a 0a20  ss_args(args).. 
+00002a20: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
+00002a30: 6e66 6967 0a0a 4361 6c6c 2074 696d 6520  nfig..Call time 
+00002a40: 6f72 6465 720a 5e5e 5e5e 5e5e 5e5e 5e5e  order.^^^^^^^^^^
+00002a50: 5e5e 5e5e 5e0a 4279 2064 6566 6175 6c74  ^^^^^.By default
+00002a60: 2068 6f6f 6b73 2061 7265 203a 7265 663a   hooks are :ref:
+00002a70: 6063 616c 6c65 6420 3c63 616c 6c69 6e67  `called <calling
+00002a80: 3e60 2069 6e20 4c49 464f 2072 6567 6973  >` in LIFO regis
+00002a90: 7465 7265 6420 6f72 6465 722c 2068 6f77  tered order, how
+00002aa0: 6576 6572 2c0a 6120 2a68 6f6f 6b69 6d70  ever,.a *hookimp
+00002ab0: 6c2a 2063 616e 2069 6e66 6c75 656e 6365  l* can influence
+00002ac0: 2069 7473 2063 616c 6c2d 7469 6d65 2069   its call-time i
+00002ad0: 6e76 6f63 6174 696f 6e20 706f 7369 7469  nvocation positi
+00002ae0: 6f6e 2075 7369 6e67 2073 7065 6369 616c  on using special
+00002af0: 0a61 7474 7269 6275 7465 732e 2049 6620  .attributes. If 
+00002b00: 6d61 726b 6564 2077 6974 6820 6120 6060  marked with a ``
+00002b10: 2274 7279 6669 7273 7422 6060 206f 7220  "tryfirst"`` or 
+00002b20: 6060 2274 7279 6c61 7374 2260 6020 6f70  ``"trylast"`` op
+00002b30: 7469 6f6e 2069 740a 7769 6c6c 2062 6520  tion it.will be 
+00002b40: 6578 6563 7574 6564 202a 6669 7273 742a  executed *first*
+00002b50: 206f 7220 2a6c 6173 742a 2072 6573 7065   or *last* respe
+00002b60: 6374 6976 656c 7920 696e 2074 6865 2068  ctively in the h
+00002b70: 6f6f 6b20 6361 6c6c 206c 6f6f 703a 0a0a  ook call loop:..
+00002b80: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00002b90: 7079 7468 6f6e 0a0a 2020 2020 696d 706f  python..    impo
+00002ba0: 7274 2073 7973 0a20 2020 2066 726f 6d20  rt sys.    from 
+00002bb0: 706c 7567 6779 2069 6d70 6f72 7420 506c  pluggy import Pl
+00002bc0: 7567 696e 4d61 6e61 6765 722c 2048 6f6f  uginManager, Hoo
+00002bd0: 6b69 6d70 6c4d 6172 6b65 720a 0a20 2020  kimplMarker..   
+00002be0: 2068 6f6f 6b69 6d70 6c20 3d20 486f 6f6b   hookimpl = Hook
+00002bf0: 696d 706c 4d61 726b 6572 2822 6d79 7072  implMarker("mypr
+00002c00: 6f6a 6563 7422 290a 0a0a 2020 2020 4068  oject")...    @h
+00002c10: 6f6f 6b69 6d70 6c28 7472 796c 6173 743d  ookimpl(trylast=
+00002c20: 5472 7565 290a 2020 2020 6465 6620 7365  True).    def se
+00002c30: 7475 705f 7072 6f6a 6563 7428 636f 6e66  tup_project(conf
+00002c40: 6967 2c20 6172 6773 293a 0a20 2020 2020  ig, args):.     
+00002c50: 2020 2022 2222 4465 6661 756c 7420 696d     """Default im
+00002c60: 706c 656d 656e 7461 7469 6f6e 2e22 2222  plementation."""
+00002c70: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
+00002c80: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00002c90: 6e66 6967 2e70 726f 6365 7373 5f61 7267  nfig.process_arg
+00002ca0: 7328 6172 6773 290a 0a20 2020 2020 2020  s(args)..       
+00002cb0: 2072 6574 7572 6e20 636f 6e66 6967 0a0a   return config..
+00002cc0: 0a20 2020 2063 6c61 7373 2053 6f6d 654f  .    class SomeO
+00002cd0: 7468 6572 506c 7567 696e 3a0a 2020 2020  therPlugin:.    
+00002ce0: 2020 2020 2222 2253 6f6d 6520 6f74 6865      """Some othe
+00002cf0: 7220 706c 7567 696e 2064 6566 696e 696e  r plugin definin
+00002d00: 6720 7468 6520 7361 6d65 2068 6f6f 6b2e  g the same hook.
+00002d10: 2222 220a 0a20 2020 2020 2020 2040 686f  """..        @ho
+00002d20: 6f6b 696d 706c 2874 7279 6669 7273 743d  okimpl(tryfirst=
+00002d30: 5472 7565 290a 2020 2020 2020 2020 6465  True).        de
+00002d40: 6620 7365 7475 705f 7072 6f6a 6563 7428  f setup_project(
+00002d50: 7365 6c66 2c20 636f 6e66 6967 2c20 6172  self, config, ar
+00002d60: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
+00002d70: 2022 2222 5265 706f 7274 2077 6861 7420   """Report what 
+00002d80: 6172 6773 2077 6572 6520 7061 7373 6564  args were passed
+00002d90: 2062 6566 6f72 6520 6361 6c6c 696e 670a   before calling.
+00002da0: 2020 2020 2020 2020 2020 2020 646f 776e              down
+00002db0: 7374 7265 616d 2068 6f6f 6b73 2e0a 2020  stream hooks..  
+00002dc0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+00002dd0: 2020 2020 2020 2020 2020 6966 2061 7267            if arg
+00002de0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00002df0: 2020 2070 7269 6e74 2822 476f 7420 6172     print("Got ar
+00002e00: 6773 3a20 7b7d 222e 666f 726d 6174 2861  gs: {}".format(a
+00002e10: 7267 7329 290a 0a20 2020 2020 2020 2020  rgs))..         
+00002e20: 2020 2072 6574 7572 6e20 636f 6e66 6967     return config
+00002e30: 0a0a 0a20 2020 2070 6d20 3d20 506c 7567  ...    pm = Plug
+00002e40: 696e 4d61 6e61 6765 7228 226d 7970 726f  inManager("mypro
+00002e50: 6a65 6374 2229 0a0a 2020 2020 2320 6c6f  ject")..    # lo
+00002e60: 6164 2066 726f 6d20 7468 6520 6c6f 6361  ad from the loca
+00002e70: 6c20 6d6f 6475 6c65 2773 206e 616d 6573  l module's names
+00002e80: 7061 6365 0a20 2020 2070 6d2e 7265 6769  pace.    pm.regi
+00002e90: 7374 6572 2873 7973 2e6d 6f64 756c 6573  ster(sys.modules
+00002ea0: 5b5f 5f6e 616d 655f 5f5d 290a 2020 2020  [__name__]).    
+00002eb0: 2320 6c6f 6164 2061 2070 6c75 6769 6e20  # load a plugin 
+00002ec0: 6465 6669 6e65 6420 6f6e 2061 2063 6c61  defined on a cla
+00002ed0: 7373 0a20 2020 2070 6d2e 7265 6769 7374  ss.    pm.regist
+00002ee0: 6572 2853 6f6d 654f 7468 6572 506c 7567  er(SomeOtherPlug
+00002ef0: 696e 2829 290a 0a46 6f72 2061 6e6f 7468  in())..For anoth
+00002f00: 6572 2065 7861 6d70 6c65 2073 6565 2074  er example see t
+00002f10: 6865 203a 7265 663a 6070 7974 6573 743a  he :ref:`pytest:
+00002f20: 706c 7567 696e 2d68 6f6f 6b6f 7264 6572  plugin-hookorder
+00002f30: 6020 7365 6374 696f 6e20 6f66 2074 6865  ` section of the
+00002f40: 0a60 6070 7974 6573 7460 6020 646f 6373  .``pytest`` docs
+00002f50: 2e0a 0a2e 2e20 6e6f 7465 3a3a 0a20 2020  ..... note::.   
+00002f60: 2060 6074 7279 6669 7273 7460 6020 616e   ``tryfirst`` an
+00002f70: 6420 6060 7472 796c 6173 7460 6020 686f  d ``trylast`` ho
+00002f80: 6f6b 7320 6172 6520 7374 696c 6c20 696e  oks are still in
+00002f90: 766f 6b65 6420 696e 204c 4946 4f20 6f72  voked in LIFO or
+00002fa0: 6465 7220 7769 7468 696e 0a20 2020 2065  der within.    e
+00002fb0: 6163 6820 6361 7465 676f 7279 2e0a 0a0a  ach category....
+00002fc0: 2e2e 205f 686f 6f6b 7772 6170 7065 7273  .. _hookwrappers
+00002fd0: 3a0a 0a57 7261 7070 6572 730a 5e5e 5e5e  :..Wrappers.^^^^
+00002fe0: 5e5e 5e5e 0a0a 2e2e 206e 6f74 653a 3a0a  ^^^^.... note::.
+00002ff0: 2020 2020 5468 6973 2073 6563 7469 6f6e      This section
+00003000: 2064 6573 6372 6962 6573 2022 6e65 772d   describes "new-
+00003010: 7374 796c 6520 686f 6f6b 2077 7261 7070  style hook wrapp
+00003020: 6572 7322 2c20 7768 6963 6820 7765 7265  ers", which were
+00003030: 2061 6464 6564 2069 6e20 506c 7567 6779   added in Pluggy
+00003040: 0a20 2020 2031 2e31 2e20 466f 7220 6561  .    1.1. For ea
+00003050: 726c 6965 7220 7665 7273 696f 6e73 2c20  rlier versions, 
+00003060: 7365 6520 7468 6520 226f 6c64 2d73 7479  see the "old-sty
+00003070: 6c65 2068 6f6f 6b20 7772 6170 7065 7273  le hook wrappers
+00003080: 2220 7365 6374 696f 6e20 6265 6c6f 772e  " section below.
+00003090: 0a20 2020 2054 6865 2074 776f 2073 7479  .    The two sty
+000030a0: 6c65 7320 6172 6520 6675 6c6c 7920 696e  les are fully in
+000030b0: 7465 726f 7065 7261 626c 652e 0a0a 4120  teroperable...A 
+000030c0: 2a68 6f6f 6b69 6d70 6c2a 2063 616e 2062  *hookimpl* can b
+000030d0: 6520 6120 6765 6e65 7261 746f 7220 6675  e a generator fu
+000030e0: 6e63 7469 6f6e 2c20 7768 6963 6820 696e  nction, which in
+000030f0: 6469 6361 7465 7320 7468 6174 2074 6865  dicates that the
+00003100: 2066 756e 6374 696f 6e20 7769 6c6c 0a62   function will.b
+00003110: 6520 6361 6c6c 6564 2074 6f20 2a77 7261  e called to *wra
+00003120: 702a 2028 6f72 2073 7572 726f 756e 6429  p* (or surround)
+00003130: 2061 6c6c 206f 7468 6572 206e 6f72 6d61   all other norma
+00003140: 6c20 2a68 6f6f 6b69 6d70 6c2a 2063 616c  l *hookimpl* cal
+00003150: 6c73 2e20 4120 2a68 6f6f 6b0a 7772 6170  ls. A *hook.wrap
+00003160: 7065 722a 2063 616e 2074 6875 7320 6578  per* can thus ex
+00003170: 6563 7574 6520 736f 6d65 2063 6f64 6520  ecute some code 
+00003180: 6168 6561 6420 616e 6420 6166 7465 7220  ahead and after 
+00003190: 7468 6520 6578 6563 7574 696f 6e20 6f66  the execution of
+000031a0: 2061 6c6c 0a63 6f72 7265 7370 6f6e 6469   all.correspondi
+000031b0: 6e67 206e 6f6e 2d77 7261 7070 7065 7220  ng non-wrappper 
+000031c0: 2a68 6f6f 6b69 6d70 6c73 2a2e 0a0a 4d75  *hookimpls*...Mu
+000031d0: 6368 2069 6e20 7468 6520 7361 6d65 2077  ch in the same w
+000031e0: 6179 2061 7320 6120 3a70 793a 6675 6e63  ay as a :py:func
+000031f0: 3a60 4063 6f6e 7465 7874 6c69 622e 636f  :`@contextlib.co
+00003200: 6e74 6578 746d 616e 6167 6572 203c 7079  ntextmanager <py
+00003210: 7468 6f6e 3a63 6f6e 7465 7874 6c69 622e  thon:contextlib.
+00003220: 636f 6e74 6578 746d 616e 6167 6572 3e60  contextmanager>`
+00003230: 2c0a 2a68 6f6f 6b20 7772 6170 7065 7273  ,.*hook wrappers
+00003240: 2a20 6d75 7374 2062 6520 696d 706c 656d  * must be implem
+00003250: 656e 7465 6420 6173 2067 656e 6572 6174  ented as generat
+00003260: 6f72 2066 756e 6374 696f 6e20 7769 7468  or function with
+00003270: 2061 2073 696e 676c 6520 6060 7969 656c   a single ``yiel
+00003280: 6460 6020 696e 2069 7473 2062 6f64 793a  d`` in its body:
+00003290: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+000032a0: 3a20 7079 7468 6f6e 0a0a 2020 2020 4068  : python..    @h
+000032b0: 6f6f 6b69 6d70 6c0a 2020 2020 6465 6620  ookimpl.    def 
+000032c0: 7365 7475 705f 7072 6f6a 6563 7428 636f  setup_project(co
+000032d0: 6e66 6967 2c20 6172 6773 293a 0a20 2020  nfig, args):.   
+000032e0: 2020 2020 2022 2222 5772 6170 2063 616c       """Wrap cal
+000032f0: 6c73 2074 6f20 6060 7365 7475 705f 7072  ls to ``setup_pr
+00003300: 6f6a 6563 7428 2960 6020 696d 706c 656d  oject()`` implem
+00003310: 656e 7461 7469 6f6e 7320 7768 6963 680a  entations which.
+00003320: 2020 2020 2020 2020 7368 6f75 6c64 2072          should r
+00003330: 6574 7572 6e20 6a73 6f6e 2065 6e63 6f64  eturn json encod
+00003340: 6564 2063 6f6e 6669 6720 6f70 7469 6f6e  ed config option
+00003350: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00003360: 2020 2020 2020 2023 2067 6574 2069 6e69         # get ini
+00003370: 7469 616c 2064 6566 6175 6c74 2063 6f6e  tial default con
+00003380: 6669 670a 2020 2020 2020 2020 6465 6661  fig.        defa
+00003390: 756c 7473 203d 2063 6f6e 6669 672e 746f  ults = config.to
+000033a0: 6a73 6f6e 2829 0a0a 2020 2020 2020 2020  json()..        
+000033b0: 6966 2063 6f6e 6669 672e 6465 6275 673a  if config.debug:
+000033c0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000033d0: 6e74 2822 5072 652d 686f 6f6b 2063 6f6e  nt("Pre-hook con
+000033e0: 6669 6720 6973 207b 7d22 2e66 6f72 6d61  fig is {}".forma
+000033f0: 7428 636f 6e66 6967 2e74 6f6a 736f 6e28  t(config.tojson(
+00003400: 2929 290a 0a20 2020 2020 2020 2023 2061  )))..        # a
+00003410: 6c6c 2063 6f72 7265 7370 6f6e 6469 6e67  ll corresponding
+00003420: 2068 6f6f 6b69 6d70 6c73 2061 7265 2069   hookimpls are i
+00003430: 6e76 6f6b 6564 2068 6572 650a 2020 2020  nvoked here.    
+00003440: 2020 2020 7265 7375 6c74 203d 2079 6965      result = yie
+00003450: 6c64 0a0a 2020 2020 2020 2020 666f 7220  ld..        for 
+00003460: 6974 656d 2069 6e20 7265 7375 6c74 3a0a  item in result:.
+00003470: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00003480: 7428 224a 534f 4e20 636f 6e66 6967 206f  t("JSON config o
+00003490: 7665 7272 6964 6520 6973 207b 7d22 2e66  verride is {}".f
+000034a0: 6f72 6d61 7428 6974 656d 2929 0a0a 2020  ormat(item))..  
+000034b0: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
+000034c0: 6465 6275 673a 0a20 2020 2020 2020 2020  debug:.         
+000034d0: 2020 2070 7269 6e74 2822 506f 7374 2d68     print("Post-h
+000034e0: 6f6f 6b20 636f 6e66 6967 2069 7320 7b7d  ook config is {}
+000034f0: 222e 666f 726d 6174 2863 6f6e 6669 672e  ".format(config.
+00003500: 746f 6a73 6f6e 2829 2929 0a0a 2020 2020  tojson()))..    
+00003510: 2020 2020 6966 2063 6f6e 6669 672e 7573      if config.us
+00003520: 655f 6465 6661 756c 7473 3a0a 2020 2020  e_defaults:.    
+00003530: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00003540: 6566 6175 6c74 730a 2020 2020 2020 2020  efaults.        
+00003550: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00003560: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00003570: 0a54 6865 2067 656e 6572 6174 6f72 2069  .The generator i
+00003580: 7320 3a70 793a 6d65 7468 3a60 7365 6e74  s :py:meth:`sent
+00003590: 203c 7079 7468 6f6e 3a67 656e 6572 6174   <python:generat
+000035a0: 6f72 2e73 656e 643e 6020 7468 6520 7265  or.send>` the re
+000035b0: 7475 726e 2076 616c 7565 0a6f 6620 7468  turn value.of th
+000035c0: 6520 686f 6f6b 2074 6875 7320 6661 722c  e hook thus far,
+000035d0: 206f 722c 2069 6620 7468 6520 7072 6576   or, if the prev
+000035e0: 696f 7573 2063 616c 6c73 2072 6169 7365  ious calls raise
+000035f0: 6420 616e 2065 7863 6570 7469 6f6e 2c20  d an exception, 
+00003600: 6974 2069 730a 3a70 793a 6d65 7468 3a60  it is.:py:meth:`
+00003610: 7468 726f 776e 203c 7079 7468 6f6e 3a67  thrown <python:g
+00003620: 656e 6572 6174 6f72 2e74 6872 6f77 3e60  enerator.throw>`
+00003630: 2074 6865 2065 7863 6570 7469 6f6e 2e0a   the exception..
+00003640: 0a54 6865 2066 756e 6374 696f 6e20 7368  .The function sh
+00003650: 6f75 6c64 2064 6f20 6f6e 6520 6f66 2074  ould do one of t
+00003660: 776f 2074 6869 6e67 733a 0a2d 2052 6574  wo things:.- Ret
+00003670: 7572 6e20 6120 7661 6c75 652c 2077 6869  urn a value, whi
+00003680: 6368 2063 616e 2062 6520 7468 6520 7361  ch can be the sa
+00003690: 6d65 2076 616c 7565 2061 7320 7265 6365  me value as rece
+000036a0: 6976 6564 2066 726f 6d20 7468 6520 6060  ived from the ``
+000036b0: 7969 656c 6460 602c 206f 720a 736f 6d65  yield``, or.some
+000036c0: 7468 696e 6720 656c 7365 2065 6e74 6972  thing else entir
+000036d0: 656c 792e 0a2d 2052 6169 7365 2061 6e20  ely..- Raise an 
+000036e0: 6578 6365 7074 696f 6e2e 0a54 6865 2072  exception..The r
+000036f0: 6574 7572 6e20 7661 6c75 6520 6f72 2065  eturn value or e
+00003700: 7863 6570 7469 6f6e 2070 726f 7061 6761  xception propaga
+00003710: 7465 2074 6f20 6675 7274 6865 7220 686f  te to further ho
+00003720: 6f6b 2077 7261 7070 6572 732c 2061 6e64  ok wrappers, and
+00003730: 2066 696e 616c 6c79 0a74 6f20 7468 6520   finally.to the 
+00003740: 686f 6f6b 2063 616c 6c65 722e 0a0a 416c  hook caller...Al
+00003750: 736f 2073 6565 2074 6865 203a 7265 663a  so see the :ref:
+00003760: 6070 7974 6573 743a 686f 6f6b 7772 6170  `pytest:hookwrap
+00003770: 7065 7260 2073 6563 7469 6f6e 2069 6e20  per` section in 
+00003780: 7468 6520 6060 7079 7465 7374 6060 2064  the ``pytest`` d
+00003790: 6f63 732e 0a0a 4f6c 642d 7374 796c 6520  ocs...Old-style 
+000037a0: 7772 6170 7065 7273 0a5e 5e5e 5e5e 5e5e  wrappers.^^^^^^^
+000037b0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 0a2e 2e20  ^^^^^^^^^^^.... 
+000037c0: 6e6f 7465 3a3a 0a20 2020 2050 7265 6665  note::.    Prefe
+000037d0: 7220 746f 2075 7365 206e 6577 2d73 7479  r to use new-sty
+000037e0: 6c65 2068 6f6f 6b20 7772 6170 7065 7273  le hook wrappers
+000037f0: 2c20 756e 6c65 7373 2079 6f75 206e 6565  , unless you nee
+00003800: 6420 746f 2073 7570 706f 7274 2050 6c75  d to support Plu
+00003810: 6767 790a 2020 2020 7665 7273 696f 6e73  ggy.    versions
+00003820: 2062 6566 6f72 6520 312e 312e 0a0a 4120   before 1.1...A 
+00003830: 2a68 6f6f 6b69 6d70 6c2a 2063 616e 2062  *hookimpl* can b
+00003840: 6520 6d61 726b 6564 2077 6974 6820 7468  e marked with th
+00003850: 6520 6060 2268 6f6f 6b77 7261 7070 6572  e ``"hookwrapper
+00003860: 2260 6020 6f70 7469 6f6e 2c20 7768 6963  "`` option, whic
+00003870: 6820 696e 6469 6361 7465 730a 7468 6174  h indicates.that
+00003880: 2074 6865 2066 756e 6374 696f 6e20 7769   the function wi
+00003890: 6c6c 2062 6520 6361 6c6c 6564 2074 6f20  ll be called to 
+000038a0: 2a77 7261 702a 2028 6f72 2073 7572 726f  *wrap* (or surro
+000038b0: 756e 6429 2061 6c6c 206f 7468 6572 206e  und) all other n
+000038c0: 6f72 6d61 6c0a 2a68 6f6f 6b69 6d70 6c2a  ormal.*hookimpl*
+000038d0: 2063 616c 6c73 2e20 4120 2a68 6f6f 6b77   calls. A *hookw
+000038e0: 7261 7070 6572 2a20 6361 6e20 7468 7573  rapper* can thus
+000038f0: 2065 7865 6375 7465 2073 6f6d 6520 636f   execute some co
+00003900: 6465 2061 6865 6164 2061 6e64 2061 6674  de ahead and aft
+00003910: 6572 2074 6865 0a65 7865 6375 7469 6f6e  er the.execution
+00003920: 206f 6620 616c 6c20 636f 7272 6573 706f   of all correspo
+00003930: 6e64 696e 6720 6e6f 6e2d 7772 6170 7070  nding non-wrappp
+00003940: 6572 202a 686f 6f6b 696d 706c 732a 2e0a  er *hookimpls*..
+00003950: 0a2a 686f 6f6b 7772 6170 7065 7273 2a20  .*hookwrappers* 
+00003960: 6d75 7374 2062 6520 696d 706c 656d 656e  must be implemen
+00003970: 7465 6420 6173 2067 656e 6572 6174 6f72  ted as generator
+00003980: 2066 756e 6374 696f 6e20 7769 7468 2061   function with a
+00003990: 2073 696e 676c 6520 6060 7969 656c 6460   single ``yield`
+000039a0: 6020 696e 2069 7473 2062 6f64 793a 0a0a  ` in its body:..
+000039b0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+000039c0: 2070 7974 686f 6e0a 0a20 2020 2040 686f   python..    @ho
+000039d0: 6f6b 696d 706c 2868 6f6f 6b77 7261 7070  okimpl(hookwrapp
+000039e0: 6572 3d54 7275 6529 0a20 2020 2064 6566  er=True).    def
+000039f0: 2073 6574 7570 5f70 726f 6a65 6374 2863   setup_project(c
+00003a00: 6f6e 6669 672c 2061 7267 7329 3a0a 2020  onfig, args):.  
+00003a10: 2020 2020 2020 2222 2257 7261 7020 6361        """Wrap ca
+00003a20: 6c6c 7320 746f 2060 6073 6574 7570 5f70  lls to ``setup_p
+00003a30: 726f 6a65 6374 2829 6060 2069 6d70 6c65  roject()`` imple
+00003a40: 6d65 6e74 6174 696f 6e73 2077 6869 6368  mentations which
+00003a50: 0a20 2020 2020 2020 2073 686f 756c 6420  .        should 
+00003a60: 7265 7475 726e 206a 736f 6e20 656e 636f  return json enco
+00003a70: 6465 6420 636f 6e66 6967 206f 7074 696f  ded config optio
+00003a80: 6e73 2e0a 2020 2020 2020 2020 2222 220a  ns..        """.
+00003a90: 2020 2020 2020 2020 2320 6765 7420 696e          # get in
+00003aa0: 6974 6961 6c20 6465 6661 756c 7420 636f  itial default co
+00003ab0: 6e66 6967 0a20 2020 2020 2020 2064 6566  nfig.        def
+00003ac0: 6175 6c74 7320 3d20 636f 6e66 6967 2e74  aults = config.t
+00003ad0: 6f6a 736f 6e28 290a 0a20 2020 2020 2020  ojson()..       
+00003ae0: 2069 6620 636f 6e66 6967 2e64 6562 7567   if config.debug
+00003af0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00003b00: 696e 7428 2250 7265 2d68 6f6f 6b20 636f  int("Pre-hook co
+00003b10: 6e66 6967 2069 7320 7b7d 222e 666f 726d  nfig is {}".form
+00003b20: 6174 2863 6f6e 6669 672e 746f 6a73 6f6e  at(config.tojson
+00003b30: 2829 2929 0a0a 2020 2020 2020 2020 2320  ()))..        # 
+00003b40: 616c 6c20 636f 7272 6573 706f 6e64 696e  all correspondin
+00003b50: 6720 686f 6f6b 696d 706c 7320 6172 6520  g hookimpls are 
+00003b60: 696e 766f 6b65 6420 6865 7265 0a20 2020  invoked here.   
+00003b70: 2020 2020 206f 7574 636f 6d65 203d 2079       outcome = y
+00003b80: 6965 6c64 0a0a 2020 2020 2020 2020 7472  ield..        tr
+00003b90: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
+00003ba0: 6573 756c 7420 3d20 6f75 7463 6f6d 652e  esult = outcome.
+00003bb0: 6765 745f 7265 7375 6c74 2829 0a20 2020  get_result().   
+00003bc0: 2020 2020 2065 7863 6570 7420 4261 7365       except Base
+00003bd0: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
+00003be0: 2020 2020 2020 2020 2020 2020 6f75 7463              outc
+00003bf0: 6f6d 652e 666f 7263 655f 6578 6365 7074  ome.force_except
+00003c00: 696f 6e28 6529 0a20 2020 2020 2020 2020  ion(e).         
+00003c10: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+00003c20: 2020 2066 6f72 2069 7465 6d20 696e 2072     for item in r
+00003c30: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
+00003c40: 2020 2070 7269 6e74 2822 4a53 4f4e 2063     print("JSON c
+00003c50: 6f6e 6669 6720 6f76 6572 7269 6465 2069  onfig override i
+00003c60: 7320 7b7d 222e 666f 726d 6174 2869 7465  s {}".format(ite
+00003c70: 6d29 290a 0a20 2020 2020 2020 2069 6620  m))..        if 
+00003c80: 636f 6e66 6967 2e64 6562 7567 3a0a 2020  config.debug:.  
+00003c90: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00003ca0: 2250 6f73 742d 686f 6f6b 2063 6f6e 6669  "Post-hook confi
+00003cb0: 6720 6973 207b 7d22 2e66 6f72 6d61 7428  g is {}".format(
+00003cc0: 636f 6e66 6967 2e74 6f6a 736f 6e28 2929  config.tojson())
+00003cd0: 290a 0a20 2020 2020 2020 2069 6620 636f  )..        if co
+00003ce0: 6e66 6967 2e75 7365 5f64 6566 6175 6c74  nfig.use_default
+00003cf0: 733a 0a20 2020 2020 2020 2020 2020 206f  s:.            o
+00003d00: 7574 636f 6d65 2e66 6f72 6365 5f72 6573  utcome.force_res
+00003d10: 756c 7428 6465 6661 756c 7473 290a 0a54  ult(defaults)..T
+00003d20: 6865 2067 656e 6572 6174 6f72 2069 7320  he generator is 
+00003d30: 3a70 793a 6d65 7468 3a60 7365 6e74 203c  :py:meth:`sent <
+00003d40: 7079 7468 6f6e 3a67 656e 6572 6174 6f72  python:generator
+00003d50: 2e73 656e 643e 6020 6120 3a70 793a 636c  .send>` a :py:cl
+00003d60: 6173 733a 6070 6c75 6767 792e 5f63 616c  ass:`pluggy._cal
+00003d70: 6c65 7273 2e5f 5265 7375 6c74 6020 6f62  lers._Result` ob
+00003d80: 6a65 6374 2077 6869 6368 2063 616e 0a62  ject which can.b
+00003d90: 6520 6173 7369 676e 6564 2069 6e20 7468  e assigned in th
+00003da0: 6520 6060 7969 656c 6460 6020 6578 7072  e ``yield`` expr
+00003db0: 6573 7369 6f6e 2061 6e64 2075 7365 6420  ession and used 
+00003dc0: 746f 2069 6e73 7065 6374 0a74 6865 2066  to inspect.the f
+00003dd0: 696e 616c 2072 6573 756c 7428 7329 206f  inal result(s) o
+00003de0: 7220 6578 6365 7074 696f 6e73 2072 6574  r exceptions ret
+00003df0: 7572 6e65 6420 6261 636b 2074 6f20 7468  urned back to th
+00003e00: 6520 6361 6c6c 6572 2075 7369 6e67 2074  e caller using t
+00003e10: 6865 0a3a 7079 3a6d 6574 683a 607e 706c  he.:py:meth:`~pl
+00003e20: 7567 6779 2e5f 6361 6c6c 6572 732e 5f52  uggy._callers._R
+00003e30: 6573 756c 742e 6765 745f 7265 7375 6c74  esult.get_result
+00003e40: 6020 6d65 7468 6f64 2c20 6f76 6572 7269  ` method, overri
+00003e50: 6465 2074 6865 2072 6573 756c 740a 7573  de the result.us
+00003e60: 696e 6720 7468 6520 3a70 793a 6d65 7468  ing the :py:meth
+00003e70: 3a60 7e70 6c75 6767 792e 5f63 616c 6c65  :`~pluggy._calle
+00003e80: 7273 2e5f 5265 7375 6c74 2e66 6f72 6365  rs._Result.force
+00003e90: 5f72 6573 756c 7460 2c20 6f72 206f 7665  _result`, or ove
+00003ea0: 7272 6964 650a 7468 6520 6578 6365 7074  rride.the except
+00003eb0: 696f 6e20 7573 696e 6720 7468 6520 3a70  ion using the :p
+00003ec0: 793a 6d65 7468 3a60 7e70 6c75 6767 792e  y:meth:`~pluggy.
+00003ed0: 5f63 616c 6c65 7273 2e5f 5265 7375 6c74  _callers._Result
+00003ee0: 2e66 6f72 6365 5f65 7863 6570 7469 6f6e  .force_exception
+00003ef0: 600a 6d65 7468 6f64 2e0a 0a2e 2e20 6e6f  `.method..... no
+00003f00: 7465 3a3a 0a20 2020 204f 6c64 2d73 7479  te::.    Old-sty
+00003f10: 6c65 2068 6f6f 6b20 7772 6170 7065 7273  le hook wrappers
+00003f20: 2063 616e 202a 2a6e 6f74 2a2a 2072 6574   can **not** ret
+00003f30: 7572 6e20 7265 7375 6c74 733b 2074 6865  urn results; the
+00003f40: 7920 6361 6e20 6f6e 6c79 206d 6f64 6966  y can only modif
+00003f50: 790a 2020 2020 7468 656d 2075 7369 6e67  y.    them using
+00003f60: 2074 6865 203a 7079 3a6d 6574 683a 607e   the :py:meth:`~
+00003f70: 706c 7567 6779 2e5f 6361 6c6c 6572 732e  pluggy._callers.
+00003f80: 5f52 6573 756c 742e 666f 7263 655f 7265  _Result.force_re
+00003f90: 7375 6c74 6020 4150 492e 0a0a 2020 2020  sult` API...    
+00003fa0: 4f6c 642d 7374 796c 6520 486f 6f6b 2077  Old-style Hook w
+00003fb0: 7261 7070 6572 7320 7368 6f75 6c64 202a  rappers should *
+00003fc0: 2a6e 6f74 2a2a 2072 6169 7365 2065 7863  *not** raise exc
+00003fd0: 6570 7469 6f6e 733b 2074 6869 7320 7769  eptions; this wi
+00003fe0: 6c6c 2063 6175 7365 0a20 2020 2066 7572  ll cause.    fur
+00003ff0: 7468 6572 2068 6f6f 6b77 7261 7070 6572  ther hookwrapper
+00004000: 7320 746f 2062 6520 736b 6970 7065 642e  s to be skipped.
+00004010: 2054 6865 7920 7368 6f75 6c64 2075 7365   They should use
+00004020: 0a20 2020 203a 7079 3a6d 6574 683a 607e  .    :py:meth:`~
+00004030: 706c 7567 6779 2e5f 6361 6c6c 6572 732e  pluggy._callers.
+00004040: 5f52 6573 756c 742e 666f 7263 655f 6578  _Result.force_ex
+00004050: 6365 7074 696f 6e60 2074 6f20 6164 6a75  ception` to adju
+00004060: 7374 2074 6865 0a20 2020 2065 7863 6570  st the.    excep
+00004070: 7469 6f6e 2e0a 0a2e 2e20 5f73 7065 6373  tion..... _specs
+00004080: 3a0a 0a53 7065 6369 6669 6361 7469 6f6e  :..Specification
+00004090: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s.--------------
+000040a0: 0a41 2068 6f6f 6b20 2a73 7065 6369 6669  .A hook *specifi
+000040b0: 6361 7469 6f6e 2a20 282a 686f 6f6b 7370  cation* (*hooksp
+000040c0: 6563 2a29 2069 7320 6120 6465 6669 6e69  ec*) is a defini
+000040d0: 7469 6f6e 2075 7365 6420 746f 2076 616c  tion used to val
+000040e0: 6964 6174 6520 6561 6368 0a2a 686f 6f6b  idate each.*hook
+000040f0: 696d 706c 2a20 656e 7375 7269 6e67 2074  impl* ensuring t
+00004100: 6861 7420 616e 2065 7874 656e 7369 6f6e  hat an extension
+00004110: 2077 7269 7465 7220 6861 7320 636f 7272   writer has corr
+00004120: 6563 746c 7920 6465 6669 6e65 6420 7468  ectly defined th
+00004130: 6569 720a 6361 6c6c 6261 636b 2066 756e  eir.callback fun
+00004140: 6374 696f 6e20 2a69 6d70 6c65 6d65 6e74  ction *implement
+00004150: 6174 696f 6e2a 202e 0a0a 2a68 6f6f 6b73  ation* ...*hooks
+00004160: 7065 6373 2a20 6172 6520 6465 6669 6e65  pecs* are define
+00004170: 6420 7573 696e 6720 7369 6d69 6c61 726c  d using similarl
+00004180: 7920 6d61 726b 6564 2066 756e 6374 696f  y marked functio
+00004190: 6e73 2068 6f77 6576 6572 206f 6e6c 7920  ns however only 
+000041a0: 7468 650a 6675 6e63 7469 6f6e 202a 7369  the.function *si
+000041b0: 676e 6174 7572 652a 2028 6974 7320 6e61  gnature* (its na
+000041c0: 6d65 2061 6e64 206e 616d 6573 206f 6620  me and names of 
+000041d0: 616c 6c20 6974 7320 6172 6775 6d65 6e74  all its argument
+000041e0: 7329 2069 7320 616e 616c 797a 6564 0a61  s) is analyzed.a
+000041f0: 6e64 2073 746f 7265 642e 2041 7320 7375  nd stored. As su
+00004200: 6368 2c20 6f66 7465 6e20 796f 7520 7769  ch, often you wi
+00004210: 6c6c 2073 6565 2061 202a 686f 6f6b 7370  ll see a *hooksp
+00004220: 6563 2a20 6465 6669 6e65 6420 7769 7468  ec* defined with
+00004230: 206f 6e6c 790a 6120 646f 6373 7472 696e   only.a docstrin
+00004240: 6720 696e 2069 7473 2062 6f64 792e 0a0a  g in its body...
+00004250: 2a68 6f6f 6b73 7065 6373 2a20 6172 6520  *hookspecs* are 
+00004260: 6c6f 6164 6564 2075 7369 6e67 2074 6865  loaded using the
+00004270: 0a3a 7079 3a6d 6574 683a 607e 706c 7567  .:py:meth:`~plug
+00004280: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
+00004290: 2e61 6464 5f68 6f6f 6b73 7065 6373 2829  .add_hookspecs()
+000042a0: 6020 6d65 7468 6f64 2061 6e64 206e 6f72  ` method and nor
+000042b0: 6d61 6c6c 790a 7368 6f75 6c64 2062 6520  mally.should be 
+000042c0: 6164 6465 6420 6265 666f 7265 2072 6567  added before reg
+000042d0: 6973 7465 7269 6e67 2063 6f72 7265 7370  istering corresp
+000042e0: 6f6e 6469 6e67 202a 686f 6f6b 696d 706c  onding *hookimpl
+000042f0: 732a 3a0a 0a2e 2e20 636f 6465 2d62 6c6f  s*:.... code-blo
+00004300: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
+00004310: 2069 6d70 6f72 7420 7379 730a 2020 2020   import sys.    
+00004320: 6672 6f6d 2070 6c75 6767 7920 696d 706f  from pluggy impo
+00004330: 7274 2050 6c75 6769 6e4d 616e 6167 6572  rt PluginManager
+00004340: 2c20 486f 6f6b 7370 6563 4d61 726b 6572  , HookspecMarker
+00004350: 0a0a 2020 2020 686f 6f6b 7370 6563 203d  ..    hookspec =
+00004360: 2048 6f6f 6b73 7065 634d 6172 6b65 7228   HookspecMarker(
+00004370: 226d 7970 726f 6a65 6374 2229 0a0a 0a20  "myproject")... 
+00004380: 2020 2040 686f 6f6b 7370 6563 0a20 2020     @hookspec.   
+00004390: 2064 6566 2073 6574 7570 5f70 726f 6a65   def setup_proje
+000043a0: 6374 2863 6f6e 6669 672c 2061 7267 7329  ct(config, args)
+000043b0: 3a0a 2020 2020 2020 2020 2222 2254 6869  :.        """Thi
+000043c0: 7320 686f 6f6b 2069 7320 7573 6564 2074  s hook is used t
+000043d0: 6f20 7072 6f63 6573 7320 7468 6520 696e  o process the in
+000043e0: 6974 6961 6c20 636f 6e66 6967 2061 6e64  itial config and
+000043f0: 2069 6e70 7574 0a20 2020 2020 2020 2061   input.        a
+00004400: 7267 756d 656e 7473 2e0a 2020 2020 2020  rguments..      
+00004410: 2020 2222 220a 0a0a 2020 2020 706d 203d    """...    pm =
+00004420: 2050 6c75 6769 6e4d 616e 6167 6572 2822   PluginManager("
+00004430: 6d79 7072 6f6a 6563 7422 290a 0a20 2020  myproject")..   
+00004440: 2023 206c 6f61 6420 6672 6f6d 2074 6865   # load from the
+00004450: 206c 6f63 616c 206d 6f64 756c 6527 7320   local module's 
+00004460: 6e61 6d65 7370 6163 650a 2020 2020 706d  namespace.    pm
+00004470: 2e61 6464 5f68 6f6f 6b73 7065 6373 2873  .add_hookspecs(s
+00004480: 7973 2e6d 6f64 756c 6573 5b5f 5f6e 616d  ys.modules[__nam
+00004490: 655f 5f5d 290a 0a0a 5265 6769 7374 6572  e__])...Register
+000044a0: 696e 6720 6120 2a68 6f6f 6b69 6d70 6c2a  ing a *hookimpl*
+000044b0: 2077 6869 6368 2064 6f65 7320 6e6f 7420   which does not 
+000044c0: 6d65 6574 2074 6865 2063 6f6e 7374 7261  meet the constra
+000044d0: 696e 7473 206f 6620 6974 730a 636f 7272  ints of its.corr
+000044e0: 6573 706f 6e64 696e 6720 2a68 6f6f 6b73  esponding *hooks
+000044f0: 7065 632a 2077 696c 6c20 7265 7375 6c74  pec* will result
+00004500: 2069 6e20 616e 2065 7272 6f72 2e0a 0a41   in an error...A
+00004510: 202a 686f 6f6b 7370 6563 2a20 6361 6e20   *hookspec* can 
+00004520: 616c 736f 2062 6520 6164 6465 6420 2a2a  also be added **
+00004530: 6166 7465 722a 2a20 736f 6d65 202a 686f  after** some *ho
+00004540: 6f6b 696d 706c 732a 2068 6176 6520 6265  okimpls* have be
+00004550: 656e 0a72 6567 6973 7465 7265 6420 686f  en.registered ho
+00004560: 7765 7665 7220 7468 6973 2069 7320 6e6f  wever this is no
+00004570: 7420 6e6f 726d 616c 6c79 2072 6563 6f6d  t normally recom
+00004580: 6d65 6e64 6564 2061 7320 6974 2072 6573  mended as it res
+00004590: 756c 7473 2069 6e0a 6465 6c61 7965 6420  ults in.delayed 
+000045a0: 686f 6f6b 2076 616c 6964 6174 696f 6e2e  hook validation.
+000045b0: 0a0a 2e2e 206e 6f74 653a 3a0a 2020 2020  .... note::.    
+000045c0: 5468 6520 7465 726d 202a 686f 6f6b 7370  The term *hooksp
+000045d0: 6563 2a20 6361 6e20 736f 6d65 7469 6d65  ec* can sometime
+000045e0: 7320 7265 6665 7220 746f 2074 6865 2070  s refer to the p
+000045f0: 6c75 6769 6e2d 6e61 6d65 7370 6163 650a  lugin-namespace.
+00004600: 2020 2020 7768 6963 6820 6465 6669 6e65      which define
+00004610: 7320 6060 686f 6f6b 7370 6563 6060 2064  s ``hookspec`` d
+00004620: 6563 6f72 6174 6564 2066 756e 6374 696f  ecorated functio
+00004630: 6e73 2061 7320 696e 2074 6865 2063 6173  ns as in the cas
+00004640: 6520 6f66 0a20 2020 2060 6070 7974 6573  e of.    ``pytes
+00004650: 7460 6027 7320 6068 6f6f 6b73 7065 6320  t``'s `hookspec 
+00004660: 6d6f 6475 6c65 605f 0a0a 2e2e 205f 656e  module`_.... _en
+00004670: 666f 7263 696e 673a 0a0a 456e 666f 7263  forcing:..Enforc
+00004680: 696e 6720 7370 6563 2076 616c 6964 6174  ing spec validat
+00004690: 696f 6e0a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ion.^^^^^^^^^^^^
+000046a0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 4279  ^^^^^^^^^^^^^.By
+000046b0: 2064 6566 6175 6c74 2074 6865 7265 2069   default there i
+000046c0: 7320 6e6f 2073 7472 6963 7420 7265 7175  s no strict requ
+000046d0: 6972 656d 656e 7420 7468 6174 2065 6163  irement that eac
+000046e0: 6820 2a68 6f6f 6b69 6d70 6c2a 2068 6173  h *hookimpl* has
+000046f0: 0a61 2063 6f72 7265 7370 6f6e 6469 6e67  .a corresponding
+00004700: 202a 686f 6f6b 7370 6563 2a2e 2048 6f77   *hookspec*. How
+00004710: 6576 6572 2c20 6966 2079 6f75 2764 206c  ever, if you'd l
+00004720: 696b 6520 796f 7520 656e 666f 7263 6520  ike you enforce 
+00004730: 7468 6973 0a62 6568 6176 696f 7220 796f  this.behavior yo
+00004740: 7520 6361 6e20 7275 6e20 6120 6368 6563  u can run a chec
+00004750: 6b20 7769 7468 2074 6865 0a3a 7079 3a6d  k with the.:py:m
+00004760: 6574 683a 607e 706c 7567 6779 2e50 6c75  eth:`~pluggy.Plu
+00004770: 6769 6e4d 616e 6167 6572 2e63 6865 636b  ginManager.check
+00004780: 5f70 656e 6469 6e67 2829 6020 6d65 7468  _pending()` meth
+00004790: 6f64 2e20 4966 2079 6f75 2764 206c 696b  od. If you'd lik
+000047a0: 650a 746f 2065 6e66 6f72 6365 2072 6571  e.to enforce req
+000047b0: 7569 7369 7465 202a 686f 6f6b 7370 6563  uisite *hookspec
+000047c0: 732a 2062 7574 2077 6974 6820 6365 7274  s* but with cert
+000047d0: 6169 6e20 6578 6365 7074 696f 6e73 2066  ain exceptions f
+000047e0: 6f72 2073 6f6d 6520 686f 6f6b 730a 7468  or some hooks.th
+000047f0: 656e 206d 616b 6520 7375 7265 2074 6f20  en make sure to 
+00004800: 6d61 726b 2074 686f 7365 2068 6f6f 6b73  mark those hooks
+00004810: 2061 7320 3a72 6566 3a60 6f70 7469 6f6e   as :ref:`option
+00004820: 616c 203c 6f70 7469 6f6e 616c 686f 6f6b  al <optionalhook
+00004830: 3e60 2e0a 0a4f 7074 2d69 6e20 6172 6775  >`...Opt-in argu
+00004840: 6d65 6e74 730a 5e5e 5e5e 5e5e 5e5e 5e5e  ments.^^^^^^^^^^
+00004850: 5e5e 5e5e 5e5e 0a54 6f20 616c 6c6f 7720  ^^^^^^.To allow 
+00004860: 666f 7220 2a68 6f6f 6b73 7065 6373 2a20  for *hookspecs* 
+00004870: 746f 2065 766f 6c76 6520 6f76 6572 2074  to evolve over t
+00004880: 6865 206c 6966 6574 696d 6520 6f66 2061  he lifetime of a
+00004890: 2070 726f 6a65 6374 2c0a 2a68 6f6f 6b69   project,.*hooki
+000048a0: 6d70 6c73 2a20 6361 6e20 6163 6365 7074  mpls* can accept
+000048b0: 202a 2a6c 6573 732a 2a20 6172 6775 6d65   **less** argume
+000048c0: 6e74 7320 7468 616e 2064 6566 696e 6564  nts than defined
+000048d0: 2069 6e20 7468 6520 7370 6563 2e0a 5468   in the spec..Th
+000048e0: 6973 2061 6c6c 6f77 7320 666f 7220 6578  is allows for ex
+000048f0: 7465 6e64 696e 6720 686f 6f6b 2061 7267  tending hook arg
+00004900: 756d 656e 7473 2028 616e 6420 7468 7573  uments (and thus
+00004910: 2073 656d 616e 7469 6373 2920 7769 7468   semantics) with
+00004920: 6f75 740a 6272 6561 6b69 6e67 2065 7869  out.breaking exi
+00004930: 7374 696e 6720 2a68 6f6f 6b69 6d70 6c73  sting *hookimpls
+00004940: 2a2e 0a0a 496e 206f 7468 6572 2077 6f72  *...In other wor
+00004950: 6473 2074 6869 7320 6973 206f 6b3a 0a0a  ds this is ok:..
+00004960: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00004970: 7079 7468 6f6e 0a0a 2020 2020 4068 6f6f  python..    @hoo
+00004980: 6b73 7065 630a 2020 2020 6465 6620 6d79  kspec.    def my
+00004990: 686f 6f6b 2863 6f6e 6669 672c 2061 7267  hook(config, arg
+000049a0: 7329 3a0a 2020 2020 2020 2020 7061 7373  s):.        pass
+000049b0: 0a0a 0a20 2020 2040 686f 6f6b 696d 706c  ...    @hookimpl
+000049c0: 0a20 2020 2064 6566 206d 7968 6f6f 6b28  .    def myhook(
+000049d0: 6172 6773 293a 0a20 2020 2020 2020 2070  args):.        p
+000049e0: 7269 6e74 2861 7267 7329 0a0a 0a77 6865  rint(args)...whe
+000049f0: 7265 6173 2074 6869 7320 6973 206e 6f74  reas this is not
+00004a00: 3a0a 0a2e 2e20 636f 6465 2d62 6c6f 636b  :.... code-block
+00004a10: 3a3a 2070 7974 686f 6e0a 0a20 2020 2040  :: python..    @
+00004a20: 686f 6f6b 7370 6563 0a20 2020 2064 6566  hookspec.    def
+00004a30: 206d 7968 6f6f 6b28 636f 6e66 6967 2c20   myhook(config, 
+00004a40: 6172 6773 293a 0a20 2020 2020 2020 2070  args):.        p
+00004a50: 6173 730a 0a0a 2020 2020 4068 6f6f 6b69  ass...    @hooki
+00004a60: 6d70 6c0a 2020 2020 6465 6620 6d79 686f  mpl.    def myho
+00004a70: 6f6b 2863 6f6e 6669 672c 2061 7267 732c  ok(config, args,
+00004a80: 2065 7874 7261 5f61 7267 293a 0a20 2020   extra_arg):.   
+00004a90: 2020 2020 2070 7269 6e74 2861 7267 7329       print(args)
+00004aa0: 0a0a 2e2e 206e 6f74 653a 3a0a 2020 2020  .... note::.    
+00004ab0: 5468 6520 6f6e 6520 6578 6365 7074 696f  The one exceptio
+00004ac0: 6e20 746f 2074 6869 7320 7275 6c65 2028  n to this rule (
+00004ad0: 7468 6174 2061 202a 686f 6f6b 7370 6563  that a *hookspec
+00004ae0: 2a20 6d75 7374 2068 6176 6520 6173 206c  * must have as l
+00004af0: 6561 7374 2061 730a 2020 2020 6d61 6e79  east as.    many
+00004b00: 2061 7267 756d 656e 7473 2061 7320 6974   arguments as it
+00004b10: 7320 2a68 6f6f 6b69 6d70 6c73 2a29 2069  s *hookimpls*) i
+00004b20: 7320 7468 6520 636f 6e76 656e 7469 6f6e  s the convention
+00004b30: 616c 203a 7265 663a 6073 656c 6620 3c70  al :ref:`self <p
+00004b40: 7974 686f 6e3a 7475 742d 7265 6d61 726b  ython:tut-remark
+00004b50: 733e 6020 6172 673b 2074 6869 730a 2020  s>` arg; this.  
+00004b60: 2020 6973 2061 6c77 6179 7320 6967 6e6f    is always igno
+00004b70: 7265 6420 7768 656e 202a 686f 6f6b 696d  red when *hookim
+00004b80: 706c 732a 2061 7265 2064 6566 696e 6564  pls* are defined
+00004b90: 2061 7320 3a72 6566 3a60 6d65 7468 6f64   as :ref:`method
+00004ba0: 7320 3c70 7974 686f 6e3a 7475 742d 6d65  s <python:tut-me
+00004bb0: 7468 6f64 6f62 6a65 6374 733e 602e 0a0a  thodobjects>`...
+00004bc0: 2e2e 205f 6669 7273 7472 6573 756c 743a  .. _firstresult:
+00004bd0: 0a0a 4669 7273 7420 7265 7375 6c74 206f  ..First result o
+00004be0: 6e6c 790a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  nly.^^^^^^^^^^^^
+00004bf0: 5e5e 5e5e 5e0a 4120 2a68 6f6f 6b73 7065  ^^^^^.A *hookspe
+00004c00: 632a 2063 616e 2062 6520 6d61 726b 6564  c* can be marked
+00004c10: 2073 7563 6820 7468 6174 2077 6865 6e20   such that when 
+00004c20: 7468 6520 2a68 6f6f 6b2a 2069 7320 6361  the *hook* is ca
+00004c30: 6c6c 6564 2074 6865 2063 616c 6c20 6c6f  lled the call lo
+00004c40: 6f70 0a77 696c 6c20 6f6e 6c79 2069 6e76  op.will only inv
+00004c50: 6f6b 6520 7570 2074 6f20 7468 6520 6669  oke up to the fi
+00004c60: 7273 7420 2a68 6f6f 6b69 6d70 6c2a 2077  rst *hookimpl* w
+00004c70: 6869 6368 2072 6574 7572 6e73 2061 2072  hich returns a r
+00004c80: 6573 756c 7420 6f74 6865 720a 7468 616e  esult other.than
+00004c90: 2060 604e 6f6e 6560 602e 0a0a 2e2e 2063   ``None``..... c
+00004ca0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00004cb0: 6f6e 0a0a 2020 2020 4068 6f6f 6b73 7065  on..    @hookspe
+00004cc0: 6328 6669 7273 7472 6573 756c 743d 5472  c(firstresult=Tr
+00004cd0: 7565 290a 2020 2020 6465 6620 6d79 686f  ue).    def myho
+00004ce0: 6f6b 2863 6f6e 6669 672c 2061 7267 7329  ok(config, args)
+00004cf0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00004d00: 5468 6973 2063 616e 2062 6520 7573 6566  This can be usef
+00004d10: 756c 2066 6f72 206f 7074 696d 697a 696e  ul for optimizin
+00004d20: 6720 6120 6361 6c6c 206c 6f6f 7020 666f  g a call loop fo
+00004d30: 7220 7768 6963 6820 796f 7520 6172 6520  r which you are 
+00004d40: 6f6e 6c79 0a69 6e74 6572 6573 7465 6420  only.interested 
+00004d50: 696e 2061 2073 696e 676c 6520 636f 7265  in a single core
+00004d60: 202a 686f 6f6b 696d 706c 2a2e 2041 6e20   *hookimpl*. An 
+00004d70: 6578 616d 706c 6520 6973 2074 6865 0a3a  example is the.:
+00004d80: 6675 6e63 3a60 7e5f 7079 7465 7374 2e68  func:`~_pytest.h
+00004d90: 6f6f 6b73 7065 632e 7079 7465 7374 5f63  ookspec.pytest_c
+00004da0: 6d64 6c69 6e65 5f6d 6169 6e60 2063 656e  mdline_main` cen
+00004db0: 7472 616c 2072 6f75 7469 6e65 206f 6620  tral routine of 
+00004dc0: 6060 7079 7465 7374 6060 2e0a 4e6f 7465  ``pytest``..Note
+00004dd0: 2074 6861 7420 616c 6c20 686f 6f6b 2077   that all hook w
+00004de0: 7261 7070 6572 7320 6172 6520 7374 696c  rappers are stil
+00004df0: 6c20 696e 766f 6b65 6420 7769 7468 2074  l invoked with t
+00004e00: 6865 2066 6972 7374 2072 6573 756c 742e  he first result.
+00004e10: 0a0a 416c 736f 2073 6565 2074 6865 203a  ..Also see the :
+00004e20: 7265 663a 6070 7974 6573 743a 6669 7273  ref:`pytest:firs
+00004e30: 7472 6573 756c 7460 2073 6563 7469 6f6e  tresult` section
+00004e40: 2069 6e20 7468 6520 6060 7079 7465 7374   in the ``pytest
+00004e50: 6060 2064 6f63 732e 0a0a 2e2e 205f 6869  `` docs..... _hi
+00004e60: 7374 6f72 6963 3a0a 0a48 6973 746f 7269  storic:..Histori
+00004e70: 6320 686f 6f6b 730a 5e5e 5e5e 5e5e 5e5e  c hooks.^^^^^^^^
+00004e80: 5e5e 5e5e 5e5e 0a59 6f75 2063 616e 206d  ^^^^^^.You can m
+00004e90: 6172 6b20 6120 2a68 6f6f 6b73 7065 632a  ark a *hookspec*
+00004ea0: 2061 7320 6265 696e 6720 2a68 6973 746f   as being *histo
+00004eb0: 7269 632a 206d 6561 6e69 6e67 2074 6861  ric* meaning tha
+00004ec0: 7420 7468 6520 686f 6f6b 0a63 616e 2062  t the hook.can b
+00004ed0: 6520 6361 6c6c 6564 2077 6974 6820 3a70  e called with :p
+00004ee0: 793a 6d65 7468 3a60 7e70 6c75 6767 792e  y:meth:`~pluggy.
+00004ef0: 5f68 6f6f 6b73 2e5f 486f 6f6b 4361 6c6c  _hooks._HookCall
+00004f00: 6572 2e63 616c 6c5f 6869 7374 6f72 6963  er.call_historic
+00004f10: 2829 6020 2a2a 6265 666f 7265 2a2a 0a68  ()` **before**.h
+00004f20: 6176 696e 6720 6265 656e 2072 6567 6973  aving been regis
+00004f30: 7465 7265 643a 0a0a 2e2e 2063 6f64 652d  tered:.... code-
+00004f40: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+00004f50: 2020 2020 4068 6f6f 6b73 7065 6328 6869      @hookspec(hi
+00004f60: 7374 6f72 6963 3d54 7275 6529 0a20 2020  storic=True).   
+00004f70: 2064 6566 206d 7968 6f6f 6b28 636f 6e66   def myhook(conf
+00004f80: 6967 2c20 6172 6773 293a 0a20 2020 2020  ig, args):.     
+00004f90: 2020 2070 6173 730a 0a54 6865 2069 6d70     pass..The imp
+00004fa0: 6c69 6361 7469 6f6e 2069 7320 7468 6174  lication is that
+00004fb0: 206c 6174 6520 7265 6769 7374 6572 6564   late registered
+00004fc0: 202a 686f 6f6b 696d 706c 732a 2077 696c   *hookimpls* wil
+00004fd0: 6c20 6265 2063 616c 6c65 6420 6261 636b  l be called back
+00004fe0: 0a69 6d6d 6564 6961 7465 6c79 2061 7420  .immediately at 
+00004ff0: 7265 6769 7374 6572 2074 696d 6520 616e  register time an
+00005000: 6420 2a2a 6361 6e20 6e6f 742a 2a20 7265  d **can not** re
+00005010: 7475 726e 2061 2072 6573 756c 7420 746f  turn a result to
+00005020: 2074 6865 2063 616c 6c65 722e 0a0a 5468   the caller...Th
+00005030: 6973 2074 7572 6e73 206f 7574 2074 6f20  is turns out to 
+00005040: 6265 2070 6172 7469 6375 6c61 726c 7920  be particularly 
+00005050: 7573 6566 756c 2077 6865 6e20 6465 616c  useful when deal
+00005060: 696e 6720 7769 7468 206c 617a 7920 6f72  ing with lazy or
+00005070: 0a64 796e 616d 6963 616c 6c79 206c 6f61  .dynamically loa
+00005080: 6465 6420 706c 7567 696e 732e 0a0a 466f  ded plugins...Fo
+00005090: 7220 6d6f 7265 2069 6e66 6f20 7365 6520  r more info see 
+000050a0: 3a72 6566 3a60 6361 6c6c 5f68 6973 746f  :ref:`call_histo
+000050b0: 7269 6360 2e0a 0a0a 5761 726e 696e 6773  ric`....Warnings
+000050c0: 206f 6e20 686f 6f6b 2069 6d70 6c65 6d65   on hook impleme
+000050d0: 6e74 6174 696f 6e0a 5e5e 5e5e 5e5e 5e5e  ntation.^^^^^^^^
+000050e0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+000050f0: 5e5e 5e5e 5e5e 5e0a 0a41 7320 7072 6f6a  ^^^^^^^..As proj
+00005100: 6563 7473 2065 766f 6c76 6520 6e65 7720  ects evolve new 
+00005110: 686f 6f6b 7320 6d61 7920 6265 2069 6e74  hooks may be int
+00005120: 726f 6475 6365 6420 616e 642f 6f72 2064  roduced and/or d
+00005130: 6570 7265 6361 7465 642e 0a0a 6966 2061  eprecated...if a
+00005140: 2068 6f6f 6b73 7065 6320 7370 6563 6966   hookspec specif
+00005150: 6965 7320 6120 6060 7761 726e 5f6f 6e5f  ies a ``warn_on_
+00005160: 696d 706c 6060 2c20 706c 7567 6779 2077  impl``, pluggy w
+00005170: 696c 6c20 7472 6967 6765 7220 6974 2066  ill trigger it f
+00005180: 6f72 2061 6e79 2070 6c75 6769 6e20 696d  or any plugin im
+00005190: 706c 656d 656e 7469 6e67 2074 6865 2068  plementing the h
+000051a0: 6f6f 6b2e 0a0a 0a2e 2e20 636f 6465 2d62  ook...... code-b
+000051b0: 6c6f 636b 3a3a 2070 7974 686f 6e0a 0a20  lock:: python.. 
+000051c0: 2020 2040 686f 6f6b 7370 6563 280a 2020     @hookspec(.  
+000051d0: 2020 2020 2020 7761 726e 5f6f 6e5f 696d        warn_on_im
+000051e0: 706c 3d44 6570 7265 6361 7469 6f6e 5761  pl=DeprecationWa
+000051f0: 726e 696e 6728 226f 6c64 686f 6f6b 2069  rning("oldhook i
+00005200: 7320 6465 7072 6563 6174 6564 2061 6e64  s deprecated and
+00005210: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
+00005220: 2073 6f6f 6e22 290a 2020 2020 290a 2020   soon").    ).  
+00005230: 2020 6465 6620 6f6c 6468 6f6f 6b28 293a    def oldhook():
+00005240: 0a20 2020 2020 2020 2070 6173 730a 0a2e  .        pass...
+00005250: 2e20 5f6d 616e 6167 653a 0a0a 5468 6520  . _manage:..The 
+00005260: 506c 7567 696e 2072 6567 6973 7472 790a  Plugin registry.
+00005270: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00005280: 2a2a 2a0a 6060 706c 7567 6779 6060 206d  ***.``pluggy`` m
+00005290: 616e 6167 6573 2070 6c75 6769 6e73 2075  anages plugins u
+000052a0: 7369 6e67 2069 6e73 7461 6e63 6573 206f  sing instances o
+000052b0: 6620 7468 650a 3a70 793a 636c 6173 733a  f the.:py:class:
+000052c0: 6070 6c75 6767 792e 506c 7567 696e 4d61  `pluggy.PluginMa
+000052d0: 6e61 6765 7260 2e0a 0a41 203a 7079 3a63  nager`...A :py:c
+000052e0: 6c61 7373 3a60 7e70 6c75 6767 792e 506c  lass:`~pluggy.Pl
+000052f0: 7567 696e 4d61 6e61 6765 7260 2069 7320  uginManager` is 
+00005300: 696e 7374 616e 7469 6174 6564 2077 6974  instantiated wit
+00005310: 6820 6120 7369 6e67 6c65 0a60 6073 7472  h a single.``str
+00005320: 6060 2061 7267 756d 656e 742c 2074 6865  `` argument, the
+00005330: 2060 6070 726f 6a65 6374 5f6e 616d 6560   ``project_name`
+00005340: 603a 0a0a 2e2e 2063 6f64 652d 626c 6f63  `:.... code-bloc
+00005350: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
+00005360: 696d 706f 7274 2070 6c75 6767 790a 0a20  import pluggy.. 
+00005370: 2020 2070 6d20 3d20 706c 7567 6779 2e50     pm = pluggy.P
+00005380: 6c75 6769 6e4d 616e 6167 6572 2822 6d79  luginManager("my
+00005390: 5f70 726f 6a65 6374 5f6e 616d 6522 290a  _project_name").
+000053a0: 0a0a 5468 6520 6060 7072 6f6a 6563 745f  ..The ``project_
+000053b0: 6e61 6d65 6060 2076 616c 7565 2069 7320  name`` value is 
+000053c0: 7573 6564 2077 6865 6e20 6120 3a70 793a  used when a :py:
+000053d0: 636c 6173 733a 607e 706c 7567 6779 2e50  class:`~pluggy.P
+000053e0: 6c75 6769 6e4d 616e 6167 6572 600a 7363  luginManager`.sc
+000053f0: 616e 7320 666f 7220 2a68 6f6f 6b2a 2066  ans for *hook* f
+00005400: 756e 6374 696f 6e73 203a 7265 663a 6064  unctions :ref:`d
+00005410: 6566 696e 6564 206f 6e20 6120 706c 7567  efined on a plug
+00005420: 696e 203c 6465 6669 6e65 3e60 2e0a 5468  in <define>`..Th
+00005430: 6973 2061 6c6c 6f77 7320 666f 7220 6d75  is allows for mu
+00005440: 6c74 6970 6c65 2070 6c75 6769 6e20 6d61  ltiple plugin ma
+00005450: 6e61 6765 7273 2066 726f 6d20 6d75 6c74  nagers from mult
+00005460: 6970 6c65 2070 726f 6a65 6374 730a 746f  iple projects.to
+00005470: 2064 6566 696e 6520 686f 6f6b 7320 616c   define hooks al
+00005480: 6f6e 6773 6964 6520 6561 6368 206f 7468  ongside each oth
+00005490: 6572 2e0a 0a2e 2e20 5f72 6567 6973 7472  er..... _registr
+000054a0: 6174 696f 6e3a 0a0a 5265 6769 7374 7261  ation:..Registra
+000054b0: 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  tion.-----------
+000054c0: 2d0a 4561 6368 203a 7079 3a63 6c61 7373  -.Each :py:class
+000054d0: 3a60 7e70 6c75 6767 792e 506c 7567 696e  :`~pluggy.Plugin
+000054e0: 4d61 6e61 6765 7260 206d 6169 6e74 6169  Manager` maintai
+000054f0: 6e73 2061 202a 706c 7567 696e 2a20 7265  ns a *plugin* re
+00005500: 6769 7374 7279 2077 6865 7265 2065 6163  gistry where eac
+00005510: 6820 2a70 6c75 6769 6e2a 0a63 6f6e 7461  h *plugin*.conta
+00005520: 696e 7320 6120 7365 7420 6f66 202a 686f  ins a set of *ho
+00005530: 6f6b 696d 706c 2a20 6465 6669 6e69 7469  okimpl* definiti
+00005540: 6f6e 732e 204c 6f61 6469 6e67 202a 686f  ons. Loading *ho
+00005550: 6f6b 696d 706c 2a20 616e 6420 2a68 6f6f  okimpl* and *hoo
+00005560: 6b73 7065 632a 0a64 6566 696e 6974 696f  kspec*.definitio
+00005570: 6e73 2074 6f20 706f 7075 6c61 7465 2074  ns to populate t
+00005580: 6865 2072 6567 6973 7472 7920 6973 2064  he registry is d
+00005590: 6573 6372 6962 6564 2069 6e20 6465 7461  escribed in deta
+000055a0: 696c 2069 6e20 7468 6520 7365 6374 696f  il in the sectio
+000055b0: 6e20 6f6e 0a3a 7265 663a 6064 6566 696e  n on.:ref:`defin
+000055c0: 6560 2e0a 0a49 6e20 7375 6d6d 6172 792c  e`...In summary,
+000055d0: 2079 6f75 2070 6173 7320 6120 706c 7567   you pass a plug
+000055e0: 696e 206e 616d 6573 7061 6365 206f 626a  in namespace obj
+000055f0: 6563 7420 746f 2074 6865 0a3a 7079 3a6d  ect to the.:py:m
+00005600: 6574 683a 607e 706c 7567 6779 2e50 6c75  eth:`~pluggy.Plu
+00005610: 6769 6e4d 616e 6167 6572 2e72 6567 6973  ginManager.regis
+00005620: 7465 7228 2960 2061 6e64 0a3a 7079 3a6d  ter()` and.:py:m
+00005630: 6574 683a 607e 706c 7567 6779 2e50 6c75  eth:`~pluggy.Plu
+00005640: 6769 6e4d 616e 6167 6572 2e61 6464 5f68  ginManager.add_h
+00005650: 6f6f 6b73 7065 6373 2829 6020 6d65 7468  ookspecs()` meth
+00005660: 6f64 7320 746f 2063 6f6c 6c65 6374 0a68  ods to collect.h
+00005670: 6f6f 6b20 2a69 6d70 6c65 6d65 6e74 6174  ook *implementat
+00005680: 696f 6e73 2a20 616e 6420 2a73 7065 6369  ions* and *speci
+00005690: 6669 6361 7469 6f6e 732a 2066 726f 6d20  fications* from 
+000056a0: 2a70 6c75 6769 6e2a 206e 616d 6573 7061  *plugin* namespa
+000056b0: 6365 7320 7265 7370 6563 7469 7665 6c79  ces respectively
+000056c0: 2e0a 0a59 6f75 2063 616e 2075 6e72 6567  ...You can unreg
+000056d0: 6973 7465 7220 616e 7920 2a70 6c75 6769  ister any *plugi
+000056e0: 6e2a 2773 2068 6f6f 6b73 2075 7369 6e67  n*'s hooks using
+000056f0: 0a3a 7079 3a6d 6574 683a 607e 706c 7567  .:py:meth:`~plug
+00005700: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
+00005710: 2e75 6e72 6567 6973 7465 7228 2960 2061  .unregister()` a
+00005720: 6e64 2063 6865 636b 2069 6620 6120 706c  nd check if a pl
+00005730: 7567 696e 2069 730a 7265 6769 7374 6572  ugin is.register
+00005740: 6564 2062 7920 7061 7373 696e 6720 6974  ed by passing it
+00005750: 7320 6e61 6d65 2074 6f20 7468 650a 3a70  s name to the.:p
+00005760: 793a 6d65 7468 3a60 7e70 6c75 6767 792e  y:meth:`~pluggy.
+00005770: 506c 7567 696e 4d61 6e61 6765 722e 6973  PluginManager.is
+00005780: 5f72 6567 6973 7465 7265 6428 2960 206d  _registered()` m
+00005790: 6574 686f 642e 0a0a 4c6f 6164 696e 6720  ethod...Loading 
+000057a0: 6060 7365 7475 7074 6f6f 6c73 6060 2065  ``setuptools`` e
+000057b0: 6e74 7279 2070 6f69 6e74 730a 5e5e 5e5e  ntry points.^^^^
+000057c0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+000057d0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  ^^^^^^^^^^^^^^^.
+000057e0: 596f 7520 6361 6e20 6175 746f 6d61 7469  You can automati
+000057f0: 6361 6c6c 7920 6c6f 6164 2070 6c75 6769  cally load plugi
+00005800: 6e73 2072 6567 6973 7465 7265 6420 7468  ns registered th
+00005810: 726f 7567 680a 3a72 6566 3a60 7365 7475  rough.:ref:`setu
+00005820: 7074 6f6f 6c73 2065 6e74 7279 2070 6f69  ptools entry poi
+00005830: 6e74 7320 3c73 6574 7570 746f 6f6c 733a  nts <setuptools:
+00005840: 656e 7472 795f 706f 696e 7473 3e60 0a77  entry_points>`.w
+00005850: 6974 6820 7468 6520 3a70 793a 6d65 7468  ith the :py:meth
+00005860: 3a60 7e70 6c75 6767 792e 506c 7567 696e  :`~pluggy.Plugin
+00005870: 4d61 6e61 6765 722e 6c6f 6164 5f73 6574  Manager.load_set
+00005880: 7570 746f 6f6c 735f 656e 7472 7970 6f69  uptools_entrypoi
+00005890: 6e74 7328 2960 0a6d 6574 686f 642e 0a0a  nts()`.method...
+000058a0: 416e 2065 7861 6d70 6c65 2075 7365 206f  An example use o
+000058b0: 6620 7468 6973 2069 7320 7468 6520 3a72  f this is the :r
+000058c0: 6566 3a60 7079 7465 7374 2065 6e74 7279  ef:`pytest entry
+000058d0: 2070 6f69 6e74 203c 7079 7465 7374 3a70   point <pytest:p
+000058e0: 6970 2d69 6e73 7461 6c6c 6162 6c65 2070  ip-installable p
+000058f0: 6c75 6769 6e73 3e60 2e0a 0a0a 426c 6f63  lugins>`....Bloc
+00005900: 6b69 6e67 0a2d 2d2d 2d2d 2d2d 2d0a 596f  king.--------.Yo
+00005910: 7520 6361 6e20 626c 6f63 6b20 616e 7920  u can block any 
+00005920: 706c 7567 696e 2066 726f 6d20 6265 696e  plugin from bein
+00005930: 6720 7265 6769 7374 6572 6564 2075 7369  g registered usi
+00005940: 6e67 0a3a 7079 3a6d 6574 683a 607e 706c  ng.:py:meth:`~pl
+00005950: 7567 6779 2e50 6c75 6769 6e4d 616e 6167  uggy.PluginManag
+00005960: 6572 2e73 6574 5f62 6c6f 636b 6564 2829  er.set_blocked()
+00005970: 6020 616e 6420 6368 6563 6b20 6966 2061  ` and check if a
+00005980: 2067 6976 656e 0a2a 706c 7567 696e 2a20   given.*plugin* 
+00005990: 6973 2062 6c6f 636b 6564 2062 7920 6e61  is blocked by na
+000059a0: 6d65 2075 7369 6e67 203a 7079 3a6d 6574  me using :py:met
+000059b0: 683a 607e 706c 7567 6779 2e50 6c75 6769  h:`~pluggy.Plugi
+000059c0: 6e4d 616e 6167 6572 2e69 735f 626c 6f63  nManager.is_bloc
+000059d0: 6b65 6428 2960 2e0a 0a0a 496e 7370 6563  ked()`....Inspec
+000059e0: 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d0a  tion.----------.
+000059f0: 596f 7520 6361 6e20 7573 6520 6120 7661  You can use a va
+00005a00: 7269 6574 7920 6f66 206d 6574 686f 6473  riety of methods
+00005a10: 2074 6f20 696e 7370 6563 7420 626f 7468   to inspect both
+00005a20: 2074 6865 2072 6567 6973 7472 790a 616e   the registry.an
+00005a30: 6420 7061 7274 6963 756c 6172 2070 6c75  d particular plu
+00005a40: 6769 6e73 2069 6e20 6974 3a0a 0a2d 203a  gins in it:..- :
+00005a50: 7079 3a6d 6574 683a 607e 706c 7567 6779  py:meth:`~pluggy
+00005a60: 2e50 6c75 6769 6e4d 616e 6167 6572 2e6c  .PluginManager.l
+00005a70: 6973 745f 6e61 6d65 5f70 6c75 6769 6e28  ist_name_plugin(
+00005a80: 2960 202d 0a20 2072 6574 7572 6e20 6120  )` -.  return a 
+00005a90: 6c69 7374 206f 6620 6e61 6d65 2d70 6c75  list of name-plu
+00005aa0: 6769 6e20 7061 6972 730a 2d20 3a70 793a  gin pairs.- :py:
+00005ab0: 6d65 7468 3a60 7e70 6c75 6767 792e 506c  meth:`~pluggy.Pl
+00005ac0: 7567 696e 4d61 6e61 6765 722e 6765 745f  uginManager.get_
+00005ad0: 706c 7567 696e 7328 2960 202d 2072 6574  plugins()` - ret
+00005ae0: 7269 6576 6520 616c 6c20 706c 7567 696e  rieve all plugin
+00005af0: 730a 2d20 3a70 793a 6d65 7468 3a60 7e70  s.- :py:meth:`~p
+00005b00: 6c75 6767 792e 506c 7567 696e 4d61 6e61  luggy.PluginMana
+00005b10: 6765 722e 6765 745f 6361 6e6f 6e69 6361  ger.get_canonica
+00005b20: 6c5f 6e61 6d65 2829 602d 2067 6574 2061  l_name()`- get a
+00005b30: 202a 706c 7567 696e 2a27 730a 2020 6361   *plugin*'s.  ca
+00005b40: 6e6f 6e69 6361 6c20 6e61 6d65 2028 7468  nonical name (th
+00005b50: 6520 6e61 6d65 2069 7420 7761 7320 7265  e name it was re
+00005b60: 6769 7374 6572 6564 2077 6974 6829 0a2d  gistered with).-
+00005b70: 203a 7079 3a6d 6574 683a 607e 706c 7567   :py:meth:`~plug
+00005b80: 6779 2e50 6c75 6769 6e4d 616e 6167 6572  gy.PluginManager
+00005b90: 2e67 6574 5f70 6c75 6769 6e28 2960 202d  .get_plugin()` -
+00005ba0: 2072 6574 7269 6576 6520 6120 706c 7567   retrieve a plug
+00005bb0: 696e 2062 7920 6974 730a 2020 6361 6e6f  in by its.  cano
+00005bc0: 6e69 6361 6c20 6e61 6d65 0a0a 0a50 6172  nical name...Par
+00005bd0: 7369 6e67 206d 6172 6b20 6f70 7469 6f6e  sing mark option
+00005be0: 730a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  s.^^^^^^^^^^^^^^
+00005bf0: 5e5e 5e5e 5e5e 0a59 6f75 2063 616e 2072  ^^^^^^.You can r
+00005c00: 6574 7269 6576 6520 7468 6520 2a6f 7074  etrieve the *opt
+00005c10: 696f 6e73 2a20 6170 706c 6965 6420 746f  ions* applied to
+00005c20: 2061 2070 6172 7469 6375 6c61 720a 2a68   a particular.*h
+00005c30: 6f6f 6b73 7065 632a 206f 7220 2a68 6f6f  ookspec* or *hoo
+00005c40: 6b69 6d70 6c2a 2061 7320 7065 7220 3a72  kimpl* as per :r
+00005c50: 6566 3a60 6d61 726b 696e 675f 686f 6f6b  ef:`marking_hook
+00005c60: 7360 2075 7369 6e67 2074 6865 0a3a 7079  s` using the.:py
+00005c70: 3a6d 6574 683a 607e 706c 7567 6779 2e50  :meth:`~pluggy.P
+00005c80: 6c75 6769 6e4d 616e 6167 6572 2e70 6172  luginManager.par
+00005c90: 7365 5f68 6f6f 6b73 7065 635f 6f70 7473  se_hookspec_opts
+00005ca0: 2829 6020 616e 640a 3a70 793a 6d65 7468  ()` and.:py:meth
+00005cb0: 3a60 7e70 6c75 6767 792e 506c 7567 696e  :`~pluggy.Plugin
+00005cc0: 4d61 6e61 6765 722e 7061 7273 655f 686f  Manager.parse_ho
+00005cd0: 6f6b 696d 706c 5f6f 7074 7328 2960 2072  okimpl_opts()` r
+00005ce0: 6573 7065 6374 6976 656c 792e 0a0a 0a2e  espectively.....
+00005cf0: 2e20 5f63 616c 6c69 6e67 3a0a 0a43 616c  . _calling:..Cal
+00005d00: 6c69 6e67 2068 6f6f 6b73 0a2a 2a2a 2a2a  ling hooks.*****
+00005d10: 2a2a 2a2a 2a2a 2a2a 0a54 6865 2063 6f72  ********.The cor
+00005d20: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
+00005d30: 6f66 2060 6070 6c75 6767 7960 6020 656e  of ``pluggy`` en
+00005d40: 6162 6c65 7320 616e 2065 7874 656e 7369  ables an extensi
+00005d50: 6f6e 2070 726f 7669 6465 720a 746f 206f  on provider.to o
+00005d60: 7665 7272 6964 6520 6675 6e63 7469 6f6e  verride function
+00005d70: 2063 616c 6c73 206d 6164 6520 6174 2063   calls made at c
+00005d80: 6572 7461 696e 2070 6f69 6e74 7320 7468  ertain points th
+00005d90: 726f 7567 686f 7574 2061 2070 726f 6772  roughout a progr
+00005da0: 616d 2e0a 0a41 2070 6172 7469 6375 6c61  am...A particula
+00005db0: 7220 2a68 6f6f 6b2a 2069 7320 696e 766f  r *hook* is invo
+00005dc0: 6b65 6420 6279 2063 616c 6c69 6e67 2061  ked by calling a
+00005dd0: 6e20 696e 7374 616e 6365 206f 660a 6120  n instance of.a 
+00005de0: 3a70 793a 636c 6173 733a 6070 6c75 6767  :py:class:`plugg
+00005df0: 792e 5f68 6f6f 6b73 2e5f 486f 6f6b 4361  y._hooks._HookCa
+00005e00: 6c6c 6572 6020 7768 6963 6820 696e 2074  ller` which in t
+00005e10: 7572 6e20 2a6c 6f6f 7073 2a20 7468 726f  urn *loops* thro
+00005e20: 7567 6820 7468 650a 6060 313a 4e60 6020  ugh the.``1:N`` 
+00005e30: 7265 6769 7374 6572 6564 202a 686f 6f6b  registered *hook
+00005e40: 696d 706c 732a 2061 6e64 2063 616c 6c73  impls* and calls
+00005e50: 2074 6865 6d20 696e 2073 6571 7565 6e63   them in sequenc
+00005e60: 652e 0a0a 4576 6572 7920 3a70 793a 636c  e...Every :py:cl
+00005e70: 6173 733a 607e 706c 7567 6779 2e50 6c75  ass:`~pluggy.Plu
+00005e80: 6769 6e4d 616e 6167 6572 6020 6861 7320  ginManager` has 
+00005e90: 6120 6060 686f 6f6b 6060 2061 7474 7269  a ``hook`` attri
+00005ea0: 6275 7465 0a77 6869 6368 2069 7320 616e  bute.which is an
+00005eb0: 2069 6e73 7461 6e63 6520 6f66 2074 6869   instance of thi
+00005ec0: 7320 3a70 793a 636c 6173 733a 6070 6c75  s :py:class:`plu
+00005ed0: 6767 792e 5f68 6f6f 6b73 2e5f 486f 6f6b  ggy._hooks._Hook
+00005ee0: 5265 6c61 7960 2e0a 5468 6520 3a70 793a  Relay`..The :py:
+00005ef0: 636c 6173 733a 607e 706c 7567 6779 2e5f  class:`~pluggy._
+00005f00: 686f 6f6b 732e 5f48 6f6f 6b52 656c 6179  hooks._HookRelay
+00005f10: 6020 6974 7365 6c66 2063 6f6e 7461 696e  ` itself contain
+00005f20: 7320 7265 6665 7265 6e63 6573 0a28 6279  s references.(by
+00005f30: 2068 6f6f 6b20 6e61 6d65 2920 746f 2065   hook name) to e
+00005f40: 6163 6820 7265 6769 7374 6572 6564 202a  ach registered *
+00005f50: 686f 6f6b 696d 706c 2a27 7320 3a70 793a  hookimpl*'s :py:
+00005f60: 636c 6173 733a 607e 706c 7567 6779 2e5f  class:`~pluggy._
+00005f70: 686f 6f6b 732e 5f48 6f6f 6b43 616c 6c65  hooks._HookCalle
+00005f80: 7260 2069 6e73 7461 6e63 652e 0a0a 4d6f  r` instance...Mo
+00005f90: 7265 2070 7261 6374 6963 616c 6c79 2079  re practically y
+00005fa0: 6f75 2063 616c 6c20 6120 2a68 6f6f 6b2a  ou call a *hook*
+00005fb0: 206c 696b 6520 736f 3a0a 0a2e 2e20 636f   like so:.... co
+00005fc0: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+00005fd0: 6e0a 0a20 2020 2069 6d70 6f72 7420 7379  n..    import sy
+00005fe0: 730a 2020 2020 696d 706f 7274 2070 6c75  s.    import plu
+00005ff0: 6767 790a 2020 2020 696d 706f 7274 206d  ggy.    import m
+00006000: 7970 6c75 6769 6e73 7065 630a 2020 2020  ypluginspec.    
+00006010: 696d 706f 7274 206d 7970 6c75 6769 6e0a  import myplugin.
+00006020: 2020 2020 6672 6f6d 2063 6f6e 6669 6775      from configu
+00006030: 7261 7469 6f6e 2069 6d70 6f72 7420 636f  ration import co
+00006040: 6e66 6967 0a0a 2020 2020 706d 203d 2070  nfig..    pm = p
+00006050: 6c75 6767 792e 506c 7567 696e 4d61 6e61  luggy.PluginMana
+00006060: 6765 7228 226d 7970 726f 6a65 6374 2229  ger("myproject")
+00006070: 0a20 2020 2070 6d2e 6164 645f 686f 6f6b  .    pm.add_hook
+00006080: 7370 6563 7328 6d79 706c 7567 696e 7370  specs(mypluginsp
+00006090: 6563 290a 2020 2020 706d 2e72 6567 6973  ec).    pm.regis
+000060a0: 7465 7228 6d79 706c 7567 696e 290a 0a20  ter(myplugin).. 
+000060b0: 2020 2023 2077 6520 696e 766f 6b65 2074     # we invoke t
+000060c0: 6865 205f 486f 6f6b 4361 6c6c 6572 2061  he _HookCaller a
+000060d0: 6e64 2074 6875 7320 616c 6c20 756e 6465  nd thus all unde
+000060e0: 726c 7969 6e67 2068 6f6f 6b69 6d70 6c73  rlying hookimpls
+000060f0: 0a20 2020 2072 6573 756c 745f 6c69 7374  .    result_list
+00006100: 203d 2070 6d2e 686f 6f6b 2e6d 7968 6f6f   = pm.hook.myhoo
+00006110: 6b28 636f 6e66 6967 3d63 6f6e 6669 672c  k(config=config,
+00006120: 2061 7267 733d 7379 732e 6172 6776 290a   args=sys.argv).
+00006130: 0a4e 6f74 6520 7468 6174 2079 6f75 202a  .Note that you *
+00006140: 2a6d 7573 742a 2a20 6361 6c6c 2068 6f6f  *must** call hoo
+00006150: 6b73 2075 7369 6e67 206b 6579 776f 7264  ks using keyword
+00006160: 203a 7374 643a 7465 726d 3a60 7079 7468   :std:term:`pyth
+00006170: 6f6e 3a61 7267 756d 656e 7460 2073 796e  on:argument` syn
+00006180: 7461 7821 0a0a 486f 6f6b 2069 6d70 6c65  tax!..Hook imple
+00006190: 6d65 6e74 6174 696f 6e73 2061 7265 2063  mentations are c
+000061a0: 616c 6c65 6420 696e 204c 4946 4f20 7265  alled in LIFO re
+000061b0: 6769 7374 6572 6564 206f 7264 6572 3a20  gistered order: 
+000061c0: 2a74 6865 206c 6173 740a 7265 6769 7374  *the last.regist
+000061d0: 6572 6564 2070 6c75 6769 6e27 7320 686f  ered plugin's ho
+000061e0: 6f6b 7320 6172 6520 6361 6c6c 6564 2066  oks are called f
+000061f0: 6972 7374 2a2e 2041 7320 616e 2065 7861  irst*. As an exa
+00006200: 6d70 6c65 2c20 7468 6520 6265 6c6f 770a  mple, the below.
+00006210: 6173 7365 7274 696f 6e20 7368 6f75 6c64  assertion should
+00006220: 206e 6f74 2065 7272 6f72 3a0a 0a2e 2e20   not error:.... 
+00006230: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00006240: 686f 6e0a 0a20 2020 2066 726f 6d20 706c  hon..    from pl
+00006250: 7567 6779 2069 6d70 6f72 7420 506c 7567  uggy import Plug
+00006260: 696e 4d61 6e61 6765 722c 2048 6f6f 6b69  inManager, Hooki
+00006270: 6d70 6c4d 6172 6b65 720a 0a20 2020 2068  mplMarker..    h
+00006280: 6f6f 6b69 6d70 6c20 3d20 486f 6f6b 696d  ookimpl = Hookim
+00006290: 706c 4d61 726b 6572 2822 6d79 7072 6f6a  plMarker("myproj
+000062a0: 6563 7422 290a 0a0a 2020 2020 636c 6173  ect")...    clas
+000062b0: 7320 506c 7567 696e 313a 0a20 2020 2020  s Plugin1:.     
+000062c0: 2020 2040 686f 6f6b 696d 706c 0a20 2020     @hookimpl.   
+000062d0: 2020 2020 2064 6566 206d 7968 6f6f 6b28       def myhook(
+000062e0: 7365 6c66 2c20 6172 6773 293a 0a20 2020  self, args):.   
+000062f0: 2020 2020 2020 2020 2022 2222 4465 6661           """Defa
+00006300: 756c 7420 696d 706c 656d 656e 7461 7469  ult implementati
+00006310: 6f6e 2e22 2222 0a20 2020 2020 2020 2020  on.""".         
+00006320: 2020 2072 6574 7572 6e20 310a 0a0a 2020     return 1...  
+00006330: 2020 636c 6173 7320 506c 7567 696e 323a    class Plugin2:
+00006340: 0a20 2020 2020 2020 2040 686f 6f6b 696d  .        @hookim
+00006350: 706c 0a20 2020 2020 2020 2064 6566 206d  pl.        def m
+00006360: 7968 6f6f 6b28 7365 6c66 2c20 6172 6773  yhook(self, args
+00006370: 293a 0a20 2020 2020 2020 2020 2020 2022  ):.            "
+00006380: 2222 4465 6661 756c 7420 696d 706c 656d  ""Default implem
+00006390: 656e 7461 7469 6f6e 2e22 2222 0a20 2020  entation.""".   
+000063a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000063b0: 320a 0a0a 2020 2020 636c 6173 7320 506c  2...    class Pl
+000063c0: 7567 696e 333a 0a20 2020 2020 2020 2040  ugin3:.        @
+000063d0: 686f 6f6b 696d 706c 0a20 2020 2020 2020  hookimpl.       
+000063e0: 2064 6566 206d 7968 6f6f 6b28 7365 6c66   def myhook(self
+000063f0: 2c20 6172 6773 293a 0a20 2020 2020 2020  , args):.       
+00006400: 2020 2020 2022 2222 4465 6661 756c 7420       """Default 
+00006410: 696d 706c 656d 656e 7461 7469 6f6e 2e22  implementation."
+00006420: 2222 0a20 2020 2020 2020 2020 2020 2072  "".            r
+00006430: 6574 7572 6e20 330a 0a0a 2020 2020 706d  eturn 3...    pm
+00006440: 203d 2050 6c75 6769 6e4d 616e 6167 6572   = PluginManager
+00006450: 2822 6d79 7072 6f6a 6563 7422 290a 2020  ("myproject").  
+00006460: 2020 706d 2e72 6567 6973 7465 7228 506c    pm.register(Pl
+00006470: 7567 696e 3128 2929 0a20 2020 2070 6d2e  ugin1()).    pm.
+00006480: 7265 6769 7374 6572 2850 6c75 6769 6e32  register(Plugin2
+00006490: 2829 290a 2020 2020 706d 2e72 6567 6973  ()).    pm.regis
+000064a0: 7465 7228 506c 7567 696e 3328 2929 0a0a  ter(Plugin3())..
+000064b0: 2020 2020 6173 7365 7274 2070 6d2e 686f      assert pm.ho
+000064c0: 6f6b 2e6d 7968 6f6f 6b28 6172 6773 3d28  ok.myhook(args=(
+000064d0: 2929 203d 3d20 5b33 2c20 322c 2031 5d0a  )) == [3, 2, 1].
+000064e0: 0a43 6f6c 6c65 6374 696e 6720 7265 7375  .Collecting resu
+000064f0: 6c74 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  lts.------------
+00006500: 2d2d 2d2d 2d2d 0a42 7920 6465 6661 756c  ------.By defaul
+00006510: 7420 6361 6c6c 696e 6720 6120 686f 6f6b  t calling a hook
+00006520: 2072 6573 756c 7473 2069 6e20 616c 6c20   results in all 
+00006530: 756e 6465 726c 7969 6e67 203a 7265 663a  underlying :ref:
+00006540: 6068 6f6f 6b69 6d70 6c73 0a3c 696d 706c  `hookimpls.<impl
+00006550: 733e 6020 6675 6e63 7469 6f6e 7320 746f  s>` functions to
+00006560: 2062 6520 696e 766f 6b65 6420 696e 2073   be invoked in s
+00006570: 6571 7565 6e63 6520 7669 6120 6120 6c6f  equence via a lo
+00006580: 6f70 2e20 416e 7920 6675 6e63 7469 6f6e  op. Any function
+00006590: 0a77 6869 6368 2072 6574 7572 6e73 2061  .which returns a
+000065a0: 2076 616c 7565 206f 7468 6572 2074 6861   value other tha
+000065b0: 6e20 6120 6060 4e6f 6e65 6060 2072 6573  n a ``None`` res
+000065c0: 756c 7420 7769 6c6c 2068 6176 6520 7468  ult will have th
+000065d0: 6174 2072 6573 756c 740a 6170 7065 6e64  at result.append
+000065e0: 6564 2074 6f20 6120 3a70 793a 636c 6173  ed to a :py:clas
+000065f0: 733a 606c 6973 7460 2077 6869 6368 2069  s:`list` which i
+00006600: 7320 7265 7475 726e 6564 2062 7920 7468  s returned by th
+00006610: 6520 6361 6c6c 2e0a 0a54 6865 206f 6e6c  e call...The onl
+00006620: 7920 6578 6365 7074 696f 6e20 746f 2074  y exception to t
+00006630: 6869 7320 6265 6861 7669 6f75 7220 6973  his behaviour is
+00006640: 2069 6620 7468 6520 686f 6f6b 2068 6173   if the hook has
+00006650: 2062 6565 6e20 6d61 726b 6564 2074 6f20   been marked to 
+00006660: 7265 7475 726e 0a69 7473 203a 7265 663a  return.its :ref:
+00006670: 6066 6972 7374 2072 6573 756c 7420 6f6e  `first result on
+00006680: 6c79 203c 6669 7273 7472 6573 756c 743e  ly <firstresult>
+00006690: 6020 696e 2077 6869 6368 2063 6173 6520  ` in which case 
+000066a0: 6f6e 6c79 2074 6865 2066 6972 7374 0a73  only the first.s
+000066b0: 696e 676c 6520 7661 6c75 6520 2877 6869  ingle value (whi
+000066c0: 6368 2069 7320 6e6f 7420 6060 4e6f 6e65  ch is not ``None
+000066d0: 6060 2920 7769 6c6c 2062 6520 7265 7475  ``) will be retu
+000066e0: 726e 6564 2e0a 0a2e 2e20 5f63 616c 6c5f  rned..... _call_
+000066f0: 6869 7374 6f72 6963 3a0a 0a45 7863 6570  historic:..Excep
+00006700: 7469 6f6e 2068 616e 646c 696e 670a 2d2d  tion handling.--
+00006710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006720: 0a49 6620 616e 7920 2a68 6f6f 6b69 6d70  .If any *hookimp
+00006730: 6c2a 2065 7272 6f72 7320 7769 7468 2061  l* errors with a
+00006740: 6e20 6578 6365 7074 696f 6e20 6e6f 2066  n exception no f
+00006750: 7572 7468 6572 2063 616c 6c62 6163 6b73  urther callbacks
+00006760: 2061 7265 2069 6e76 6f6b 6564 2061 6e64   are invoked and
+00006770: 0a74 6865 2065 7863 6570 7469 6f6e 2069  .the exception i
+00006780: 7320 6465 6c69 7665 7265 6420 746f 2061  s delivered to a
+00006790: 6e79 203a 7265 663a 6077 7261 7070 6572  ny :ref:`wrapper
+000067a0: 7320 3c68 6f6f 6b77 7261 7070 6572 733e  s <hookwrappers>
+000067b0: 6020 6265 666f 7265 2062 6569 6e67 0a72  ` before being.r
+000067c0: 652d 7261 6973 6564 2061 7420 7468 6520  e-raised at the 
+000067d0: 686f 6f6b 2069 6e76 6f63 6174 696f 6e20  hook invocation 
+000067e0: 706f 696e 743a 0a0a 2e2e 2063 6f64 652d  point:.... code-
+000067f0: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+00006800: 2020 2020 6672 6f6d 2070 6c75 6767 7920      from pluggy 
+00006810: 696d 706f 7274 2050 6c75 6769 6e4d 616e  import PluginMan
+00006820: 6167 6572 2c20 486f 6f6b 696d 706c 4d61  ager, HookimplMa
+00006830: 726b 6572 0a0a 2020 2020 686f 6f6b 696d  rker..    hookim
+00006840: 706c 203d 2048 6f6f 6b69 6d70 6c4d 6172  pl = HookimplMar
+00006850: 6b65 7228 226d 7970 726f 6a65 6374 2229  ker("myproject")
+00006860: 0a0a 0a20 2020 2063 6c61 7373 2050 6c75  ...    class Plu
+00006870: 6769 6e31 3a0a 2020 2020 2020 2020 4068  gin1:.        @h
+00006880: 6f6f 6b69 6d70 6c0a 2020 2020 2020 2020  ookimpl.        
+00006890: 6465 6620 6d79 686f 6f6b 2873 656c 662c  def myhook(self,
+000068a0: 2061 7267 7329 3a0a 2020 2020 2020 2020   args):.        
+000068b0: 2020 2020 7265 7475 726e 2031 0a0a 0a20      return 1... 
+000068c0: 2020 2063 6c61 7373 2050 6c75 6769 6e32     class Plugin2
+000068d0: 3a0a 2020 2020 2020 2020 4068 6f6f 6b69  :.        @hooki
+000068e0: 6d70 6c0a 2020 2020 2020 2020 6465 6620  mpl.        def 
+000068f0: 6d79 686f 6f6b 2873 656c 662c 2061 7267  myhook(self, arg
+00006900: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00006910: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+00006920: 6f72 0a0a 0a20 2020 2063 6c61 7373 2050  or...    class P
+00006930: 6c75 6769 6e33 3a0a 2020 2020 2020 2020  lugin3:.        
+00006940: 4068 6f6f 6b69 6d70 6c0a 2020 2020 2020  @hookimpl.      
+00006950: 2020 6465 6620 6d79 686f 6f6b 2873 656c    def myhook(sel
+00006960: 662c 2061 7267 7329 3a0a 2020 2020 2020  f, args):.      
+00006970: 2020 2020 2020 7265 7475 726e 2033 0a0a        return 3..
+00006980: 0a20 2020 2040 686f 6f6b 696d 706c 0a20  .    @hookimpl. 
+00006990: 2020 2064 6566 206d 7968 6f6f 6b28 7365     def myhook(se
+000069a0: 6c66 2c20 6172 6773 293a 0a20 2020 2020  lf, args):.     
+000069b0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000069c0: 2020 2020 7265 7475 726e 2028 7969 656c      return (yiel
+000069d0: 6429 0a20 2020 2020 2020 2065 7863 6570  d).        excep
+000069e0: 7420 5275 6e74 696d 6545 7272 6f72 2061  t RuntimeError a
+000069f0: 7320 6578 633a 0a20 2020 2020 2020 2020  s exc:.         
+00006a00: 2020 2023 206c 6f67 2072 756e 7469 6d65     # log runtime
+00006a10: 2065 7272 6f72 2064 6574 6169 6c73 0a20   error details. 
+00006a20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00006a30: 2865 7863 290a 2020 2020 2020 2020 2020  (exc).          
+00006a40: 2020 7261 6973 650a 0a0a 2020 2020 706d    raise...    pm
+00006a50: 203d 2050 6c75 6769 6e4d 616e 6167 6572   = PluginManager
+00006a60: 2822 6d79 7072 6f6a 6563 7422 290a 0a20  ("myproject").. 
+00006a70: 2020 2023 2072 6567 6973 7465 7220 706c     # register pl
+00006a80: 7567 696e 730a 2020 2020 706d 2e72 6567  ugins.    pm.reg
+00006a90: 6973 7465 7228 506c 7567 696e 3128 2929  ister(Plugin1())
+00006aa0: 0a20 2020 2070 6d2e 7265 6769 7374 6572  .    pm.register
+00006ab0: 2850 6c75 6769 6e32 2829 290a 2020 2020  (Plugin2()).    
+00006ac0: 706d 2e72 6567 6973 7465 7228 506c 7567  pm.register(Plug
+00006ad0: 696e 3328 2929 0a0a 2020 2020 2320 7265  in3())..    # re
+00006ae0: 6769 7374 6572 2077 7261 7070 6572 0a20  gister wrapper. 
+00006af0: 2020 2070 6d2e 7265 6769 7374 6572 2873     pm.register(s
+00006b00: 7973 2e6d 6f64 756c 6573 5b5f 5f6e 616d  ys.modules[__nam
+00006b10: 655f 5f5d 290a 0a20 2020 2023 2074 6869  e__])..    # thi
+00006b20: 7320 7261 6973 6573 2052 756e 7469 6d65  s raises Runtime
+00006b30: 4572 726f 7220 6475 6520 746f 2050 6c75  Error due to Plu
+00006b40: 6769 6e32 0a20 2020 2070 6d2e 686f 6f6b  gin2.    pm.hook
+00006b50: 2e6d 7968 6f6f 6b28 6172 6773 3d28 2929  .myhook(args=())
+00006b60: 0a0a 4869 7374 6f72 6963 2063 616c 6c73  ..Historic calls
+00006b70: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  .--------------.
+00006b80: 4120 2a68 6973 746f 7269 6320 6361 6c6c  A *historic call
+00006b90: 2a20 616c 6c6f 7773 2066 6f72 2061 6c6c  * allows for all
+00006ba0: 206e 6577 6c79 2072 6567 6973 7465 7265   newly registere
+00006bb0: 6420 6675 6e63 7469 6f6e 7320 746f 2072  d functions to r
+00006bc0: 6563 6569 7665 2061 6c6c 2068 6f6f 6b0a  eceive all hook.
+00006bd0: 6361 6c6c 7320 7468 6174 2068 6170 7065  calls that happe
+00006be0: 6e65 6420 6265 666f 7265 2074 6865 6972  ned before their
+00006bf0: 2072 6567 6973 7472 6174 696f 6e2e 2054   registration. T
+00006c00: 6865 2069 6d70 6c69 6361 7469 6f6e 2069  he implication i
+00006c10: 7320 7468 6174 2074 6869 7320 6973 0a6f  s that this is.o
+00006c20: 6e6c 7920 7573 6566 756c 2069 6620 796f  nly useful if yo
+00006c30: 7520 6578 7065 6374 2074 6861 7420 736f  u expect that so
+00006c40: 6d65 202a 686f 6f6b 696d 706c 732a 206d  me *hookimpls* m
+00006c50: 6179 2062 6520 7265 6769 7374 6572 6564  ay be registered
+00006c60: 202a 2a61 6674 6572 2a2a 2074 6865 0a68   **after** the.h
+00006c70: 6f6f 6b20 6973 2069 6e69 7469 616c 6c79  ook is initially
+00006c80: 2069 6e76 6f6b 6564 2e0a 0a48 6973 746f   invoked...Histo
+00006c90: 7269 6320 686f 6f6b 7320 6d75 7374 2062  ric hooks must b
+00006ca0: 6520 3a72 6566 3a60 7370 6563 6961 6c6c  e :ref:`speciall
+00006cb0: 7920 6d61 726b 6564 203c 6869 7374 6f72  y marked <histor
+00006cc0: 6963 3e60 2061 6e64 2063 616c 6c65 640a  ic>` and called.
+00006cd0: 7573 696e 6720 7468 6520 3a70 793a 6d65  using the :py:me
+00006ce0: 7468 3a60 7e70 6c75 6767 792e 5f68 6f6f  th:`~pluggy._hoo
+00006cf0: 6b73 2e5f 486f 6f6b 4361 6c6c 6572 2e63  ks._HookCaller.c
+00006d00: 616c 6c5f 6869 7374 6f72 6963 2829 6020  all_historic()` 
+00006d10: 6d65 7468 6f64 3a0a 0a2e 2e20 636f 6465  method:.... code
+00006d20: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00006d30: 0a20 2020 2064 6566 2063 616c 6c62 6163  .    def callbac
+00006d40: 6b28 7265 7375 6c74 293a 0a20 2020 2020  k(result):.     
+00006d50: 2020 2070 7269 6e74 2822 6869 7374 6f72     print("histor
+00006d60: 6963 2063 616c 6c20 7265 7375 6c74 2069  ic call result i
+00006d70: 7320 7b72 6573 756c 747d 222e 666f 726d  s {result}".form
+00006d80: 6174 2872 6573 756c 743d 7265 7375 6c74  at(result=result
+00006d90: 2929 0a0a 0a20 2020 2023 2063 616c 6c20  ))...    # call 
+00006da0: 7769 7468 2068 6973 746f 7279 3b20 6e6f  with history; no
+00006db0: 2072 6573 756c 7473 2072 6574 7572 6e65   results returne
+00006dc0: 640a 2020 2020 706d 2e68 6f6f 6b2e 6d79  d.    pm.hook.my
+00006dd0: 686f 6f6b 2e63 616c 6c5f 6869 7374 6f72  hook.call_histor
+00006de0: 6963 280a 2020 2020 2020 2020 6b77 6172  ic(.        kwar
+00006df0: 6773 3d7b 2263 6f6e 6669 6722 3a20 636f  gs={"config": co
+00006e00: 6e66 6967 2c20 2261 7267 7322 3a20 7379  nfig, "args": sy
+00006e10: 732e 6172 6776 7d2c 2072 6573 756c 745f  s.argv}, result_
+00006e20: 6361 6c6c 6261 636b 3d63 616c 6c62 6163  callback=callbac
+00006e30: 6b0a 2020 2020 290a 0a20 2020 2023 202e  k.    )..    # .
+00006e40: 2e2e 206d 6f72 6520 6f66 206f 7572 2070  .. more of our p
+00006e50: 726f 6772 616d 202e 2e2e 0a0a 2020 2020  rogram .....    
+00006e60: 2320 6c61 7465 206c 6f61 6469 6e67 206f  # late loading o
+00006e70: 6620 736f 6d65 2070 6c75 6769 6e0a 2020  f some plugin.  
+00006e80: 2020 696d 706f 7274 206d 796c 6174 6570    import mylatep
+00006e90: 6c75 6769 6e0a 0a20 2020 2023 2068 6973  lugin..    # his
+00006ea0: 746f 7269 6320 6361 6c6c 6261 636b 2069  toric callback i
+00006eb0: 7320 696e 766f 6b65 6420 6865 7265 0a20  s invoked here. 
+00006ec0: 2020 2070 6d2e 7265 6769 7374 6572 286d     pm.register(m
+00006ed0: 796c 6174 6570 6c75 6769 6e29 0a0a 4e6f  ylateplugin)..No
+00006ee0: 7465 2074 6861 7420 6966 2079 6f75 203a  te that if you :
+00006ef0: 7079 3a6d 6574 683a 607e 706c 7567 6779  py:meth:`~pluggy
+00006f00: 2e5f 686f 6f6b 732e 5f48 6f6f 6b43 616c  ._hooks._HookCal
+00006f10: 6c65 722e 6361 6c6c 5f68 6973 746f 7269  ler.call_histori
+00006f20: 6328 2960 0a74 6865 203a 7079 3a63 6c61  c()`.the :py:cla
+00006f30: 7373 3a60 7e70 6c75 6767 792e 5f68 6f6f  ss:`~pluggy._hoo
+00006f40: 6b73 2e5f 486f 6f6b 4361 6c6c 6572 6020  ks._HookCaller` 
+00006f50: 2861 6e64 2074 6875 7320 796f 7572 2063  (and thus your c
+00006f60: 616c 6c69 6e67 2063 6f64 6529 0a63 616e  alling code).can
+00006f70: 206e 6f74 2072 6563 6569 7665 2072 6573   not receive res
+00006f80: 756c 7473 2062 6163 6b20 6672 6f6d 2074  ults back from t
+00006f90: 6865 2075 6e64 6572 6c79 696e 6720 2a68  he underlying *h
+00006fa0: 6f6f 6b69 6d70 6c2a 2066 756e 6374 696f  ookimpl* functio
+00006fb0: 6e73 2e0a 496e 7374 6561 6420 796f 7520  ns..Instead you 
+00006fc0: 6361 6e20 7072 6f76 6964 6520 6120 2a63  can provide a *c
+00006fd0: 616c 6c62 6163 6b2a 2066 6f72 2070 726f  allback* for pro
+00006fe0: 6365 7373 696e 6720 7265 7375 6c74 7320  cessing results 
+00006ff0: 286c 696b 6520 7468 650a 6060 6361 6c6c  (like the.``call
+00007000: 6261 636b 6060 2066 756e 6374 696f 6e20  back`` function 
+00007010: 6162 6f76 6529 2077 6869 6368 2077 696c  above) which wil
+00007020: 6c20 6265 2063 616c 6c65 6420 6173 2065  l be called as e
+00007030: 6163 6820 6e65 7720 706c 7567 696e 0a69  ach new plugin.i
+00007040: 7320 7265 6769 7374 6572 6564 2e0a 0a2e  s registered....
+00007050: 2e20 6e6f 7465 3a3a 0a20 2020 202a 6869  . note::.    *hi
+00007060: 7374 6f72 6963 2a20 6361 6c6c 7320 6172  storic* calls ar
+00007070: 6520 696e 636f 6d70 6174 6962 6c65 2077  e incompatible w
+00007080: 6974 6820 3a72 6566 3a60 6669 7273 7472  ith :ref:`firstr
+00007090: 6573 756c 7460 206d 6172 6b65 640a 2020  esult` marked.  
+000070a0: 2020 686f 6f6b 7320 7369 6e63 6520 6f6e    hooks since on
+000070b0: 6c79 2074 6865 2066 6972 7374 2072 6567  ly the first reg
+000070c0: 6973 7465 7265 6420 706c 7567 696e 2773  istered plugin's
+000070d0: 2068 6f6f 6b28 7329 2077 6f75 6c64 0a20   hook(s) would. 
+000070e0: 2020 2065 7665 7220 6265 2063 616c 6c65     ever be calle
+000070f0: 642e 0a0a 4361 6c6c 696e 6720 7769 7468  d...Calling with
+00007100: 2065 7874 7261 730a 2d2d 2d2d 2d2d 2d2d   extras.--------
+00007110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 596f 7520  -----------.You 
+00007120: 6361 6e20 6361 6c6c 2061 2068 6f6f 6b20  can call a hook 
+00007130: 7769 7468 2074 656d 706f 7261 7269 6c79  with temporarily
+00007140: 2070 6172 7469 6369 7061 7469 6e67 202a   participating *
+00007150: 696d 706c 656d 656e 7461 7469 6f6e 2a20  implementation* 
+00007160: 6675 6e63 7469 6f6e 730a 2874 6861 7420  functions.(that 
+00007170: 6172 656e 2774 2069 6e20 7468 6520 7265  aren't in the re
+00007180: 6769 7374 7279 2920 7573 696e 6720 7468  gistry) using th
+00007190: 650a 3a70 793a 6d65 7468 3a60 706c 7567  e.:py:meth:`plug
+000071a0: 6779 2e5f 686f 6f6b 732e 5f48 6f6f 6b43  gy._hooks._HookC
+000071b0: 616c 6c65 722e 6361 6c6c 5f65 7874 7261  aller.call_extra
+000071c0: 2829 6020 6d65 7468 6f64 2e0a 0a0a 4361  ()` method....Ca
+000071d0: 6c6c 696e 6720 7769 7468 2061 2073 7562  lling with a sub
+000071e0: 7365 7420 6f66 2072 6567 6973 7465 7265  set of registere
+000071f0: 6420 706c 7567 696e 730a 2d2d 2d2d 2d2d  d plugins.------
+00007200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007220: 2d2d 2d2d 2d0a 596f 7520 6361 6e20 6d61  -----.You can ma
+00007230: 6b65 2061 2063 616c 6c20 7573 696e 6720  ke a call using 
+00007240: 6120 7375 6273 6574 206f 6620 706c 7567  a subset of plug
+00007250: 696e 7320 6279 2061 736b 696e 6720 7468  ins by asking th
+00007260: 650a 3a70 793a 636c 6173 733a 607e 706c  e.:py:class:`~pl
+00007270: 7567 6779 2e50 6c75 6769 6e4d 616e 6167  uggy.PluginManag
+00007280: 6572 6020 6669 7273 7420 666f 7220 610a  er` first for a.
+00007290: 3a70 793a 636c 6173 733a 607e 706c 7567  :py:class:`~plug
+000072a0: 6779 2e5f 686f 6f6b 732e 5f48 6f6f 6b43  gy._hooks._HookC
+000072b0: 616c 6c65 7260 2077 6974 6820 7468 6f73  aller` with thos
+000072c0: 6520 706c 7567 696e 7320 7265 6d6f 7665  e plugins remove
+000072d0: 640a 7573 696e 6720 7468 6520 3a70 793a  d.using the :py:
+000072e0: 6d65 7468 3a60 706c 7567 6779 2e50 6c75  meth:`pluggy.Plu
+000072f0: 6769 6e4d 616e 6167 6572 2e73 7562 7365  ginManager.subse
+00007300: 745f 686f 6f6b 5f63 616c 6c65 7228 2960  t_hook_caller()`
+00007310: 206d 6574 686f 642e 0a0a 596f 7520 7468   method...You th
+00007320: 656e 2063 616e 2075 7365 2074 6861 7420  en can use that 
+00007330: 3a70 793a 636c 6173 733a 605f 486f 6f6b  :py:class:`_Hook
+00007340: 4361 6c6c 6572 203c 706c 7567 6779 2e5f  Caller <pluggy._
+00007350: 686f 6f6b 732e 5f48 6f6f 6b43 616c 6c65  hooks._HookCalle
+00007360: 723e 600a 746f 206d 616b 6520 6e6f 726d  r>`.to make norm
+00007370: 616c 2c20 3a70 793a 6d65 7468 3a60 7e70  al, :py:meth:`~p
+00007380: 6c75 6767 792e 5f68 6f6f 6b73 2e5f 486f  luggy._hooks._Ho
+00007390: 6f6b 4361 6c6c 6572 2e63 616c 6c5f 6869  okCaller.call_hi
+000073a0: 7374 6f72 6963 602c 206f 720a 3a70 793a  storic`, or.:py:
+000073b0: 6d65 7468 3a60 7e70 6c75 6767 792e 5f68  meth:`~pluggy._h
+000073c0: 6f6f 6b73 2e5f 486f 6f6b 4361 6c6c 6572  ooks._HookCaller
+000073d0: 2e63 616c 6c5f 6578 7472 6160 2063 616c  .call_extra` cal
+000073e0: 6c73 2061 7320 6e65 6365 7373 6172 792e  ls as necessary.
+000073f0: 0a0a 4275 696c 742d 696e 2074 7261 6369  ..Built-in traci
+00007400: 6e67 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ng.*************
+00007410: 2a2a 2a0a 6060 706c 7567 6779 6060 2063  ***.``pluggy`` c
+00007420: 6f6d 6573 2077 6974 6820 736f 6d65 2062  omes with some b
+00007430: 6174 7465 7269 6573 2069 6e63 6c75 6465  atteries include
+00007440: 6420 686f 6f6b 2074 7261 6369 6e67 2066  d hook tracing f
+00007450: 6f72 2079 6f75 720a 6465 6275 6767 696e  or your.debuggin
+00007460: 6720 6e65 6564 732e 0a0a 0a43 616c 6c20  g needs....Call 
+00007470: 7472 6163 696e 670a 2d2d 2d2d 2d2d 2d2d  tracing.--------
+00007480: 2d2d 2d2d 0a54 6f20 656e 6162 6c65 2074  ----.To enable t
+00007490: 7261 6369 6e67 2075 7365 2074 6865 0a3a  racing use the.:
+000074a0: 7079 3a6d 6574 683a 6070 6c75 6767 792e  py:meth:`pluggy.
+000074b0: 506c 7567 696e 4d61 6e61 6765 722e 656e  PluginManager.en
+000074c0: 6162 6c65 5f74 7261 6369 6e67 2829 6020  able_tracing()` 
+000074d0: 6d65 7468 6f64 2077 6869 6368 2072 6574  method which ret
+000074e0: 7572 6e73 2061 6e0a 756e 646f 2066 756e  urns an.undo fun
+000074f0: 6374 696f 6e20 746f 2064 6973 6162 6c65  ction to disable
+00007500: 2074 6865 2062 6568 6176 696f 7572 2e0a   the behaviour..
+00007510: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00007520: 2070 7974 686f 6e0a 0a20 2020 2070 6d20   python..    pm 
+00007530: 3d20 506c 7567 696e 4d61 6e61 6765 7228  = PluginManager(
+00007540: 226d 7970 726f 6a65 6374 2229 0a20 2020  "myproject").   
+00007550: 2023 206d 6167 6963 206c 696e 6520 746f   # magic line to
+00007560: 2073 6574 2061 2077 7269 7465 7220 6675   set a writer fu
+00007570: 6e63 7469 6f6e 0a20 2020 2070 6d2e 7472  nction.    pm.tr
+00007580: 6163 652e 726f 6f74 2e73 6574 7772 6974  ace.root.setwrit
+00007590: 6572 2870 7269 6e74 290a 2020 2020 756e  er(print).    un
+000075a0: 646f 203d 2070 6d2e 656e 6162 6c65 5f74  do = pm.enable_t
+000075b0: 7261 6369 6e67 2829 0a0a 0a43 616c 6c20  racing()...Call 
+000075c0: 6d6f 6e69 746f 7269 6e67 0a2d 2d2d 2d2d  monitoring.-----
+000075d0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a49 6e73 7465  ----------.Inste
+000075e0: 6164 206f 6620 7573 696e 6720 7468 6520  ad of using the 
+000075f0: 6275 696c 742d 696e 2074 7261 6369 6e67  built-in tracing
+00007600: 206d 6563 6861 6e69 736d 2079 6f75 2063   mechanism you c
+00007610: 616e 2061 6c73 6f20 6164 6420 796f 7572  an also add your
+00007620: 0a6f 776e 2060 6062 6566 6f72 6560 6020  .own ``before`` 
+00007630: 616e 6420 6060 6166 7465 7260 6020 6d6f  and ``after`` mo
+00007640: 6e69 746f 7269 6e67 2066 756e 6374 696f  nitoring functio
+00007650: 6e73 2075 7369 6e67 0a3a 7079 3a63 6c61  ns using.:py:cla
+00007660: 7373 3a60 706c 7567 6779 2e50 6c75 6769  ss:`pluggy.Plugi
+00007670: 6e4d 616e 6167 6572 2e61 6464 5f68 6f6f  nManager.add_hoo
+00007680: 6b63 616c 6c5f 6d6f 6e69 746f 7269 6e67  kcall_monitoring
+00007690: 2829 602e 0a0a 5468 6520 6578 7065 6374  ()`...The expect
+000076a0: 6564 2073 6967 6e61 7475 7265 2061 6e64  ed signature and
+000076b0: 2064 6566 6175 6c74 2069 6d70 6c65 6d65   default impleme
+000076c0: 6e74 6174 696f 6e73 2066 6f72 2074 6865  ntations for the
+000076d0: 7365 2066 756e 6374 696f 6e73 2069 733a  se functions is:
+000076e0: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+000076f0: 3a20 7079 7468 6f6e 0a0a 2020 2020 6465  : python..    de
+00007700: 6620 6265 666f 7265 2868 6f6f 6b5f 6e61  f before(hook_na
+00007710: 6d65 2c20 6d65 7468 6f64 732c 206b 7761  me, methods, kwa
+00007720: 7267 7329 3a0a 2020 2020 2020 2020 7061  rgs):.        pa
+00007730: 7373 0a0a 0a20 2020 2064 6566 2061 6674  ss...    def aft
+00007740: 6572 286f 7574 636f 6d65 2c20 686f 6f6b  er(outcome, hook
+00007750: 5f6e 616d 652c 206d 6574 686f 6473 2c20  _name, methods, 
+00007760: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00007770: 2070 6173 730a 0a50 7562 6c69 6320 4150   pass..Public AP
+00007780: 490a 2a2a 2a2a 2a2a 2a2a 2a2a 0a50 6c65  I.**********.Ple
+00007790: 6173 6520 7365 6520 7468 6520 3a64 6f63  ase see the :doc
+000077a0: 3a60 6170 695f 7265 6665 7265 6e63 6560  :`api_reference`
+000077b0: 2e0a 0a44 6576 656c 6f70 6d65 6e74 0a2a  ...Development.*
+000077c0: 2a2a 2a2a 2a2a 2a2a 2a2a 0a47 7265 6174  **********.Great
+000077d0: 2063 6172 6520 6d75 7374 2074 616b 656e   care must taken
+000077e0: 2077 6865 6e20 6861 636b 696e 6720 6f6e   when hacking on
+000077f0: 2060 6070 6c75 6767 7960 6020 7369 6e63   ``pluggy`` sinc
+00007800: 6520 6d75 6c74 6970 6c65 206d 6174 7572  e multiple matur
+00007810: 650a 7072 6f6a 6563 7473 2072 656c 7920  e.projects rely 
+00007820: 6f6e 2069 742e 204f 7572 2047 6974 6875  on it. Our Githu
+00007830: 6220 696e 7465 6772 6174 6564 2043 4920  b integrated CI 
+00007840: 7072 6f63 6573 7320 7275 6e73 2074 6865  process runs the
+00007850: 2066 756c 6c0a 6074 6f78 2074 6573 7420   full.`tox test 
+00007860: 7375 6974 6560 5f20 6f6e 2065 6163 6820  suite`_ on each 
+00007870: 636f 6d6d 6974 2073 6f20 6265 2073 7572  commit so be sur
+00007880: 6520 796f 7572 2063 6861 6e67 6573 2063  e your changes c
+00007890: 616e 2072 756e 206f 6e0a 616c 6c20 7265  an run on.all re
+000078a0: 7175 6972 6564 2060 5079 7468 6f6e 2069  quired `Python i
+000078b0: 6e74 6572 7072 6574 6572 7360 5f20 616e  nterpreters`_ an
+000078c0: 6420 6060 7079 7465 7374 6060 2076 6572  d ``pytest`` ver
+000078d0: 7369 6f6e 732e 0a0a 466f 7220 6465 7665  sions...For deve
+000078e0: 6c6f 706d 656e 742c 2077 6520 7375 6767  lopment, we sugg
+000078f0: 6573 7420 746f 2063 7265 6174 6520 6120  est to create a 
+00007900: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
+00007910: 656e 7420 616e 6420 696e 7374 616c 6c20  ent and install 
+00007920: 6060 706c 7567 6779 6060 2069 6e0a 6564  ``pluggy`` in.ed
+00007930: 6974 6162 6c65 206d 6f64 6520 616e 6420  itable mode and 
+00007940: 6060 6465 7660 6020 6465 7065 6e64 656e  ``dev`` dependen
+00007950: 6369 6573 3a3a 0a0a 2020 2020 2420 7079  cies::..    $ py
+00007960: 7468 6f6e 3320 2d6d 2076 656e 7620 2e65  thon3 -m venv .e
+00007970: 6e76 0a20 2020 2024 2073 6f75 7263 6520  nv.    $ source 
+00007980: 2e65 6e76 2f62 696e 2f61 6374 6976 6174  .env/bin/activat
+00007990: 650a 2020 2020 2420 7069 7020 696e 7374  e.    $ pip inst
+000079a0: 616c 6c20 2d65 202e 5b64 6576 5d0a 0a54  all -e .[dev]..T
+000079b0: 6f20 6d61 6b65 2073 7572 6520 796f 7520  o make sure you 
+000079c0: 666f 6c6c 6f77 2074 6865 2063 6f64 6520  follow the code 
+000079d0: 7374 796c 6520 7573 6564 2069 6e20 7468  style used in th
+000079e0: 6520 7072 6f6a 6563 742c 2069 6e73 7461  e project, insta
+000079f0: 6c6c 2070 7265 2d63 6f6d 6d69 745f 2077  ll pre-commit_ w
+00007a00: 6869 6368 0a77 696c 6c20 7275 6e20 7374  hich.will run st
+00007a10: 796c 6520 6368 6563 6b73 2062 6566 6f72  yle checks befor
+00007a20: 6520 6561 6368 2063 6f6d 6d69 743a 3a0a  e each commit::.
+00007a30: 0a20 2020 2024 2070 7265 2d63 6f6d 6d69  .    $ pre-commi
+00007a40: 7420 696e 7374 616c 6c0a 0a0a 5265 6c65  t install...Rele
+00007a50: 6173 6520 506f 6c69 6379 0a2a 2a2a 2a2a  ase Policy.*****
+00007a60: 2a2a 2a2a 2a2a 2a2a 2a0a 506c 7567 6779  *********.Pluggy
+00007a70: 2075 7365 7320 6053 656d 616e 7469 6320   uses `Semantic 
+00007a80: 5665 7273 696f 6e69 6e67 605f 2e20 4272  Versioning`_. Br
+00007a90: 6561 6b69 6e67 2063 6861 6e67 6573 2061  eaking changes a
+00007aa0: 7265 206f 6e6c 7920 666f 7265 7365 656e  re only foreseen
+00007ab0: 2066 6f72 0a4d 616a 6f72 2072 656c 6561   for.Major relea
+00007ac0: 7365 7320 2869 6e63 7265 6d65 6e74 6564  ses (incremented
+00007ad0: 2058 2069 6e20 2258 2e59 2e5a 2229 2e20   X in "X.Y.Z"). 
+00007ae0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+00007af0: 7573 6520 6060 706c 7567 6779 6060 0a69  use ``pluggy``.i
+00007b00: 6e20 796f 7572 2070 726f 6a65 6374 2079  n your project y
+00007b10: 6f75 2073 686f 756c 6420 7468 7573 2075  ou should thus u
+00007b20: 7365 2061 2064 6570 656e 6465 6e63 7920  se a dependency 
+00007b30: 7265 7374 7269 6374 696f 6e20 6c69 6b65  restriction like
+00007b40: 0a60 6022 706c 7567 6779 3e3d 302e 312e  .``"pluggy>=0.1.
+00007b50: 302c 3c31 2e30 2260 6020 746f 2061 766f  0,<1.0"`` to avo
+00007b60: 6964 2073 7572 7072 6973 6573 2e0a 0a0a  id surprises....
+00007b70: 5461 626c 6520 6f66 2063 6f6e 7465 6e74  Table of content
+00007b80: 730a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  s.**************
+00007b90: 2a2a 2a0a 0a2e 2e20 746f 6374 7265 653a  ***.... toctree:
+00007ba0: 3a0a 2020 2020 3a6d 6178 6465 7074 683a  :.    :maxdepth:
+00007bb0: 2032 0a0a 2020 2020 6170 695f 7265 6665   2..    api_refe
+00007bc0: 7265 6e63 650a 2020 2020 6368 616e 6765  rence.    change
+00007bd0: 6c6f 670a 0a0a 0a2e 2e20 6879 7065 726c  log...... hyperl
+00007be0: 696e 6b73 0a2e 2e20 5f68 6f6f 6b73 7065  inks... _hookspe
+00007bf0: 6320 6d6f 6475 6c65 3a0a 2020 2020 6874  c module:.    ht
+00007c00: 7470 733a 2f2f 646f 6373 2e70 7974 6573  tps://docs.pytes
+00007c10: 742e 6f72 672f 656e 2f6c 6174 6573 742f  t.org/en/latest/
+00007c20: 5f6d 6f64 756c 6573 2f5f 7079 7465 7374  _modules/_pytest
+00007c30: 2f68 6f6f 6b73 7065 632e 6874 6d6c 0a2e  /hookspec.html..
+00007c40: 2e20 5f72 6571 7565 7374 2d72 6573 706f  . _request-respo
+00007c50: 6e73 6520 7061 7474 6572 6e3a 0a20 2020  nse pattern:.   
+00007c60: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+00007c70: 7065 6469 612e 6f72 672f 7769 6b69 2f52  pedia.org/wiki/R
+00007c80: 6571 7565 7374 2545 3225 3830 2539 3372  equest%E2%80%93r
+00007c90: 6573 706f 6e73 650a 2e2e 205f 7075 626c  esponse... _publ
+00007ca0: 6973 682d 7375 6273 6372 6962 653a 0a20  ish-subscribe:. 
+00007cb0: 2020 2068 7474 7073 3a2f 2f65 6e2e 7769     https://en.wi
+00007cc0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00007cd0: 2f50 7562 6c69 7368 2545 3225 3830 2539  /Publish%E2%80%9
+00007ce0: 3373 7562 7363 7269 6265 5f70 6174 7465  3subscribe_patte
+00007cf0: 726e 0a2e 2e20 5f68 6f6f 6b69 6e67 3a0a  rn... _hooking:.
+00007d00: 2020 2020 6874 7470 733a 2f2f 656e 2e77      https://en.w
+00007d10: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00007d20: 692f 486f 6f6b 696e 670a 2e2e 205f 6361  i/Hooking... _ca
+00007d30: 6c6c 6261 636b 733a 0a20 2020 2068 7474  llbacks:.    htt
+00007d40: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00007d50: 612e 6f72 672f 7769 6b69 2f43 616c 6c62  a.org/wiki/Callb
+00007d60: 6163 6b5f 2863 6f6d 7075 7465 725f 7072  ack_(computer_pr
+00007d70: 6f67 7261 6d6d 696e 6729 0a2e 2e20 5f74  ogramming)... _t
+00007d80: 6f78 2074 6573 7420 7375 6974 653a 0a20  ox test suite:. 
+00007d90: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
+00007da0: 622e 636f 6d2f 7079 7465 7374 2d64 6576  b.com/pytest-dev
+00007db0: 2f70 6c75 6767 792f 626c 6f62 2f6d 6173  /pluggy/blob/mas
+00007dc0: 7465 722f 746f 782e 696e 690a 2e2e 205f  ter/tox.ini... _
+00007dd0: 5365 6d61 6e74 6963 2056 6572 7369 6f6e  Semantic Version
+00007de0: 696e 673a 0a20 2020 2068 7474 7073 3a2f  ing:.    https:/
+00007df0: 2f73 656d 7665 722e 6f72 672f 0a2e 2e20  /semver.org/... 
+00007e00: 5f50 7974 686f 6e20 696e 7465 7270 7265  _Python interpre
+00007e10: 7465 7273 3a0a 2020 2020 6874 7470 733a  ters:.    https:
+00007e20: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7974  //github.com/pyt
+00007e30: 6573 742d 6465 762f 706c 7567 6779 2f62  est-dev/pluggy/b
+00007e40: 6c6f 622f 6d61 7374 6572 2f74 6f78 2e69  lob/master/tox.i
+00007e50: 6e69 234c 320a 2e2e 205f 3530 302b 2070  ni#L2... _500+ p
+00007e60: 6c75 6769 6e73 3a0a 2020 2020 6874 7470  lugins:.    http
+00007e70: 733a 2f2f 646f 6373 2e70 7974 6573 742e  s://docs.pytest.
+00007e80: 6f72 672f 656e 2f6c 6174 6573 742f 7265  org/en/latest/re
+00007e90: 6665 7265 6e63 652f 706c 7567 696e 5f6c  ference/plugin_l
+00007ea0: 6973 742e 6874 6d6c 0a2e 2e20 5f70 7265  ist.html... _pre
+00007eb0: 2d63 6f6d 6d69 743a 0a20 2020 2068 7474  -commit:.    htt
+00007ec0: 7073 3a2f 2f70 7265 2d63 6f6d 6d69 742e  ps://pre-commit.
+00007ed0: 636f 6d2f 0a0a 0a2e 2e20 496e 6469 6365  com/..... Indice
+00007ee0: 7320 616e 6420 7461 626c 6573 0a2e 2e20  s and tables... 
+00007ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007f00: 3d3d 0a2e 2e20 2a20 3a72 6566 3a60 6765  ==... * :ref:`ge
+00007f10: 6e69 6e64 6578 600a 2e2e 202a 203a 7265  nindex`... * :re
+00007f20: 663a 606d 6f64 696e 6465 7860 0a2e 2e20  f:`modindex`... 
+00007f30: 2a20 3a72 6566 3a60 7365 6172 6368 600a  * :ref:`search`.
```

### Comparing `pluggy-1.0.0.dev0/docs/_static/img/plug.png` & `pluggy-1.1.0/docs/_static/img/plug.png`

 * *Files identical despite different names*

### Comparing `pluggy-1.0.0.dev0/changelog/_template.rst` & `pluggy-1.1.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `pluggy-1.0.0.dev0/changelog/README.rst` & `pluggy-1.1.0/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `pluggy-1.0.0.dev0/src/pluggy/manager.py` & `pluggy-1.1.0/src/pluggy/_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,256 +1,312 @@
+from __future__ import annotations
+
 import inspect
 import sys
-from . import _tracing
-from .callers import _Result, _multicall
-from .hooks import HookImpl, _HookRelay, _HookCaller, normalize_hookimpl_opts
+import types
 import warnings
+from typing import Any
+from typing import Callable
+from typing import cast
+from typing import Iterable
+from typing import Mapping
+from typing import Sequence
+from typing import TYPE_CHECKING
+
+from . import _tracing
+from ._callers import _multicall
+from ._hooks import _HookCaller
+from ._hooks import _HookImplFunction
+from ._hooks import _HookRelay
+from ._hooks import _Namespace
+from ._hooks import _Plugin
+from ._hooks import _SubsetHookCaller
+from ._hooks import HookImpl
+from ._hooks import HookSpec
+from ._hooks import normalize_hookimpl_opts
+from ._result import _Result
 
 if sys.version_info >= (3, 8):
     from importlib import metadata as importlib_metadata
 else:
     import importlib_metadata
 
+if TYPE_CHECKING:
+    from typing_extensions import Final
+
+    from ._hooks import _HookImplOpts, _HookSpecOpts
+
+_BeforeTrace = Callable[[str, Sequence[HookImpl], Mapping[str, Any]], None]
+_AfterTrace = Callable[[_Result[Any], str, Sequence[HookImpl], Mapping[str, Any]], None]
 
-def _warn_for_function(warning, function):
+
+def _warn_for_function(warning: Warning, function: Callable[..., object]) -> None:
+    func = cast(types.FunctionType, function)
     warnings.warn_explicit(
         warning,
         type(warning),
-        lineno=function.__code__.co_firstlineno,
-        filename=function.__code__.co_filename,
+        lineno=func.__code__.co_firstlineno,
+        filename=func.__code__.co_filename,
     )
 
 
 class PluginValidationError(Exception):
-    """ plugin failed validation.
+    """Plugin failed validation.
 
-    :param object plugin: the plugin which failed validation,
-        may be a module or an arbitrary object.
+    :param plugin: The plugin which failed validation.
     """
 
-    def __init__(self, plugin, message):
+    def __init__(self, plugin: _Plugin, message: str) -> None:
+        super().__init__(message)
         self.plugin = plugin
-        super(Exception, self).__init__(message)
 
 
-class DistFacade(object):
+class DistFacade:
     """Emulate a pkg_resources Distribution"""
 
-    def __init__(self, dist):
+    def __init__(self, dist: importlib_metadata.Distribution) -> None:
         self._dist = dist
 
     @property
-    def project_name(self):
-        return self.metadata["name"]
+    def project_name(self) -> str:
+        name: str = self.metadata["name"]
+        return name
 
-    def __getattr__(self, attr, default=None):
+    def __getattr__(self, attr: str, default=None):
         return getattr(self._dist, attr, default)
 
-    def __dir__(self):
+    def __dir__(self) -> list[str]:
         return sorted(dir(self._dist) + ["_dist", "project_name"])
 
 
-class PluginManager(object):
-    """ Core :py:class:`.PluginManager` class which manages registration
-    of plugin objects and 1:N hook calling.
-
-    You can register new hooks by calling :py:meth:`add_hookspecs(module_or_class)
-    <.PluginManager.add_hookspecs>`.
-    You can register plugin objects (which contain hooks) by calling
-    :py:meth:`register(plugin) <.PluginManager.register>`.  The :py:class:`.PluginManager`
-    is initialized with a prefix that is searched for in the names of the dict
-    of registered plugin objects.
+class PluginManager:
+    """Core class which manages registration of plugin objects and 1:N hook
+    calling.
+
+    You can register new hooks by calling :meth:`add_hookspecs(module_or_class)
+    <PluginManager.add_hookspecs>`.
+
+    You can register plugin objects (which contain hook implementations) by
+    calling :meth:`register(plugin) <PluginManager.register>`.
 
-    For debugging purposes you can call :py:meth:`.PluginManager.enable_tracing`
+    For debugging purposes you can call :meth:`PluginManager.enable_tracing`
     which will subsequently send debug information to the trace helper.
     """
 
-    def __init__(self, project_name, implprefix=None):
-        """If ``implprefix`` is given implementation functions
-        will be recognized if their name matches the ``implprefix``. """
-        self.project_name = project_name
-        self._name2plugin = {}
-        self._plugin2hookcallers = {}
-        self._plugin_distinfo = []
-        self.trace = _tracing.TagTracer().get("pluginmanage")
-        self.hook = _HookRelay()
-        if implprefix is not None:
-            warnings.warn(
-                "Support for the `implprefix` arg is now deprecated and will "
-                "be removed in an upcoming release. Please use HookimplMarker.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        self._implprefix = implprefix
-        self._inner_hookexec = lambda hook, methods, kwargs: _multicall(
-            methods,
-            kwargs,
-            firstresult=hook.spec.opts.get("firstresult") if hook.spec else False,
-        )
+    __slots__ = (
+        "project_name",
+        "_name2plugin",
+        "_plugin2hookcallers",
+        "_plugin_distinfo",
+        "trace",
+        "hook",
+        "_inner_hookexec",
+    )
 
-    def _hookexec(self, hook, methods, kwargs):
+    def __init__(self, project_name: str) -> None:
+        self.project_name: Final = project_name
+        self._name2plugin: Final[dict[str, _Plugin]] = {}
+        self._plugin_distinfo: Final[list[tuple[_Plugin, DistFacade]]] = []
+        self.trace: Final = _tracing.TagTracer().get("pluginmanage")
+        self.hook: Final = _HookRelay()
+        self._inner_hookexec = _multicall
+
+    def _hookexec(
+        self,
+        hook_name: str,
+        methods: Sequence[HookImpl],
+        kwargs: Mapping[str, object],
+        firstresult: bool,
+    ) -> object | list[object]:
         # called from all hookcaller instances.
         # enable_tracing will set its own wrapping function at self._inner_hookexec
-        return self._inner_hookexec(hook, methods, kwargs)
+        return self._inner_hookexec(hook_name, methods, kwargs, firstresult)
+
+    def register(self, plugin: _Plugin, name: str | None = None) -> str | None:
+        """Register a plugin and return its name.
 
-    def register(self, plugin, name=None):
-        """ Register a plugin and return its canonical name or ``None`` if the name
-        is blocked from registering.  Raise a :py:class:`ValueError` if the plugin
-        is already registered. """
+        If a name is not specified, a name is generated using
+        :func:`get_canonical_name`.
+
+        If the name is blocked from registering, returns ``None``.
+
+        If the plugin is already registered, raises a :class:`ValueError`.
+        """
         plugin_name = name or self.get_canonical_name(plugin)
 
-        if plugin_name in self._name2plugin or plugin in self._plugin2hookcallers:
+        if plugin_name in self._name2plugin:
             if self._name2plugin.get(plugin_name, -1) is None:
-                return  # blocked plugin, return None to indicate no registration
+                return None  # blocked plugin, return None to indicate no registration
             raise ValueError(
-                "Plugin already registered: %s=%s\n%s"
+                "Plugin name already registered: %s=%s\n%s"
+                % (plugin_name, plugin, self._name2plugin)
+            )
+
+        if plugin in self._name2plugin.values():
+            raise ValueError(
+                "Plugin already registered under a different name: %s=%s\n%s"
                 % (plugin_name, plugin, self._name2plugin)
             )
 
         # XXX if an error happens we should make sure no state has been
         # changed at point of return
         self._name2plugin[plugin_name] = plugin
 
         # register matching hook implementations of the plugin
-        self._plugin2hookcallers[plugin] = hookcallers = []
         for name in dir(plugin):
             hookimpl_opts = self.parse_hookimpl_opts(plugin, name)
             if hookimpl_opts is not None:
                 normalize_hookimpl_opts(hookimpl_opts)
-                method = getattr(plugin, name)
+                method: _HookImplFunction[object] = getattr(plugin, name)
                 hookimpl = HookImpl(plugin, plugin_name, method, hookimpl_opts)
                 name = hookimpl_opts.get("specname") or name
-                hook = getattr(self.hook, name, None)
+                hook: _HookCaller | None = getattr(self.hook, name, None)
                 if hook is None:
                     hook = _HookCaller(name, self._hookexec)
                     setattr(self.hook, name, hook)
                 elif hook.has_spec():
                     self._verify_hook(hook, hookimpl)
                     hook._maybe_apply_history(hookimpl)
                 hook._add_hookimpl(hookimpl)
-                hookcallers.append(hook)
         return plugin_name
 
-    def parse_hookimpl_opts(self, plugin, name):
-        method = getattr(plugin, name)
+    def parse_hookimpl_opts(self, plugin: _Plugin, name: str) -> _HookImplOpts | None:
+        method: object = getattr(plugin, name)
         if not inspect.isroutine(method):
-            return
+            return None
         try:
-            res = getattr(method, self.project_name + "_impl", None)
+            res: _HookImplOpts | None = getattr(
+                method, self.project_name + "_impl", None
+            )
         except Exception:
-            res = {}
+            res = {}  # type: ignore[assignment]
         if res is not None and not isinstance(res, dict):
             # false positive
-            res = None
-        # TODO: remove when we drop implprefix in 1.0
-        elif res is None and self._implprefix and name.startswith(self._implprefix):
-            _warn_for_function(
-                DeprecationWarning(
-                    "The `implprefix` system is deprecated please decorate "
-                    "this function using an instance of HookimplMarker."
-                ),
-                method,
-            )
-            res = {}
+            res = None  # type:ignore[unreachable]
         return res
 
-    def unregister(self, plugin=None, name=None):
-        """ unregister a plugin object and all its contained hook implementations
-        from internal data structures. """
+    def unregister(
+        self, plugin: _Plugin | None = None, name: str | None = None
+    ) -> _Plugin:
+        """Unregister a plugin and all of its hook implementations.
+
+        The plugin can be specified either by the plugin object or the plugin
+        name. If both are specified, they must agree.
+        """
         if name is None:
             assert plugin is not None, "one of name or plugin needs to be specified"
             name = self.get_name(plugin)
+            assert name is not None, "plugin is not registered"
 
         if plugin is None:
             plugin = self.get_plugin(name)
 
+        hookcallers = self.get_hookcallers(plugin)
+        if hookcallers:
+            for hookcaller in hookcallers:
+                hookcaller._remove_plugin(plugin)
+
         # if self._name2plugin[name] == None registration was blocked: ignore
         if self._name2plugin.get(name):
+            assert name is not None
             del self._name2plugin[name]
 
-        for hookcaller in self._plugin2hookcallers.pop(plugin, []):
-            hookcaller._remove_plugin(plugin)
-
         return plugin
 
-    def set_blocked(self, name):
-        """ block registrations of the given name, unregister if already registered. """
+    def set_blocked(self, name: str) -> None:
+        """Block registrations of the given name, unregister if already registered."""
         self.unregister(name=name)
         self._name2plugin[name] = None
 
-    def is_blocked(self, name):
-        """ return ``True`` if the given plugin name is blocked. """
+    def is_blocked(self, name: str) -> bool:
+        """Return whether the given plugin name is blocked."""
         return name in self._name2plugin and self._name2plugin[name] is None
 
-    def add_hookspecs(self, module_or_class):
-        """ add new hook specifications defined in the given ``module_or_class``.
-        Functions are recognized if they have been decorated accordingly. """
+    def add_hookspecs(self, module_or_class: _Namespace) -> None:
+        """Add new hook specifications defined in the given ``module_or_class``.
+
+        Functions are recognized as hook specifications if they have been
+        decorated with a matching :class:`HookspecMarker`.
+        """
         names = []
         for name in dir(module_or_class):
             spec_opts = self.parse_hookspec_opts(module_or_class, name)
             if spec_opts is not None:
-                hc = getattr(self.hook, name, None)
+                hc: _HookCaller | None = getattr(self.hook, name, None)
                 if hc is None:
                     hc = _HookCaller(name, self._hookexec, module_or_class, spec_opts)
                     setattr(self.hook, name, hc)
                 else:
-                    # plugins registered this hook without knowing the spec
+                    # Plugins registered this hook without knowing the spec.
                     hc.set_specification(module_or_class, spec_opts)
                     for hookfunction in hc.get_hookimpls():
                         self._verify_hook(hc, hookfunction)
                 names.append(name)
 
         if not names:
             raise ValueError(
-                "did not find any %r hooks in %r" % (self.project_name, module_or_class)
+                f"did not find any {self.project_name!r} hooks in {module_or_class!r}"
             )
 
-    def parse_hookspec_opts(self, module_or_class, name):
-        method = getattr(module_or_class, name)
-        return getattr(method, self.project_name + "_spec", None)
-
-    def get_plugins(self):
-        """ return the set of registered plugins. """
-        return set(self._plugin2hookcallers)
-
-    def is_registered(self, plugin):
-        """ Return ``True`` if the plugin is already registered. """
-        return plugin in self._plugin2hookcallers
-
-    def get_canonical_name(self, plugin):
-        """ Return canonical name for a plugin object. Note that a plugin
-        may be registered under a different name which was specified
-        by the caller of :py:meth:`register(plugin, name) <.PluginManager.register>`.
-        To obtain the name of an registered plugin use :py:meth:`get_name(plugin)
-        <.PluginManager.get_name>` instead."""
-        return getattr(plugin, "__name__", None) or str(id(plugin))
+    def parse_hookspec_opts(
+        self, module_or_class: _Namespace, name: str
+    ) -> _HookSpecOpts | None:
+        method: HookSpec = getattr(module_or_class, name)
+        opts: _HookSpecOpts | None = getattr(method, self.project_name + "_spec", None)
+        return opts
+
+    def get_plugins(self) -> set[Any]:
+        """Return a set of all registered plugin objects."""
+        return set(self._name2plugin.values())
+
+    def is_registered(self, plugin: _Plugin) -> bool:
+        """Return whether the plugin is already registered."""
+        return any(plugin == val for val in self._name2plugin.values())
+
+    def get_canonical_name(self, plugin: _Plugin) -> str:
+        """Return a canonical name for a plugin object.
+
+        Note that a plugin may be registered under a different name
+        specified by the caller of :meth:`register(plugin, name) <register>`.
+        To obtain the name of n registered plugin use :meth:`get_name(plugin)
+        <get_name>` instead.
+        """
+        name: str | None = getattr(plugin, "__name__", None)
+        return name or str(id(plugin))
 
-    def get_plugin(self, name):
-        """ Return a plugin or ``None`` for the given name. """
+    def get_plugin(self, name: str) -> Any | None:
+        """Return the plugin registered under the given name, if any."""
         return self._name2plugin.get(name)
 
-    def has_plugin(self, name):
-        """ Return ``True`` if a plugin with the given name is registered. """
+    def has_plugin(self, name: str) -> bool:
+        """Return whether a plugin with the given name is registered."""
         return self.get_plugin(name) is not None
 
-    def get_name(self, plugin):
-        """ Return name for registered plugin or ``None`` if not registered. """
+    def get_name(self, plugin: _Plugin) -> str | None:
+        """Return the name the plugin is registered under, or ``None`` if
+        is isn't."""
         for name, val in self._name2plugin.items():
             if plugin == val:
                 return name
+        return None
 
-    def _verify_hook(self, hook, hookimpl):
-        if hook.is_historic() and hookimpl.hookwrapper:
+    def _verify_hook(self, hook: _HookCaller, hookimpl: HookImpl) -> None:
+        if hook.is_historic() and (
+            hookimpl.hookwrapper or hookimpl.isgeneratorfunction
+        ):
             raise PluginValidationError(
                 hookimpl.plugin,
-                "Plugin %r\nhook %r\nhistoric incompatible to hookwrapper"
+                "Plugin %r\nhook %r\nhistoric incompatible with yield/hookwrapper"
                 % (hookimpl.plugin_name, hook.name),
             )
+
+        assert hook.spec is not None
         if hook.spec.warn_on_impl:
             _warn_for_function(hook.spec.warn_on_impl, hookimpl.function)
+
         # positional arg checking
         notinspec = set(hookimpl.argnames) - set(hook.spec.argnames)
         if notinspec:
             raise PluginValidationError(
                 hookimpl.plugin,
                 "Plugin %r for hook %r\nhookimpl definition: %s\n"
                 "Argument(s) %s are declared in the hookimpl but "
@@ -259,39 +315,48 @@
                     hookimpl.plugin_name,
                     hook.name,
                     _formatdef(hookimpl.function),
                     notinspec,
                 ),
             )
 
-    def check_pending(self):
-        """ Verify that all hooks which have not been verified against
-        a hook specification are optional, otherwise raise :py:class:`.PluginValidationError`."""
+        if hookimpl.hookwrapper and not inspect.isgeneratorfunction(hookimpl.function):
+            raise PluginValidationError(
+                hookimpl.plugin,
+                "Plugin %r for hook %r\nhookimpl definition: %s\n"
+                "Declared as hookwrapper=True but function is not a generator function"
+                % (hookimpl.plugin_name, hook.name, _formatdef(hookimpl.function)),
+            )
+
+    def check_pending(self) -> None:
+        """Verify that all hooks which have not been verified against a
+        hook specification are optional, otherwise raise
+        :class:`PluginValidationError`."""
         for name in self.hook.__dict__:
             if name[0] != "_":
-                hook = getattr(self.hook, name)
+                hook: _HookCaller = getattr(self.hook, name)
                 if not hook.has_spec():
                     for hookimpl in hook.get_hookimpls():
                         if not hookimpl.optionalhook:
                             raise PluginValidationError(
                                 hookimpl.plugin,
                                 "unknown hook %r in plugin %r"
                                 % (name, hookimpl.plugin),
                             )
 
-    def load_setuptools_entrypoints(self, group, name=None):
-        """ Load modules from querying the specified setuptools ``group``.
+    def load_setuptools_entrypoints(self, group: str, name: str | None = None) -> int:
+        """Load modules from querying the specified setuptools ``group``.
 
-        :param str group: entry point group to load plugins
-        :param str name: if given, loads only plugins with the given ``name``.
+        :param str group: Entry point group to load plugins.
+        :param str name: If given, loads only plugins with the given ``name``.
         :rtype: int
-        :return: return the number of loaded plugins by this call.
+        :return: The number of plugins loaded by this call.
         """
         count = 0
-        for dist in importlib_metadata.distributions():
+        for dist in list(importlib_metadata.distributions()):
             for ep in dist.entry_points:
                 if (
                     ep.group != group
                     or (name is not None and ep.name != name)
                     # already registered
                     or self.get_plugin(ep.name)
                     or self.is_blocked(ep.name)
@@ -299,97 +364,104 @@
                     continue
                 plugin = ep.load()
                 self.register(plugin, name=ep.name)
                 self._plugin_distinfo.append((plugin, DistFacade(dist)))
                 count += 1
         return count
 
-    def list_plugin_distinfo(self):
-        """ return list of distinfo/plugin tuples for all setuptools registered
-        plugins. """
+    def list_plugin_distinfo(self) -> list[tuple[_Plugin, DistFacade]]:
+        """Return a list of (plugin, distinfo) pairs for all
+        setuptools-registered plugins."""
         return list(self._plugin_distinfo)
 
-    def list_name_plugin(self):
-        """ return list of name/plugin pairs. """
+    def list_name_plugin(self) -> list[tuple[str, _Plugin]]:
+        """Return a list of (name, plugin) pairs for all registered plugins."""
         return list(self._name2plugin.items())
 
-    def get_hookcallers(self, plugin):
-        """ get all hook callers for the specified plugin. """
-        return self._plugin2hookcallers.get(plugin)
-
-    def add_hookcall_monitoring(self, before, after):
-        """ add before/after tracing functions for all hooks
-        and return an undo function which, when called,
-        will remove the added tracers.
+    def get_hookcallers(self, plugin: _Plugin) -> list[_HookCaller] | None:
+        """Get all hook callers for the specified plugin."""
+        if self.get_name(plugin) is None:
+            return None
+        hookcallers = []
+        for hookcaller in self.hook.__dict__.values():
+            for hookimpl in hookcaller.get_hookimpls():
+                if hookimpl.plugin is plugin:
+                    hookcallers.append(hookcaller)
+        return hookcallers
+
+    def add_hookcall_monitoring(
+        self, before: _BeforeTrace, after: _AfterTrace
+    ) -> Callable[[], None]:
+        """Add before/after tracing functions for all hooks.
+
+        Returns an undo function which, when called, removes the added tracers.
 
         ``before(hook_name, hook_impls, kwargs)`` will be called ahead
         of all hook calls and receive a hookcaller instance, a list
         of HookImpl instances and the keyword arguments for the hook call.
 
         ``after(outcome, hook_name, hook_impls, kwargs)`` receives the
-        same arguments as ``before`` but also a :py:class:`pluggy.callers._Result` object
+        same arguments as ``before`` but also a :class:`_Result` object
         which represents the result of the overall hook call.
         """
         oldcall = self._inner_hookexec
 
-        def traced_hookexec(hook, hook_impls, kwargs):
-            before(hook.name, hook_impls, kwargs)
-            outcome = _Result.from_call(lambda: oldcall(hook, hook_impls, kwargs))
-            after(outcome, hook.name, hook_impls, kwargs)
+        def traced_hookexec(
+            hook_name: str,
+            hook_impls: Sequence[HookImpl],
+            caller_kwargs: Mapping[str, object],
+            firstresult: bool,
+        ) -> object | list[object]:
+            before(hook_name, hook_impls, caller_kwargs)
+            outcome = _Result.from_call(
+                lambda: oldcall(hook_name, hook_impls, caller_kwargs, firstresult)
+            )
+            after(outcome, hook_name, hook_impls, caller_kwargs)
             return outcome.get_result()
 
         self._inner_hookexec = traced_hookexec
 
-        def undo():
+        def undo() -> None:
             self._inner_hookexec = oldcall
 
         return undo
 
-    def enable_tracing(self):
-        """ enable tracing of hook calls and return an undo function. """
+    def enable_tracing(self) -> Callable[[], None]:
+        """Enable tracing of hook calls.
+
+        Returns an undo function which, when called, removes the added tracing.
+        """
         hooktrace = self.trace.root.get("hook")
 
-        def before(hook_name, methods, kwargs):
+        def before(
+            hook_name: str, methods: Sequence[HookImpl], kwargs: Mapping[str, object]
+        ) -> None:
             hooktrace.root.indent += 1
             hooktrace(hook_name, kwargs)
 
-        def after(outcome, hook_name, methods, kwargs):
-            if outcome.excinfo is None:
+        def after(
+            outcome: _Result[object],
+            hook_name: str,
+            methods: Sequence[HookImpl],
+            kwargs: Mapping[str, object],
+        ) -> None:
+            if outcome.exception is None:
                 hooktrace("finish", hook_name, "-->", outcome.get_result())
             hooktrace.root.indent -= 1
 
         return self.add_hookcall_monitoring(before, after)
 
-    def subset_hook_caller(self, name, remove_plugins):
-        """ Return a new :py:class:`.hooks._HookCaller` instance for the named method
-        which manages calls to all registered plugins except the
-        ones from remove_plugins. """
-        orig = getattr(self.hook, name)
-        plugins_to_remove = [plug for plug in remove_plugins if hasattr(plug, name)]
+    def subset_hook_caller(
+        self, name: str, remove_plugins: Iterable[_Plugin]
+    ) -> _HookCaller:
+        """Return a proxy :py:class:`._hooks._HookCaller` instance for the named
+        method which manages calls to all registered plugins except the ones
+        from remove_plugins."""
+        orig: _HookCaller = getattr(self.hook, name)
+        plugins_to_remove = {plug for plug in remove_plugins if hasattr(plug, name)}
         if plugins_to_remove:
-            hc = _HookCaller(
-                orig.name, orig._hookexec, orig.spec.namespace, orig.spec.opts
-            )
-            for hookimpl in orig.get_hookimpls():
-                plugin = hookimpl.plugin
-                if plugin not in plugins_to_remove:
-                    hc._add_hookimpl(hookimpl)
-                    # we also keep track of this hook caller so it
-                    # gets properly removed on plugin unregistration
-                    self._plugin2hookcallers.setdefault(plugin, []).append(hc)
-            return hc
+            return _SubsetHookCaller(orig, plugins_to_remove)
         return orig
 
 
-if hasattr(inspect, "signature"):
-
-    def _formatdef(func):
-        return "%s%s" % (func.__name__, str(inspect.signature(func)))
-
-
-else:
-
-    def _formatdef(func):
-        return "%s%s" % (
-            func.__name__,
-            inspect.formatargspec(*inspect.getargspec(func)),
-        )
+def _formatdef(func: Callable[..., object]) -> str:
+    return f"{func.__name__}{inspect.signature(func)}"
```

### Comparing `pluggy-1.0.0.dev0/src/pluggy.egg-info/SOURCES.txt` & `pluggy-1.1.0/src/pluggy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
-.travis.yml
 CHANGELOG.rst
-HOWTORELEASE.rst
 LICENSE
 MANIFEST.in
 README.rst
-appveyor.yml
+RELEASING.rst
 codecov.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
-changelog/59.removal.rst
+.github/workflows/main.yml
 changelog/README.rst
 changelog/_template.rst
 docs/api_reference.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/_static/img/plug.png
@@ -26,28 +24,30 @@
 docs/examples/eggsample-spam/eggsample_spam.py
 docs/examples/eggsample-spam/setup.py
 docs/examples/eggsample/eggsample/__init__.py
 docs/examples/eggsample/eggsample/hookspecs.py
 docs/examples/eggsample/eggsample/host.py
 docs/examples/eggsample/eggsample/lib.py
 scripts/release.py
+scripts/towncrier-draft-to-file.py
+scripts/upload-coverage.sh
 src/pluggy/__init__.py
+src/pluggy/_callers.py
+src/pluggy/_hooks.py
+src/pluggy/_manager.py
+src/pluggy/_result.py
 src/pluggy/_tracing.py
 src/pluggy/_version.py
-src/pluggy/callers.py
-src/pluggy/hooks.py
-src/pluggy/manager.py
 src/pluggy.egg-info/PKG-INFO
 src/pluggy.egg-info/SOURCES.txt
 src/pluggy.egg-info/dependency_links.txt
 src/pluggy.egg-info/requires.txt
 src/pluggy.egg-info/top_level.txt
 testing/benchmark.py
 testing/conftest.py
-testing/test_deprecations.py
 testing/test_details.py
 testing/test_helpers.py
 testing/test_hookcaller.py
 testing/test_invocations.py
 testing/test_multicall.py
 testing/test_pluginmanager.py
 testing/test_tracer.py
```

### Comparing `pluggy-1.0.0.dev0/tox.ini` & `pluggy-1.1.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 [tox]
-envlist=linting,docs,py{27,34,35,36,37,38,py,py3},py{36,37}-pytest{master,features}
+envlist=linting,docs,py{37,38,39,310,311,py3},py{37}-pytest{main}
 
 [testenv]
 commands=
   {env:_PLUGGY_TOX_CMD:pytest} {posargs}
   coverage: coverage report -m
   coverage: coverage xml
 setenv=
   _PYTEST_SETUP_SKIP_PLUGGY_DEP=1
   coverage: _PLUGGY_TOX_CMD=coverage run -m pytest
 extras=testing
 deps=
   coverage: coverage
-  pytestmaster: git+https://github.com/pytest-dev/pytest.git@master
+  pytestmain: git+https://github.com/pytest-dev/pytest.git@main
 
 [testenv:benchmark]
 commands=pytest {posargs:testing/benchmark.py}
 deps=
   pytest
   pytest-benchmark
 
-[testenv:linting]
-skip_install = true
-basepython = python3.6
-deps = pre-commit
-commands = pre-commit run --all-files --show-diff-on-failure
-
 [testenv:docs]
 deps =
   sphinx
   pygments
+  towncrier
 commands =
-  sphinx-build -W -b html {toxinidir}/docs {toxinidir}/build/html-docs
+  python scripts/towncrier-draft-to-file.py
+  # the '-t changelog_towncrier_draft' tags makes sphinx include the draft
+  # changelog in the docs; this does not happen on ReadTheDocs because it uses
+  # the standard sphinx command so the 'changelog_towncrier_draft' is never set there
+  sphinx-build -W -b html {toxinidir}/docs {toxinidir}/build/html-docs -t changelog_towncrier_draft {posargs:}
 
 [pytest]
 minversion=2.0
 testpaths = testing
 #--pyargs --doctest-modules --ignore=.tox
 addopts=-r a
 filterwarnings =
   error
 
 [flake8]
 max-line-length=99
 
 [testenv:release]
-decription = do a release, required posarg of the version number
+description = do a release, required posarg of the version number
 basepython = python3
 skipsdist = True
 usedevelop = True
 passenv = *
 deps =
     colorama
     gitpython
```

### Comparing `pluggy-1.0.0.dev0/.gitignore` & `pluggy-1.1.0/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -35,30 +35,35 @@
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .coverage
 .coverage.*
 .cache
+.mypy_cache/
 nosetests.xml
 coverage.xml
 *,cover
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
 
 # Sphinx documentation
 docs/_build/
+docs/_changelog_towncrier_draft.rst
 
 # PyBuilder
 target/
 *.swp
 
 # generated by setuptools_scm
 src/pluggy/_version.py
 
 # generated by pip
 pip-wheel-metadata/
+
+# pytest-benchmark
+.benchmarks/
```

### Comparing `pluggy-1.0.0.dev0/scripts/release.py` & `pluggy-1.1.0/scripts/release.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
 Release script.
 """
 import argparse
 import sys
 from subprocess import check_call
 
-from colorama import init, Fore
-from git import Repo, Remote
+from colorama import Fore
+from colorama import init
+from git import Remote
+from git import Repo
 
 
 def create_branch(version):
-    """Create a fresh branch from upstream/master"""
+    """Create a fresh branch from upstream/main"""
     repo = Repo.init(".")
     if repo.is_dirty(untracked_files=True):
         raise RuntimeError("Repository is dirty, please commit/stash your changes.")
 
     branch_name = f"release-{version}"
-    print(f"{Fore.CYAN}Create {branch_name} branch from upstream master")
+    print(f"{Fore.CYAN}Create {branch_name} branch from upstream main")
     upstream = get_upstream(repo)
     upstream.fetch()
-    release_branch = repo.create_head(branch_name, upstream.refs.master, force=True)
+    release_branch = repo.create_head(branch_name, upstream.refs.main, force=True)
     release_branch.checkout()
     return repo
 
 
 def get_upstream(repo: Repo) -> Remote:
     """Find upstream repository for pluggy on the remotes"""
     for remote in repo.remotes:
@@ -46,15 +48,15 @@
 
 def changelog(version, write_out=False):
     if write_out:
         addopts = []
     else:
         addopts = ["--draft"]
     print(f"{Fore.CYAN}Generating CHANGELOG")
-    check_call(["towncrier", "--yes", "--version", version] + addopts)
+    check_call(["towncrier", "build", "--yes", "--version", version] + addopts)
 
 
 def main():
     init(autoreset=True)
     parser = argparse.ArgumentParser()
     parser.add_argument("version", help="Release version")
     options = parser.parse_args()
```

### Comparing `pluggy-1.0.0.dev0/LICENSE` & `pluggy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pluggy-1.0.0.dev0/README.rst` & `pluggy-1.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ====================================================
 pluggy - A minimalist production ready plugin system
 ====================================================
 
-|pypi| |conda-forge| |versions| |travis| |appveyor| |gitter| |black| |codecov|
+|pypi| |conda-forge| |versions| |github-actions| |gitter| |black| |codecov|
 
 This is the core framework used by the `pytest`_, `tox`_, and `devpi`_ projects.
 
 Please `read the docs`_ to learn more!
 
 A definitive example
 ====================
@@ -14,37 +14,33 @@
 
     import pluggy
 
     hookspec = pluggy.HookspecMarker("myproject")
     hookimpl = pluggy.HookimplMarker("myproject")
 
 
-    class MySpec(object):
-        """A hook specification namespace.
-        """
+    class MySpec:
+        """A hook specification namespace."""
 
         @hookspec
         def myhook(self, arg1, arg2):
-            """My special little hook that you can customize.
-            """
+            """My special little hook that you can customize."""
 
 
-    class Plugin_1(object):
-        """A hook implementation namespace.
-        """
+    class Plugin_1:
+        """A hook implementation namespace."""
 
         @hookimpl
         def myhook(self, arg1, arg2):
             print("inside Plugin_1.myhook()")
             return arg1 + arg2
 
 
-    class Plugin_2(object):
-        """A 2nd hook implementation namespace.
-        """
+    class Plugin_2:
+        """A 2nd hook implementation namespace."""
 
         @hookimpl
         def myhook(self, arg1, arg2):
             print("inside Plugin_2.myhook()")
             return arg1 - arg2
 
 
@@ -73,19 +69,16 @@
 
 .. |pypi| image:: https://img.shields.io/pypi/v/pluggy.svg
     :target: https://pypi.org/pypi/pluggy
 
 .. |versions| image:: https://img.shields.io/pypi/pyversions/pluggy.svg
     :target: https://pypi.org/pypi/pluggy
 
-.. |travis| image:: https://img.shields.io/travis/pytest-dev/pluggy/master.svg
-    :target: https://travis-ci.org/pytest-dev/pluggy
-
-.. |appveyor| image:: https://img.shields.io/appveyor/ci/pytestbot/pluggy/master.svg
-    :target: https://ci.appveyor.com/project/pytestbot/pluggy
+.. |github-actions| image:: https://github.com/pytest-dev/pluggy/workflows/main/badge.svg
+    :target: https://github.com/pytest-dev/pluggy/actions
 
 .. |conda-forge| image:: https://img.shields.io/conda/vn/conda-forge/pluggy.svg
     :target: https://anaconda.org/conda-forge/pytest
 
 .. |gitter| image:: https://badges.gitter.im/pytest-dev/pluggy.svg
     :alt: Join the chat at https://gitter.im/pytest-dev/pluggy
     :target: https://gitter.im/pytest-dev/pluggy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
```

### Comparing `pluggy-1.0.0.dev0/.pre-commit-config.yaml` & `pluggy-1.1.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,55 @@
 repos:
--   repo: https://github.com/ambv/black
-    rev: 19.10b0
+-   repo: https://github.com/PyCQA/autoflake
+    rev: v2.1.1
     hooks:
-    -   id: black
-        args: [--safe, --quiet]
-        language_version: python3.6
--   repo: https://github.com/asottile/blacken-docs
-    rev: v0.5.0
+    -   id: autoflake
+        name: autoflake
+        args: ["--in-place", "--remove-unused-variables", "--remove-all-unused-imports"]
+        language: python
+        files: \.py$
+-   repo: https://github.com/asottile/reorder-python-imports
+    rev: v3.9.0
     hooks:
-    -   id: blacken-docs
-        additional_dependencies: [black==19.10b0]
-        language_version: python3.6
+    -   id: reorder-python-imports
+        args: ['--application-directories=.:src', --py37-plus]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.1.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: flake8
+        additional_dependencies: [flake8-typing-imports]
+-   repo: https://github.com/pre-commit/pygrep-hooks
+    rev: v1.10.0
+    hooks:
+    -   id: rst-backticks
+-   repo: https://github.com/asottile/pyupgrade
+    rev: v3.6.0
+    hooks:
+    -   id: pyupgrade
+        args: [--py37-plus]
+-   repo: https://github.com/psf/black
+    rev: 23.3.0
+    hooks:
+    -   id: black
+        args: [--safe, --quiet]
+-   repo: https://github.com/asottile/blacken-docs
+    rev: 1.13.0
+    hooks:
+    -   id: blacken-docs
+        additional_dependencies: [black==22.10.0]
 -   repo: local
     hooks:
     -   id: rst
         name: rst
         entry: rst-lint --encoding utf-8
-        files: ^(CHANGELOG.rst|HOWTORELEASE.rst|README.rst|changelog/.*)$
+        files: ^(HOWTORELEASE.rst|README.rst)$
         language: python
         additional_dependencies: [pygments, restructuredtext_lint]
-        language_version: python3.6
--   repo: https://github.com/pre-commit/pygrep-hooks
+-   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
-    -   id: rst-backticks
+    -   id: mypy
+        files: ^(src/|testing/)
+        args: []
+        additional_dependencies: [pytest]
```

### Comparing `pluggy-1.0.0.dev0/HOWTORELEASE.rst` & `pluggy-1.1.0/RELEASING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 #. From a clean work tree, execute::
 
     tox -e release -- VERSION
 
    This will create the branch ready to be pushed.
 
-#. Open a PR targeting ``master``.
+#. Open a PR targeting ``main``.
 
 #. All tests must pass and the PR must be approved by at least another maintainer.
 
 #. Publish to PyPI by pushing a tag::
 
      git tag X.Y.Z release-X.Y.Z
      git push git@github.com:pytest-dev/pluggy.git X.Y.Z
 
    The tag will trigger a new build, which will deploy to PyPI.
 
 #. Make sure it is `available on PyPI <https://pypi.org/project/pluggy>`_.
 
-#. Merge the PR into ``master``, either manually or using GitHub's web interface.
+#. Merge the PR into ``main``, either manually or using GitHub's web interface.
```

### Comparing `pluggy-1.0.0.dev0/testing/test_invocations.py` & `pluggy-1.1.0/testing/test_invocations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,216 +1,289 @@
 import pytest
-from pluggy import PluginValidationError, HookimplMarker, HookspecMarker
+
+from pluggy import HookimplMarker
+from pluggy import HookspecMarker
+from pluggy import PluginManager
+from pluggy import PluginValidationError
 
 
 hookspec = HookspecMarker("example")
 hookimpl = HookimplMarker("example")
 
 
-def test_argmismatch(pm):
-    class Api(object):
+def test_argmismatch(pm: PluginManager) -> None:
+    class Api:
         @hookspec
         def hello(self, arg):
             "api hook 1"
 
     pm.add_hookspecs(Api)
 
-    class Plugin(object):
+    class Plugin:
         @hookimpl
         def hello(self, argwrong):
             pass
 
     with pytest.raises(PluginValidationError) as exc:
         pm.register(Plugin())
 
     assert "argwrong" in str(exc.value)
 
 
-def test_only_kwargs(pm):
-    class Api(object):
+def test_only_kwargs(pm: PluginManager) -> None:
+    class Api:
         @hookspec
         def hello(self, arg):
             "api hook 1"
 
     pm.add_hookspecs(Api)
     with pytest.raises(TypeError) as exc:
-        pm.hook.hello(3)
+        pm.hook.hello(3)  # type: ignore[call-arg]
 
-    comprehensible = "hook calling supports only keyword arguments"
-    assert comprehensible in str(exc.value)
+    message = "__call__() takes 1 positional argument but 2 were given"
+    assert message in str(exc.value)
 
 
-def test_opt_in_args(pm):
-    """Verfiy that two hookimpls with mutex args can serve
+def test_opt_in_args(pm: PluginManager) -> None:
+    """Verify that two hookimpls with mutex args can serve
     under the same spec.
     """
 
-    class Api(object):
+    class Api:
         @hookspec
         def hello(self, arg1, arg2, common_arg):
             "api hook 1"
 
-    class Plugin1(object):
+    class Plugin1:
         @hookimpl
         def hello(self, arg1, common_arg):
             return arg1 + common_arg
 
-    class Plugin2(object):
+    class Plugin2:
         @hookimpl
         def hello(self, arg2, common_arg):
             return arg2 + common_arg
 
     pm.add_hookspecs(Api)
     pm.register(Plugin1())
     pm.register(Plugin2())
 
     results = pm.hook.hello(arg1=1, arg2=2, common_arg=0)
     assert results == [2, 1]
 
 
-def test_call_order(pm):
-    class Api(object):
+def test_call_order(pm: PluginManager) -> None:
+    class Api:
         @hookspec
         def hello(self, arg):
             "api hook 1"
 
     pm.add_hookspecs(Api)
 
-    class Plugin1(object):
+    class Plugin1:
         @hookimpl
         def hello(self, arg):
             return 1
 
-    class Plugin2(object):
+    class Plugin2:
         @hookimpl
         def hello(self, arg):
             return 2
 
-    class Plugin3(object):
+    class Plugin3:
         @hookimpl
         def hello(self, arg):
             return 3
 
-    class Plugin4(object):
+    class Plugin4:
         @hookimpl(hookwrapper=True)
         def hello(self, arg):
             assert arg == 0
             outcome = yield
             assert outcome.get_result() == [3, 2, 1]
+            assert outcome.exception is None
+            assert outcome.excinfo is None
+
+    class Plugin5:
+        @hookimpl
+        def hello(self, arg):
+            assert arg == 0
+            outcome = yield
+            assert outcome == [3, 2, 1]
+            return outcome
 
     pm.register(Plugin1())
     pm.register(Plugin2())
     pm.register(Plugin3())
     pm.register(Plugin4())  # hookwrapper should get same list result
+    pm.register(Plugin5())  # hookwrapper should get same list result
     res = pm.hook.hello(arg=0)
     assert res == [3, 2, 1]
 
 
-def test_firstresult_definition(pm):
-    class Api(object):
+def test_firstresult_definition(pm: PluginManager) -> None:
+    class Api:
         @hookspec(firstresult=True)
         def hello(self, arg):
             "api hook 1"
 
     pm.add_hookspecs(Api)
 
-    class Plugin1(object):
+    class Plugin1:
         @hookimpl
         def hello(self, arg):
             return arg + 1
 
-    class Plugin2(object):
+    class Plugin2:
         @hookimpl
         def hello(self, arg):
             return arg - 1
 
-    class Plugin3(object):
+    class Plugin3:
         @hookimpl
         def hello(self, arg):
             return None
 
-    class Plugin4(object):
+    class Plugin4:
+        def hello(self, arg):
+            assert arg == 3
+            outcome = yield
+            assert outcome == 2
+            return outcome
+
+    class Plugin5:
         @hookimpl(hookwrapper=True)
         def hello(self, arg):
             assert arg == 3
             outcome = yield
             assert outcome.get_result() == 2
 
     pm.register(Plugin1())  # discarded - not the last registered plugin
     pm.register(Plugin2())  # used as result
     pm.register(Plugin3())  # None result is ignored
     pm.register(Plugin4())  # hookwrapper should get same non-list result
+    pm.register(Plugin5())  # hookwrapper should get same non-list result
     res = pm.hook.hello(arg=3)
     assert res == 2
 
 
-def test_firstresult_force_result(pm):
-    """Verify forcing a result in a wrapper.
-    """
+def test_firstresult_force_result_hookwrapper(pm: PluginManager) -> None:
+    """Verify forcing a result in a wrapper."""
 
-    class Api(object):
+    class Api:
         @hookspec(firstresult=True)
         def hello(self, arg):
             "api hook 1"
 
     pm.add_hookspecs(Api)
 
-    class Plugin1(object):
+    class Plugin1:
         @hookimpl
         def hello(self, arg):
             return arg + 1
 
-    class Plugin2(object):
+    class Plugin2:
         @hookimpl(hookwrapper=True)
         def hello(self, arg):
             assert arg == 3
             outcome = yield
             assert outcome.get_result() == 4
             outcome.force_result(0)
 
-    class Plugin3(object):
+    class Plugin3:
+        @hookimpl
+        def hello(self, arg):
+            return None
+
+    pm.register(Plugin1())
+    pm.register(Plugin2())  # wrapper
+    pm.register(Plugin3())  # ignored since returns None
+    res = pm.hook.hello(arg=3)
+    assert res == 0  # this result is forced and not a list
+
+
+def test_firstresult_force_result(pm: PluginManager) -> None:
+    """Verify forcing a result in a wrapper."""
+
+    class Api:
+        @hookspec(firstresult=True)
+        def hello(self, arg):
+            "api hook 1"
+
+    pm.add_hookspecs(Api)
+
+    class Plugin1:
+        @hookimpl
+        def hello(self, arg):
+            return arg + 1
+
+    class Plugin2:
+        @hookimpl
+        def hello(self, arg):
+            assert arg == 3
+            outcome = yield
+            assert outcome == 4
+            return 0
+
+    class Plugin3:
         @hookimpl
         def hello(self, arg):
             return None
 
     pm.register(Plugin1())
     pm.register(Plugin2())  # wrapper
     pm.register(Plugin3())  # ignored since returns None
     res = pm.hook.hello(arg=3)
     assert res == 0  # this result is forced and not a list
 
 
-def test_firstresult_returns_none(pm):
+def test_firstresult_returns_none(pm: PluginManager) -> None:
     """If None results are returned by underlying implementations ensure
     the multi-call loop returns a None value.
     """
 
-    class Api(object):
+    class Api:
         @hookspec(firstresult=True)
         def hello(self, arg):
             "api hook 1"
 
     pm.add_hookspecs(Api)
 
-    class Plugin1(object):
+    class Plugin1:
         @hookimpl
         def hello(self, arg):
             return None
 
     pm.register(Plugin1())
     res = pm.hook.hello(arg=3)
     assert res is None
 
 
-def test_firstresult_no_plugin(pm):
+def test_firstresult_no_plugin(pm: PluginManager) -> None:
     """If no implementations/plugins have been registered for a firstresult
     hook the multi-call loop should return a None value.
     """
 
-    class Api(object):
+    class Api:
         @hookspec(firstresult=True)
         def hello(self, arg):
             "api hook 1"
 
     pm.add_hookspecs(Api)
     res = pm.hook.hello(arg=3)
     assert res is None
+
+
+def test_no_hookspec(pm: PluginManager) -> None:
+    """A hook with hookimpls can still be called even if no hookspec
+    was registered for it (and call_pending wasn't called to check
+    against it).
+    """
+
+    class Plugin:
+        @hookimpl
+        def hello(self, arg):
+            return "Plugin.hello"
+
+    pm.register(Plugin())
+
+    assert pm.hook.hello(arg=10, extra=20) == ["Plugin.hello"]
```

### Comparing `pluggy-1.0.0.dev0/testing/test_tracer.py` & `pluggy-1.1.0/testing/test_tracer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from pluggy._tracing import TagTracer
+from typing import List
 
 import pytest
 
+from pluggy._tracing import TagTracer
+
 
 @pytest.fixture
-def rootlogger():
+def rootlogger() -> TagTracer:
     return TagTracer()
 
 
-def test_simple(rootlogger):
+def test_simple(rootlogger: TagTracer) -> None:
     log = rootlogger.get("pytest")
     log("hello")
-    out = []
+    out: List[str] = []
     rootlogger.setwriter(out.append)
     log("world")
     assert len(out) == 1
     assert out[0] == "world [pytest]\n"
     sublog = log.get("collection")
     sublog("hello")
     assert out[1] == "hello [pytest:collection]\n"
 
 
-def test_indent(rootlogger):
+def test_indent(rootlogger: TagTracer) -> None:
     log = rootlogger.get("1")
     out = []
     log.root.setwriter(lambda arg: out.append(arg))
     log("hello")
     log.root.indent += 1
     log("line1")
     log("line2")
@@ -45,24 +47,23 @@
         "    line3",
         "    line4",
         "  line5",
         "last",
     ]
 
 
-def test_readable_output_dictargs(rootlogger):
-
+def test_readable_output_dictargs(rootlogger: TagTracer) -> None:
     out = rootlogger._format_message(["test"], [1])
     assert out == "1 [test]\n"
 
     out2 = rootlogger._format_message(["test"], ["test", {"a": 1}])
     assert out2 == "test [test]\n    a: 1\n"
 
 
-def test_setprocessor(rootlogger):
+def test_setprocessor(rootlogger: TagTracer) -> None:
     log = rootlogger.get("1")
     log2 = log.get("2")
     assert log2.tags == tuple("12")
     out = []
     rootlogger.setprocessor(tuple("12"), lambda *args: out.append(args))
     log("not seen")
     log2("seen")
```

### Comparing `pluggy-1.0.0.dev0/testing/test_details.py` & `pluggy-1.1.0/testing/test_details.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,86 @@
-import warnings
 import pytest
-from pluggy import PluginManager, HookimplMarker, HookspecMarker
+
+from pluggy import HookimplMarker
+from pluggy import HookspecMarker
+from pluggy import PluginManager
 
 hookspec = HookspecMarker("example")
 hookimpl = HookimplMarker("example")
 
 
-def test_parse_hookimpl_override():
+def test_parse_hookimpl_override() -> None:
     class MyPluginManager(PluginManager):
         def parse_hookimpl_opts(self, module_or_class, name):
             opts = PluginManager.parse_hookimpl_opts(self, module_or_class, name)
             if opts is None:
                 if name.startswith("x1"):
-                    opts = {}
+                    opts = {}  # type: ignore[assignment]
             return opts
 
-    class Plugin(object):
+    class Plugin:
         def x1meth(self):
             pass
 
         @hookimpl(hookwrapper=True, tryfirst=True)
         def x1meth2(self):
-            pass
+            yield  # pragma: no cover
+
+        @hookimpl(trylast=True)
+        def x1meth3(self):
+            return (yield)  # pragma: no cover
 
-    class Spec(object):
+    class Spec:
         @hookspec
         def x1meth(self):
             pass
 
         @hookspec
         def x1meth2(self):
             pass
 
+        @hookspec
+        def x1meth3(self):
+            pass
+
     pm = MyPluginManager(hookspec.project_name)
     pm.register(Plugin())
     pm.add_hookspecs(Spec)
-    assert not pm.hook.x1meth._nonwrappers[0].hookwrapper
-    assert not pm.hook.x1meth._nonwrappers[0].tryfirst
-    assert not pm.hook.x1meth._nonwrappers[0].trylast
-    assert not pm.hook.x1meth._nonwrappers[0].optionalhook
 
-    assert pm.hook.x1meth2._wrappers[0].tryfirst
-    assert pm.hook.x1meth2._wrappers[0].hookwrapper
+    hookimpls = pm.hook.x1meth.get_hookimpls()
+    assert len(hookimpls) == 1
+    assert not hookimpls[0].hookwrapper
+    assert not hookimpls[0].isgeneratorfunction
+    assert not hookimpls[0].tryfirst
+    assert not hookimpls[0].trylast
+    assert not hookimpls[0].optionalhook
+
+    hookimpls = pm.hook.x1meth2.get_hookimpls()
+    assert len(hookimpls) == 1
+    assert hookimpls[0].hookwrapper
+    assert hookimpls[0].isgeneratorfunction
+    assert hookimpls[0].tryfirst
+
+    hookimpls = pm.hook.x1meth3.get_hookimpls()
+    assert len(hookimpls) == 1
+    assert not hookimpls[0].hookwrapper
+    assert hookimpls[0].isgeneratorfunction
+    assert not hookimpls[0].tryfirst
+    assert hookimpls[0].trylast
 
 
-def test_warn_when_deprecated_specified(recwarn):
+def test_warn_when_deprecated_specified(recwarn) -> None:
     warning = DeprecationWarning("foo is deprecated")
 
-    class Spec(object):
+    class Spec:
         @hookspec(warn_on_impl=warning)
         def foo(self):
             pass
 
-    class Plugin(object):
+    class Plugin:
         @hookimpl
         def foo(self):
             pass
 
     pm = PluginManager(hookspec.project_name)
     pm.add_hookspecs(Spec)
 
@@ -64,72 +88,70 @@
         pm.register(Plugin())
     (record,) = records
     assert record.message is warning
     assert record.filename == Plugin.foo.__code__.co_filename
     assert record.lineno == Plugin.foo.__code__.co_firstlineno
 
 
-def test_plugin_getattr_raises_errors():
+def test_plugin_getattr_raises_errors() -> None:
     """Pluggy must be able to handle plugins which raise weird exceptions
     when getattr() gets called (#11).
     """
 
-    class DontTouchMe(object):
+    class DontTouchMe:
         def __getattr__(self, x):
-            raise Exception("cant touch me")
+            raise Exception("can't touch me")
 
-    class Module(object):
+    class Module:
         pass
 
     module = Module()
-    module.x = DontTouchMe()
+    module.x = DontTouchMe()  # type: ignore[attr-defined]
 
     pm = PluginManager(hookspec.project_name)
     # register() would raise an error
     pm.register(module, "donttouch")
     assert pm.get_plugin("donttouch") is module
 
 
-def test_warning_on_call_vs_hookspec_arg_mismatch():
-    """Verify that is a hook is called with less arguments then defined in the
-    spec that a warning is emitted.
-    """
+def test_not_all_arguments_are_provided_issues_a_warning(pm: PluginManager) -> None:
+    """Calling a hook without providing all arguments specified in
+    the hook spec issues a warning."""
 
     class Spec:
         @hookspec
-        def myhook(self, arg1, arg2):
+        def hello(self, arg1, arg2):
             pass
 
-    class Plugin:
-        @hookimpl
-        def myhook(self, arg1):
+        @hookspec(historic=True)
+        def herstory(self, arg1, arg2):
             pass
 
-    pm = PluginManager(hookspec.project_name)
-    pm.register(Plugin())
-    pm.add_hookspecs(Spec())
+    pm.add_hookspecs(Spec)
 
-    with warnings.catch_warnings(record=True) as warns:
-        warnings.simplefilter("always")
+    with pytest.warns(UserWarning, match=r"'arg1', 'arg2'.*cannot be found.*$"):
+        pm.hook.hello()
+    with pytest.warns(UserWarning, match=r"'arg2'.*cannot be found.*$"):
+        pm.hook.hello(arg1=1)
+    with pytest.warns(UserWarning, match=r"'arg1'.*cannot be found.*$"):
+        pm.hook.hello(arg2=2)
 
-        # calling should trigger a warning
-        pm.hook.myhook(arg1=1)
+    with pytest.warns(UserWarning, match=r"'arg1', 'arg2'.*cannot be found.*$"):
+        pm.hook.hello.call_extra([], kwargs=dict())
 
-        assert len(warns) == 1
-        warning = warns[-1]
-        assert issubclass(warning.category, Warning)
-        assert "Argument(s) ('arg2',)" in str(warning.message)
+    with pytest.warns(UserWarning, match=r"'arg1', 'arg2'.*cannot be found.*$"):
+        pm.hook.herstory.call_historic(kwargs=dict())
 
 
-def test_repr():
+def test_repr() -> None:
     class Plugin:
         @hookimpl
-        def myhook():
+        def myhook(self):
             raise NotImplementedError()
 
     pm = PluginManager(hookspec.project_name)
 
     plugin = Plugin()
     pname = pm.register(plugin)
-    assert repr(pm.hook.myhook._nonwrappers[0]) == (
-        "<HookImpl plugin_name=%r, plugin=%r>" % (pname, plugin)
+    assert repr(pm.hook.myhook.get_hookimpls()[0]) == (
+        f"<HookImpl plugin_name={pname!r}, plugin={plugin!r}>"
     )
```

