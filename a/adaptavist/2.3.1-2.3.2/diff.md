# Comparing `tmp/adaptavist-2.3.1.tar.gz` & `tmp/adaptavist-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptavist-2.3.1.tar", last modified: Fri Dec  2 07:39:10 2022, max compression
+gzip compressed data, was "adaptavist-2.3.2.tar", last modified: Wed Jun 21 15:23:48 2023, max compression
```

## Comparing `adaptavist-2.3.1.tar` & `adaptavist-2.3.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.567317 adaptavist-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-12-02 07:38:55.000000 adaptavist-2.3.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)       71 2022-12-02 07:38:55.000000 adaptavist-2.3.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.559317 adaptavist-2.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.563317 adaptavist-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2022-12-02 07:38:55.000000 adaptavist-2.3.1/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (122)      590 2022-12-02 07:38:55.000000 adaptavist-2.3.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1818 2022-12-02 07:38:55.000000 adaptavist-2.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      332 2022-12-02 07:38:55.000000 adaptavist-2.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-12-02 07:38:55.000000 adaptavist-2.3.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2022-12-02 07:38:55.000000 adaptavist-2.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2022-12-02 07:38:55.000000 adaptavist-2.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     3088 2022-12-02 07:39:10.567317 adaptavist-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2022-12-02 07:38:55.000000 adaptavist-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.563317 adaptavist-2.3.1/adaptavist/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2022-12-02 07:38:55.000000 adaptavist-2.3.1/adaptavist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2022-12-02 07:38:55.000000 adaptavist-2.3.1/adaptavist/_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    51117 2022-12-02 07:38:55.000000 adaptavist-2.3.1/adaptavist/adaptavist.py
--rw-r--r--   0 runner    (1001) docker     (122)      494 2022-12-02 07:38:55.000000 adaptavist-2.3.1/adaptavist/const.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 07:38:55.000000 adaptavist-2.3.1/adaptavist/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.563317 adaptavist-2.3.1/adaptavist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3088 2022-12-02 07:39:10.000000 adaptavist-2.3.1/adaptavist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2022-12-02 07:39:10.000000 adaptavist-2.3.1/adaptavist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 07:39:10.000000 adaptavist-2.3.1/adaptavist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-12-02 07:39:10.000000 adaptavist-2.3.1/adaptavist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-12-02 07:39:10.000000 adaptavist-2.3.1/adaptavist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.563317 adaptavist-2.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2022-12-02 07:38:55.000000 adaptavist-2.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.563317 adaptavist-2.3.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2022-12-02 07:38:55.000000 adaptavist-2.3.1/docs/_templates/docs-navbar.html
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-12-02 07:38:55.000000 adaptavist-2.3.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2022-12-02 07:38:55.000000 adaptavist-2.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-12-02 07:38:55.000000 adaptavist-2.3.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.563317 adaptavist-2.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)      465 2022-12-02 07:38:55.000000 adaptavist-2.3.1/docs/source/adaptavist.rst
--rw-r--r--   0 runner    (1001) docker     (122)      213 2022-12-02 07:38:55.000000 adaptavist-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 07:39:10.567317 adaptavist-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2022-12-02 07:38:55.000000 adaptavist-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.563317 adaptavist-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 07:39:10.567317 adaptavist-2.3.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/create_environment.json
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/create_folder.json
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/create_test_case.json
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/create_test_plan.json
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/create_test_result.json
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/create_test_results.json
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/create_test_run.json
--rw-r--r--   0 runner    (1001) docker     (122)      263 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_environments.json
--rw-r--r--   0 runner    (1001) docker     (122)      352 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_folders.json
--rw-r--r--   0 runner    (1001) docker     (122)       91 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_projects.json
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_case.json
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_case_links.json
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_cases.json
--rw-r--r--   0 runner    (1001) docker     (122)      857 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_execution_results.json
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_plan.json
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_plans.json
--rw-r--r--   0 runner    (1001) docker     (122)      322 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_result_attachments.json
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_results.json
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_run.json
--rw-r--r--   0 runner    (1001) docker     (122)      869 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_run_by_name.json
--rw-r--r--   0 runner    (1001) docker     (122)      971 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_test_runs.json
--rw-r--r--   0 runner    (1001) docker     (122)       42 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/fixtures/get_users.json
--rw-r--r--   0 runner    (1001) docker     (122)    37770 2022-12-02 07:38:55.000000 adaptavist-2.3.1/tests/test_adaptavist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.034875 adaptavist-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.022875 adaptavist-2.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.022875 adaptavist-2.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 15:23:29.000000 adaptavist-2.3.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-21 15:23:29.000000 adaptavist-2.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 15:23:29.000000 adaptavist-2.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-21 15:23:48.034875 adaptavist-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-21 15:23:29.000000 adaptavist-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.022875 adaptavist-2.3.2/adaptavist/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-21 15:23:29.000000 adaptavist-2.3.2/adaptavist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-21 15:23:29.000000 adaptavist-2.3.2/adaptavist/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51288 2023-06-21 15:23:29.000000 adaptavist-2.3.2/adaptavist/adaptavist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 15:23:29.000000 adaptavist-2.3.2/adaptavist/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:29.000000 adaptavist-2.3.2/adaptavist/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.026875 adaptavist-2.3.2/adaptavist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-21 15:23:47.000000 adaptavist-2.3.2/adaptavist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-21 15:23:48.000000 adaptavist-2.3.2/adaptavist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:23:47.000000 adaptavist-2.3.2/adaptavist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 15:23:47.000000 adaptavist-2.3.2/adaptavist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 15:23:47.000000 adaptavist-2.3.2/adaptavist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.026875 adaptavist-2.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 15:23:29.000000 adaptavist-2.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.026875 adaptavist-2.3.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-21 15:23:29.000000 adaptavist-2.3.2/docs/_templates/docs-navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 15:23:29.000000 adaptavist-2.3.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-21 15:23:29.000000 adaptavist-2.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 15:23:29.000000 adaptavist-2.3.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.026875 adaptavist-2.3.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-21 15:23:29.000000 adaptavist-2.3.2/docs/source/adaptavist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 15:23:29.000000 adaptavist-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:23:48.034875 adaptavist-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-21 15:23:29.000000 adaptavist-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.026875 adaptavist-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:23:48.034875 adaptavist-2.3.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/create_environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/create_folder.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/create_test_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/create_test_plan.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/create_test_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/create_test_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/create_test_run.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_environments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_folders.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_projects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_case_links.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_execution_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_plan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_plans.json
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_result_attachments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_run.json
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_run_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_test_runs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/fixtures/get_users.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37884 2023-06-21 15:23:29.000000 adaptavist-2.3.2/tests/test_adaptavist.py
```

### Comparing `adaptavist-2.3.1/.github/workflows/pythonpackage.yml` & `adaptavist-2.3.2/.github/workflows/pythonpackage.yml`

 * *Files 11% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 jobs:
 
   format:
     name: Check formatting
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3
+      uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: 3.8
     - name: Check formatting
       uses: pre-commit/action@v3.0.0
 
   lint:
     name: Lint
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3
+      uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: 3.8
     - name: Lint with flake8
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8
         flake8 adaptavist --count --show-source --statistics --max-line-length 160
@@ -40,25 +40,44 @@
         pylint --errors-only --score=n adaptavist
         pylint --exit-zero --score=n --disable=C,E,R --enable=useless-suppression adaptavist
     - name: Lint with mypy
       run: |
         python -m pip install mypy types-requests
         mypy --ignore-missing-imports adaptavist
 
+  test36:
+    name: Test with Python 3.6
+    runs-on: ubuntu-20.04
+    steps:
+    - name: Checkout sources
+      uses: actions/checkout@v3.5.3
+    - name: Set up Python 3.6
+      uses: actions/setup-python@v4.6.1
+      with:
+        python-version: 3.6
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        python -m pip install pytest-cov
+        python -m pip install .[test]
+    - name: Test with pytest
+      run: |
+        pytest --cov=adaptavist
+
   test:
     name: Test with Python ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3
+      uses: actions/checkout@v3.5.3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest-cov
         python -m pip install .[test]
```

### Comparing `adaptavist-2.3.1/.github/workflows/pythonpublish.yml` & `adaptavist-2.3.2/.github/workflows/pythonpublish.yml`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [created]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build twine
     - name: Build and publish
```

### Comparing `adaptavist-2.3.1/.gitignore` & `adaptavist-2.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/CHANGELOG.md` & `adaptavist-2.3.2/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.3.2] - 2023/06/21
+
+### Fixed
+
+- Test cases without steps now work properly
+- get_test_result now gets the last test execution
+
 ## [2.3.1] - 2022/12/02
 
 ### Fixed
 
 - Use request sessions to reduce overhead
 
 ## [2.3.0] - 2022/09/16
```

### Comparing `adaptavist-2.3.1/LICENSE.md` & `adaptavist-2.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/PKG-INFO` & `adaptavist-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptavist
-Version: 2.3.1
+Version: 2.3.2
 Summary: python package providing functionality for Jira Test Management (tm4j)
 Home-page: https://github.com/devolo/adaptavist
 Author: Stephan Steinberg, Guido Schmitz, Markus Bong
 Author-email: guido.schmitz@devolo.de, markus.bong@devolo.de
 License: MIT
 Keywords: python adaptavist kanoah tm4j jira test testmanagement report
 Platform: any
```

### Comparing `adaptavist-2.3.1/README.md` & `adaptavist-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/adaptavist/_helper.py` & `adaptavist-2.3.2/adaptavist/_helper.py`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/adaptavist/adaptavist.py` & `adaptavist-2.3.2/adaptavist/adaptavist.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,15 +710,16 @@
         request_url = f"{self._adaptavist_api_url}/testrun/{test_run_key}/testresults"
         self._logger.debug("Getting all test results for run %s", test_run_key)
         request = self._get(request_url)
         if not request:
             return []
         results = request.json()
         for result in results:
-            result["scriptResults"] = sorted(result["scriptResults"], key=lambda result: result["index"])
+            if len(result["scriptResults"]) > 1:
+                result["scriptResults"] = sorted(result["scriptResults"], key=lambda result: result["index"])
         return results
 
     def create_test_results(
         self, test_run_key: str, results: List[Dict[str, Any]], exclude_existing_test_cases: bool = True, **kwargs: Any
     ) -> List[int]:
         """
         Create new test results for a given test run.
@@ -759,22 +760,28 @@
         self._logger.debug("Creating test results for run %s", test_run_key)
         request = self._post(request_url, request_data)
 
         return [result["id"] for result in request.json()] if request else []
 
     def get_test_result(self, test_run_key: str, test_case_key: str) -> Dict[str, Any]:
         """
-        Get the test result for a given test run and test case.
+        Get the last test result for a given test run and test case.
 
         :param test_run_key: Test run key of the result to be updated. ex. "JQA-R1234"
         :param test_case_key: Test case key of the result to be updated. ex. "JQA-T1234"
         :returns: Test result
         """
         response = self.get_test_results(test_run_key)
-        return next((item for item in response if item["testCaseKey"] == test_case_key), {})
+        return (
+            max(
+                (item for item in response if item["testCaseKey"] == test_case_key),
+                key=lambda item: item["id"],
+            )
+            or {}
+        )
 
     def create_test_result(
         self, test_run_key: str, test_case_key: str, status: str = STATUS_NOT_EXECUTED, **kwargs: Any
     ) -> Optional[int]:
         """
         Create a new test result for a given test run and test case with the given status.
```

### Comparing `adaptavist-2.3.1/adaptavist.egg-info/PKG-INFO` & `adaptavist-2.3.2/adaptavist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptavist
-Version: 2.3.1
+Version: 2.3.2
 Summary: python package providing functionality for Jira Test Management (tm4j)
 Home-page: https://github.com/devolo/adaptavist
 Author: Stephan Steinberg, Guido Schmitz, Markus Bong
 Author-email: guido.schmitz@devolo.de, markus.bong@devolo.de
 License: MIT
 Keywords: python adaptavist kanoah tm4j jira test testmanagement report
 Platform: any
```

### Comparing `adaptavist-2.3.1/adaptavist.egg-info/SOURCES.txt` & `adaptavist-2.3.2/adaptavist.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGELOG.md
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
+.github/dependabot.yml
 .github/workflows/pythonpackage.yml
 .github/workflows/pythonpublish.yml
 adaptavist/__init__.py
 adaptavist/_helper.py
 adaptavist/adaptavist.py
 adaptavist/const.py
 adaptavist/py.typed
```

### Comparing `adaptavist-2.3.1/docs/Makefile` & `adaptavist-2.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/docs/_templates/docs-navbar.html` & `adaptavist-2.3.2/docs/_templates/docs-navbar.html`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/docs/conf.py` & `adaptavist-2.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/setup.py` & `adaptavist-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_case.json` & `adaptavist-2.3.2/tests/fixtures/get_test_case.json`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_case_links.json` & `adaptavist-2.3.2/tests/fixtures/get_test_case_links.json`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_cases.json` & `adaptavist-2.3.2/tests/fixtures/get_test_cases.json`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_execution_results.json` & `adaptavist-2.3.2/tests/fixtures/get_test_execution_results.json`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_plan.json` & `adaptavist-2.3.2/tests/fixtures/get_test_plan.json`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_plans.json` & `adaptavist-2.3.2/tests/fixtures/get_test_plans.json`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_results.json` & `adaptavist-2.3.2/tests/fixtures/get_test_run.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('executionResultsSummary', OrderedDict([('Pass', 1), ('Fail', 1)])), "*

 * *            "('key', 'JQA-R123'), ('projectKey', 'JQA'), ('name', 'Full regression'), ('status', "*

 * *            "'Done'), ('iteration', 'Sprint 1'), ('folder', '/root folder/child folder'), "*

 * *            "('version', '1.1.0'), ('issueKey', 'JQA-123'), ('owner', 'admin'), "*

 * *            "('plannedStartDate', '2016-02-24T08:10:59.514Z'), ('plannedEndDate', "*

 * *            "'2016-02-26T12:00:00.000Z'), ('estimatedTime […]*

```diff
@@ -1,35 +1,48 @@
-[
-    {
-        "actualEndDate": "2016-02-14T19:22:00-0300",
-        "actualStartDate": "2016-02-12T19:22:00-0300",
-        "assignedTo": "cristiano.caetano",
-        "automated": true,
-        "comment": "The test has failed on some automation tool procedure.",
-        "customFields": {
-            "CI Server": "Bamboo"
+{
+    "estimatedTime": 2338000,
+    "executionResultsSummary": {
+        "Fail": 1,
+        "Pass": 1
+    },
+    "executionTime": 150000,
+    "folder": "/root folder/child folder",
+    "issueCount": 1,
+    "issueKey": "JQA-123",
+    "items": [
+        {
+            "actualEndDate": "2016-02-14T19:22:00-0300",
+            "actualStartDate": "2016-02-12T19:22:00-0300",
+            "assignedTo": "cristiano.caetano",
+            "customFields": {
+                "multichoice": "Brazil, England",
+                "single choice": "Propulsion engines"
+            },
+            "environment": "Chrome",
+            "executedBy": "vitor.pelizza",
+            "executionDate": "2017-05-16T16:42:06.000Z",
+            "id": 500020,
+            "plannedEndDate": "2016-02-12T19:22:00-0300",
+            "plannedStartDate": "2016-02-10T19:22:00-0300",
+            "status": "Fail",
+            "testCaseKey": "JQA-T123",
+            "userKey": "vitor.pelizza"
         },
-        "environment": "Firefox",
-        "executedBy": "vitor.pelizza",
-        "executionDate": "2016-02-14T19:22:00-0300",
-        "executionTime": 180000,
-        "id": 500020,
-        "issueLinks": [
-            "JQA-123",
-            "JQA-456"
-        ],
-        "iteration": "Sprint 1",
-        "plannedEndDate": "2016-02-12T19:22:00-0300",
-        "plannedStartDate": "2016-02-10T19:22:00-0300",
-        "scriptResults": [
-            {
-                "comment": "This step has failed.",
-                "index": 0,
-                "status": "Fail"
-            }
-        ],
-        "status": "Fail",
-        "testCaseKey": "JQA-T123",
-        "userKey": "vitor.pelizza",
-        "version": "1.1.0"
-    }
-]
+        {
+            "environment": "Firefox",
+            "executionDate": "2017-05-16T16:31:28.000Z",
+            "id": 500021,
+            "status": "Pass",
+            "testCaseKey": "JQA-T456"
+        }
+    ],
+    "iteration": "Sprint 1",
+    "key": "JQA-R123",
+    "name": "Full regression",
+    "owner": "admin",
+    "plannedEndDate": "2016-02-26T12:00:00.000Z",
+    "plannedStartDate": "2016-02-24T08:10:59.514Z",
+    "projectKey": "JQA",
+    "status": "Done",
+    "testCaseCount": 2,
+    "version": "1.1.0"
+}
```

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_run.json` & `adaptavist-2.3.2/tests/fixtures/get_test_runs.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

```diff
@@ -1,48 +1,33 @@
-{
-    "estimatedTime": 2338000,
-    "executionResultsSummary": {
-        "Fail": 1,
-        "Pass": 1
-    },
-    "executionTime": 150000,
-    "folder": "/root folder/child folder",
-    "issueCount": 1,
-    "issueKey": "JQA-123",
-    "items": [
-        {
-            "actualEndDate": "2016-02-14T19:22:00-0300",
-            "actualStartDate": "2016-02-12T19:22:00-0300",
-            "assignedTo": "cristiano.caetano",
-            "customFields": {
-                "multichoice": "Brazil, England",
-                "single choice": "Propulsion engines"
+[
+    {
+        "estimatedTime": 2338000,
+        "executionTime": 150000,
+        "folder": "/root folder/child folder",
+        "issueCount": 1,
+        "issueKey": "JQA-123",
+        "items": [
+            {
+                "customFields": {
+                    "multichoice": "Brazil, England",
+                    "single choice": "Propulsion engines"
+                },
+                "environment": "Chrome",
+                "testCaseKey": "JQA-T123",
+                "userKey": "vitor.pelizza"
             },
-            "environment": "Chrome",
-            "executedBy": "vitor.pelizza",
-            "executionDate": "2017-05-16T16:42:06.000Z",
-            "id": 500020,
-            "plannedEndDate": "2016-02-12T19:22:00-0300",
-            "plannedStartDate": "2016-02-10T19:22:00-0300",
-            "status": "Fail",
-            "testCaseKey": "JQA-T123",
-            "userKey": "vitor.pelizza"
-        },
-        {
-            "environment": "Firefox",
-            "executionDate": "2017-05-16T16:31:28.000Z",
-            "id": 500021,
-            "status": "Pass",
-            "testCaseKey": "JQA-T456"
-        }
-    ],
-    "iteration": "Sprint 1",
-    "key": "JQA-R123",
-    "name": "Full regression",
-    "owner": "admin",
-    "plannedEndDate": "2016-02-26T12:00:00.000Z",
-    "plannedStartDate": "2016-02-24T08:10:59.514Z",
-    "projectKey": "JQA",
-    "status": "Done",
-    "testCaseCount": 2,
-    "version": "1.1.0"
-}
+            {
+                "environment": "Firefox",
+                "testCaseKey": "JQA-T456"
+            }
+        ],
+        "iteration": "Sprint 1",
+        "key": "JQA-R123",
+        "name": "Full regression",
+        "plannedEndDate": "2016-02-26T12:00:00.000Z",
+        "plannedStartDate": "2016-02-24T08:10:59.514Z",
+        "projectKey": "JQA",
+        "status": "In Progress",
+        "testCaseCount": 2,
+        "version": "1.1.0"
+    }
+]
```

### Comparing `adaptavist-2.3.1/tests/fixtures/get_test_run_by_name.json` & `adaptavist-2.3.2/tests/fixtures/get_test_run_by_name.json`

 * *Files identical despite different names*

### Comparing `adaptavist-2.3.1/tests/test_adaptavist.py` & `adaptavist-2.3.2/tests/test_adaptavist.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from adaptavist import Adaptavist
 from adaptavist.const import STATUS_FAIL, STATUS_PASS
 
 from . import load_fixture
 
 
 class TestAdaptavist:
+    """Test the Adaptavist module."""
 
     _jira_url = "mock://jira"
     _adaptavist_api_url = f"{_jira_url}/rest/atm/1.0"
 
     def test_get_users(self, requests_mock: Mocker):
         """Test getting all users."""
         requests_mock.get(
@@ -410,15 +411,16 @@
         """Test getting test results of a test run."""
         requests_mock.get(
             f"{TestAdaptavist._adaptavist_api_url}/testrun/JQA-T123/testresults", text=load_fixture("get_test_results.json")
         )
         adaptavist = Adaptavist(jira_server=TestAdaptavist._jira_url, jira_username="User", jira_password="Password")
 
         results = adaptavist.get_test_results(test_run_key="JQA-T123")
-        assert results[0]["testCaseKey"] == "JQA-T123"
+        assert len(results) == 5
+        assert results[1]["testCaseKey"] == "JQA-T123"
 
     def test_create_test_results(self, requests_mock: Mocker):
         """Test creating test results."""
         requests_mock.post(
             f"{TestAdaptavist._adaptavist_api_url}/testrun/JQA-R123/testresults", text=load_fixture("create_test_results.json")
         )
         adaptavist = Adaptavist(jira_server=TestAdaptavist._jira_url, jira_username="User", jira_password="Password")
@@ -441,14 +443,15 @@
     def test_get_test_result(self):
         """Test getting a test result of a test run."""
         adaptavist = Adaptavist(jira_server=TestAdaptavist._jira_url, jira_username="User", jira_password="Password")
 
         with patch("adaptavist.Adaptavist.get_test_results", return_value=json.loads(load_fixture("get_test_results.json"))):
             result = adaptavist.get_test_result(test_run_key="JQA-R123", test_case_key="JQA-T123")
             assert result["testCaseKey"] == "JQA-T123"
+            assert result["id"] == 2321153
 
     def test_create_test_result(self, requests_mock: Mocker):
         """Test creating a test result."""
         requests_mock.post(
             f"{TestAdaptavist._adaptavist_api_url}/testrun/JQA-R123/testcase/JQA-T123/testresult",
             text=load_fixture("create_test_result.json"),
         )
```

