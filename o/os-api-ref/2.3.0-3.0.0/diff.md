# Comparing `tmp/os-api-ref-2.3.0.tar.gz` & `tmp/os-api-ref-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-api-ref-2.3.0.tar", last modified: Thu Oct 28 10:45:36 2021, max compression
+gzip compressed data, was "os-api-ref-3.0.0.tar", last modified: Wed Jun 21 11:09:51 2023, max compression
```

## Comparing `os-api-ref-2.3.0.tar` & `os-api-ref-3.0.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.781576 os-api-ref-2.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1602 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5128 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5767 2021-10-28 10:45:36.781576 os-api-ref-2.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/RELEASING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/TESTS.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.773577 os-api-ref-2.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.773577 os-api-ref-2.3.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2535 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1999 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/doc/source/http-status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10468 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.773577 os-api-ref-2.3.0/os_api_ref/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24984 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.777576 os-api-ref-2.3.0/os_api_ref/assets/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4054 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/assets/api-site.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6675 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/assets/api-site.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13326 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/assets/combobox.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45404 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/assets/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23424 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/assets/glyphicons-halflings-regular.woff
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7968 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/http_codes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.777576 os-api-ref-2.3.0/os_api_ref/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3195 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.769577 os-api-ref-2.3.0/os_api_ref/tests/examples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.777576 os-api-ref-2.3.0/os_api_ref/tests/examples/basic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/basic/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/basic/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/basic/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/basic/status.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.777576 os-api-ref-2.3.0/os_api_ref/tests/examples/microversions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/microversions/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/microversions/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/microversions/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.781576 os-api-ref-2.3.0/os_api_ref/tests/examples/warnings/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/warnings/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/warnings/empty_parameters_file.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/warnings/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/examples/warnings/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5674 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/test_basic_example.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4346 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/test_microversions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/test_os_api_ref.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3625 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/os_api_ref/tests/test_warnings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-28 10:45:36.777576 os-api-ref-2.3.0/os_api_ref.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5767 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/os_api_ref.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/os_api_ref.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/os_api_ref.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/os_api_ref.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/os_api_ref.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/os_api_ref.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2021-10-28 10:45:36.000000 os-api-ref-2.3.0/os_api_ref.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-10-28 10:45:36.781576 os-api-ref-2.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2021-10-28 10:44:56.000000 os-api-ref-2.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.490884 os-api-ref-3.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5389 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5767 2023-06-21 11:09:51.490884 os-api-ref-3.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/RELEASING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/TESTS.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.482885 os-api-ref-3.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.486884 os-api-ref-3.0.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2531 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1999 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/doc/source/http-status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10468 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.486884 os-api-ref-3.0.0/os_api_ref/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25113 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.486884 os-api-ref-3.0.0/os_api_ref/assets/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4054 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/assets/api-site.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6675 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/assets/api-site.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13326 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/assets/combobox.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45404 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/assets/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23424 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/assets/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7968 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/http_codes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.490884 os-api-ref-3.0.0/os_api_ref/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4047 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.478885 os-api-ref-3.0.0/os_api_ref/tests/examples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.490884 os-api-ref-3.0.0/os_api_ref/tests/examples/basic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/basic/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/basic/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/basic/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/basic/status.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.490884 os-api-ref-3.0.0/os_api_ref/tests/examples/microversions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/microversions/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/microversions/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/microversions/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.490884 os-api-ref-3.0.0/os_api_ref/tests/examples/warnings/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/warnings/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/warnings/empty_parameters_file.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/warnings/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/examples/warnings/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5040 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/test_basic_example.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4292 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/test_microversions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/test_os_api_ref.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3552 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/os_api_ref/tests/test_warnings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:09:51.486884 os-api-ref-3.0.0/os_api_ref.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5767 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/os_api_ref.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/os_api_ref.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/os_api_ref.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/os_api_ref.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/os_api_ref.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/os_api_ref.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-06-21 11:09:51.000000 os-api-ref-3.0.0/os_api_ref.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2023-06-21 11:09:51.490884 os-api-ref-3.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2023-06-21 11:09:21.000000 os-api-ref-3.0.0/tox.ini
```

### Comparing `os-api-ref-2.3.0/.pre-commit-config.yaml` & `os-api-ref-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/.zuul.yaml` & `os-api-ref-3.0.0/.zuul.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       zuul_work_dir: src/opendev.org/openstack/nova
     required-projects:
       - openstack/nova
       - openstack/os-api-ref
 
 - project:
     templates:
-      - openstack-python3-xena-jobs
+      - openstack-python3-jobs
       - check-requirements
       - publish-openstack-docs-pti
     check:
       jobs:
         - os-api-ref-nova-src
     gate:
       jobs:
```

### Comparing `os-api-ref-2.3.0/AUTHORS` & `os-api-ref-3.0.0/AUTHORS`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Akihiro Motoki <amotoki@gmail.com>
+Alexander Fadeev <fadeevab.com@gmail.com>
 Andreas Jaeger <aj@suse.com>
 Anne Gentle <agentle@cisco.com>
 Cao Xuan Hoang <hoangcx@vn.fujitsu.com>
 Corey Bryant <corey.bryant@canonical.com>
 Daniel Bengtsson <dbengt@redhat.com>
+Daniel Garcia Moreno <daniel.garcia@suse.com>
 Daniel Gonzalez <daniel@gonzalez-nothnagel.de>
 Dirk Mueller <dirk@dmllr.de>
 Dmitry Shachnev <mitya57@ubuntu.com>
 Doug Hellmann <doug@doughellmann.com>
 Flavio Percoco <flaper87@gmail.com>
 Gergely Csatari <gergely.csatari@nokia.com>
 Graham Hayes <gr@ham.ie>
@@ -31,15 +33,17 @@
 Yuval Brik <yuval@brik.org.il>
 ZhijunWei <wzj334965317@outlook.com>
 gengchc2 <geng.changcai2@zte.com.cn>
 ghanshyam <ghanshyammann@gmail.com>
 jacky06 <zhang.min@99cloud.net>
 maaoyu <maaoyu@inspur.com>
 melissaml <ma.lei@99cloud.net>
+niuke <niuke19970315@163.com>
 ricolin <rico.lin@easystack.cn>
 shangxiaobj <shangxiaobj@inspur.com>
 shashi.kant <shashi.kant@nectechnologies.in>
 tengqm <tengqim@cn.ibm.com>
+tushargite96 <tushargite96@gmail.com>
 yanghuichan <yanghc@fiberhome.com>
 yangyawei <yangyawei@inspur.com>
 zhoulinhui <df.some@foxmail.com>
 zhulingjie <easyzlj@gmail.com>
```

### Comparing `os-api-ref-2.3.0/CONTRIBUTING.rst` & `os-api-ref-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/ChangeLog` & `os-api-ref-3.0.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+3.0.0
+-----
+
+* remove unicode prefix from code
+* Fix the 'No such file or directory' error
+* Remove deprecated sphinx-testing dependency
+* Drop python3.6/3.7 support in testing runtime
+* Update CI to use unversioned jobs template
+* Add Python3 yoga unit tests
+
 2.3.0
 -----
 
 * Fix exception logging
 * tox: Don't use distutils entrypoint for coverage
 * Remove six
 * Drop support for Sphinx < 4.x
```

### Comparing `os-api-ref-2.3.0/LICENSE` & `os-api-ref-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/PKG-INFO` & `os-api-ref-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-api-ref
-Version: 2.3.0
+Version: 3.0.0
 Summary: Sphinx Extensions to support API reference sites in OpenStack
 Home-page: https://docs.openstack.org/os-api-ref/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -124,12 +124,12 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
```

### Comparing `os-api-ref-2.3.0/README.rst` & `os-api-ref-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/RELEASING.rst` & `os-api-ref-3.0.0/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/doc/source/conf.py` & `os-api-ref-3.0.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'os-api-ref'
-copyright = u'2018, The contributors'
+project = 'os-api-ref'
+copyright = '2018, The contributors'
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
 add_module_names = True
@@ -71,10 +71,10 @@
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto/manual]).
 latex_documents = [
     ('index',
      '%s.tex' % project,
-     u'%s Documentation' % project,
-     u'OpenStack Foundation', 'manual'),
+     '%s Documentation' % project,
+     'OpenStack Foundation', 'manual'),
 ]
```

### Comparing `os-api-ref-2.3.0/doc/source/http-status.yaml` & `os-api-ref-3.0.0/doc/source/http-status.yaml`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/doc/source/usage.rst` & `os-api-ref-3.0.0/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/__init__.py` & `os-api-ref-3.0.0/os_api_ref/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -638,14 +638,17 @@
     fonts = (
         'glyphicons-halflings-regular.ttf',
         'glyphicons-halflings-regular.woff'
     )
     builders = ('html', 'readthedocs', 'readthedocssinglehtmllocalmedia')
     if app.builder.name not in builders or exception:
         return
+    dirtree = os.path.join(app.builder.outdir, '_static/fonts')
+    if not os.path.exists(dirtree):
+        os.makedirs(dirtree)
     LOG.info('Copying assets: %s', ', '.join(assets))
     LOG.info('Copying fonts: %s', ', '.join(fonts))
     for asset in assets:
         dest = os.path.join(app.builder.outdir, '_static', asset)
         source = os.path.abspath(os.path.dirname(__file__))
         copyfile(os.path.join(source, 'assets', asset), dest)
     for font in fonts:
```

### Comparing `os-api-ref-2.3.0/os_api_ref/assets/api-site.css` & `os-api-ref-3.0.0/os_api_ref/assets/api-site.css`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/assets/api-site.js` & `os-api-ref-3.0.0/os_api_ref/assets/api-site.js`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/assets/combobox.js` & `os-api-ref-3.0.0/os_api_ref/assets/combobox.js`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/assets/glyphicons-halflings-regular.ttf` & `os-api-ref-3.0.0/os_api_ref/assets/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/assets/glyphicons-halflings-regular.woff` & `os-api-ref-3.0.0/os_api_ref/assets/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/http_codes.py` & `os-api-ref-3.0.0/os_api_ref/http_codes.py`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/base.py` & `os-api-ref-3.0.0/os_api_ref/tests/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,51 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import os
 
 import fixtures
+import tempfile
 import testtools
 
+from sphinx.testing.path import path
+from sphinx.testing.util import SphinxTestApp
+
 
 def example_dir(name=""):
     return os.path.join(os.path.dirname(__file__), 'examples', name)
 
 
 _TRUE_VALUES = ('True', 'true', '1', 'yes')
 
 
+class with_app:
+    def __init__(self, **kwargs):
+        if 'srcdir' in kwargs:
+            self.srcdir = path(kwargs['srcdir'])
+        self.sphinx_app_args = kwargs
+
+    def __call__(self, f):
+        def newf(*args, **kwargs):
+            with tempfile.TemporaryDirectory() as tmpdirname:
+                tmpdir = path(tmpdirname)
+                tmproot = tmpdir / self.srcdir.basename()
+                self.srcdir.copytree(tmproot)
+                self.sphinx_app_args['srcdir'] = tmproot
+                self.builddir = tmproot.joinpath('_build')
+
+                app = SphinxTestApp(freshenv=True, **self.sphinx_app_args)
+
+                f(*args, app, app._status, app._warning, **kwargs)
+
+                app.cleanup()
+        return newf
+
+
 class OutputStreamCapture(fixtures.Fixture):
     """Capture output streams during tests.
 
     This fixture captures errant printing to stderr / stdout during
     the tests and lets us see those streams at the end of the test
     runs instead. Useful to see what was happening during failed
     tests.
```

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/examples/basic/conf.py` & `os-api-ref-3.0.0/os_api_ref/tests/examples/basic/conf.py`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/examples/basic/status.yaml` & `os-api-ref-3.0.0/os_api_ref/tests/examples/basic/status.yaml`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/examples/microversions/conf.py` & `os-api-ref-3.0.0/os_api_ref/tests/examples/microversions/conf.py`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/examples/warnings/conf.py` & `os-api-ref-3.0.0/os_api_ref/tests/examples/warnings/conf.py`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/examples/warnings/index.rst` & `os-api-ref-3.0.0/os_api_ref/tests/examples/warnings/index.rst`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/test_basic_example.py` & `os-api-ref-3.0.0/os_api_ref/tests/test_basic_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,40 +14,26 @@
 test_os_api_ref
 ----------------------------------
 
 Tests for `os_api_ref` module.
 """
 
 from bs4 import BeautifulSoup
-import sphinx
-from sphinx_testing import with_app
 
 from os_api_ref.tests import base
 
 
-# FIXME(stephenfin): This is horrible. We're monkeypatching this to work around
-# the fact that Sphinx 1.8+ started called 'abspath' from within the
-# 'sphinx.application.Application' class [1]. This means our careful use of
-# 'sphinx_testing.path.path' for 'Application.outdir' etc. gets stomped on.
-# We're correcting that but we're doing so globally because mock doesn't work
-# for some reason and this is bound to have some side effects
-#
-# [1] https://github.com/sphinx-doc/sphinx/commit/3a85b3502f
-sphinx.application.abspath = lambda x: x
-
-
 class TestBasicExample(base.TestCase):
     """Test basic rendering.
 
     This can be used to test that basic rendering works for these
     examples, so if someone breaks something we know.
     """
 
-    @with_app(buildername='html', srcdir=base.example_dir('basic'),
-              copy_srcdir_to_tmpdir=True)
+    @base.with_app(buildername='html', srcdir=base.example_dir('basic'))
     def setUp(self, app, status, warning):
         super(TestBasicExample, self).setUp()
         self.app = app
         self.status = status
         self.warning = warning
         self.app.build()
         self.html = (app.outdir / 'index.html').read_text(encoding='utf-8')
```

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/test_microversions.py` & `os-api-ref-3.0.0/os_api_ref/tests/test_microversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 test_os_api_ref
 ----------------------------------
 
 Tests for `os_api_ref` module.
 """
 
 from bs4 import BeautifulSoup
-from sphinx_testing import with_app
 
 from os_api_ref.tests import base
 
 
 class TestMicroversions(base.TestCase):
     """Test basic rendering.
 
     This can be used to test that basic rendering works for these
     examples, so if someone breaks something we know.
     """
 
-    @with_app(buildername='html', srcdir=base.example_dir('microversions'),
-              copy_srcdir_to_tmpdir=True)
+    @base.with_app(buildername='html',
+                   srcdir=base.example_dir('microversions'))
     def setUp(self, app, status, warning):
         super(TestMicroversions, self).setUp()
         self.app = app
         self.app.build()
         self.status = status.getvalue()
         self.warning = warning.getvalue()
         self.html = (app.outdir / 'index.html').read_text(encoding='utf-8')
```

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/test_os_api_ref.py` & `os-api-ref-3.0.0/os_api_ref/tests/test_os_api_ref.py`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/os_api_ref/tests/test_warnings.py` & `os-api-ref-3.0.0/os_api_ref/tests/test_warnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 test_os_api_ref
 ----------------------------------
 
 Tests for `os_api_ref` module.
 """
 
 from bs4 import BeautifulSoup
-from sphinx_testing import with_app
 
 from os_api_ref.tests import base
 
 
 class TestWarnings(base.TestCase):
     """Test basic rendering.
 
     This can be used to test that basic rendering works for these
     examples, so if someone breaks something we know.
     """
 
-    @with_app(buildername='html', srcdir=base.example_dir('warnings'),
-              copy_srcdir_to_tmpdir=True)
+    @base.with_app(buildername='html', srcdir=base.example_dir('warnings'))
     def setUp(self, app, status, warning):
         super(TestWarnings, self).setUp()
         self.app = app
         self.app.build()
         self.status = status.getvalue()
         self.warning = warning.getvalue()
         self.html = (app.outdir / 'index.html').read_text(encoding='utf-8')
```

### Comparing `os-api-ref-2.3.0/os_api_ref.egg-info/PKG-INFO` & `os-api-ref-3.0.0/os_api_ref.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-api-ref
-Version: 2.3.0
+Version: 3.0.0
 Summary: Sphinx Extensions to support API reference sites in OpenStack
 Home-page: https://docs.openstack.org/os-api-ref/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -124,12 +124,12 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
```

### Comparing `os-api-ref-2.3.0/os_api_ref.egg-info/SOURCES.txt` & `os-api-ref-3.0.0/os_api_ref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/setup.cfg` & `os-api-ref-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 name = os-api-ref
 summary = Sphinx Extensions to support API reference sites in OpenStack
 description_file = 
 	README.rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://docs.openstack.org/os-api-ref/latest/
-python_requires = >=3.6
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	os_api_ref
```

### Comparing `os-api-ref-2.3.0/setup.py` & `os-api-ref-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `os-api-ref-2.3.0/tox.ini` & `os-api-ref-3.0.0/tox.ini`

 * *Files identical despite different names*

