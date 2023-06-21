# Comparing `tmp/db2ixf-0.2.0.tar.gz` & `tmp/db2ixf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2ixf-0.2.0.tar", last modified: Sat Jun 17 01:43:40 2023, max compression
+gzip compressed data, was "db2ixf-0.2.1.tar", last modified: Wed Jun 21 16:16:35 2023, max compression
```

## Comparing `db2ixf-0.2.0.tar` & `db2ixf-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.338937 db2ixf-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-17 01:42:28.000000 db2ixf-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-06-17 01:42:28.000000 db2ixf-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-17 01:43:40.338937 db2ixf-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-17 01:42:28.000000 db2ixf-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-17 01:42:28.000000 db2ixf-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:43:40.338937 db2ixf-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 01:42:28.000000 db2ixf-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.334937 db2ixf-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.334937 db2ixf-0.2.0/src/db2ixf/
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/ibmcodecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/ixf.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-17 01:42:28.000000 db2ixf-0.2.0/src/db2ixf/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:43:40.334937 db2ixf-0.2.0/src/db2ixf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:43:39.000000 db2ixf-0.2.0/src/db2ixf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 01:43:40.000000 db2ixf-0.2.0/src/db2ixf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:35.774188 db2ixf-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-21 16:15:22.000000 db2ixf-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-06-21 16:15:22.000000 db2ixf-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-21 16:16:35.774188 db2ixf-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-21 16:15:22.000000 db2ixf-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-21 16:15:22.000000 db2ixf-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:16:35.774188 db2ixf-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 16:15:22.000000 db2ixf-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:35.770188 db2ixf-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:35.770188 db2ixf-0.2.1/src/db2ixf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/ibmcodecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/ixf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-21 16:15:22.000000 db2ixf-0.2.1/src/db2ixf/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:16:35.774188 db2ixf-0.2.1/src/db2ixf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 16:16:35.000000 db2ixf-0.2.1/src/db2ixf.egg-info/top_level.txt
```

### Comparing `db2ixf-0.2.0/CHANGELOG.md` & `db2ixf-0.2.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,62 +2,80 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres
 to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the
-changes for the upcoming release may be found
-in [here](https://github.com/ismailhammounou/db2ixf/tree/main/resources/changelog)
-.
+This project uses [*towncrier*](https://towncrier.readthedocs.io/).
 
 <!-- release notes start -->
-## [0.2.0](https://github.com/ismailhammounou/db2ixf/tree/0.2.0) - 2023-06-17
+## [0.2.1](https://github.com/ismailhammounou/db2ixf/tree/0.2.1) - 2023-06-21
 
 
 ### Added
 
-- Add unit tests [db2ixf-3](https://github.com/ismailhammounou/db2ixf/issues/3)
-- Add ibm encoding to use on the fly by reading ixf file [db2ixf-23](https://github.com/ismailhammounou/db2ixf/issues/23)
+- Add ixf sample data (db2) [db2ixf-25](https://github.com/ismailhammounou/db2ixf/issues/25)
+- Add more unit tests to improve coverage [db2ixf-26](https://github.com/ismailhammounou/db2ixf/issues/26)
+- Add tests in CI pipeline [db2ixf-27](https://github.com/ismailhammounou/db2ixf/issues/27)
 
 
 ### Changed
 
-- improve CLI and adapt it [db2ixf-24](https://github.com/ismailhammounou/db2ixf/issues/24)
-
+- Improve ibm codecs mapping [db2ixf-28](https://github.com/ismailhammounou/db2ixf/issues/28)
 
-### Removed
 
-- Delete encoding because IXF file contains the encoding [db2ixf-20](https://github.com/ismailhammounou/db2ixf/issues/20)
-- Drop support for python 3.7 [db2ixf-22](https://github.com/ismailhammounou/db2ixf/issues/22)
+### Fixed
 
+- fix issues with some data type collector [db2ixf-29](https://github.com/ismailhammounou/db2ixf/issues/29)
 
-## [0.1.7](https://github.com/ismailhammounou/db2ixf/tree/0.1.7) - 2023-06-06
 
+## [0.2.0](https://github.com/ismailhammounou/db2ixf/tree/0.2.0) - 2023-06-17
 
 ### Added
 
-- Add support for CLOB data type [db2ixf-16](https://github.com/ismailhammounou/db2ixf/issues/16)
-- Add support for BLOB data type [db2ixf-17](https://github.com/ismailhammounou/db2ixf/issues/17)
-- Add support for binary data type [db2ixf-19](https://github.com/ismailhammounou/db2ixf/issues/19)
-
+- Add unit tests [db2ixf-3](https://github.com/ismailhammounou/db2ixf/issues/3)
+- Add ibm encoding to use on the fly by reading ixf
+  file [db2ixf-23](https://github.com/ismailhammounou/db2ixf/issues/23)
 
 ### Changed
 
-- Improve documentation [db2ixf-18](https://github.com/ismailhammounou/db2ixf/issues/18)
+- improve CLI and adapt
+  it [db2ixf-24](https://github.com/ismailhammounou/db2ixf/issues/24)
 
+### Removed
 
-## [0.1.6](https://github.com/ismailhammounou/db2ixf/tree/0.1.6) - 2023-06-05
+- Delete encoding because IXF file contains the
+  encoding [db2ixf-20](https://github.com/ismailhammounou/db2ixf/issues/20)
+- Drop support for python
+  3.7 [db2ixf-22](https://github.com/ismailhammounou/db2ixf/issues/22)
 
+## [0.1.7](https://github.com/ismailhammounou/db2ixf/tree/0.1.7) - 2023-06-06
 
-### Fixed
+### Added
+
+- Add support for CLOB data
+  type [db2ixf-16](https://github.com/ismailhammounou/db2ixf/issues/16)
+- Add support for BLOB data
+  type [db2ixf-17](https://github.com/ismailhammounou/db2ixf/issues/17)
+- Add support for binary data
+  type [db2ixf-19](https://github.com/ismailhammounou/db2ixf/issues/19)
+
+### Changed
+
+- Improve
+  documentation [db2ixf-18](https://github.com/ismailhammounou/db2ixf/issues/18)
 
-- Fix bug with parquet_version param default value and pass it to pyarrow parquet writer [db2ixf-15](https://github.com/ismailhammounou/db2ixf/issues/15)
+## [0.1.6](https://github.com/ismailhammounou/db2ixf/tree/0.1.6) - 2023-06-05
+
+### Fixed
 
+- Fix bug with parquet_version param default value and pass it to pyarrow
+  parquet
+  writer [db2ixf-15](https://github.com/ismailhammounou/db2ixf/issues/15)
 
 ## [0.1.5](https://github.com/ismailhammounou/db2ixf/tree/0.1.5) - 2023-06-05
 
 ### Added
 
 - Support of floating point data
   type [db2ixf-14](https://github.com/ismailhammounou/db2ixf/issues/14)
```

### Comparing `db2ixf-0.2.0/LICENSE` & `db2ixf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `db2ixf-0.2.0/PKG-INFO` & `db2ixf-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://pypi.org/project/db2ixf/
 Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
@@ -23,15 +23,15 @@
 
 
 [![Language](https://img.shields.io/pypi/pyversions/db2ixf?color=ffde57&logo=python&style=for-the-badge)](https://www.python.org/)
 [![License](https://img.shields.io/pypi/l/db2ixf?color=3775A9&style=for-the-badge&logo=unlicense)](https://www.gnu.org/licenses/agpl-3.0)
 
 [![Pipeline](https://img.shields.io/github/actions/workflow/status/ismailhammounou/db2ixf/db2ixf.yml?branch=main&style=for-the-badge&logo=gitHub-actions)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
 [![Release](https://img.shields.io/github/v/release/ismailhammounou/db2ixf?display_name=tag&sort=semver&style=for-the-badge&logo=semver)](https://github.com/ismailhammounou/db2ixf/releases/latest)
-[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://pypi.org/project/db2ixf/)
 
 
 [![Downloads](https://img.shields.io/pypi/dm/db2ixf?style=for-the-badge)](https://pypi.org/project/db2ixf/)
 
 
 # DB2IXF Parser
 
@@ -191,17 +191,17 @@
 
 Thank you for considering contributing to IXF Parser. Let's work together to
 create a powerful and dependable tool for working with DB2's IXF files.
 
 ### Todo
 
 - [ ] Search for contributors/maintainers/sponsors.
-- [ ] Add tests (Manual testing was done but need write unit tests).
+- [x] Add tests (Manual testing was done but need write unit tests).
 - [x] Adding new collector for the floating point data type.
-- [ ] Adding new collectors for other ixf data types: binary ...etc.
+- [x] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [x] Add better ci-cd.
 - [x] Improve Makefile.
 - [x] ~~Support multiprocessing.~~
 - [x] ~~Support archived inputs: only python not CLI ?~~
```

### Comparing `db2ixf-0.2.0/README.md` & `db2ixf-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 [![Language](https://img.shields.io/pypi/pyversions/db2ixf?color=ffde57&logo=python&style=for-the-badge)](https://www.python.org/)
 [![License](https://img.shields.io/pypi/l/db2ixf?color=3775A9&style=for-the-badge&logo=unlicense)](https://www.gnu.org/licenses/agpl-3.0)
 
 [![Pipeline](https://img.shields.io/github/actions/workflow/status/ismailhammounou/db2ixf/db2ixf.yml?branch=main&style=for-the-badge&logo=gitHub-actions)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
 [![Release](https://img.shields.io/github/v/release/ismailhammounou/db2ixf?display_name=tag&sort=semver&style=for-the-badge&logo=semver)](https://github.com/ismailhammounou/db2ixf/releases/latest)
-[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://pypi.org/project/db2ixf/)
 
 
 [![Downloads](https://img.shields.io/pypi/dm/db2ixf?style=for-the-badge)](https://pypi.org/project/db2ixf/)
 
 
 # DB2IXF Parser
 
@@ -168,17 +168,17 @@
 
 Thank you for considering contributing to IXF Parser. Let's work together to
 create a powerful and dependable tool for working with DB2's IXF files.
 
 ### Todo
 
 - [ ] Search for contributors/maintainers/sponsors.
-- [ ] Add tests (Manual testing was done but need write unit tests).
+- [x] Add tests (Manual testing was done but need write unit tests).
 - [x] Adding new collector for the floating point data type.
-- [ ] Adding new collectors for other ixf data types: binary ...etc.
+- [x] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [x] Add better ci-cd.
 - [x] Improve Makefile.
 - [x] ~~Support multiprocessing.~~
 - [x] ~~Support archived inputs: only python not CLI ?~~
```

### Comparing `db2ixf-0.2.0/pyproject.toml` & `db2ixf-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `db2ixf-0.2.0/src/db2ixf/__init__.py` & `db2ixf-0.2.1/src/db2ixf/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,25 +25,75 @@
 Each column has its data type.
 
 For more information about data types; Please visit this
 [link](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
 """
 import codecs
 import ebcdic
-from db2ixf.ibmcodecs import (ibm_utf_32_be, ibm_utf_32_le, ibm_utf_32,
-                              ibm_utf_16_be, ibm_utf_16_le, ibm_utf_16,
-                              ibm_utf_8, ibm_latin1, ibm_latin9, ibm_37,
-                              ibm_813, ibm_859, ibm_1383, ibm_867, ibm_874,
-                              ibm_912, ibm_915, ibm_916, ibm_920, ibm_921,
-                              ibm_922, ibm_923, ibm_924, ibm_942, ibm_943,
-                              ibm_948, ibm_949, ibm_954, ibm_964, ibm_970,
-                              ibm_1089, ibm_1363, ibm_1375, ibm_1386, ibm_1392,
-                              ibm_5050, ibm_5054, ibm_5346, ibm_5347, ibm_5348,
-                              ibm_5349, ibm_5350, ibm_5351, ibm_5352, ibm_5353,
-                              ibm_5354, ibm_5488, ibm_9030, ibm_25546,
+from db2ixf.ibmcodecs import (ibm_utf_32_be,
+                              ibm_utf_32_le,
+                              ibm_utf_32,
+                              ibm_utf_16_be,
+                              ibm_utf_16_le,
+                              ibm_utf_16,
+                              ibm_utf_8,
+                              ibm_latin1,
+                              ibm_latin9,
+                              ibm_37,
+                              ibm_39,
+                              ibm_813,
+                              ibm_859,
+                              ibm_867,
+                              ibm_874,
+                              ibm_912,
+                              ibm_915,
+                              ibm_916,
+                              ibm_920,
+                              ibm_921,
+                              ibm_922,
+                              ibm_923,
+                              ibm_924,
+                              ibm_943,
+                              ibm_947,
+                              ibm_951,
+                              ibm_954,
+                              ibm_964,
+                              ibm_970,
+                              ibm_1088,
+                              ibm_1089,
+                              ibm_1098,
+                              ibm_1114,
+                              ibm_1115,
+                              ibm_1124,
+                              ibm_1351,
+                              ibm_1362,
+                              ibm_1363,
+                              ibm_1375,
+                              ibm_1380,
+                              ibm_1381,
+                              ibm_1383,
+                              ibm_1385,
+                              ibm_1386,
+                              ibm_1390,
+                              ibm_1392,
+                              ibm_5050,
+                              ibm_5054,
+                              ibm_5346,
+                              ibm_5347,
+                              ibm_5348,
+                              ibm_5349,
+                              ibm_5350,
+                              ibm_5351,
+                              ibm_5352,
+                              ibm_5353,
+                              ibm_5354,
+                              ibm_5488,
+                              ibm_9030,
+                              ibm_9066,
+                              ibm_25546,
                               ibm_33722)
 from db2ixf.ixf import IXFParser
 
 search_functions = (
     ebcdic._find_ebcdic_codec,
     ibm_utf_32_be,
     ibm_utf_32_le,
@@ -51,52 +101,64 @@
     ibm_utf_16_be,
     ibm_utf_16_le,
     ibm_utf_16,
     ibm_utf_8,
     ibm_latin1,
     ibm_latin9,
     ibm_37,
+    ibm_39,
     ibm_813,
     ibm_859,
     ibm_867,
     ibm_874,
     ibm_912,
     ibm_915,
     ibm_916,
     ibm_920,
     ibm_921,
     ibm_922,
     ibm_923,
     ibm_924,
-    ibm_942,
     ibm_943,
-    ibm_948,
-    ibm_949,
+    ibm_947,
+    ibm_951,
     ibm_954,
     ibm_964,
     ibm_970,
+    ibm_1088,
     ibm_1089,
+    ibm_1098,
+    ibm_1114,
+    ibm_1115,
+    ibm_1124,
+    ibm_1351,
+    ibm_1362,
     ibm_1363,
     ibm_1375,
+    ibm_1380,
+    ibm_1381,
     ibm_1383,
+    ibm_1385,
     ibm_1386,
+    ibm_1390,
     ibm_1392,
     ibm_5050,
     ibm_5054,
     ibm_5346,
     ibm_5347,
     ibm_5348,
     ibm_5349,
     ibm_5350,
     ibm_5351,
     ibm_5352,
     ibm_5353,
     ibm_5354,
     ibm_5488,
     ibm_9030,
+    ibm_9066,
     ibm_25546,
     ibm_33722,
 )
 
 for sf in search_functions:
     codecs.register(sf)
```

### Comparing `db2ixf-0.2.0/src/db2ixf/cli.py` & `db2ixf-0.2.1/src/db2ixf/cli.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.2.0/src/db2ixf/collectors.py` & `db2ixf-0.2.1/src/db2ixf/collectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,41 +3,42 @@
 from datetime import datetime, date, time
 from db2ixf.exceptions import (LargeObjectLengthException,
                                BinaryLengthException,
                                CLOBCodePageException,
                                CharLengthException,
                                VarCharLengthException)
 from db2ixf.helpers import get_ccsid_from_column
+from db2ixf.logger import logger
 from struct import unpack
 from typing import Union
 
 
-def collect_binary(c, fields, pos) -> bytes:
-    """Collects BINARY data type from ixf as a bytes.
+def collect_binary(c, fields, pos) -> str:
+    """Collects BINARY data type from ixf as a string.
 
     Parameters
     ----------
     c : dict
         Column descriptor extracted from IXF file.
     fields : str
         Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
 
     Returns
     -------
-    bytes:
+    str:
         a binary string data.
     """
     length = int(c['IXFCLENG'])
     if length > 254:
         msg = 'Length of a binary data types should not exceed 254 bytes.'
         raise BinaryLengthException(msg)
 
-    field = fields[pos:pos + length]
+    field = str(fields[pos:pos + length], 'utf-8')
 
     return field
 
 
 def collect_smallint(c, fields, pos) -> int:
     """Collects SMALLINT data type from ixf as an integer.
 
@@ -51,15 +52,15 @@
         Position of the column in the `fields`.
 
     Returns
     -------
     int:
         Integer.
     """
-    field = int(unpack('<i', fields[pos:pos + 2])[0])
+    field = int(unpack('<h', fields[pos:pos + 2])[0])
     return field
 
 
 def collect_integer(c, fields, pos) -> int:
     """Collects INTEGER data type from ixf as an integer.
 
     Parameters
@@ -170,29 +171,29 @@
     fields : str
         Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
 
     Returns
     -------
-    str:
+    str
         String.
     """
     length = int(c['IXFCLENG'])
     if length > 254:
         msg = 'Length of a char data types should not exceed 254 bytes.'
         raise CharLengthException(msg)
 
     sbcp, dbcp = get_ccsid_from_column(c)
 
     if dbcp != 0:
         field = fields[pos:pos + length].decode(f'cp{dbcp}')
     else:
         if sbcp == 0:
-            field = bin(int(fields[pos:pos + length], 2))
+            field = str(fields[pos:pos + length], 'utf-8')
         else:
             field = fields[pos:pos + length].decode(f'cp{sbcp}')
 
     return field.strip()
 
 
 def collect_varchar(c, fields, pos) -> str:
@@ -207,14 +208,19 @@
     pos : int
         Position of the column in the `fields`.
 
     Returns
     -------
     str:
         String.
+
+    Raises
+    ------
+    VarCharLengthException
+        Length of var char exceeds maximum length.
     """
     max_length = int(c['IXFCLENG'])
     # if max_length > 254:
     #     msg = f'Max length of a varchar data type (={max_length}) ' \
     #           f'must be less than 254 bytes.'
     #     raise ExceedingDefinedMaximumLengthException(msg)
 
@@ -227,15 +233,15 @@
 
     sbcp, dbcp = get_ccsid_from_column(c)
 
     if dbcp != 0:
         field = fields[pos:pos + length].decode(f'cp{dbcp}')
     else:
         if sbcp == 0:
-            field = bin(int(fields[pos:pos + length], 2))
+            field = str(fields[pos:pos + length], 'utf-8')
         else:
             field = fields[pos:pos + length].decode(f'cp{sbcp}')
 
     return field.strip()
 
 
 def collect_date(c, fields, pos) -> date:
@@ -321,42 +327,42 @@
     Returns
     -------
     str
         String representing the CLOB (Character Large Object).
 
     Raises
     ------
-    ExceedingDefinedMaximumLengthException
-        When the maximum length exceeds the defined limit which is 32767 bytes.
     LargeObjectLengthException
         When the length of the large object exceeds the maximum length.
     CLOBCodePageException
         When SBCP and DBCP are simultaneously equal to 0.
     """
     max_length = int(c['IXFCLENG'])
     # if max_length > 32767:
     #     msg = f'For CLOB data type, max length (={max_length}) must be ' \
     #           f'less than 32767 Bytes.'
     #     raise ExceedingDefinedMaximumLengthException(msg)
 
-    length = int(unpack('<h', fields[pos:pos + 4])[0])
+    length = int(unpack('<i', fields[pos:pos + 4])[0])
     if length > max_length:
         msg = f'Length {length} exceeds the maximum length {max_length}.'
+        logger.error(msg)
         raise LargeObjectLengthException(msg)
 
     pos += 4
 
     sbcp, dbcp = get_ccsid_from_column(c)
 
     if dbcp != 0:
         field = fields[pos:pos + length].decode(f'cp{dbcp}')
     else:
         if sbcp == 0:
             msg = 'CLOB data type can not be a bit string as BLOB, ' \
                   'the SBCP and DBCP should not simultaneously be equal to 0.'
+            logger.error(msg)
             raise CLOBCodePageException(msg)
         else:
             field = fields[pos:pos + length].decode(f'cp{sbcp}')
 
     return field.strip()
 
 
@@ -371,38 +377,29 @@
         Bytes string containing data of the row.
     pos : int
         Position of the column in the `fields`.
 
     Returns
     -------
     str
-        string representing the BLOB (Blob Large Object) or a string
-        of bit data.
+        string representing the BLOB (Blob Large Object).
 
     Raises
     ------
-    ExceedingDefinedMaximumLengthException
-        When the maximum length exceeds the defined limit which is 32767 bytes.
     LargeObjectLengthException
         When the length of the large object exceeds the maximum length.
-
     """
     max_length = int(c['IXFCLENG'])
     # if max_length > 32767:
     #     msg = 'For BLOB data type, max length must be less than 32767 Bytes.'
     #     raise ExceedingDefinedMaximumLengthException(msg)
 
-    length = int(unpack('<h', fields[pos:pos + 4])[0])
+    length = int(unpack('<i', fields[pos:pos + 4])[0])
     if length > max_length:
         msg = f'Length {length} exceeds the maximum length {max_length}.'
+        logger.error(msg)
         raise LargeObjectLengthException(msg)
 
     pos += 4
-
-    sbcp, _ = get_ccsid_from_column(c)
-
-    if sbcp == 0:
-        field = bin(int(fields[pos:pos + length], 2))
-    else:
-        field = fields[pos:pos + length].decode(f'cp{sbcp}')
+    field = str(fields[pos:pos + length], 'utf-8')
 
     return field.strip()
```

### Comparing `db2ixf-0.2.0/src/db2ixf/constants.py` & `db2ixf-0.2.1/src/db2ixf/constants.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.2.0/src/db2ixf/exceptions.py` & `db2ixf-0.2.1/src/db2ixf/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,7 +119,21 @@
     Read the
     [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
+
+
+class BlobBinaryStringException(Exception):
+    """Exception raised when encountering a data type different of binary string
+    which occurs when single byte code page equals to 0 but we re not getting
+    a binary string but an other type like character string.
+
+    Read the
+    [doc](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
```

### Comparing `db2ixf-0.2.0/src/db2ixf/helpers.py` & `db2ixf-0.2.1/src/db2ixf/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -215,46 +215,25 @@
 
     # Yield the remaining rows as the last batch
     if rows:
         batch = merge_dicts(rows)
         yield batch
 
 
-def get_ccsid_from_header(header: dict) -> Tuple[int, int]:
-    """
-    Get the coded character set identifiers for single and double
-    bytes data type. Which means the code page for singular/double byte
-    data type.
-    """
-    sbcp = str(header['IXFHSBCP'], 'utf-8').strip()
-    dbcp = str(header['IXFHDBCP'], 'utf-8').strip()
-
-    sbcp = int(sbcp) if sbcp else 0
-    dbcp = int(dbcp) if dbcp else 0
-
-    if sbcp == 0:
-        dbcp = 0
-
-    return sbcp, dbcp
-
-
 def get_ccsid_from_column(column: dict) -> Tuple[int, int]:
     """
     Get the coded character set identifiers for single and double bytes
     data type. Which means the code page for singular/double byte data type.
     """
     sbcp = str(column['IXFCSBCP'], 'utf-8').strip()
     dbcp = str(column['IXFCDBCP'], 'utf-8').strip()
 
     sbcp = int(sbcp) if sbcp else 0
     dbcp = int(dbcp) if dbcp else 0
 
-    if sbcp == 0:
-        dbcp = 0
-
     return sbcp, dbcp
 
 
 def get_record_length_and_type(file: BinaryIO) -> Tuple[int, str]:
     """Get record length and its type.
 
     Parameters
```

### Comparing `db2ixf-0.2.0/src/db2ixf/ixf.py` & `db2ixf-0.2.1/src/db2ixf/ixf.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,17 @@
     schema: dict
     """Schema extracted from metadata in the input ixf file."""
     current_data_record: dict
     """Contains current data record from input ixf file."""
     end_data_records: bool
     """Flag the end of data records in the input ixf file."""
     current_row: dict
-    """Contains parsed data extracted from a data record of the input ixf 
-    file."""
+    """
+    Contains parsed data extracted from a data record of the input ixf file.
+    """
     number_rows: int
     """Number of rows extracted from the input ixf file."""
 
     def __init__(self, file: Union[str, Path, PathLike, BinaryIO]):
         """Init the instance."""
         logger.debug('Start initializing the parser')
```

### Comparing `db2ixf-0.2.0/src/db2ixf/logger.py` & `db2ixf-0.2.1/src/db2ixf/logger.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.2.0/src/db2ixf.egg-info/PKG-INFO` & `db2ixf-0.2.1/src/db2ixf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://pypi.org/project/db2ixf/
 Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
@@ -23,15 +23,15 @@
 
 
 [![Language](https://img.shields.io/pypi/pyversions/db2ixf?color=ffde57&logo=python&style=for-the-badge)](https://www.python.org/)
 [![License](https://img.shields.io/pypi/l/db2ixf?color=3775A9&style=for-the-badge&logo=unlicense)](https://www.gnu.org/licenses/agpl-3.0)
 
 [![Pipeline](https://img.shields.io/github/actions/workflow/status/ismailhammounou/db2ixf/db2ixf.yml?branch=main&style=for-the-badge&logo=gitHub-actions)](https://github.com/ismailhammounou/db2ixf/actions/workflows/db2ixf.yml)
 [![Release](https://img.shields.io/github/v/release/ismailhammounou/db2ixf?display_name=tag&sort=semver&style=for-the-badge&logo=semver)](https://github.com/ismailhammounou/db2ixf/releases/latest)
-[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://github.com/ismailhammounou/db2ixf/releases/latest)
+[![Pypi](https://img.shields.io/pypi/v/db2ixf?color=3775A9&logo=pypi&style=for-the-badge)](https://pypi.org/project/db2ixf/)
 
 
 [![Downloads](https://img.shields.io/pypi/dm/db2ixf?style=for-the-badge)](https://pypi.org/project/db2ixf/)
 
 
 # DB2IXF Parser
 
@@ -191,17 +191,17 @@
 
 Thank you for considering contributing to IXF Parser. Let's work together to
 create a powerful and dependable tool for working with DB2's IXF files.
 
 ### Todo
 
 - [ ] Search for contributors/maintainers/sponsors.
-- [ ] Add tests (Manual testing was done but need write unit tests).
+- [x] Add tests (Manual testing was done but need write unit tests).
 - [x] Adding new collector for the floating point data type.
-- [ ] Adding new collectors for other ixf data types: binary ...etc.
+- [x] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [x] Add better ci-cd.
 - [x] Improve Makefile.
 - [x] ~~Support multiprocessing.~~
 - [x] ~~Support archived inputs: only python not CLI ?~~
```

### Comparing `db2ixf-0.2.0/src/db2ixf.egg-info/SOURCES.txt` & `db2ixf-0.2.1/src/db2ixf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

