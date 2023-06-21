# Comparing `tmp/prance-0.9.0.tar.gz` & `tmp/prance-23.6.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/prance-0.9.0.tar", last modified: Sat Feb 24 13:57:29 2018, max compression
+gzip compressed data, was "/home/runner/work/prance/prance/dist/.tmp-3_5roag9/prance-23.6.21.0.tar", last modified: Wed Jun 21 20:01:44 2023, max compression
```

## Comparing `prance-0.9.0.tar` & `prance-23.6.21.0.tar`

### file list

```diff
@@ -1,63 +1,145 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/docs/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/docs/source/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/docs/source/_templates/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/docs/source/_templates/autosummary/
--rw-r--r--   0 travis    (2000) travis    (2000)      788 2018-02-24 13:53:42.000000 prance-0.9.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 travis    (2000) travis    (2000)        4 2018-02-24 13:53:42.000000 prance-0.9.0/docs/source/.gitignore
--rw-r--r--   0 travis    (2000) travis    (2000)    10270 2018-02-24 13:53:42.000000 prance-0.9.0/docs/source/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)      589 2018-02-24 13:53:42.000000 prance-0.9.0/docs/source/index.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     7636 2018-02-24 13:53:42.000000 prance-0.9.0/docs/Makefile
--rwxr-xr-x   0 travis    (2000) travis    (2000)      382 2018-02-24 13:53:42.000000 prance-0.9.0/docs/deploy.sh
--rw-r--r--   0 travis    (2000) travis    (2000)     7460 2018-02-24 13:53:42.000000 prance-0.9.0/docs/make.bat
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/prance/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/prance/util/
--rw-r--r--   0 travis    (2000) travis    (2000)      857 2018-02-24 13:53:42.000000 prance-0.9.0/prance/util/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5438 2018-02-24 13:53:42.000000 prance-0.9.0/prance/util/formats.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6054 2018-02-24 13:53:42.000000 prance-0.9.0/prance/util/fs.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2666 2018-02-24 13:53:42.000000 prance-0.9.0/prance/util/iterators.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5314 2018-02-24 13:53:42.000000 prance-0.9.0/prance/util/resolver.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4694 2018-02-24 13:53:42.000000 prance-0.9.0/prance/util/url.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5978 2018-02-24 13:53:42.000000 prance-0.9.0/prance/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3653 2018-02-24 13:53:42.000000 prance-0.9.0/prance/cli.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2253 2018-02-24 13:53:42.000000 prance-0.9.0/prance/mixins.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     8359 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)     1147 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       43 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/entry_points.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      282 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        7 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-02-24 13:57:29.000000 prance-0.9.0/prance.egg-info/zip-safe
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/tests/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-02-24 13:57:29.000000 prance-0.9.0/tests/schema/
--rw-r--r--   0 travis    (2000) travis    (2000)      117 2018-02-24 13:53:42.000000 prance-0.9.0/tests/schema/ChangePasswordEntity.json
--rw-r--r--   0 travis    (2000) travis    (2000)      203 2018-02-24 13:53:42.000000 prance-0.9.0/tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      207 2018-02-24 13:53:42.000000 prance-0.9.0/tests/definitions.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)       99 2018-02-24 13:53:42.000000 prance-0.9.0/tests/error.json
--rw-r--r--   0 travis    (2000) travis    (2000)      384 2018-02-24 13:53:42.000000 prance-0.9.0/tests/issue_1.json
--rw-r--r--   0 travis    (2000) travis    (2000)      253 2018-02-24 13:53:42.000000 prance-0.9.0/tests/issue_5.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     2069 2018-02-24 13:53:42.000000 prance-0.9.0/tests/missing_reference.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     2150 2018-02-24 13:53:42.000000 prance-0.9.0/tests/petstore.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     2075 2018-02-24 13:53:42.000000 prance-0.9.0/tests/recursive.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)      194 2018-02-24 13:53:42.000000 prance-0.9.0/tests/recursive_definitions.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     1937 2018-02-24 13:53:42.000000 prance-0.9.0/tests/symlink_test
--rw-r--r--   0 travis    (2000) travis    (2000)     2640 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_base_parser.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2695 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_cli.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3539 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_resolving_parser.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1483 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_util.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2572 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_util_formats.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4290 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_util_fs.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2192 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_util_iterators.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1730 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_util_resolver.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2138 2018-02-24 13:53:42.000000 prance-0.9.0/tests/test_util_url.py
--rw-r--r--   0 travis    (2000) travis    (2000)       29 2018-02-24 13:53:42.000000 prance-0.9.0/tests/utf8bom.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     1937 2018-02-24 13:53:42.000000 prance-0.9.0/tests/with_externals.yaml
--rw-r--r--   0 travis    (2000) travis    (2000)     1668 2018-02-24 13:53:42.000000 prance-0.9.0/LICENSE.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      251 2018-02-24 13:53:42.000000 prance-0.9.0/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     5961 2018-02-24 13:53:42.000000 prance-0.9.0/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       18 2018-02-24 13:53:42.000000 prance-0.9.0/requirements.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      564 2018-02-24 13:57:29.000000 prance-0.9.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     2479 2018-02-24 13:53:42.000000 prance-0.9.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      606 2018-02-24 13:53:42.000000 prance-0.9.0/tox.ini
--rw-r--r--   0 travis    (2000) travis    (2000)     8359 2018-02-24 13:57:29.000000 prance-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-21 20:01:32.000000 prance-23.6.21.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-21 20:01:32.000000 prance-23.6.21.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 20:01:32.000000 prance-23.6.21.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-21 20:01:32.000000 prance-23.6.21.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-21 20:01:32.000000 prance-23.6.21.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 20:01:32.000000 prance-23.6.21.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-21 20:01:32.000000 prance-23.6.21.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-21 20:01:32.000000 prance-23.6.21.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-21 20:01:32.000000 prance-23.6.21.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-21 20:01:32.000000 prance-23.6.21.0/COMPATIBILITY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-21 20:01:32.000000 prance-23.6.21.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 20:01:32.000000 prance-23.6.21.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-21 20:01:32.000000 prance-23.6.21.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-06-21 20:01:44.000000 prance-23.6.21.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-21 20:01:32.000000 prance-23.6.21.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-21 20:01:32.000000 prance-23.6.21.0/appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:32.000000 prance-23.6.21.0/changelog.d/.nodelete
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    31305 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/images/prance_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32993 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/images/prance_logo_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/images/prance_logo_512.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1148699 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/images/prance_redbubble.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2201853 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/images/prance_redbubble.xcf
+-rw-r--r--   0 runner    (1001) docker     (123)   109481 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/images/prance_social.png
+-rw-r--r--   0 runner    (1001) docker     (123)   166330 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/images/prance_social.xcf
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/source/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:43.000000 prance-23.6.21.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-21 20:01:32.000000 prance-23.6.21.0/docs/towncrier_template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/prance/
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/prance/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-21 20:01:32.000000 prance-23.6.21.0/prance/util/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/prance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:01:43.000000 prance-23.6.21.0/prance.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 20:01:32.000000 prance-23.6.21.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 20:01:32.000000 prance-23.6.21.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 20:01:32.000000 prance-23.6.21.0/requirements_bare.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 20:01:32.000000 prance-23.6.21.0/requirements_flex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 20:01:32.000000 prance-23.6.21.0/requirements_no_icu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 20:01:32.000000 prance-23.6.21.0/requirements_no_osv_or_icu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-21 20:01:44.000000 prance-23.6.21.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/mock_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/tests/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/definitions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/error.json
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_20.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_36.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_38_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_38_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_39.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/tests/specs/issue_51/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_51/openapi-main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_51/openapi-part-iso-8859-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_51/openapi-part.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/tests/specs/issue_78/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_78/_schemas.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_78/openapi.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/tests/specs/issue_83/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_83/bad_get.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/issue_83/bad_spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)  5502026 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/kubernetes_api_docs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/missing_reference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/petstore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/recursion_limit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/recursion_limit_defs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/recursion_limit_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/recursive_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/recursive_files_definitions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/recursive_objs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/recursive_objs_definitions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/tests/specs/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/schema/ChangePasswordEntity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/symlink_test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:01:44.000000 prance-23.6.21.0/tests/specs/translating_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/different_file_reference_from_file.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/different_file_reference_from_file_schemas1.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/different_file_reference_from_file_schemas2.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/file_reference_from_root.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/file_reference_from_root_schemas.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/local_reference_from_file.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/local_reference_from_file_schemas.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/local_reference_from_root.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/nested_recursive_reference_in_file.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/nested_recursive_reference_in_file_schemas.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/recursive_reference_in_file.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/recursive_reference_in_file_schemas.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/recursive_reference_in_root.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/root_file_reference_from_file.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/root_file_reference_from_file_schemas.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/root_file_reference_from_root.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/same_file_reference_from_file.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/translating_parser/same_file_reference_from_file_schemas.spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/utf8bom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/specs/with_externals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_resolving_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_translating_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_util_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-21 20:01:32.000000 prance-23.6.21.0/tests/test_zzz_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-21 20:01:32.000000 prance-23.6.21.0/tox.ini
```

### Comparing `prance-0.9.0/docs/source/_templates/autosummary/module.rst` & `prance-23.6.21.0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `prance-0.9.0/docs/source/conf.py` & `prance-23.6.21.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,88 +1,84 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 #
 # prance documentation build configuration file, created by
 # sphinx-quickstart on Tue Oct 25 10:28:07 2016.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
-
 # -- General configuration ------------------------------------------------
-
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
-
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.doctest',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.githubpages',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.doctest",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.githubpages",
 ]
 
 # Autosummary
 autosummary_generate = True
 
 # Autodoc
-autodoc_member_order = 'groupwise'
-autodoc_mock_imports = ['icu']
+autodoc_member_order = "groupwise"
+autodoc_mock_imports = ["icu"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 #
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'prance'
-copyright = '2016-2017, Jens Finkhaeuser'
-author = 'Jens Finkhaeuser'
+project = "prance"
+copyright = "2016-2017, Jens Finkhaeuser"
+author = "Jens Finkhaeuser"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '0.9.0'
+from prance import __version__ as release
 
 # The short X.Y version.
 import re
-version = '.'.join(re.findall(r'[\w]+', release)[0:2])
+
+version = ".".join(re.findall(r"[\w]+", release)[0:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
@@ -117,15 +113,15 @@
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 #
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
@@ -134,26 +130,26 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
-  'github_user': 'jfinkhaeuser',
-  'github_repo': 'prance',
-  'github_banner': True,
-  'show_related': True,
-  'fixed_sidebar': True,
+    "github_user": "RonnyPfannschmidt",
+    "github_repo": "prance",
+    "github_banner": True,
+    "show_related": True,
+    "fixed_sidebar": True,
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.
 # "<project> v<release> documentation" by default.
@@ -174,15 +170,15 @@
 # pixels large.
 #
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 #
 # html_extra_path = []
 
@@ -254,42 +250,38 @@
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
 #
 # html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'prancedoc'
+htmlhelp_basename = "prancedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-     # The paper size ('letterpaper' or 'a4paper').
-     #
-     # 'papersize': 'letterpaper',
-
-     # The font size ('10pt', '11pt' or '12pt').
-     #
-     # 'pointsize': '10pt',
-
-     # Additional stuff for the LaTeX preamble.
-     #
-     # 'preamble': '',
-
-     # Latex figure (float) alignment
-     #
-     # 'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'prance.tex', 'prance Documentation',
-     'Jens Finkhaeuser', 'manual'),
+    (master_doc, "prance.tex", "prance Documentation", "Jens Finkhaeuser", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #
 # latex_logo = None
 
@@ -321,33 +313,36 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'prance', 'prance Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "prance", "prance Documentation", [author], 1)]
 
 # If true, show URL addresses after external links.
 #
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'prance', 'prance Documentation',
-     author, 'prance', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "prance",
+        "prance Documentation",
+        author,
+        "prance",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
 #
 # texinfo_appendices = []
 
 # If false, no module index is generated.
```

### Comparing `prance-0.9.0/docs/Makefile` & `prance-23.6.21.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `prance-0.9.0/docs/make.bat` & `prance-23.6.21.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `prance-0.9.0/prance/util/iterators.py` & `prance-23.6.21.0/prance/util/iterators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,83 @@
-# -*- coding: utf-8 -*-
 """This submodule contains specialty iterators over specs."""
 
-__author__ = 'Jens Finkhaeuser'
-__copyright__ = 'Copyright (c) 2016-2017 Jens Finkhaeuser'
-__license__ = 'MIT +no-false-attribs'
+__author__ = "Jens Finkhaeuser"
+__copyright__ = "Copyright (c) 2016-2018 Jens Finkhaeuser"
+__license__ = "MIT"
 __all__ = ()
 
 
-def item_iterator(value, path = ()):
-  """
-  Return item iterator over the a nested dict- or list-like object.
-
-  Returns each item value as the second item to unpack, and a tuple path to the
-  item as the first value - in that, it behaves much like viewitems(). For list
-  like values, the path is made up of numeric indices.
-
-  Given a spec such as this::
-
-    spec = {
-      'foo': 42,
-      'bar': {
-        'some': 'dict',
-      },
-      'baz': [
-        { 1: 2 },
-        { 3: 4 },
-      ]
-    }
-
-  Here, (parts of) the yielded values would be:
-
-    ======== =============
-    item     path
-    ======== =============
-    [...]    ('baz',)
-    { 1: 2 } ('baz', 0)
-    2        ('baz', 0, 1)
-    ======== =============
-
-  :param dict/list value: The specifications to iterate over.
-  :return: An iterator over all items in the value.
-  :rtype: iterator
-  """
-  # Yield the top-level object, always
-  yield path, value
-
-  # For dict and list like objects, we also need to yield each item
-  # recursively.
-  import collections
-  import six
-  if isinstance(value, collections.Mapping):
-    for key, item in six.viewitems(value):
-      for inner_path, inner in item_iterator(item, path + (key,)):
-        yield inner_path, inner
-  elif isinstance(value, collections.Sequence) and not isinstance(value,
-         six.string_types):
-    for idx, item in enumerate(value):
-      for inner_path, inner in item_iterator(item, path + (idx,)):
-        yield inner_path, inner
-
-
-def reference_iterator(specs, path = ()):
-  """
-  Iterate through the given specs, returning only references.
-
-  The iterator returns three values:
-    - The key, mimicking the behaviour of other iterators, although
-      it will always equal '$ref'
-    - The value
-    - The path to the item. This is a tuple of all the item's ancestors,
-      in sequence, so that you can reasonably easily find the containing
-      item. It does not include the final '$ref' key.
-
-  :param dict specs: The specifications to iterate over.
-  :return: An iterator over all references in the specs.
-  :rtype: iterator
-  """
-  # We need to iterate through the nested specification dict, so let's
-  # start with an appropriate iterator. We can immediately optimize it by
-  # only returning '$ref' items.
-  for item_path, item in item_iterator(specs, path):
-    if len(item_path) <= 0:
-      continue
-    key = item_path[-1]
-    if key == '$ref':
-      yield key, item, item_path[:-1]
+def item_iterator(value, path=()):
+    """
+    Return item iterator over the a nested dict- or list-like object.
+
+    Returns each item value as the second item to unpack, and a tuple path to the
+    item as the first value - in that, it behaves much like viewitems(). For list
+    like values, the path is made up of numeric indices.
+
+    Given a spec such as this::
+
+      spec = {
+        'foo': 42,
+        'bar': {
+          'some': 'dict',
+        },
+        'baz': [
+          { 1: 2 },
+          { 3: 4 },
+        ]
+      }
+
+    Here, (parts of) the yielded values would be:
+
+      ======== =============
+      item     path
+      ======== =============
+      [...]    ('baz',)
+      { 1: 2 } ('baz', 0)
+      2        ('baz', 0, 1)
+      ======== =============
+
+    :param dict/list value: The specifications to iterate over.
+    :return: An iterator over all items in the value.
+    :rtype: iterator
+    """
+    # Yield the top-level object, always
+    yield path, value
+
+    from collections.abc import Mapping, Sequence
+
+    # For dict and list like objects, we also need to yield each item
+    # recursively.
+    if isinstance(value, Mapping):
+        for key, item in value.items():
+            yield from item_iterator(item, path + (key,))
+    elif isinstance(value, Sequence) and not isinstance(value, str):
+        for idx, item in enumerate(value):
+            yield from item_iterator(item, path + (idx,))
+
+
+def reference_iterator(specs, path=()):
+    """
+    Iterate through the given specs, returning only references.
+
+    The iterator returns three values:
+      - The key, mimicking the behaviour of other iterators, although
+        it will always equal '$ref'
+      - The value
+      - The path to the item. This is a tuple of all the item's ancestors,
+        in sequence, so that you can reasonably easily find the containing
+        item. It does not include the final '$ref' key.
+
+    :param dict specs: The specifications to iterate over.
+    :return: An iterator over all references in the specs.
+    :rtype: iterator
+    """
+    # We need to iterate through the nested specification dict, so let's
+    # start with an appropriate iterator. We can immediately optimize it by
+    # only returning '$ref' items.
+    for item_path, item in item_iterator(specs, path):
+        if len(item_path) <= 0:
+            continue
+        key = item_path[-1]
+        if key == "$ref":
+            yield key, item, item_path[:-1]
```

### Comparing `prance-0.9.0/prance/mixins.py` & `prance-23.6.21.0/prance/mixins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,90 @@
-# -*- coding: utf-8 -*-
 """
 Defines Mixins for parsers.
 
 The Mixins are here mostly for separation of concerns.
 """
 
-__author__ = 'Jens Finkhaeuser'
-__copyright__ = 'Copyright (c) 2016-2017 Jens Finkhaeuser'
-__license__ = 'MIT +no-false-attribs'
+__author__ = "Jens Finkhaeuser"
+__copyright__ = "Copyright (c) 2016-2018 Jens Finkhaeuser"
+__license__ = "MIT"
 __all__ = ()
 
 
-class CacheSpecsMixin(object):
-  """
-  CacheSpecsMixin helps determine if self.specification changed.
-
-  It does so by caching a shallow copy on-demand.
-  """
-
-  __CACHED_SPECS = '__cached_specs'
-
-  def specs_updated(self):
+class CacheSpecsMixin:
     """
-    Test if self.specficiation changed.
+    CacheSpecsMixin helps determine if self.specification changed.
 
-    :return: Whether the specs changed.
-    :rtype: bool
+    It does so by caching a shallow copy on-demand.
     """
-    # Cache specs and return true if no specs have been cached
-    if not getattr(self, self.__CACHED_SPECS, None):
-      setattr(self, self.__CACHED_SPECS, self.specification.copy())
-      return True
 
-    # If specs have been cached, compare them to the current
-    # specs.
-    cached = getattr(self, self.__CACHED_SPECS)
-    if cached != self.specification:
-      setattr(self, self.__CACHED_SPECS, self.specification.copy())
-      return True
+    __CACHED_SPECS = "__cached_specs"
 
-    # Return false if they're the same
-    return False
+    def specs_updated(self):
+        """
+        Test if self.specficiation changed.
 
+        :return: Whether the specs changed.
+        :rtype: bool
+        """
+        # Cache specs and return true if no specs have been cached
+        if not getattr(self, self.__CACHED_SPECS, None):
+            setattr(self, self.__CACHED_SPECS, self.specification.copy())
+            return True
 
-class YAMLMixin(CacheSpecsMixin):
-  """
-  YAMLMixin returns a YAML representation of the specification.
+        # If specs have been cached, compare them to the current
+        # specs.
+        cached = getattr(self, self.__CACHED_SPECS)
+        if cached != self.specification:
+            setattr(self, self.__CACHED_SPECS, self.specification.copy())
+            return True
 
-  It uses :py:class:`CacheSpecsMixin` for lazy evaluation.
-  """
+        # Return false if they're the same
+        return False
 
-  __YAML = '__yaml'
 
-  def yaml(self):
+class YAMLMixin(CacheSpecsMixin):
     """
-    Return a YAML representation of the specifications.
+    YAMLMixin returns a YAML representation of the specification.
 
-    :return: YAML representation.
-    :rtype: dict
+    It uses :py:class:`CacheSpecsMixin` for lazy evaluation.
     """
-    # Query specs_updated first to start caching
-    if self.specs_updated() or not getattr(self, self.__YAML, None):
-      import yaml
-      setattr(self, self.__YAML, yaml.dump(self.specification))
-    return getattr(self, self.__YAML)
 
+    __YAML = "__yaml"
 
-class JSONMixin(CacheSpecsMixin):
-  """
-  JSONMixin returns a JSON representation of the specification.
+    def yaml(self):
+        """
+        Return a YAML representation of the specifications.
 
-  It uses :py:class:`CacheSpecsMixin` for lazy evaluation.
-  """
+        :return: YAML representation.
+        :rtype: dict
+        """
+        # Query specs_updated first to start caching
+        if self.specs_updated() or not getattr(self, self.__YAML, None):
+            import yaml
 
-  __JSON = '__json'
+            setattr(self, self.__YAML, yaml.dump(self.specification))
+        return getattr(self, self.__YAML)
 
-  def json(self):
+
+class JSONMixin(CacheSpecsMixin):
     """
-    Return a JSON representation of the specifications.
+    JSONMixin returns a JSON representation of the specification.
 
-    :return: JSON representation.
-    :rtype: dict
+    It uses :py:class:`CacheSpecsMixin` for lazy evaluation.
     """
-    # Query specs_updated first to start caching
-    if self.specs_updated() or not getattr(self, self.__JSON, None):
-      import json
-      setattr(self, self.__JSON, json.dumps(self.specification))
-    return getattr(self, self.__JSON)
+
+    __JSON = "__json"
+
+    def json(self):
+        """
+        Return a JSON representation of the specifications.
+
+        :return: JSON representation.
+        :rtype: dict
+        """
+        # Query specs_updated first to start caching
+        if self.specs_updated() or not getattr(self, self.__JSON, None):
+            import json
+
+            setattr(self, self.__JSON, json.dumps(self.specification))
+        return getattr(self, self.__JSON)
```

### Comparing `prance-0.9.0/tests/missing_reference.yaml` & `prance-23.6.21.0/tests/specs/missing_reference.yaml`

 * *Files identical despite different names*

### Comparing `prance-0.9.0/tests/petstore.yaml` & `prance-23.6.21.0/tests/specs/petstore.yaml`

 * *Files identical despite different names*

### Comparing `prance-0.9.0/tests/recursive.yaml` & `prance-23.6.21.0/tests/specs/recursive_objs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             $ref: '#/definitions/Recursive'
 definitions:
   Recursive:
     required:
       - foo
     properties:
       foo:
-        $ref: 'recursive_definitions.yaml#/bar'
+        $ref: 'recursive_objs_definitions.yaml#/bar'
   Pet:
     required:
       - id
       - name
     properties:
       id:
         type: integer
```

### Comparing `prance-0.9.0/tests/symlink_test` & `prance-23.6.21.0/tests/specs/symlink_test`

 * *Files 18% similar despite different names*

```diff
@@ -54,24 +54,25 @@
   /pets/{petId}:
     get:
       summary: Info for a specific pet
       operationId: showPetById
       tags:
         - pets
       parameters:
-        - name: petId
-          in: path
-          required: true
-          description: The id of the pet to retrieve
-          type: string
+        - overwritten: some value
+          $ref: 'definitions.yaml#/id'
       responses:
         "200":
           description: Expected response to a valid request
           schema:
             $ref: 'http://finkhaeuser.de/projects/prance/petstore.yaml#/definitions/Pet'
+        "203":
+          description: Expected response to a valid request
+          schema:
+            $ref: 'python://tests/specs/petstore.yaml#/definitions/Pet'
         default:
           description: unexpected error
           schema:
             $ref: '#/definitions/Error'
 definitions:
   Error:
     required:
```

### Comparing `prance-0.9.0/tests/test_util_iterators.py` & `prance-23.6.21.0/tests/test_util_iterators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# -*- coding: utf-8 -*-
 """Test suite for prance.util.iterators ."""
 
-__author__ = 'Jens Finkhaeuser'
-__copyright__ = 'Copyright (c) 2016-2017 Jens Finkhaeuser'
-__license__ = 'MIT +no-false-attribs'
+__author__ = "Jens Finkhaeuser"
+__copyright__ = "Copyright (c) 2016-2021 Jens Finkhaeuser"
+__license__ = "MIT"
 __all__ = ()
 
 
 from prance.util import iterators
 
+
 def test_item_iterator():
-  tester = {
-    'foo': 42,
-    'bar': {
-      'some': 'dict',
-    },
-    'baz': [
-      { 1: 2 },
-      { 3: 4 },
-    ]
-  }
-
-  frozen = tuple(iterators.item_iterator(tester))
-  assert len(frozen) == 9, "Iterator did not yield the correct number of items!"
-
-  # Test for a few paths
-  assert ((), tester) in frozen
-  assert (('bar', 'some'), 'dict') in frozen
-  assert (('baz', 0, 1), 2) in frozen
-  assert (('baz', 1), { 3: 4 }) in frozen
+    tester = {
+        "foo": 42,
+        "bar": {
+            "some": "dict",
+        },
+        "baz": [
+            {1: 2},
+            {3: 4},
+        ],
+    }
+
+    frozen = tuple(iterators.item_iterator(tester))
+    assert len(frozen) == 9, "Iterator did not yield the correct number of items!"
+
+    # Test for a few paths
+    assert ((), tester) in frozen
+    assert (("bar", "some"), "dict") in frozen
+    assert (("baz", 0, 1), 2) in frozen
+    assert (("baz", 1), {3: 4}) in frozen
 
 
 def test_item_iterator_empty():
-  frozen = tuple(iterators.item_iterator({}))
-  assert len(frozen) == 1, "Must return at least the item itself!"
-  assert ((), {}) in frozen
-
-  frozen = tuple(iterators.item_iterator([]))
-  assert len(frozen) == 1, "Must return at least the item itself!"
-  assert ((), []) in frozen
+    frozen = tuple(iterators.item_iterator({}))
+    assert len(frozen) == 1, "Must return at least the item itself!"
+    assert ((), {}) in frozen
+
+    frozen = tuple(iterators.item_iterator([]))
+    assert len(frozen) == 1, "Must return at least the item itself!"
+    assert ((), []) in frozen
 
 
 def test_reference_iterator_empty_dict():
-  tester = {}
-  frozen = tuple(iterators.reference_iterator(tester))
-  assert len(frozen) == 0, 'Found items when it should not have!'
+    tester = {}
+    frozen = tuple(iterators.reference_iterator(tester))
+    assert len(frozen) == 0, "Found items when it should not have!"
 
 
 def test_reference_iterator_dict_without_references():
-  tester = {
-    'foo': 42,
-    'bar': 'baz',
-    'baz': {
-      'quux': {
-        'fnord': False,
-      },
-    },
-  }
-  frozen = tuple(iterators.reference_iterator(tester))
-  assert len(frozen) == 0, 'Found items when it should not have!'
+    tester = {
+        "foo": 42,
+        "bar": "baz",
+        "baz": {
+            "quux": {
+                "fnord": False,
+            },
+        },
+    }
+    frozen = tuple(iterators.reference_iterator(tester))
+    assert len(frozen) == 0, "Found items when it should not have!"
 
 
 def test_reference_iterator_dict_with_references():
-  tester = {
-    'foo': 42,
-    'bar': 'baz',
-    '$ref': 'root',
-    'baz': {
-      '$ref': 'branch',
-      'quux': {
-        'fnord': False,
-        '$ref': 'leaf',
-      },
-    },
-  }
-  frozen = tuple(iterators.reference_iterator(tester))
-  assert len(frozen) == 3, 'Found a different item count than expected!'
-
-  # We have three references with their paths here, but we don't know which
-  # order the tuple has them in. Let's go through them all:
-  expectations = {
-    0: 'root',
-    1: 'branch',
-    2: 'leaf',
-  }
-  for key, value, path in iterators.reference_iterator(tester):
-    assert value == expectations[len(path)]
+    tester = {
+        "foo": 42,
+        "bar": "baz",
+        "$ref": "root",
+        "baz": {
+            "$ref": "branch",
+            "quux": {
+                "fnord": False,
+                "$ref": "leaf",
+            },
+        },
+    }
+    frozen = tuple(iterators.reference_iterator(tester))
+    assert len(frozen) == 3, "Found a different item count than expected!"
+
+    # We have three references with their paths here, but we don't know which
+    # order the tuple has them in. Let's go through them all:
+    expectations = {
+        0: "root",
+        1: "branch",
+        2: "leaf",
+    }
+    for key, value, path in iterators.reference_iterator(tester):
+        assert value == expectations[len(path)]
```

### Comparing `prance-0.9.0/tests/with_externals.yaml` & `prance-23.6.21.0/tests/specs/with_externals.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -54,24 +54,25 @@
   /pets/{petId}:
     get:
       summary: Info for a specific pet
       operationId: showPetById
       tags:
         - pets
       parameters:
-        - name: petId
-          in: path
-          required: true
-          description: The id of the pet to retrieve
-          type: string
+        - overwritten: some value
+          $ref: 'definitions.yaml#/id'
       responses:
         "200":
           description: Expected response to a valid request
           schema:
             $ref: 'http://finkhaeuser.de/projects/prance/petstore.yaml#/definitions/Pet'
+        "203":
+          description: Expected response to a valid request
+          schema:
+            $ref: 'python://tests/specs/petstore.yaml#/definitions/Pet'
         default:
           description: unexpected error
           schema:
             $ref: '#/definitions/Error'
 definitions:
   Error:
     required:
```

### Comparing `prance-0.9.0/LICENSE.txt` & `prance-23.6.21.0/LICENSE.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,9 @@
 Copyright (C) Jens Finkhaeuser and other Prance contributors. All rights
 not covered below are reserved.
 
-MIT +no-false-attribs License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-Distributions of all or part of the Software intended to be used by the
-recipients as they would use the unmodified Software, containing modifications
-that substantially alter, remove, or disable functionality of the Software,
-outside of the documented configuration mechanisms provided by the Software,
-shall be modified such that the Original Author's bug reporting email addresses
-and urls are either replaced with the contact information of the parties
-responsible for the changes, or removed entirely.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

