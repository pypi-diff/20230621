# Comparing `tmp/kiara_plugin.html-0.4.1.tar.gz` & `tmp/kiara_plugin.html-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.html-0.4.1.tar", last modified: Mon Feb 13 20:47:06 2023, max compression
+gzip compressed data, was "kiara_plugin.html-0.4.2.tar", last modified: Wed Jun 21 10:03:58 2023, max compression
```

## Comparing `kiara_plugin.html-0.4.1.tar` & `kiara_plugin.html-0.4.2.tar`

### file list

```diff
@@ -1,91 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.201945 kiara_plugin.html-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.189945 kiara_plugin.html-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-02-13 20:47:06.201945 kiara_plugin.html-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.189945 kiara_plugin.html-0.4.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/examples/data/journals/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-02-13 20:47:06.201945 kiara_plugin.html-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/core_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/included_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/renderers/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.193945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.201945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/lineage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.201945 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/lineage/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js
--rw-r--r--   0 runner    (1001) docker     (123)    31573 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/lineage/lineage.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.197945 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-02-13 20:47:06.000000 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-13 20:47:06.000000 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:47:06.000000 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-13 20:47:06.000000 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:46:37.000000 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-13 20:47:06.000000 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-13 20:47:06.000000 kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:47:06.201945 kiara_plugin.html-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      218 2023-02-13 20:46:29.000000 kiara_plugin.html-0.4.1/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.923573 kiara_plugin.html-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.923573 kiara_plugin.html-0.4.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/pipelines/example_pipeline_html.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/core_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/included_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31573 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/lineage.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:03:30.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      218 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.html-0.4.1/.cruft.json` & `kiara_plugin.html-0.4.2/.cruft.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'f30a92644095dd13556ab071b97d20008badaed3'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "0bd18052c72f941452b3d789592c259da24d2a61",
+    "commit": "f30a92644095dd13556ab071b97d20008badaed3",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.html-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/.github/workflows/build-darwin.yaml` & `kiara_plugin.html-0.4.2/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/.github/workflows/build-linux.yaml` & `kiara_plugin.html-0.4.2/.github/workflows/build-linux.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.html
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[all,dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: Test with pytest
         run: make test
 
 # Uncomment this if you have coveralls.io setup with this repo
 #  coverage:
@@ -39,38 +39,37 @@
 #    steps:
 #      - name: "Set up Python 3.9"
 #        uses: actions/setup-python@v4
 #        with:
 #          python-version: "3.9"
 #      - uses: actions/checkout@v3
 #      - name: install kiara
-#        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+#        run: pip install -U .[all,dev_testing]
 #      - name: display installed kiara and module package versions
 #        run: pip list | grep kiara
 #      - name: Run coverage
 #        run: coverage run -m pytest tests
-#      - name: Upload coverage data to coveralls.io
-#        run: coveralls --service=github
-#        env:
-#          GITHUB_TOKEN:  ${{ secrets.GITHUB_TOKEN }}""
+#      - name: coveralls
+#        uses: coverallsapp/github-action@v2
 
+# Uncomment this if you want to run mypy
 #  mypy-linux:
 #    name: mypy check on linux
 #    runs-on: ubuntu-latest
 #    strategy:
 #      matrix:
 #        python_version: ["3.8", "3.9", "3.10", "3.11"]
 #    steps:
 #      - name: "Set up Python ${{ matrix.python_version }}"
 #        uses: actions/setup-python@v4
 #        with:
 #          python-version: "${{ matrix.python_version }}"
 #      - uses: actions/checkout@v3
 #      - name: install kiara_plugin.html
-#        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+#        run: pip install -U .[all,dev_testing]
 #      - name: Test with mypy
 #        run: make mypy
 
   linting-linux:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
@@ -97,23 +96,23 @@
     if: ${{ github.ref == 'refs/heads/develop' }} || ${{ github.ref == 'refs/heads/main' }} || startsWith(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     needs:
       - test-linux
 #      - mypy-linux
 #      - linting-linux
     steps:
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: install kiara_plugin.html package
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_documentation]
+        run: pip install -U .[all,dev_documentation]
       - run: git config --global user.email "Markus Binsteiner"
       - run: git config --global user.name "markus@frkl.io"
       - name: create latest documentation
         if: ${{ ( github.ref == 'refs/heads/develop') }}
         run: FAIL_DOC_BUILD_ON_ERROR=true mike deploy --push latest && mike set-default --push latest
       - name: extract tag name
         run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
@@ -128,25 +127,25 @@
     needs:
       - test-linux
 #      - mypy-linux
 #      - linting-linux
     env:
         GEMFURY_PUSH_TOKEN: ${{ secrets.GEMFURY_PUSH_TOKEN }}
     steps:
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: install pip
         run: pip install pip==21.2.4 setuptools==57.4.0
       - name: install kiara
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ -e .[all]
+        run: pip install -U -e .[all]
       - name: install 'build' package
         run: pip install -U build
       - name: create packages
         run: python -m build
       - name: upload source package
         run: curl -F package=@$(ls dist/kiara*.tar.gz) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/
       - name: upload wheel
@@ -162,29 +161,31 @@
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
     needs:
       - test-linux
 #      - mypy-linux
 #      - linting-linux
     steps:
-      - name: "Set up Python 3.9"
+      - name: "Set up Python 3.11"
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - name: pip cache
         id: pip-cache
         uses: actions/cache@v3
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
+      - name: install kiara
+        run: pip install kiara
       - name: install required plugin packages
-        run: pip install -U --pre --extra-index-url https://pypi.fury.io/dharpa/ kiara_plugin.develop
+        run: pip install git+https://github.com/DHARPA-Project/kiara_plugin.develop.git@develop
       - name: build conda package
         if: ${{ ( github.ref == 'refs/heads/develop') }}
         run: kiara conda build-package --patch-data ci/conda/conda-pkg-patch.yaml .
       - name: extract tag name
         run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
       - name: build & publish conda package
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
```

### Comparing `kiara_plugin.html-0.4.1/.github/workflows/build-windows.yaml` & `kiara_plugin.html-0.4.2/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/.gitignore` & `kiara_plugin.html-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/.pre-commit-config.yaml` & `kiara_plugin.html-0.4.2/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     files: "^src/"
     pass_filenames: true
     args: ["--config-file", "setup.cfg", "--ignore-missing-imports", "--explicit-package-bases"]
     additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, anyio>=3.0.0, pyzmq>=22.0.3, bidict, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil, dag_cbor, multiformats, textual, regex, types-pytz, types-orjson, types-Markdown]
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.0.237'
+  rev: 'v0.0.272'
   hooks:
     - id: ruff
 
 - repo: https://github.com/Kludex/no-optional
   rev: 0.4.0
   hooks:
     - id: no_optional
```

### Comparing `kiara_plugin.html-0.4.1/LICENSE` & `kiara_plugin.html-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/Makefile` & `kiara_plugin.html-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/PKG-INFO` & `kiara_plugin.html-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.html
-Version: 0.4.1
+Version: 0.4.2
 Summary: Kiara plugin for html-related tasks.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.html
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.html
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.html
 Keywords: kiara
```

### Comparing `kiara_plugin.html-0.4.1/README.md` & `kiara_plugin.html-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/docs/development.md` & `kiara_plugin.html-0.4.2/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/docs/index.md` & `kiara_plugin.html-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.html-0.4.2/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.html-0.4.2/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/mkdocs.yml` & `kiara_plugin.html-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/pyproject.toml` & `kiara_plugin.html-0.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara_plugin.core_types>=0.4.16",
+    "kiara>=0.4.41",
+    "kiara_plugin.core_types>=0.4.20",
     "hypercorn",
     "json2html>=1.3.0",
     "markdown>=3.2.1",
     "pymdown-extensions>=9.9",
     "airium>=0.2.3"
 ]
 dynamic = ["version"]
@@ -53,22 +54,17 @@
     "pygraphviz>=1.10",
 ]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
 dev_testing = [
     "kiara[dev_testing]",
-    "types-Markdown",
-    "ruff>=0.0.237"
 ]
 dev_utils = [
     "kiara[dev_utils]",
-    "types-Markdown",
-    "ruff>=0.0.237"
-
 ]
 dev_all = [
     "kiara[dev_all]"
 ]
 
 [project.entry-points."kiara.plugin"]
 html = "kiara_plugin.html"
@@ -141,16 +137,15 @@
     "PD",
     "PLC",
     "PLE",
     "PLR",
     "PLW",
     "PIE",
 ]
-#select = ["E", "F", "RUF100", "W", "I001"]
-ignore = ["E501", "S101", "SIM118", "SIM108", "PLR2004"]
+ignore = ["E501", "S101", "SIM118", "SIM108", "PLR2004", "PLR0913", "S110", "PLR0912", "PLR0915", "PIE810"]
 
 fix = true
 fixable = ["E", "F", "RUF100", "I001", "Q"]
 
 
 #fixable = ["E", "F", "RUF100", "I001"]
 # Enable Pyflakes `E` and `F` codes by default.
```

### Comparing `kiara_plugin.html-0.4.1/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.html-0.4.2/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/scripts/documentation/gen_info_pages.py` & `kiara_plugin.html-0.4.2/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/scripts/documentation/gen_module_doc.py` & `kiara_plugin.html-0.4.2/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/setup.cfg` & `kiara_plugin.html-0.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	tests
 
 [aliases]
 build = bdist_wheel
 release = build upload
 
 [bdist_wheel]
-universal = 1
+universal = 0
 
 [devpi:upload]
 no-vcs = 1
 formats = sdist, bdist_wheel
 
 [tool:pytest]
 addopts =
```

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/__init__.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/defaults.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/models/__init__.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/__init__.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict, Union
 
+from kiara.api import KiaraModule, Value, ValueMap, ValueMapSchema
 from kiara.defaults import DEFAULT_PRETTY_PRINT_CONFIG
-from kiara.models.values.value import Value, ValueMap
-from kiara.modules import KiaraModule, ValueSetSchema
 from kiara.modules.included_core_modules.pretty_print import PrettyPrintModule
 from kiara.utils.output import ArrowTabularWrap
 
 
 class RenderMarkdown(KiaraModule):
 
     _module_type_name = "render.markdown.to.html"
 
     def create_inputs_schema(
         self,
-    ) -> ValueSetSchema:
+    ) -> ValueMapSchema:
 
         return {"markdown": {"type": "string", "doc": "The markdown string"}}
 
     def create_outputs_schema(
         self,
-    ) -> ValueSetSchema:
+    ) -> ValueMapSchema:
 
         return {"html": {"type": "html", "doc": "The rendered html"}}
 
     def process(self, inputs: ValueMap, outputs: ValueMap):
 
         import markdown
```

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/core_types.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/core_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import orjson
 from pygments import highlight
 from pygments.lexers.data import JsonLexer
 from pymdownx.highlight import HtmlFormatter
 
 from kiara.api import Value
 from kiara.exceptions import KiaraProcessingException
-from kiara.models.data_types import DictModel
+from kiara.models.data_types import KiaraDict
 from kiara.models.rendering import RenderScene, RenderValueResult
 from kiara.modules.included_core_modules.render_value import RenderValueModule
 from kiara.utils.json import orjson_dumps
 
 
 class RenderCoreTypeModuleWeb(RenderValueModule):
     _module_type_name = "render.core_types.for.web"
@@ -20,15 +20,15 @@
     def render__dict__as__html(self, value: Value, render_config: Mapping[str, Any]):
 
         render_scene = render_config.get("scene_name", "data")
         # input_number_of_rows = render_config.get("number_of_rows", 20)
         # input_row_offset = render_config.get("row_offset", 0)
         as_table = render_config.get("as_table", True)
 
-        dict_model: DictModel = value.data
+        dict_model: KiaraDict = value.data
 
         if render_scene == "data":
             to_render = dict_model.dict_data
         elif render_scene == "schema":
             to_render = dict_model.data_schema
         else:
             raise KiaraProcessingException(
```

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/included_types.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/included_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/modules/tabular.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/tabular.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/renderers/lineage.py` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/lineage.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js` & `kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/PKG-INFO` & `kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.html
-Version: 0.4.1
+Version: 0.4.2
 Summary: Kiara plugin for html-related tasks.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.html
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.html
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.html
 Keywords: kiara
```

### Comparing `kiara_plugin.html-0.4.1/src/kiara_plugin.html.egg-info/SOURCES.txt` & `kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 docs/index.md
 docs/usage.md
 docs/stylesheets/extra.css
 examples/data/Readme.md
 examples/data/journals/JournalEdges1902.csv
 examples/data/journals/JournalNodes1902.csv
 examples/data/journals/Readme.md
+examples/jobs/Readme.md
+examples/pipelines/Readme.md
+examples/pipelines/example_pipeline_html.yaml
 scripts/documentation/gen_api_doc_pages.py
 scripts/documentation/gen_info_pages.py
 scripts/documentation/gen_module_doc.py
 src/kiara_plugin.html.egg-info/PKG-INFO
 src/kiara_plugin.html.egg-info/SOURCES.txt
 src/kiara_plugin.html.egg-info/dependency_links.txt
 src/kiara_plugin.html.egg-info/entry_points.txt
@@ -55,8 +58,10 @@
 src/kiara_plugin/html/renderers/__init__.py
 src/kiara_plugin/html/renderers/lineage.py
 src/kiara_plugin/html/resources/.gitkeep
 src/kiara_plugin/html/resources/templates/lineage/lineage.html.j2
 src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js
 src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js
 tests/conftest.py
-tests/test_kiara_modules_default.py
+tests/test_job_descs.py
+tests/test_kiara_modules_default.py
+tests/resources/.gitkeep
```

