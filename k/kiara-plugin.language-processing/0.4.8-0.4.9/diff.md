# Comparing `tmp/kiara_plugin.language_processing-0.4.8.tar.gz` & `tmp/kiara_plugin.language_processing-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.language_processing-0.4.8.tar", last modified: Thu Jan  5 17:50:52 2023, max compression
+gzip compressed data, was "kiara_plugin.language_processing-0.4.9.tar", last modified: Thu Jan 12 12:12:34 2023, max compression
```

## Comparing `kiara_plugin.language_processing-0.4.8.tar` & `kiara_plugin.language_processing-0.4.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.650773 kiara_plugin.language_processing-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.630773 kiara_plugin.language_processing-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.638773 kiara_plugin.language_processing-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.638773 kiara_plugin.language_processing-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-01-05 17:50:52.650773 kiara_plugin.language_processing-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.630773 kiara_plugin.language_processing-0.4.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.638773 kiara_plugin.language_processing-0.4.8/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.642773 kiara_plugin.language_processing-0.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.642773 kiara_plugin.language_processing-0.4.8/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.634773 kiara_plugin.language_processing-0.4.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.642773 kiara_plugin.language_processing-0.4.8/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.642773 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.634773 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.646773 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16793 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.646773 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/
--rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20647 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21017 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.646773 kiara_plugin.language_processing-0.4.8/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/examples/pipelines/topic_modeling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.634773 kiara_plugin.language_processing-0.4.8/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.646773 kiara_plugin.language_processing-0.4.8/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-01-05 17:50:52.654773 kiara_plugin.language_processing-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.634773 kiara_plugin.language_processing-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.634773 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.650773 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.650773 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/lda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/lemmatize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.650773 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.650773 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.646773 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-01-05 17:50:52.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-01-05 17:50:52.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 17:50:52.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-05 17:50:52.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 17:49:39.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-01-05 17:50:52.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-05 17:50:52.000000 kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 17:50:52.650773 kiara_plugin.language_processing-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-01-05 17:49:27.000000 kiara_plugin.language_processing-0.4.8/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.568412 kiara_plugin.language_processing-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.552412 kiara_plugin.language_processing-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-01-12 12:12:34.568412 kiara_plugin.language_processing-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.556412 kiara_plugin.language_processing-0.4.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.556412 kiara_plugin.language_processing-0.4.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.556412 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.560412 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16793 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.564412 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/
+-rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20647 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21017 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.564412 kiara_plugin.language_processing-0.4.9/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/examples/pipelines/topic_modeling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.556412 kiara_plugin.language_processing-0.4.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.564412 kiara_plugin.language_processing-0.4.9/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-01-12 12:12:34.568412 kiara_plugin.language_processing-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.556412 kiara_plugin.language_processing-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.556412 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.564412 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.564412 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/lda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/lemmatize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.564412 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.568412 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.564412 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-01-12 12:12:34.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-01-12 12:12:34.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 12:12:34.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-12 12:12:34.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 12:11:44.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-01-12 12:12:34.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-12 12:12:34.000000 kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:12:34.568412 kiara_plugin.language_processing-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-01-12 12:11:32.000000 kiara_plugin.language_processing-0.4.9/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.language_processing-0.4.8/.cruft.json` & `kiara_plugin.language_processing-0.4.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.language_processing-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.language_processing-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/.github/workflows/build-darwin.yaml` & `kiara_plugin.language_processing-0.4.9/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/.github/workflows/build-linux.yaml` & `kiara_plugin.language_processing-0.4.9/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/.github/workflows/build-windows.yaml` & `kiara_plugin.language_processing-0.4.9/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/.gitignore` & `kiara_plugin.language_processing-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/.pre-commit-config.yaml` & `kiara_plugin.language_processing-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/LICENSE` & `kiara_plugin.language_processing-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/Makefile` & `kiara_plugin.language_processing-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/PKG-INFO` & `kiara_plugin.language_processing-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.language_processing
-Version: 0.4.8
+Version: 0.4.9
 Summary: Language-processing kiara modules and data types.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.language_processing
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.language_processing
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.language_processing
 Keywords: kiara
```

### Comparing `kiara_plugin.language_processing-0.4.8/README.md` & `kiara_plugin.language_processing-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/docs/development.md` & `kiara_plugin.language_processing-0.4.9/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/docs/index.md` & `kiara_plugin.language_processing-0.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt` & `kiara_plugin.language_processing-0.4.9/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/examples/pipelines/topic_modeling.yaml` & `kiara_plugin.language_processing-0.4.9/examples/pipelines/topic_modeling.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 pipeline_name: topic_modeling
 doc: Example topic-modeling end-to-end workflow.
 steps:
   - module_type: import.file_bundle
     step_id: import_text_corpus
-  - module_type: create.table.from.text_file_bundle
+  - module_type: create.table.from.file_bundle
     step_id: create_text_corpus
     input_links:
-      text_file_bundle: import_text_corpus.file_bundle
+      file_bundle: import_text_corpus.file_bundle
   - module_type: table.cut_column
     step_id: extract_texts_column
     input_links:
       table: create_text_corpus.table
   - module_type: table.cut_column
     step_id: extract_filename_column
     input_links:
```

### Comparing `kiara_plugin.language_processing-0.4.8/mkdocs.yml` & `kiara_plugin.language_processing-0.4.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/pyproject.toml` & `kiara_plugin.language_processing-0.4.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.22",
-    "kiara_plugin.tabular>=0.4.17",
+    "kiara>=0.4.25",
+    "kiara_plugin.tabular>=0.4.18",
     "gensim>=4.2.0",
     "nltk>=3.7"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
```

### Comparing `kiara_plugin.language_processing-0.4.8/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.language_processing-0.4.9/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/scripts/documentation/gen_info_pages.py` & `kiara_plugin.language_processing-0.4.9/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/scripts/documentation/gen_module_doc.py` & `kiara_plugin.language_processing-0.4.9/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/setup.cfg` & `kiara_plugin.language_processing-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/__init__.py` & `kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/models.py` & `kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/lda.py` & `kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/lda.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 import logging
 import re
 from typing import Any, Dict, Mapping
 
+from kiara.exceptions import KiaraProcessingException
 from kiara.models.values.value import ValueMap
 from kiara.modules import KiaraModule, ValueSetSchema
 from kiara_plugin.tabular.models.array import KiaraArray
 
 
 class LDAModule(KiaraModule):
     """Perform Latent Dirichlet Allocation on a tokenized corpus.
@@ -30,14 +31,15 @@
                 "type": "integer",
                 "doc": "The minimal number of topics.",
                 "default": 7,
             },
             "num_topics_max": {
                 "type": "integer",
                 "doc": "The max number of topics.",
+                "default": 7,
                 "optional": True,
             },
             "compute_coherence": {
                 "type": "boolean",
                 "doc": "Whether to compute the coherence score for each model.",
                 "default": False,
             },
@@ -133,17 +135,22 @@
         tokens_array: KiaraArray = inputs.get_value_data("tokens_array")
         tokens = tokens_array.arrow_array.to_pylist()
 
         words_per_topic = inputs.get_value_data("words_per_topic")
 
         num_topics_min = inputs.get_value_data("num_topics_min")
         num_topics_max = inputs.get_value_data("num_topics_max")
-        if num_topics_max is None:
+        if not num_topics_max:
             num_topics_max = num_topics_min
 
+        if num_topics_max < num_topics_min:
+            raise KiaraProcessingException(
+                "The max number of topics must be larger or equal to the min number of topics."
+            )
+
         compute_coherence = inputs.get_value_data("compute_coherence")
         id2word = corpora.Dictionary(tokens)
         corpus = [id2word.doc2bow(text) for text in tokens]
 
         # model = gensim.models.ldamulticore.LdaMulticore(
         #     corpus, id2word=id2word, num_topics=num_topics, eval_every=None
         # )
```

### Comparing `kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/lemmatize.py` & `kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/lemmatize.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.language_processing-0.4.8/src/kiara_plugin/language_processing/modules/tokens.py` & `kiara_plugin.language_processing-0.4.9/src/kiara_plugin/language_processing/modules/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import io
-from typing import Any, Dict, Iterable, Optional
+from typing import Any, Dict, Iterable, Union
 
 import structlog
 from kiara.exceptions import KiaraProcessingException
 from kiara.models.module import KiaraModuleConfig
 from kiara.models.values.value import ValueMap
 from kiara.modules import KiaraModule, ValueSetSchema
 from kiara_plugin.core_types.models import ListModel
@@ -354,16 +354,16 @@
             "remove_all_numeric": {
                 "type": "boolean",
                 "doc": "Remove all tokens that contain numbers only (e.g. 876).",
                 "default": False,
             },
             "remove_short_tokens": {
                 "type": "integer",
-                "doc": "Remove tokens shorter than a certain length. If value is <= 0, no filtering will be done.",
-                "default": False,
+                "doc": "Remove tokens shorter or equal to this value. If value is <= 0, no filtering will be done.",
+                "default": 0,
             },
             "remove_stopwords": {
                 "type": "list",
                 "doc": "Remove stopwords.",
                 "optional": True,
             },
         }
@@ -392,23 +392,24 @@
         remove_short_tokens: int = inputs.get_value_data("remove_short_tokens")
 
         if remove_short_tokens is None:
             remove_short_tokens = -1
 
         _remove_stopwords = inputs.get_value_obj("remove_stopwords")
         if _remove_stopwords.is_set:
-            stopword_list: Optional[Iterable[str]] = _remove_stopwords.data.list_data
+            stopword_list: Union[Iterable[str], None] = _remove_stopwords.data.list_data
         else:
             stopword_list = None
 
         # it's better to have one method every token goes through, then do every test seperately for the token list
         # because that way each token only needs to be touched once (which is more effective)
-        def check_token(token: str) -> Optional[str]:
+        def check_token(token: str) -> Union[str, None]:
 
             # remove short tokens first, since we can save ourselves all the other checks (which are more expensive)
+            assert isinstance(remove_short_tokens, int)
             if remove_short_tokens > 0:
                 if len(token) <= remove_short_tokens:
                     return None
 
             _token: str = token
             if lowercase:
                 _token = _token.lower()
```

### Comparing `kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/PKG-INFO` & `kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.language-processing
-Version: 0.4.8
+Version: 0.4.9
 Summary: Language-processing kiara modules and data types.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.language_processing
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.language_processing
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.language_processing
 Keywords: kiara
```

### Comparing `kiara_plugin.language_processing-0.4.8/src/kiara_plugin.language_processing.egg-info/SOURCES.txt` & `kiara_plugin.language_processing-0.4.9/src/kiara_plugin.language_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

