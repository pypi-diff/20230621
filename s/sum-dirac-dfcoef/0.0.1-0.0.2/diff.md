# Comparing `tmp/sum_dirac_dfcoef-0.0.1.tar.gz` & `tmp/sum_dirac_dfcoef-0.0.2.tar.gz`

## Comparing `sum_dirac_dfcoef-0.0.1.tar` & `sum_dirac_dfcoef-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/requirements.txt
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/src/sum_dirac_dfcoef/__about__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/src/sum_dirac_dfcoef/__init__.py
--rwxr-xr-x   0        0        0    20035 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/test/.gitignore
--rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/test/unit_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/test/results/.gitkeep
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/LICENSE
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/scripts/versionup.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/release-pr.yml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/reusable_test.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/__about__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/__init__.py
+-rwxr-xr-x   0        0        0    20035 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/test/.gitignore
+-rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/test/unit_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/test/results/.gitkeep
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/PKG-INFO
```

### Comparing `sum_dirac_dfcoef-0.0.1/.github/workflows/build.yml` & `sum_dirac_dfcoef-0.0.2/.github/workflows/reusable_test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-name: pymolecule-parser-build
+name: reusable_test
 
 on:
-  push:
-    tags:
-      - v*
-    branches: [main]
-  workflow_dispatch:
+  workflow_call:
 
+# Ref : https://github.com/pytest-dev/pytest/issues/7443#issue-650484842
+env:
+  PYTEST_ADDOPTS: "--color=yes"
+
+defaults:
+  run:
+    shell: bash
 jobs:
-  test:
-    uses: ./.github/workflows/ci.yml
-  build:
-    needs: test
+  test-linux:
+    timeout-minutes: 10 # Max execution time (min)
     runs-on: ubuntu-latest
-    timeout-minutes: 10
+    strategy:
+      matrix:
+        python-version: ["3.7", "3.8", "3.9", "3.10"]
     steps:
       - uses: actions/checkout@v3
-      - name: Set up Python 3.10
-        uses: actions/setup-python@v2
+      - name: Install python
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: ${{ matrix.python-version }}
+          architecture: "x64"
       - name: Install dependencies
+        run: python -m pip install -r requirements.txt
+      - name: Run unittest
         run: |
-          python -m pip install --upgrade pip
-          python -m pip install hatch twine
-      - name: Build
-        run: hatch build
-      - name: Publish
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          pytest
```

### Comparing `sum_dirac_dfcoef-0.0.1/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py` & `sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.1/test/unit_test.py` & `sum_dirac_dfcoef-0.0.2/test/unit_test.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.1/.gitignore` & `sum_dirac_dfcoef-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.1/LICENSE` & `sum_dirac_dfcoef-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.1/README.md` & `sum_dirac_dfcoef-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sum_dirac_dfcoef : SUMMARIZE DIRAC DFCOEF COEFFICIENTS
 
-[![summarize_dirac_coefficients_test](https://github.com/kohei-noda-qcrg/summarize_dirac_dfcoef_coefficients/actions/workflows/ci.yml/badge.svg)](https://github.com/kohei-noda-qcrg/summarize_dirac_dfcoef_coefficients/actions/workflows/ci.yml)
+[![sum_dirac_dfcoef_test](https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/actions/workflows/test.yml/badge.svg)](https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/actions/workflows/test.yml)
 
 This program provides a utility to summarize the contribution of each atomic orbital per molecular orbital from the [DIRAC](http://diracprogram.org/doku.php) output file that the [*PRIVEC and .VECPRI options](http://www.diracprogram.org/doc/release-22/manual/analyze/privec.html) are used.
 
 ## Requirements
 
 - [Python](https://python.org) (version ≧ 3.6)
   - If you don't know how to install python, I recommend you to use [pyenv](https://github.com/pyenv/pyenv)
```

### Comparing `sum_dirac_dfcoef-0.0.1/pyproject.toml` & `sum_dirac_dfcoef-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.1/PKG-INFO` & `sum_dirac_dfcoef-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sum_dirac_dfcoef
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a utility to summarize the contribution of each atomic orbital per molecular orbital from the DIRAC output file that the *PRIVEC and .VECPRI options are used.
 Project-URL: Documentation, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef#readme
 Project-URL: Issues, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/issues
 Project-URL: Source, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef
 Author-email: Kohei Noda <kohei-noda@hiroshima-u.ac.jp>
 License-Expression: MIT
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Requires-Dist: pymolecule-parser
 Description-Content-Type: text/markdown
 
 # sum_dirac_dfcoef : SUMMARIZE DIRAC DFCOEF COEFFICIENTS
 
-[![summarize_dirac_coefficients_test](https://github.com/kohei-noda-qcrg/summarize_dirac_dfcoef_coefficients/actions/workflows/ci.yml/badge.svg)](https://github.com/kohei-noda-qcrg/summarize_dirac_dfcoef_coefficients/actions/workflows/ci.yml)
+[![sum_dirac_dfcoef_test](https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/actions/workflows/test.yml/badge.svg)](https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/actions/workflows/test.yml)
 
 This program provides a utility to summarize the contribution of each atomic orbital per molecular orbital from the [DIRAC](http://diracprogram.org/doku.php) output file that the [*PRIVEC and .VECPRI options](http://www.diracprogram.org/doc/release-22/manual/analyze/privec.html) are used.
 
 ## Requirements
 
 - [Python](https://python.org) (version ≧ 3.6)
   - If you don't know how to install python, I recommend you to use [pyenv](https://github.com/pyenv/pyenv)
```

