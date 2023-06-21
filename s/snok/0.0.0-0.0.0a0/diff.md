# Comparing `tmp/snok-0.0.0.tar.gz` & `tmp/snok-0.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snok-0.0.0.tar", last modified: Wed Jun 21 17:48:33 2023, max compression
+gzip compressed data, was "snok-0.0.0a0.tar", last modified: Mon Jan 16 17:36:40 2023, max compression
```

## Comparing `snok-0.0.0.tar` & `snok-0.0.0a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:33.675827 snok-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 17:48:09.000000 snok-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-21 17:48:33.675827 snok-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-21 17:48:09.000000 snok-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-21 17:48:09.000000 snok-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 17:48:33.675827 snok-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:33.675827 snok-0.0.0/snok/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 17:48:09.000000 snok-0.0.0/snok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-21 17:48:09.000000 snok-0.0.0/snok/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 17:48:09.000000 snok-0.0.0/snok/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:09.000000 snok-0.0.0/snok/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:33.675827 snok-0.0.0/snok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-21 17:48:33.000000 snok-0.0.0/snok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-21 17:48:33.000000 snok-0.0.0/snok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:48:33.000000 snok-0.0.0/snok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:48:33.000000 snok-0.0.0/snok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-21 17:48:33.000000 snok-0.0.0/snok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 17:48:33.000000 snok-0.0.0/snok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:48:33.675827 snok-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-21 17:48:09.000000 snok-0.0.0/tests/test_cli_new.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 17:48:09.000000 snok-0.0.0/tests/test_version.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-01-16 17:36:40.192709 snok-0.0.0a0/
+-rw-r--r--   0 anthony    (501) staff       (20)     1056 2023-01-16 02:14:20.000000 snok-0.0.0a0/LICENSE
+-rw-r--r--   0 anthony    (501) staff       (20)      952 2023-01-16 17:36:40.192772 snok-0.0.0a0/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)      629 2023-01-16 02:14:47.000000 snok-0.0.0a0/README.md
+-rw-r--r--   0 anthony    (501) staff       (20)      911 2023-01-16 02:14:50.000000 snok-0.0.0a0/pyproject.toml
+-rw-r--r--   0 anthony    (501) staff       (20)      173 2023-01-16 17:36:40.193038 snok-0.0.0a0/setup.cfg
+-rw-r--r--   0 anthony    (501) staff       (20)       38 2023-01-16 02:14:20.000000 snok-0.0.0a0/setup.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-01-16 17:36:40.191124 snok-0.0.0a0/snok/
+-rw-r--r--   0 anthony    (501) staff       (20)       36 2023-01-16 17:36:24.000000 snok-0.0.0a0/snok/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)       73 2023-01-16 02:14:20.000000 snok-0.0.0a0/snok/main.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-01-16 17:36:40.192109 snok-0.0.0a0/snok.egg-info/
+-rw-r--r--   0 anthony    (501) staff       (20)      952 2023-01-16 17:36:40.000000 snok-0.0.0a0/snok.egg-info/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)      297 2023-01-16 17:36:40.000000 snok-0.0.0a0/snok.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony    (501) staff       (20)        1 2023-01-16 17:36:40.000000 snok-0.0.0a0/snok.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony    (501) staff       (20)      122 2023-01-16 17:36:40.000000 snok-0.0.0a0/snok.egg-info/requires.txt
+-rw-r--r--   0 anthony    (501) staff       (20)       11 2023-01-16 17:36:40.000000 snok-0.0.0a0/snok.egg-info/top_level.txt
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-01-16 17:36:40.192610 snok-0.0.0a0/tests/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2023-01-16 02:14:20.000000 snok-0.0.0a0/tests/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)      176 2023-01-16 02:14:20.000000 snok-0.0.0a0/tests/conftest.py
+-rw-r--r--   0 anthony    (501) staff       (20)      131 2023-01-16 02:14:40.000000 snok-0.0.0a0/tests/test_main.py
+-rw-r--r--   0 anthony    (501) staff       (20)       94 2023-01-16 02:14:40.000000 snok-0.0.0a0/tests/test_version.py
```

### Comparing `snok-0.0.0/LICENSE` & `snok-0.0.0a0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) Anthony Corletti
+Copyright 2021 Anthony Corletti
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

