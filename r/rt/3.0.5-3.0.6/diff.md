# Comparing `tmp/rt-3.0.5.tar.gz` & `tmp/rt-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rt-3.0.5.tar", last modified: Thu Feb  2 14:37:44 2023, max compression
+gzip compressed data, was "rt-3.0.6.tar", last modified: Wed Jun 21 15:49:00 2023, max compression
```

## Comparing `rt-3.0.5.tar` & `rt-3.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:37:44.084254 rt-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-02 14:37:21.000000 rt-3.0.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-02 14:37:21.000000 rt-3.0.5/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-02-02 14:37:21.000000 rt-3.0.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-02 14:37:21.000000 rt-3.0.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-02-02 14:37:21.000000 rt-3.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-02 14:37:21.000000 rt-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-02 14:37:21.000000 rt-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-02-02 14:37:44.084254 rt-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-02-02 14:37:21.000000 rt-3.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:37:44.080254 rt-3.0.5/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-02-02 14:37:21.000000 rt-3.0.5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-02-02 14:37:21.000000 rt-3.0.5/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-02-02 14:37:21.000000 rt-3.0.5/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-02 14:37:21.000000 rt-3.0.5/doc/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-02 14:37:21.000000 rt-3.0.5/doc/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-02 14:37:21.000000 rt-3.0.5/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-02 14:37:21.000000 rt-3.0.5/doc/rest1.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-02 14:37:21.000000 rt-3.0.5/doc/rest2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-02-02 14:37:21.000000 rt-3.0.5/doc/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-02-02 14:37:21.000000 rt-3.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:37:44.080254 rt-3.0.5/rt/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-02 14:37:21.000000 rt-3.0.5/rt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-02 14:37:21.000000 rt-3.0.5/rt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 14:37:21.000000 rt-3.0.5/rt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64987 2023-02-02 14:37:21.000000 rt-3.0.5/rt/rest1.py
--rw-r--r--   0 runner    (1001) docker     (123)    60728 2023-02-02 14:37:21.000000 rt-3.0.5/rt/rest2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:37:44.080254 rt-3.0.5/rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-02-02 14:37:44.000000 rt-3.0.5/rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-02 14:37:44.000000 rt-3.0.5/rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 14:37:44.000000 rt-3.0.5/rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-02 14:37:44.000000 rt-3.0.5/rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-02 14:37:44.000000 rt-3.0.5/rt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 14:37:44.084254 rt-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-02 14:37:21.000000 rt-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:37:44.084254 rt-3.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-02 14:37:21.000000 rt-3.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-02 14:37:21.000000 rt-3.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-02-02 14:37:21.000000 rt-3.0.5/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-02-02 14:37:21.000000 rt-3.0.5/tests/test_rest1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-02-02 14:37:21.000000 rt-3.0.5/tests/test_tickets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.058401 rt-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 15:48:45.000000 rt-3.0.6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 15:48:45.000000 rt-3.0.6/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-06-21 15:48:45.000000 rt-3.0.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 15:48:45.000000 rt-3.0.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-21 15:48:45.000000 rt-3.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-21 15:48:45.000000 rt-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-21 15:48:45.000000 rt-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-21 15:49:00.058401 rt-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-21 15:48:45.000000 rt-3.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.054401 rt-3.0.6/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-21 15:48:45.000000 rt-3.0.6/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-21 15:48:45.000000 rt-3.0.6/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-21 15:48:45.000000 rt-3.0.6/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 15:48:45.000000 rt-3.0.6/doc/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 15:48:45.000000 rt-3.0.6/doc/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-21 15:48:45.000000 rt-3.0.6/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 15:48:45.000000 rt-3.0.6/doc/rest1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 15:48:45.000000 rt-3.0.6/doc/rest2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-21 15:48:45.000000 rt-3.0.6/doc/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-21 15:48:45.000000 rt-3.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.054401 rt-3.0.6/rt/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 15:48:45.000000 rt-3.0.6/rt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-21 15:48:45.000000 rt-3.0.6/rt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:48:45.000000 rt-3.0.6/rt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64987 2023-06-21 15:48:45.000000 rt-3.0.6/rt/rest1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60728 2023-06-21 15:48:45.000000 rt-3.0.6/rt/rest2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.058401 rt-3.0.6/rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:49:00.058401 rt-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 15:48:45.000000 rt-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.058401 rt-3.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 15:48:45.000000 rt-3.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-21 15:48:45.000000 rt-3.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-06-21 15:48:45.000000 rt-3.0.6/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-21 15:48:45.000000 rt-3.0.6/tests/test_rest1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-21 15:48:45.000000 rt-3.0.6/tests/test_tickets.py
```

### Comparing `rt-3.0.5/.pylintrc` & `rt-3.0.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/CHANGELOG.md` & `rt-3.0.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v3.0.6], 2023-06-21
+### Added
+- Fixed bug in rest1 (#86)
+
 ## [v3.0.5], 2023-02-02
 ### Added
 - Added support for specifying custom fields on user creation/edit (#82).
 
 ## [v3.0.4], 2022-11-08
 ### Fixes
 - Workaround for parsing issues with tickets with only 1 attachment (#80), due to probably an upstream bug.
```

### Comparing `rt-3.0.5/LICENSE` & `rt-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/PKG-INFO` & `rt-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt
-Version: 3.0.5
+Version: 3.0.6
 Summary: Python interface to Request Tracker API
 Author-email: Georges Toth <georges.toth@govcert.etat.lu>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/python-rt/python-rt
 Project-URL: Documentation, https://python-rt.readthedocs.io/
 Project-URL: Source, https://github.com/python-rt/python-rt
 Project-URL: Tracker, https://github.com/python-rt/python-rt/issues
```

### Comparing `rt-3.0.5/README.rst` & `rt-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/doc/Makefile` & `rt-3.0.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/doc/changelog.rst` & `rt-3.0.6/doc/changelog.rst`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/doc/conf.py` & `rt-3.0.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/doc/index.rst` & `rt-3.0.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/doc/usage.rst` & `rt-3.0.6/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/pyproject.toml` & `rt-3.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/rt/exceptions.py` & `rt-3.0.6/rt/exceptions.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/rt/rest1.py` & `rt-3.0.6/rt/rest1.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         if (len(msg) > 2) and self.RE_PATTERNS['not_allowed_pattern'].match(msg[2]):
             raise NotAllowedError(msg[2][2:])
         if self.RE_PATTERNS['credentials_required_pattern'].match(msg[0]):
             raise AuthorizationError('Credentials required.')
         if self.RE_PATTERNS['syntax_error_pattern'].match(msg[0]):
             raise APISyntaxError(msg[2][2:] if len(msg) > 2 else 'Syntax error.')
         if self.RE_PATTERNS['bad_request_pattern'].match(msg[0]):
-            raise BadRequestError(msg[3] if len(msg) > 2 else 'Bad request.')
+            raise BadRequestError(msg[2] if len(msg) > 2 else 'Bad request.')
 
     @staticmethod
     def __normalize_list(msg: typing.Union[str, typing.Sequence[str]]) -> typing.Sequence[str]:
         """Split message to list by commas and trim whitespace."""
         if isinstance(msg, list):
             _msg = "".join(msg)
         elif isinstance(msg, str):
```

### Comparing `rt-3.0.5/rt/rest2.py` & `rt-3.0.6/rt/rest2.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/rt.egg-info/PKG-INFO` & `rt-3.0.6/rt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt
-Version: 3.0.5
+Version: 3.0.6
 Summary: Python interface to Request Tracker API
 Author-email: Georges Toth <georges.toth@govcert.etat.lu>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/python-rt/python-rt
 Project-URL: Documentation, https://python-rt.readthedocs.io/
 Project-URL: Source, https://github.com/python-rt/python-rt
 Project-URL: Tracker, https://github.com/python-rt/python-rt/issues
```

### Comparing `rt-3.0.5/rt.egg-info/SOURCES.txt` & `rt-3.0.6/rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/tests/test_basic.py` & `rt-3.0.6/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/tests/test_rest1.py` & `rt-3.0.6/tests/test_rest1.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.5/tests/test_tickets.py` & `rt-3.0.6/tests/test_tickets.py`

 * *Files identical despite different names*

