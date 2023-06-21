# Comparing `tmp/citation_date-0.1.4.tar.gz` & `tmp/citation_date-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_date-0.1.4.tar", max compression
+gzip compressed data, was "citation_date-0.1.5.tar", max compression
```

## Comparing `citation_date-0.1.4.tar` & `citation_date-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1491 2023-05-15 16:21:45.737331 citation_date-0.1.4/LICENSE
--rw-r--r--   0        0        0      519 2023-05-15 16:15:08.545130 citation_date-0.1.4/README.md
--rw-r--r--   0        0        0      142 2023-05-15 16:22:09.884585 citation_date-0.1.4/citation_date/__init__.py
--rw-r--r--   0        0        0      164 2023-02-23 08:10:46.211794 citation_date-0.1.4/citation_date/base/__init__.py
--rw-r--r--   0        0        0      292 2022-10-13 00:31:37.797284 citation_date-0.1.4/citation_date/base/day.py
--rw-r--r--   0        0        0      338 2022-10-13 00:31:37.797429 citation_date-0.1.4/citation_date/base/month.py
--rw-r--r--   0        0        0     1568 2023-01-24 03:37:55.769600 citation_date-0.1.4/citation_date/base/report.py
--rw-r--r--   0        0        0     1249 2023-01-24 03:41:18.844828 citation_date-0.1.4/citation_date/base/us_uk.py
--rw-r--r--   0        0        0      475 2022-10-13 00:31:37.797893 citation_date-0.1.4/citation_date/base/year.py
--rw-r--r--   0        0        0     2995 2023-01-24 03:32:20.303154 citation_date-0.1.4/citation_date/decoder.py
--rw-r--r--   0        0        0     1665 2023-05-15 16:21:25.130477 citation_date-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 citation_date-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:10:18.765929 citation_date-0.1.5/LICENSE
+-rw-r--r--   0        0        0      519 2023-06-21 15:10:18.766016 citation_date-0.1.5/README.md
+-rw-r--r--   0        0        0      119 2023-06-21 15:13:27.970051 citation_date-0.1.5/citation_date/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-21 15:10:18.766286 citation_date-0.1.5/citation_date/base/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-21 15:14:47.893306 citation_date-0.1.5/citation_date/base/day.py
+-rw-r--r--   0        0        0      338 2023-06-21 15:10:18.766459 citation_date-0.1.5/citation_date/base/month.py
+-rw-r--r--   0        0        0     1568 2023-06-21 15:10:18.766568 citation_date-0.1.5/citation_date/base/report.py
+-rw-r--r--   0        0        0     1249 2023-06-21 15:10:18.766685 citation_date-0.1.5/citation_date/base/us_uk.py
+-rw-r--r--   0        0        0      475 2023-06-21 15:10:18.766766 citation_date-0.1.5/citation_date/base/year.py
+-rw-r--r--   0        0        0     2995 2023-06-21 15:14:39.390131 citation_date-0.1.5/citation_date/decoder.py
+-rw-r--r--   0        0        0     1650 2023-06-21 15:13:05.449000 citation_date-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 citation_date-0.1.5/PKG-INFO
```

### Comparing `citation_date-0.1.4/LICENSE` & `citation_date-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.4/README.md` & `citation_date-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.4/citation_date/base/report.py` & `citation_date-0.1.5/citation_date/base/report.py`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.4/citation_date/base/us_uk.py` & `citation_date-0.1.5/citation_date/base/us_uk.py`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.4/citation_date/decoder.py` & `citation_date-0.1.5/citation_date/decoder.py`

 * *Files identical despite different names*

### Comparing `citation_date-0.1.4/pyproject.toml` & `citation_date-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "citation-date"
-version = "0.1.4"
+version = "0.1.5"
 description = "Regex date formula and decoder - Philippine Supreme Court Decisions"
-authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
+authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
-license = "MIT"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-date"
 documentation = "https://justmars.github.io/citation-date"
 classifiers = [
   "Topic :: Text Processing :: General",
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
@@ -16,23 +15,23 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dateutil = "^2.8"
-types-python-dateutil = "^2.8.19"
 
 [tool.poetry.group.dev.dependencies]
+types-python-dateutil = "^2.8.19"
 pytest = "^7.2"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
-mkdocs = "^1.4.2"
-mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.1"
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material = "^9.1.15"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --cov --doctest-modules"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
```

### Comparing `citation_date-0.1.4/PKG-INFO` & `citation_date-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: citation-date
-Version: 0.1.4
+Version: 0.1.5
 Summary: Regex date formula and decoder - Philippine Supreme Court Decisions
 Home-page: https://lawsql.com
-License: MIT
 Author: Marcelino G. Veloso III
-Author-email: mars@veloso.one
+Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
 Requires-Dist: python-dateutil (>=2.8,<3.0)
-Requires-Dist: types-python-dateutil (>=2.8.19,<3.0.0)
 Project-URL: Documentation, https://justmars.github.io/citation-date
 Project-URL: Repository, https://github.com/justmars/citation-date
 Description-Content-Type: text/markdown
 
 # citation-date
 
 ![Github CI](https://github.com/justmars/citation-date/actions/workflows/main.yml/badge.svg)
```

