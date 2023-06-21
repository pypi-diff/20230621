# Comparing `tmp/hera_cli_utils-0.0.1.tar.gz` & `tmp/hera_cli_utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_cli_utils-0.0.1.tar", max compression
+gzip compressed data, was "hera_cli_utils-0.1.0.tar", max compression
```

## Comparing `hera_cli_utils-0.0.1.tar` & `hera_cli_utils-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-15 22:45:11.544617 hera_cli_utils-0.0.1/LICENSE
--rw-r--r--   0        0        0     2444 2023-06-15 22:45:11.524617 hera_cli_utils-0.0.1/README.md
--rw-r--r--   0        0        0     2687 2023-06-20 01:59:48.322848 hera_cli_utils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     9486 2023-06-20 01:48:38.248902 hera_cli_utils-0.0.1/src/hera_cli_utils/__init__.py
--rw-r--r--   0        0        0      207 2023-06-15 23:07:41.824032 hera_cli_utils-0.0.1/src/hera_cli_utils/__main__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:45:11.554617 hera_cli_utils-0.0.1/src/hera_cli_utils/py.typed
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 hera_cli_utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-21 05:03:06.812186 hera_cli_utils-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2444 2023-06-21 05:03:06.812186 hera_cli_utils-0.1.0/README.md
+-rw-r--r--   0        0        0     2703 2023-06-21 05:03:23.093540 hera_cli_utils-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5592 2023-06-21 05:03:23.093540 hera_cli_utils-0.1.0/src/hera_cli_utils/__init__.py
+-rw-r--r--   0        0        0    13193 2023-06-21 05:03:23.093540 hera_cli_utils-0.1.0/src/hera_cli_utils/logging.py
+-rw-r--r--   0        0        0     3108 2023-06-21 05:03:23.093540 hera_cli_utils-0.1.0/src/hera_cli_utils/profiling.py
+-rw-r--r--   0        0        0        0 2023-06-21 05:03:06.812186 hera_cli_utils-0.1.0/src/hera_cli_utils/py.typed
+-rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 hera_cli_utils-0.1.0/setup.py
+-rw-r--r--   0        0        0     3502 1970-01-01 00:00:00.000000 hera_cli_utils-0.1.0/PKG-INFO
```

### Comparing `hera_cli_utils-0.0.1/LICENSE` & `hera_cli_utils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hera_cli_utils-0.0.1/README.md` & `hera_cli_utils-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hera_cli_utils-0.0.1/pyproject.toml` & `hera_cli_utils-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hera-cli-utils"
-version = "0.0.1"
+version = "0.1.0"
 description = "HERA CLI Utils"
 authors = ["Steven Murray <steven.g.murray@asu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/steven-murray/hera-cli-utils"
 repository = "https://github.com/steven-murray/hera-cli-utils"
 documentation = "https://hera-cli-utils.readthedocs.io"
@@ -16,14 +16,15 @@
 Changelog = "https://github.com/steven-murray/hera-cli-utils/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=8.0.1"
 rich = "^13.4.2"
 psutil = "^5.9.5"
+line-profiler = "^4.0.3"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
@@ -56,15 +57,15 @@
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
-source = ["hera_cli_utils", "tests"]
+source = ["hera_cli_utils"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 100
 
 [tool.isort]
 profile = "black"
```

### Comparing `hera_cli_utils-0.0.1/PKG-INFO` & `hera_cli_utils-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera-cli-utils
-Version: 0.0.1
+Version: 0.1.0
 Summary: HERA CLI Utils
 Home-page: https://github.com/steven-murray/hera-cli-utils
 License: MIT
 Author: Steven Murray
 Author-email: steven.g.murray@asu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1)
+Requires-Dist: line-profiler (>=4.0.3,<5.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Changelog, https://github.com/steven-murray/hera-cli-utils/releases
 Project-URL: Documentation, https://hera-cli-utils.readthedocs.io
 Project-URL: Repository, https://github.com/steven-murray/hera-cli-utils
 Description-Content-Type: text/markdown
```

