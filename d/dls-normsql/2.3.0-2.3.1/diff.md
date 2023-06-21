# Comparing `tmp/dls-normsql-2.3.0.tar.gz` & `tmp/dls-normsql-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-normsql-2.3.0.tar", last modified: Wed Jun  7 14:07:38 2023, max compression
+gzip compressed data, was "dls-normsql-2.3.1.tar", last modified: Wed Jun 21 12:11:44 2023, max compression
```

## Comparing `dls-normsql-2.3.0.tar` & `dls-normsql-2.3.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.670619 dls-normsql-2.3.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.678619 dls-normsql-2.3.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.670619 dls-normsql-2.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.682618 dls-normsql-2.3.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.686619 dls-normsql-2.3.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.670619 dls-normsql-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.690619 dls-normsql-2.3.0/src/dls_normsql/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/src/dls_normsql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.690619 dls-normsql-2.3.0/src/dls_normsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 14:07:38.000000 dls-normsql-2.3.0/src/dls_normsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:38.694619 dls-normsql-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/my_database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/my_table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_backup_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-07 14:07:27.000000 dls-normsql-2.3.0/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.888669 dls-normsql-2.3.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.888669 dls-normsql-2.3.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.892669 dls-normsql-2.3.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.888669 dls-normsql-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/src/dls_normsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 12:11:44.000000 dls-normsql-2.3.1/src/dls_normsql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22130 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/src/dls_normsql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/src/dls_normsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-06-21 12:11:44.000000 dls-normsql-2.3.1/src/dls_normsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-21 12:11:44.000000 dls-normsql-2.3.1/src/dls_normsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:11:44.000000 dls-normsql-2.3.1/src/dls_normsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 12:11:44.000000 dls-normsql-2.3.1/src/dls_normsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-21 12:11:44.000000 dls-normsql-2.3.1/src/dls_normsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 12:11:44.000000 dls-normsql-2.3.1/src/dls_normsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:44.896669 dls-normsql-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/my_database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/my_table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/test_aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/test_backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-21 12:11:35.000000 dls-normsql-2.3.1/tests/test_revision.py
```

### Comparing `dls-normsql-2.3.0/.dae-devops/Makefile` & `dls-normsql-2.3.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/docs/conventions.rst` & `dls-normsql-2.3.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/docs/developing.rst` & `dls-normsql-2.3.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/docs/devops.rst` & `dls-normsql-2.3.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/docs/docs_structure.rst` & `dls-normsql-2.3.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/docs/documenting.rst` & `dls-normsql-2.3.1/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/docs/installing.rst` & `dls-normsql-2.3.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/docs/testing.rst` & `dls-normsql-2.3.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.dae-devops/project.yaml` & `dls-normsql-2.3.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.devcontainer/Dockerfile` & `dls-normsql-2.3.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.devcontainer/devcontainer.json` & `dls-normsql-2.3.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/CONTRIBUTING.rst` & `dls-normsql-2.3.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/actions/install_requirements/action.yml` & `dls-normsql-2.3.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/dependabot.yml` & `dls-normsql-2.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/pages/make_switcher.py` & `dls-normsql-2.3.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/workflows/code.yml` & `dls-normsql-2.3.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/workflows/docs.yml` & `dls-normsql-2.3.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/workflows/docs_clean.yml` & `dls-normsql-2.3.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.github/workflows/linkcheck.yml` & `dls-normsql-2.3.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.gitignore` & `dls-normsql-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.gitlab-ci.yml` & `dls-normsql-2.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/.vscode/launch.json` & `dls-normsql-2.3.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/LICENSE` & `dls-normsql-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/PKG-INFO` & `dls-normsql-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.3.0
+Version: 2.3.1
 Summary: Normalized API over various sql libraries for consistency across multiple projects.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.3.0/docs/conf.py` & `dls-normsql-2.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/docs/images/dls-favicon.ico` & `dls-normsql-2.3.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/docs/images/dls-logo.svg` & `dls-normsql-2.3.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/pyproject.toml` & `dls-normsql-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/src/dls_normsql/__main__.py` & `dls-normsql-2.3.1/src/dls_normsql/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/src/dls_normsql/aiomysql.py` & `dls-normsql-2.3.1/src/dls_normsql/aiomysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,17 +211,23 @@
         await self.__database_definition_object.apply_revision(self, revision)
 
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
 
         if self.__connection is not None:
             # Commit final transaction if not currently autocommitting.
-            if not self.__connection.get_autocommit():
-                logger.debug(f"[DISSHU] {callsign(self)} committing final transaction")
+            try:
                 await self.__connection.commit()
+                logger.debug(
+                    f"[DISSHU] {callsign(self)} successfully committed final transaction"
+                )
+            except Exception as exception:
+                logger.warning(
+                    callsign(self, explain(exception, "committing final transaction"))
+                )
             logger.debug(f"[DISSHU] {callsign(self)} closing connection to server")
             self.__connection.close()
             self.__connection = None
 
     # ----------------------------------------------------------------------------------------
     async def __create_directory(self, filename):
```

### Comparing `dls-normsql-2.3.0/src/dls_normsql/aiosqlite.py` & `dls-normsql-2.3.1/src/dls_normsql/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/src/dls_normsql/constants.py` & `dls-normsql-2.3.1/src/dls_normsql/constants.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/src/dls_normsql/databases.py` & `dls-normsql-2.3.1/src/dls_normsql/databases.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/src/dls_normsql/version.py` & `dls-normsql-2.3.1/src/dls_normsql/version.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/src/dls_normsql.egg-info/PKG-INFO` & `dls-normsql-2.3.1/src/dls_normsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.3.0
+Version: 2.3.1
 Summary: Normalized API over various sql libraries for consistency across multiple projects.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.3.0/src/dls_normsql.egg-info/SOURCES.txt` & `dls-normsql-2.3.1/src/dls_normsql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/base_tester.py` & `dls-normsql-2.3.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/conftest.py` & `dls-normsql-2.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/my_database_definition.py` & `dls-normsql-2.3.1/tests/my_database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/my_table_definition.py` & `dls-normsql-2.3.1/tests/my_table_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/test_aiomysql.py` & `dls-normsql-2.3.1/tests/test_aiomysql.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/test_backup_restore.py` & `dls-normsql-2.3.1/tests/test_backup_restore.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/test_database.py` & `dls-normsql-2.3.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.3.0/tests/test_revision.py` & `dls-normsql-2.3.1/tests/test_revision.py`

 * *Files identical despite different names*

