# Comparing `tmp/Missing-4.2.tar.gz` & `tmp/Missing-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Missing-4.2.tar", last modified: Wed Nov 16 08:30:20 2022, max compression
+gzip compressed data, was "Missing-5.0.tar", last modified: Wed Jun 21 06:19:51 2023, max compression
```

## Comparing `Missing-4.2.tar` & `Missing-5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-16 08:30:20.822238 Missing-4.2/
--rw-r--r--   0 jens       (501) staff       (20)     1220 2022-11-16 08:20:23.000000 Missing-4.2/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      804 2022-11-16 08:20:00.000000 Missing-4.2/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2022-11-15 12:38:15.000000 Missing-4.2/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2022-11-15 12:38:15.000000 Missing-4.2/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      196 2022-11-16 08:20:00.000000 Missing-4.2/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)     3381 2022-11-16 08:30:20.822320 Missing-4.2/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      748 2022-11-16 08:26:43.000000 Missing-4.2/README.rst
--rw-r--r--   0 jens       (501) staff       (20)       90 2022-11-16 08:27:57.000000 Missing-4.2/buildout.cfg
--rw-r--r--   0 jens       (501) staff       (20)      468 2022-11-16 08:30:20.822587 Missing-4.2/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     2471 2022-11-16 08:23:14.000000 Missing-4.2/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-16 08:30:20.819342 Missing-4.2/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-16 08:30:20.821328 Missing-4.2/src/Missing/
--rw-r--r--   0 jens       (501) staff       (20)      106 2022-11-16 08:20:00.000000 Missing-4.2/src/Missing/_Missing.py
--rw-r--r--   0 jens       (501) staff       (20)     2631 2022-11-16 08:20:00.000000 Missing-4.2/src/Missing/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     9588 2022-11-16 08:20:00.000000 Missing-4.2/src/Missing/tests.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-16 08:30:20.822120 Missing-4.2/src/Missing.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)     3381 2022-11-16 08:30:20.000000 Missing-4.2/src/Missing.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      393 2022-11-16 08:30:20.000000 Missing-4.2/src/Missing.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-16 08:30:20.000000 Missing-4.2/src/Missing.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-15 12:44:38.000000 Missing-4.2/src/Missing.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)       22 2022-11-16 08:30:20.000000 Missing-4.2/src/Missing.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        8 2022-11-16 08:30:20.000000 Missing-4.2/src/Missing.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1460 2022-11-16 08:20:00.000000 Missing-4.2/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-21 06:19:51.727861 Missing-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)     1360 2023-06-21 06:19:51.000000 Missing-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-06-21 06:19:51.000000 Missing-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-06-21 06:19:51.000000 Missing-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-06-21 06:19:51.000000 Missing-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      196 2023-06-21 06:19:51.000000 Missing-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     3283 2023-06-21 06:19:51.727993 Missing-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      748 2023-06-21 06:19:51.000000 Missing-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)       90 2023-06-21 06:19:51.000000 Missing-5.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      469 2023-06-21 06:19:51.728575 Missing-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2283 2023-06-21 06:19:51.000000 Missing-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-21 06:19:51.720931 Missing-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-21 06:19:51.725529 Missing-5.0/src/Missing/
+-rw-r--r--   0 mac        (513) staff       (20)      421 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing/_Missing.py
+-rw-r--r--   0 mac        (513) staff       (20)     2175 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    12397 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing/tests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-21 06:19:51.727593 Missing-5.0/src/Missing.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     3283 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      393 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       42 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        8 2023-06-21 06:19:51.000000 Missing-5.0/src/Missing.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1427 2023-06-21 06:19:51.000000 Missing-5.0/tox.ini
```

### Comparing `Missing-4.2/CHANGES.rst` & `Missing-5.0/CHANGES.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+5.0 (2023-06-21)
+----------------
+
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Deprecate ``._Missing`` which containes just BBB imports.
+
+
 4.2 (2022-11-16)
 ----------------
 
 - Add support for Python 3.8, 3.9, 3.10, 3.11
 
 
 4.1 (2018-10-05)
```

### Comparing `Missing-4.2/CONTRIBUTING.md` & `Missing-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Missing-4.2/LICENSE.txt` & `Missing-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Missing-4.2/PKG-INFO` & `Missing-5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: Missing
-Version: 4.2
+Version: 5.0
 Summary: Special Missing objects used in Zope.
 Home-page: https://github.com/zopefoundation/Missing
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Missing/issues
 Project-URL: Sources, https://github.com/zopefoundation/Missing
 Keywords: zope missing object
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Zope :: 4
+Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 .. image:: https://github.com/zopefoundation/Missing/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/Missing/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/Missing/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/Missing?branch=master
@@ -49,14 +45,23 @@
 
 Missing provides special objects used in some Zope internals like the ZCatalog.
 
 
 Changelog
 =========
 
+5.0 (2023-06-21)
+----------------
+
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Deprecate ``._Missing`` which containes just BBB imports.
+
+
 4.2 (2022-11-16)
 ----------------
 
 - Add support for Python 3.8, 3.9, 3.10, 3.11
 
 
 4.1 (2018-10-05)
```

### Comparing `Missing-4.2/README.rst` & `Missing-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `Missing-4.2/setup.py` & `Missing-5.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,50 +15,49 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
 README = open('README.rst').read()
 CHANGES = open('CHANGES.rst').read()
 
-version = '4.2'
+version = '5.0'
 
 setup(
     name='Missing',
     version=version,
     url='https://github.com/zopefoundation/Missing',
     project_urls={
         'Issue Tracker': 'https://github.com/zopefoundation/Missing/issues',
         'Sources': 'https://github.com/zopefoundation/Missing',
     },
     license='ZPL 2.1',
     description="Special Missing objects used in Zope.",
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     long_description='\n\n'.join([README, CHANGES]),
     keywords="zope missing object",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
-        "Framework :: Zope :: 4",
+        "Framework :: Zope :: 5",
         "License :: OSI Approved :: Zope Public License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
-    install_requires=['ExtensionClass >= 4.1a1'],
+    python_requires='>=3.7',
+    install_requires=[
+        'ExtensionClass >= 4.1a1',
+        'zope.deferredimport',
+    ],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `Missing-4.2/src/Missing/__init__.py` & `Missing-5.0/src/Missing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,10 @@
-import sys
-
 from ExtensionClass import Base
 
 
-if sys.version_info >= (3, 5):
-    PY3 = True
-    PY35 = True
-elif sys.version_info >= (3, ):
-    PY3 = True
-    PY35 = False
-else:
-    PY3 = False
-    PY35 = False
-
-
 class Missing(Base):
 
     _valid = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
     __hash__ = None
 
     def __call__(self):
         return self
@@ -35,25 +22,14 @@
         if self is V:
             return 'V'
         return (type(self), ())
 
     def __bool__(self):
         return False
 
-    if not PY3:
-        __nonzero__ = __bool__
-
-        def __coerce__(self, other):
-            return (self, notMissing)
-
-        def __cmp__(self, other):
-            if self is notMissing:
-                return -1
-            return other is notMissing
-
     def __eq__(self, other):
         if self is notMissing:
             return True if other is notMissing else False
         return other is self
 
     def __ne__(self, other):
         return not self.__eq__(other)
@@ -82,17 +58,15 @@
     __add__ = __radd__ = __sub__ = __rsub__ = _calc
     __mul__ = __rmul__ = __div__ = __rdiv__ = _calc
     __floordiv__ = __rfloordiv__ = __truediv__ = __rtruediv__ = _calc
     __pow__ = __rpow__ = _calc
     __mod__ = __rmod__ = __divmod__ = __rdivmod__ = _calc
     __lshift__ = __rshift__ = __rlshift__ = __rrshift__ = _calc
     __and__ = __rand__ = __or__ = __ror__ = __xor__ = __rxor__ = _calc
-
-    if PY35:
-        __matmul__ = __rmatmul__ = _calc
+    __matmul__ = __rmatmul__ = _calc
 
     def _change(self):
         return self
 
     __neg__ = __pos__ = __abs__ = __invert__ = _change
 
     def __setattr__(self, key, value):
```

### Comparing `Missing-4.2/src/Missing.egg-info/PKG-INFO` & `Missing-5.0/src/Missing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: Missing
-Version: 4.2
+Version: 5.0
 Summary: Special Missing objects used in Zope.
 Home-page: https://github.com/zopefoundation/Missing
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Missing/issues
 Project-URL: Sources, https://github.com/zopefoundation/Missing
 Keywords: zope missing object
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Zope :: 4
+Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 .. image:: https://github.com/zopefoundation/Missing/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/Missing/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/Missing/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/Missing?branch=master
@@ -49,14 +45,23 @@
 
 Missing provides special objects used in some Zope internals like the ZCatalog.
 
 
 Changelog
 =========
 
+5.0 (2023-06-21)
+----------------
+
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Deprecate ``._Missing`` which containes just BBB imports.
+
+
 4.2 (2022-11-16)
 ----------------
 
 - Add support for Python 3.8, 3.9, 3.10, 3.11
 
 
 4.1 (2018-10-05)
```

### Comparing `Missing-4.2/tox.ini` & `Missing-5.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
     py311
-    pypy
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
 deps =
     zope.testrunner
@@ -38,37 +34,36 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
     zope.testrunner
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=88
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = Missing
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

