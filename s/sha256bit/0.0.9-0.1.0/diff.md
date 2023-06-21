# Comparing `tmp/sha256bit-0.0.9.tar.gz` & `tmp/sha256bit-0.1.0.tar.gz`

## Comparing `sha256bit-0.0.9.tar` & `sha256bit-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,32 @@
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 sha256bit-0.0.9/build
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sha256bit-0.0.9/requirements.txt
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sha256bit-0.0.9/.github/workflows/build.yml
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 sha256bit-0.0.9/.github/workflows/test.yml
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 sha256bit-0.0.9/sha256bit/__init__.py
--rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/SHA256LongMsg.rsp
--rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/SHA256ShortMsg.rsp
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/__init__.py
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_api.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_cavp.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_hardcoded.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sha256bit-0.0.9/test/test_vs_hashlib.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.9/LICENSE
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 sha256bit-0.0.9/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 sha256bit-0.0.9/hatch.toml
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 sha256bit-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 sha256bit-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 sha256bit-0.1.0/.readthedocs.yaml
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 sha256bit-0.1.0/build
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 sha256bit-0.1.0/lint
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sha256bit-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sha256bit-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 sha256bit-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/Pipfile
+-rw-r--r--   0        0        0    19370 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/Pipfile.lock
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/source/examples_python3.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 sha256bit-0.1.0/docs/source/installation.rst
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 sha256bit-0.1.0/sha256bit/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 sha256bit-0.1.0/sha256bit/cli.py
+-rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/SHA256LongMsg.rsp
+-rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/SHA256ShortMsg.rsp
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/test.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/test_api.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/test_cavp.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/test_hardcoded.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sha256bit-0.1.0/test/test_vs_hashlib.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 sha256bit-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 sha256bit-0.1.0/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 sha256bit-0.1.0/hatch.toml
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 sha256bit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 sha256bit-0.1.0/PKG-INFO
```

### Comparing `sha256bit-0.0.9/.github/workflows/build.yml` & `sha256bit-0.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.9/.github/workflows/test.yml` & `sha256bit-0.1.0/.github/workflows/test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   FORCE_COLOR: "1"
 
 jobs:
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
-      fail-fast: false
+      fail-fast: true
       matrix:
       #  os: [ubuntu-latest, windows-latest, macos-latest]
         os: [ubuntu-latest]
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
@@ -42,8 +42,15 @@
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
 
     - if: matrix.python-version == '3.11' && runner.os == 'Linux'
       name: Lint
       run: hatch run lint:all
 
     - name: Run tests
-      run: hatch run cov
+      run: hatch run cov
+
+    - if: matrix.python-version == '3.11' && runner.os == 'Linux'
+      name: Doc
+      run: |
+        cd docs
+        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        make clean doctest html
```

### Comparing `sha256bit-0.0.9/test/SHA256LongMsg.rsp` & `sha256bit-0.1.0/test/SHA256LongMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.9/test/SHA256ShortMsg.rsp` & `sha256bit-0.1.0/test/SHA256ShortMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.9/.gitignore` & `sha256bit-0.1.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.vscode/settings.json
```

### Comparing `sha256bit-0.0.9/LICENSE` & `sha256bit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.9/hatch.toml` & `sha256bit-0.1.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.9/pyproject.toml` & `sha256bit-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -70,27 +70,30 @@
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
+exclude = ["docs"]
 
 [tool.ruff.isort]
 known-first-party = ["sha256bit"]
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use relative imports and assertions and print
 "test/**/*" = ["TID252", "S101", "T201"]
+# CLI can print
+"sha256bit/cli.py" = ["T201"]
 
 [tool.mypy]
 disallow_untyped_defs = false
 follow_imports = "normal"
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
```

### Comparing `sha256bit-0.0.9/PKG-INFO` & `sha256bit-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sha256bit
-Version: 0.0.9
+Version: 0.1.0
 Summary: SHA256 with bit granularity for message input length
 Project-URL: Homepage, https://github.com/sebastien-riou/sha256bit
 Project-URL: Bug Tracker, https://github.com/sebastien-riou/sha256bit/issues
 Author: Sebastien Riou
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,23 +22,25 @@
 Description-Content-Type: text/markdown
 
 # sha256bit
 
 
 | | |
 | --- | --- |
-| CI/CD | [![CI - Test](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml) [![CD - Build](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml) |
+| CI/CD | [![CI - Test](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/test.yml) [![CD - Build](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml/badge.svg)](https://github.com/sebastien-riou/sha256bit/actions/workflows/build.yml) [![Documentation Status](https://readthedocs.org/projects/sha256bit/badge/?version=latest)](https://sha256bit.readthedocs.io/en/latest/?badge=latest)|
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/sha256bit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/sha256bits/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sha256bit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/sha256bit/) |
-| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)  [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![License - apache-2.0](https://img.shields.io/badge/license-apache--2.0-blue)](https://spdx.org/licenses/) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)  [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![License - apache-2.0](https://img.shields.io/badge/license-apache--2.0-blue)](https://spdx.org/licenses/) |
 
 
 Pure python implementation of SHA256 with features which are often lacking:
 - bit granularity for message input length
 - import/export API to "persist" the state in the middle of a hash computation
 
+[User documentation](https://sha256bit.rtfd.io) is hosted on readthedocs.
+
 ## Installation
 
     python3 -m pip install sha256bit
 
 ## Usage
 
 ### One liner 
@@ -76,15 +78,35 @@
 you can also run each test separately:
 
     python3 -m test.test_api
     python3 -m test.test_cavp
     python3 -m test.test_hardcoded
     python3 -m test.test_vs_hashlib
 
+## Generate the doc
+
+    cd docs
+    pipenv shell
+    make clean doctest html
+
+## Update pipenv for the doc
+
+    cd docs
+    pipenv shell
+    #use pip to update whatever ou want
+    pip freeze > requirements.txt
+    pipenv update
+    
 ## Build the package
 Build is done using `hatchling`. The script `build` allows to build for different version of python3:
 
     ./build python3.9
 
 
 ## Create a new version
-Version is managed by `hatch-vcs`, you just need to create a tag in github. 
+Version is managed by `hatch-vcs`, you just need to create a tag in github. 
+
+## Launch linters
+They use the configuration from `pyproject.toml`
+
+    ./lint
+
```

