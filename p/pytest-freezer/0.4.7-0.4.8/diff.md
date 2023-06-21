# Comparing `tmp/pytest_freezer-0.4.7.tar.gz` & `tmp/pytest_freezer-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pytest_freezer-0.4.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_freezer-0.4.7.tar` & `pytest_freezer-0.4.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pytest_freezer-0.4.7/pytest_freezer.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pytest_freezer-0.4.7/tests/conftest.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 pytest_freezer-0.4.7/tests/test_plugin.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pytest_freezer-0.4.7/LICENSE
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pytest_freezer-0.4.7/README.rst
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pytest_freezer-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 pytest_freezer-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-10-18 03:43:44.601323 pytest_freezer-0.4.8/LICENSE
+-rw-r--r--   0        0        0     1940 2022-10-18 06:11:30.005452 pytest_freezer-0.4.8/README.rst
+-rw-r--r--   0        0        0      677 2023-06-21 05:31:03.457245 pytest_freezer-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      751 2022-10-20 01:22:35.328880 pytest_freezer-0.4.8/pytest_freezer.py
+-rw-r--r--   0        0        0       30 2022-10-18 03:41:25.768417 pytest_freezer-0.4.8/tests/conftest.py
+-rw-r--r--   0        0        0     2761 2022-10-20 01:41:40.446693 pytest_freezer-0.4.8/tests/test_plugin.py
+-rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 pytest_freezer-0.4.8/PKG-INFO
```

### Comparing `pytest_freezer-0.4.7/pytest_freezer.py` & `pytest_freezer-0.4.8/pytest_freezer.py`

 * *Files identical despite different names*

### Comparing `pytest_freezer-0.4.7/tests/test_plugin.py` & `pytest_freezer-0.4.8/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_freezer-0.4.7/LICENSE` & `pytest_freezer-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_freezer-0.4.7/README.rst` & `pytest_freezer-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_freezer-0.4.7/pyproject.toml` & `pytest_freezer-0.4.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
 [project]
 name = "pytest_freezer"
 authors = [{name = "Wim Glenn", email = "hey@wimglenn.com"}]
-license = "MIT"
+license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Framework :: Pytest",
 ]
-version = "0.4.7"
+version = "0.4.8"
 dependencies = ["pytest >= 3.6", "freezegun >= 1.0"]
 requires-python = ">= 3.6"
 readme = "README.rst"
 description = "Pytest plugin providing a fixture interface for spulec/freezegun"
 
 [project.urls]
 Homepage = "https://github.com/pytest-dev/pytest-freezer"
 
 [project.entry-points.pytest11]
 freezer = "pytest_freezer"
 
-[tool.hatch.build]
-include = [
-    "LICENSE",
-    "README.rst",
-    "pyproject.toml",
-    "pytest_freezer.py",
-    "/tests",
-]
-exclude = [
-    ".coverage",
-    ".idea",
-    ".pytest_cache",
-    ".venv",
-]
+[tool.flit.sdist]
+include = ["tests/"]
```

### Comparing `pytest_freezer-0.4.7/PKG-INFO` & `pytest_freezer-0.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: pytest_freezer
-Version: 0.4.7
+Version: 0.4.8
 Summary: Pytest plugin providing a fixture interface for spulec/freezegun
-Project-URL: Homepage, https://github.com/pytest-dev/pytest-freezer
 Author-email: Wim Glenn <hey@wimglenn.com>
-License-Expression: MIT
-License-File: LICENSE
-Classifier: Framework :: Pytest
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Requires-Dist: freezegun>=1.0
-Requires-Dist: pytest>=3.6
+Requires-Python: >= 3.6
 Description-Content-Type: text/x-rst
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Framework :: Pytest
+Requires-Dist: pytest >= 3.6
+Requires-Dist: freezegun >= 1.0
+Project-URL: Homepage, https://github.com/pytest-dev/pytest-freezer
 
 |actions|_ |codecov|_ |pypi|_ |womm|_
 
 .. |actions| image:: https://github.com/pytest-dev/pytest-freezer/actions/workflows/tests.yml/badge.svg
 .. _actions: https://github.com/pytest-dev/pytest-freezer/actions/workflows/tests.yml/
 
 .. |codecov| image:: https://codecov.io/gh/pytest-dev/pytest-freezer/branch/main/graph/badge.svg
@@ -72,7 +70,8 @@
 
 Credit to Tomasz Kontusz for the original pytest-freezegun_ plugin.
 
 .. _Pytest: https://docs.pytest.org/
 .. _freezegun: https://github.com/spulec/freezegun
 .. _pytest-freezegun: https://github.com/ktosiek/pytest-freezegun
 .. _usage: https://github.com/spulec/freezegun#usage
+
```

