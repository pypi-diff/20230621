# Comparing `tmp/cubicweb-sentry-0.8.1.tar.gz` & `tmp/cubicweb-sentry-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-sentry-0.8.1.tar", last modified: Mon Jan  9 11:00:09 2023, max compression
+gzip compressed data, was "cubicweb-sentry-0.8.2.tar", last modified: Wed Jun 21 15:46:35 2023, max compression
```

## Comparing `cubicweb-sentry-0.8.1.tar` & `cubicweb-sentry-0.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 11:00:09.015276 cubicweb-sentry-0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      502 2023-01-09 11:00:09.015276 cubicweb-sentry-0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 11:00:09.015276 cubicweb-sentry-0.8.1/cubicweb_sentry/
--rw-rw-rw-   0 root         (0) root         (0)     1125 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/cubicweb_sentry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/cubicweb_sentry/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/cubicweb_sentry/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/cubicweb_sentry/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 11:00:09.015276 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/
--rw-r--r--   0 root         (0) root         (0)      502 2023-01-09 11:00:08.000000 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-01-09 11:00:08.000000 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 11:00:08.000000 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-01-09 11:00:08.000000 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 11:00:08.000000 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-01-09 11:00:08.000000 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-09 11:00:08.000000 cubicweb-sentry-0.8.1/cubicweb_sentry.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-09 11:00:09.015276 cubicweb-sentry-0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-01-09 10:59:54.000000 cubicweb-sentry-0.8.1/tox.ini
+drwxr-xr-x   0 nspanti   (1000) nspanti   (1000)        0 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)      313 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/MANIFEST.in
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)      989 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/PKG-INFO
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)      311 2023-06-20 13:53:01.000000 cubicweb-sentry-0.8.2/README.md
+drwxr-xr-x   0 nspanti   (1000) nspanti   (1000)        0 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/cubicweb_sentry/
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)     1125 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/__init__.py
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)      776 2023-06-20 13:53:01.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/__pkginfo__.py
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)      890 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/entities.py
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)     1166 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/site_cubicweb.py
+drwxr-xr-x   0 nspanti   (1000) nspanti   (1000)        0 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)      989 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)      432 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)        1 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)       43 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)        1 2023-06-20 13:34:43.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/not-zip-safe
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)       43 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/requires.txt
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)       16 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/top_level.txt
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)       38 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/setup.cfg
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)     2604 2023-06-20 15:46:41.000000 cubicweb-sentry-0.8.2/setup.py
+-rw-r--r--   0 nspanti   (1000) nspanti   (1000)     1021 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/tox.ini
```

### Comparing `cubicweb-sentry-0.8.1/cubicweb_sentry/__init__.py` & `cubicweb-sentry-0.8.2/cubicweb_sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-sentry-0.8.1/cubicweb_sentry/entities.py` & `cubicweb-sentry-0.8.2/cubicweb_sentry/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-sentry-0.8.1/cubicweb_sentry/site_cubicweb.py` & `cubicweb-sentry-0.8.2/cubicweb_sentry/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-sentry-0.8.1/setup.py` & `cubicweb-sentry-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
-# contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
+# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of cubiweb-sentry.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
 # CubicWeb is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
-
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
-# along with CubicWeb.  If not, see <http://www.gnu.org/licenses/>.
+# along with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb_sentry setup module using data from
 cubicweb_sentry/__pkginfo__.py file
 """
 
 from os.path import join, dirname
 
 from setuptools import find_packages, setup
@@ -43,15 +42,15 @@
 license = __pkginfo__["license"]
 description = __pkginfo__["description"]
 web = __pkginfo__["web"]
 author = __pkginfo__["author"]
 author_email = __pkginfo__["author_email"]
 classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, "README.rst")) as f:
+with open(join(here, "README.md")) as f:
     long_description = f.read()
 
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
```

### Comparing `cubicweb-sentry-0.8.1/tox.ini` & `cubicweb-sentry-0.8.2/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,22 @@
 skip_install = true
 deps =
   flake8
 commands =
   {envpython} -m flake8 {toxinidir} {posargs}
 
 [flake8]
-format = pylint
 max-line-length = 100
 ignore = E731,W503
 exclude = __pkginfo__.py,migration/*,test/data/*,setup.py,.tox/*
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -51,8 +50,8 @@
 commands = black --check .
 
 [testenv:black-run]
 basepython = python3
 skip_install = true
 deps =
   black >= 22.12
-commands = black .
+commands = black .
```

