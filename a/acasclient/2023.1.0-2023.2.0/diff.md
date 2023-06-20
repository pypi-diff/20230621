# Comparing `tmp/acasclient-2023.1.0.tar.gz` & `tmp/acasclient-2023.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acasclient-2023.1.0.tar", last modified: Fri Feb 24 15:52:40 2023, max compression
+gzip compressed data, was "acasclient-2023.2.0.tar", last modified: Tue Jun 20 22:44:52 2023, max compression
```

## Comparing `acasclient-2023.1.0.tar` & `acasclient-2023.2.0.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:52:40.683192 acasclient-2023.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-24 15:52:24.000000 acasclient-2023.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-02-24 15:52:24.000000 acasclient-2023.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-24 15:52:24.000000 acasclient-2023.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-02-24 15:52:24.000000 acasclient-2023.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-24 15:52:24.000000 acasclient-2023.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-24 15:52:40.683192 acasclient-2023.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-24 15:52:24.000000 acasclient-2023.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:52:40.659191 acasclient-2023.1.0/acasclient/
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/CmpdReg.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/StereoCategory.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88376 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/acasclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/ddict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)   106612 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/lsthing.py
--rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/selfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-02-24 15:52:24.000000 acasclient-2023.1.0/acasclient/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:52:40.659191 acasclient-2023.1.0/acasclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-24 15:52:40.000000 acasclient-2023.1.0/acasclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-02-24 15:52:40.000000 acasclient-2023.1.0/acasclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 15:52:40.000000 acasclient-2023.1.0/acasclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-24 15:52:40.000000 acasclient-2023.1.0/acasclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 15:52:40.000000 acasclient-2023.1.0/acasclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-24 15:52:40.000000 acasclient-2023.1.0/acasclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 15:52:40.000000 acasclient-2023.1.0/acasclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:52:40.663191 acasclient-2023.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/acasclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-24 15:52:24.000000 acasclient-2023.1.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-24 15:52:40.683192 acasclient-2023.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-24 15:52:24.000000 acasclient-2023.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:52:40.663191 acasclient-2023.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/project_thing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:52:40.679192 acasclient-2023.1.0/tests/test_acasclient/
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls
--rw-r--r--   0 runner    (1001) docker     (123)    29696 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/1_1_Generic.xls
--rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/1_1_Generic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/1_1_Generic_empty_column.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv
--rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/4 parameter D-R-validation.csv
--rw-r--r--   0 runner    (1001) docker     (123)    68873 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/4 parameter D-R.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2442910 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/50k-lines.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/blob_test.png
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/dummy.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/dummy2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/escaped_quotes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    29184 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/escaped_quotes.xls
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/ibuprofen_big_lot_number.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/ibuprofen_methyl_ester.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/infinite-numeric-values.csv
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/malformatted-single-quote.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1000988 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/nci1000.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/non-uniform-commas-with-quoted-text.csv
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/quoted-with-new-line-character-in-string.csv
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/same-header-different-data-types.csv
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_000_creds_from_file_credentials
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_005_swap_parent_structures.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_012_register_sdf.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_047_register_sdf_with_salts.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (123)  5477940 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/text_010_partial_parent_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient/uniform-commas-with-quoted-text.csv
--rw-r--r--   0 runner    (1001) docker     (123)   205173 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_acasclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    49206 2023-02-24 15:52:24.000000 acasclient-2023.1.0/tests/test_lsthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:44:52.384143 acasclient-2023.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-20 22:44:35.000000 acasclient-2023.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-20 22:44:35.000000 acasclient-2023.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 22:44:35.000000 acasclient-2023.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-20 22:44:35.000000 acasclient-2023.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 22:44:35.000000 acasclient-2023.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-20 22:44:52.384143 acasclient-2023.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-20 22:44:35.000000 acasclient-2023.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:44:52.364143 acasclient-2023.2.0/acasclient/
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/CmpdReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/StereoCategory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92439 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/acasclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/ddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106612 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/lsthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31011 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/selfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-20 22:44:35.000000 acasclient-2023.2.0/acasclient/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:44:52.368143 acasclient-2023.2.0/acasclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-20 22:44:52.000000 acasclient-2023.2.0/acasclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-20 22:44:52.000000 acasclient-2023.2.0/acasclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:44:52.000000 acasclient-2023.2.0/acasclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 22:44:52.000000 acasclient-2023.2.0/acasclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:44:52.000000 acasclient-2023.2.0/acasclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 22:44:52.000000 acasclient-2023.2.0/acasclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 22:44:52.000000 acasclient-2023.2.0/acasclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:44:52.368143 acasclient-2023.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/acasclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 22:44:35.000000 acasclient-2023.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 22:44:52.384143 acasclient-2023.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-20 22:44:35.000000 acasclient-2023.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:44:52.368143 acasclient-2023.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/project_thing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:44:52.384143 acasclient-2023.2.0/tests/test_acasclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/12_1_MultipleImage.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   261659 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/12_2_MultipleImage.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    29696 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/1_1_Generic.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/1_1_Generic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/1_1_Generic_empty_column.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/4 parameter D-R-validation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    68873 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/4 parameter D-R.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2442910 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/50k-lines.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/blob_test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/dummy.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/dummy2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/escaped_quotes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29184 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/escaped_quotes.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/ibuprofen_big_lot_number.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/ibuprofen_methyl_ester.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/infinite-numeric-values.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/malformatted-single-quote.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1000988 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/nci1000.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/non-uniform-commas-with-quoted-text.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/quoted-with-new-line-character-in-string.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/same-header-different-data-types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_000_creds_from_file_credentials
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_005_swap_parent_structures.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_012_register_sdf.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_047_register_sdf_with_salts.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)  5477940 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/text_010_partial_parent_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient/uniform-commas-with-quoted-text.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   217375 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_acasclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49206 2023-06-20 22:44:35.000000 acasclient-2023.2.0/tests/test_lsthing.py
```

### Comparing `acasclient-2023.1.0/CONTRIBUTING.rst` & `acasclient-2023.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/LICENSE` & `acasclient-2023.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/PKG-INFO` & `acasclient-2023.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acasclient
-Version: 2023.1.0
+Version: 2023.2.0
 Summary: ACAS API Client
 Home-page: https://github.com/mcneilco/acasclient
 Author: Brian Bolt
 Author-email: brian.bolt@boltengineered.com
 License: GNU General Public License v3
 Keywords: acasclient
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acasclient-2023.1.0/README.rst` & `acasclient-2023.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/acasclient/CmpdReg.py` & `acasclient-2023.2.0/acasclient/CmpdReg.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/acasclient/StereoCategory.py` & `acasclient-2023.2.0/acasclient/StereoCategory.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/acasclient/acasclient.py` & `acasclient-2023.2.0/acasclient/acasclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 VALID_STRUCTURE_SEARCH_TYPES = {"substructure", "duplicate",
                         "duplicate_tautomer", "duplicate_no_tautomer",
                         "stereo_ignore", "full_tautomer", "substructure",
                         "similarity", "full"}
 
 def isBase64(s):
+    """Checks if a string is base64 encoded.
+    """
+    if not isinstance(s, str):
+        return False
     return (len(s) % 4 == 0) and re.match('^[A-Za-z0-9+/]+[=]{0,2}$', s)
 
 
 def creds_from_file(fpath, profile="default"):
     """Fetches crecentials from a file
 
     Retrieves credentials from a file.
@@ -151,14 +155,42 @@
                     if (not v["deleted"] and not v["ignored"] and
                             v["lsType"] == value_type and
                             v["lsKind"] == value_kind):
                         value = v
                         break
     return value
 
+def get_entity_values_by_state_type_kind_value_type(entity, state_type,
+                                                        state_kind, value_type):
+    """Gets values from an acas entity dict object.
+
+    Gets values from an acas entity dict object by state type, state kind and value type.
+
+    Args:
+        entity: Any ACAS entity (protocol, experiment, analysis_group,
+        treatment_group, container...etc.)
+        state_type: String. The state type of the value.
+        state_kind: String. The state kind of the value.
+        value_type: String. The value type of the value.
+
+    Returns:
+        A list of dict objects representing the values if they exits. Otherwise it
+        returns an empty list
+
+    """
+    values = []
+    if len(entity["lsStates"]) > 0:
+        for s in entity["lsStates"]:
+            if (not s["deleted"] and not s["ignored"] and
+                    s["lsType"] == state_type and s["lsKind"] == state_kind):
+                for v in s["lsValues"]:
+                    if (not v["deleted"] and not v["ignored"] and
+                            v["lsType"] == value_type):
+                        values.append(v)
+    return values
 
 def get_entity_label_by_label_type_kind(entity: dict, label_type: str, label_kind: str) -> str:
     """Get a label from an acas entity dict object.
 
     Gets a specific label from an acas entity dict object.
 
     Args:
@@ -1105,23 +1137,25 @@
         Args:
             data_file (str): A path to an experiment loader formatted file
             user (str): A username
             dry_run (bool): If true, then validate but do not load the data into the database
             report_file (str): A path to a report file (optional)
             images_file (str): A path to an images file (optional)
         """
-        data_file = self.upload_files([data_file])['files'][0]["name"]
+        data_file_path = self.upload_files([data_file])['files'][0]["name"]
+        report_file_path = ""
         if report_file and report_file != "":
-            report_file = self.upload_files([report_file])['files'][0]["name"]
+            report_file_path = self.upload_files([report_file])['files'][0]["name"]
+        images_file_path = ""
         if images_file and images_file != "":
-            images_file = self.upload_files([images_file])['files'][0]["name"]
+            images_file_path = self.upload_files([images_file])['files'][0]["name"]
         request = {"user": user,
-                   "fileToParse": data_file,
-                   "reportFile": report_file,
-                   "imagesFile": images_file,
+                   "fileToParse": data_file_path,
+                   "reportFile": report_file_path,
+                   "imagesFile": images_file_path,
                    "moduleName": None if validate_dose_response_curves else "DoseResponseDataParserController",
                    "dryRunMode": dry_run}
         resp = self.experiment_loader_request(request)
         return resp
 
     def dose_response_experiment_loader(self, model_fit_type, fit_settings, **kwargs):
         """Dose response experiment loader
@@ -1926,14 +1960,40 @@
         if type(validation_resp) is list and len(validation_resp) > 0:
             raise ValueError(validation_resp[0]['message'])
         # Create
         resp = self.session.post(url_base, json=codeTable)
         resp.raise_for_status()
         return resp.json()
     
+    def get_assay_scientists(self):
+        """
+        Fetch the list of possible assay scientists for  assay loading
+        """
+        resp = self.session.get("{}/api/authors?additionalCodeType=assay&additionalCodeKind=scientist&roleName=ROLE_ACAS-USERS".format(self.url))
+        resp.raise_for_status()
+        return resp.json()
+
+    def create_assay_scientist(self, code, name):
+        """
+        Create a new scientist for assay loading
+        """
+        url_base = "{}/api/codeTablesAdmin/assay/scientist".format(self.url)
+        body = {'code': code, 'name': name}
+        return self._validate_then_save_codetable(url_base, body)
+    
+    def update_assay_scientist(self, scientist: dict):
+        """
+        Update a scientist for  assay loading
+        """
+        if 'id' not in scientist:
+            raise ValueError("id attribute of scientist dict is required")
+        resp = self.session.put("{}/api/codeTablesAdmin/assay/scientist/{}".format(self.url, scientist['id']), json=scientist)
+        resp.raise_for_status()
+        return resp.json()
+    
     def get_cmpdreg_scientists(self):
         """
         Fetch the list of possible lot chemists for CmpdReg
         """
         resp = self.session.get("{}/cmpdreg/scientists".format(self.url))
         resp.raise_for_status()
         return resp.json()
@@ -2109,15 +2169,32 @@
                             "read": true,
                             "write": true
                         },
                         "code": "EXPT-00000009",
                         "comments": "CMPD-0000001-001",
                         "description": "6 results",
                         "ignored": false,
-                        "name": "BLAH"
+                        "name": "BLAH",
+                        "analysisGroups": [
+                            {
+                                "code": "AG-00000001",
+                                "values": [
+                                    {
+                                        "id": 1,
+                                        "lsKind": "key",
+                                        "lsType": "numericValue",
+                                        "value": 6
+                                    }
+                                ]
+                            }
+                        ],
+                        "protocol": {
+                            "code": "PROT-00000001",
+                            "name": "Test Protocol"
+                        }
                     }
                 ],
                 "linkedLots": [
                     {
                         "acls": {
                             "delete": false,
                             "read": true,
@@ -2247,34 +2324,53 @@
         # Look up the compound to find a lot, so we can access a MetaLot
         search_results = self.cmpd_search(corpNameList=parent_corp_name)
         if len(search_results['foundCompounds']) == 0:
             raise RuntimeError(f'Parent corp name {parent_corp_name} could not be found')
         lot_corp_name = search_results['foundCompounds'][0]['lotIDs'][0]['corpName']
         return self.get_meta_lot(lot_corp_name)
     
+    def get_parent_alias_kinds(self) -> List[Dict]:
+        """Get the list of parent alias kinds
+        """
+        resp = self.session.get("{}/cmpdreg/aliases/parentAliasKinds/".format(self.url))
+        resp.raise_for_status()
+        return resp.json()
+    
     def get_parent_aliases(self, parent_corp_name: str) -> List[str]:
         """Get the current parent aliases by parent_corp_name
         """
         meta_lot = self._get_meta_lot_by_parent_corp_name(parent_corp_name)
         # Find the parent aliases nested within the meta_lot
         alias_objects = meta_lot['lot']['saltForm']['parent']['parentAliases']
         # Flatten them to a list of strings
         aliases = [x['aliasName'] for x in alias_objects if not x['ignored']]
         return aliases
     
-    def add_parent_alias(self, parent_corp_name: str, alias: str) -> None:
+    def add_parent_alias(self, parent_corp_name: str, alias: str, ls_type: str = None, ls_kind: str = None) -> None:
         """Adds a new alias to the specified parent. Does not alter existing aliases.
+
+        Args:
+            parent_corp_name (str): The parent compound to add the alias to
+            alias (str): The alias to add
+            ls_type (str): The LS type of the alias, default None
+            ls_kind (str): The LS kind of the alias, default None
+
+        Returns:
+            The updated MetaLot object
         """
         meta_lot = self._get_meta_lot_by_parent_corp_name(parent_corp_name)
         # Format the alias string into a basic object
-        alias_obj = {'aliasName': alias}
+        alias_obj = {'aliasName': alias, 'lsType': ls_type, 'lsKind': ls_kind, 'ignored': False}
         # Add it to the list of aliases
         meta_lot['lot']['saltForm']['parent']['parentAliases'].append(alias_obj)
         # Persist the change
-        self.save_meta_lot(meta_lot)
+        response = self.save_meta_lot(meta_lot)
+        if len(response['errors']) != 0:
+            raise RuntimeError(f'Failed to add alias {alias} to parent {parent_corp_name}: {response["errors"]}')
+        return response['metalot']
 
     def set_parent_aliases(self, parent_corp_name: str, alias_list: List[str]) -> None:
         """Sets the aliases of the specified parent to ONLY the provided list.
         This will remove existing aliases if they are not in `alias_list`.
         To add aliases without removing existing ones, use the `add_parent_alias` method.
         """
         meta_lot = self._get_meta_lot_by_parent_corp_name(parent_corp_name)
```

### Comparing `acasclient-2023.1.0/acasclient/ddict.py` & `acasclient-2023.2.0/acasclient/ddict.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/acasclient/interactions.py` & `acasclient-2023.2.0/acasclient/interactions.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/acasclient/lsthing.py` & `acasclient-2023.2.0/acasclient/lsthing.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/acasclient/selfile.py` & `acasclient-2023.2.0/acasclient/selfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 A module to read, edit, and write ACAS 'Single Experiment
 Loader' files.
+
 Common formats are supported for both input and output: csv, and
 excel
+
+
 """
 # Contributors:  Shawn Watts
 
 
 ################################################################################
 # Packages
 ################################################################################
@@ -45,16 +48,16 @@
 LOT_AMOUNT_UNITS = 'Lot Amount Units'
 LOT_PURITY = 'Lot Purity'
 LOT_PURITY_MEASURED_BY = 'Lot Purity Measured By'
 LOT_SALT_ABBREV = 'Lot Salt Abbrev'
 LOT_SALT_EQ = 'Lot Salt Equivalents'
 REG_LOT_CORP_NAME = 'Registered Lot Corp Name'
 REG_PARENT_CORP_NAME = 'Registered Parent Corp Name'
-REG_LOT_AMOUNT =  'Registered Lot Amount'
-REG_LOT_AMOUNT_UNITS =  'Registered Lot Amount Units'
+REG_LOT_AMOUNT = 'Registered Lot Amount'
+REG_LOT_AMOUNT_UNITS = 'Registered Lot Amount Units'
 REG_PARENT_ALIASES = 'Registered Parent Aliases'
 REG_LEVEL = 'Registration Level'
 
 
 ################################################################################
 # Logging
 ################################################################################
@@ -64,56 +67,66 @@
 ################################################################################
 # Functions
 ################################################################################
 def get_file_type(file_name):
     """
     :return: The file extension
     :rtype: str
+
     :param file_name: Path to file to check.
     :type file_name: str
+
     :note: a guess at the file format based on the extension:  csv, xls, or xlsx.
+
     :raise: ValueError if the file extension is not recognized.
+
     """
 
     try:
         ext = os.path.splitext(file_name)[1].lower()
-    except TypeError as err:
+    except (TypeError, ValueError) as err:
+        logger.critical(err)
         raise ValueError(f"Unknown file name extension: {file_name}")
 
     allowed_extensions = (CSV, XLSX, XLS)
     if ext in allowed_extensions:
         return ext
     else:
         raise ValueError(f"Unknown file type: {file_name}")
 
 
 def get_read_func_by_file_type(file_type):
     """
     :return: The pandas read_x function
     :rtype: function
+
     :param file_type: File extension.
     :type file_type: str
+
     """
 
     if file_type == CSV:
         read_func = partial(pd.read_csv, dtype=str)
     elif file_type == XLSX:
         read_func = partial(pd.read_excel, engine='openpyxl', dtype=str)
     else:
         read_func = partial(pd.read_excel, dtype=str)
     return read_func
 
 
 def load_from_str(file_str, file_type):
     """
     'Factory function' for Generic or DoseResponse experiments.
+
     :param file_str:  Contents of an experiment file to load.
     :type file_str: str
+
     :param file_type: File extension that indicates the file format.
     :type file_type: Module constant
+
     """
 
     expt = Generic()
     expt.loadStr(file_str, file_type)
     if expt.format == GENERIC:
         return expt
     expt = DoseResponse()
@@ -123,14 +136,15 @@
 
 ################################################################################
 # Classes
 ################################################################################
 class AbstractExperiment():
     """
     Interface for reading formatted ACAS SEL files.
+
     """
 
     META_HEADER = [
         'Experiment Meta Data',
         'Format',
         'Protocol Name',
         'Experiment Name',
@@ -158,14 +172,15 @@
     blank = ""
     _meta_rows = 15  # Scan this many rows for the end of meta/start of payload.
 
     def __init__(self, file_name=None):
         """
         :param file_name: Path to the ACAS Experiment file to load.
         :type file_name:  str
+
         """
 
         self.file_name = file_name
 
         # These map to the meta fields.
         self._experimental_meta_data = self.blank
         self._format = self.blank
@@ -187,14 +202,19 @@
         self._id = None
 
         # OrderedDict of 'Datatype', Column keys for type.
         self._datatype = collections.OrderedDict(
             [('Corporate Batch ID', 'Datatype')]
         )
 
+        # OrderedDict of 'Datatype' for raw results, Column keys for type.
+        self._raw_datatype = collections.OrderedDict(
+            [('curve id', 'temp id')]
+        )
+
         # Experimental results payload is a data frame.
         self._expt_df = pd.DataFrame()
 
         # Autoload optional file_name.
         if file_name:
             self.loadFile(file_name)
 
@@ -218,27 +238,30 @@
             'expt_df': self.expt_df.to_dict(),
         }
 
     def loadFile(self, file_name):
         """
         :param file_name: Path to the file to load.
         :type file_name: str
+
         """
 
         self.file_name = file_name
         self._file_type = get_file_type(file_name)
         read_func = get_read_func_by_file_type(self._file_type)
         self._parse(read_func)
 
     def loadStr(self, file_str, file_type):
         """
         :param file_str:  Contents of an experiment file to load.
         :type file_str: str
+
         :param file_type: File extension that indicates the file format.
         :type file_type: Module constant
+
         """
 
         self._file_type = file_type
         if type(file_str) == str:
             self.file_name = io.StringIO(file_str)
         else:
             self.file_name = io.BytesIO(file_str)
@@ -246,14 +269,15 @@
         self._parse(read_func)
 
     def saveAs(self, file_name):
         """Save to a file on disk"""
         raise NotImplementedError("Defined by subclass")
 
     def validate(self):
+        """Validate the contents"""
         raise NotImplementedError("Defined by subclass")
 
     def getCorporateBatchIds(self):
         """Return a set of Lot Corp Names recorded in the experiment"""
 
         lot_corp_names = set()
         if LOT_CORP_NAME in self.expt_df.columns:
@@ -263,115 +287,115 @@
     def getEndpointNames(self):
         """Return set of Assay-Endpoints recorded in the experiment"""
 
         endpoint_names = set(self.expt_df.columns.tolist())
         endpoint_names.discard(LOT_CORP_NAME)
         return endpoint_names
 
-
     # Meta data property() decorators to flag when the representation
     # is altered.
     @property
     def meta_has_changed(self):
         """Return boolean,  True if the meta data changed after file parsing."""
         return self._meta_has_changed
+
     @meta_has_changed.setter
     def meta_has_changed(self, value):
         # Only set this if True so subsequent checks that are not changes
         # can't unset.
         if value:
             self._meta_has_changed = value
 
-
     @property
     def experimental_meta_data(self):
         """Experimental Meta Data (Meta Data)"""
         return self._experimental_meta_data
+
     @experimental_meta_data.setter
     def experimental_meta_data(self, value):
         self.meta_has_changed = (value != self._experimental_meta_data)
         self._experimental_meta_data = value
 
-
     @property
     def format(self):
         """Format (Meta Data)"""
         return self._format
+
     @format.setter
     def format(self, value):
         self.meta_has_changed = (value != self._format)
         self._format = value
 
-
     @property
     def protocol_name(self):
         """Protocol Name (Meta Data)"""
         return self._protocol_name
+
     @protocol_name.setter
     def protocol_name(self, value):
         self.meta_has_changed = (value != self._protocol_name)
         self._protocol_name = value
 
-
     @property
     def experiment_name(self):
         """Experiment Name (Meta Data)"""
         return self._experiment_name
+
     @experiment_name.setter
     def experiment_name(self, value):
         self.meta_has_changed = (value != self._experiment_name)
         self._experiment_name = value
     # Alias
     name = experiment_name
 
-
     @property
     def scientist(self):
         """Scientist (Meta Data)"""
         return self._scientist
+
     @scientist.setter
     def scientist(self, value):
         self.meta_has_changed = (value != self._scientist)
         self._scientist = value
 
-
     @property
     def notebook(self):
         """Notebook (Meta Data)"""
         return self._notebook
+
     @notebook.setter
     def notebook(self, value):
         self.meta_has_changed = (value != self._notebook)
         self._notebook = value
 
-
     @property
     def page(self):
         """Page (Meta Data)"""
         return self._page
+
     @page.setter
     def page(self, value):
         self.meta_has_changed = (value != self._page)
         self._page = value
 
-
     @property
     def assay_date(self):
         """Assay Date (Meta Data)"""
         return self._assay_date
+
     @assay_date.setter
     def assay_date(self, value):
         self.meta_has_changed = (value != self._assay_date)
         self._assay_date = value
 
-
     @property
     def project(self):
         """Project (Meta Data)"""
         return self._project
+
     @project.setter
     def project(self, value):
         self.meta_has_changed = (value != self._project)
         self._project = value
 
     @property
     def id(self):
@@ -379,77 +403,96 @@
         return self._id
     @id.setter
     def id(self, value):
         self._id = value
 
     @property
     def expt_df(self):
-        """pd.DataFrame container for the experimental results data.  Also aliased as calculated_results_df"""
+        """
+        pd.DataFrame container for the experimental results data.  Also aliased
+        as calculated_results_df
+        """
         return self._expt_df.copy()
+
     @expt_df.setter
     def expt_df(self, new_expt_df):
         self._expt_has_changed = self._expt_df.equals(new_expt_df)
         self._expt_df = new_expt_df
 
     @property
     def calculated_results_df(self):
         """
         pd.DataFrame container for the 'Calculated Results'.
-        :note:  The df.columns are just the 'Corporate Batch ID' and endpoints, rows represent the values to register.  See calculated_results_datatype for the 'Datatype' mapping of the endpoints to type.
+
+        :note:  The df.columns are just the 'Corporate Batch ID' and endpoints,
+        rows represent the values to register.  See calculated_results_datatype
+        for the 'Datatype' mapping of the endpoints to type.
+
         """
         return self._expt_df.copy()
 
     @calculated_results_df.setter
     def calculated_results_df(self, new_expt_df):
         self._expt_has_changed = self._expt_df.equals(new_expt_df)
         self._expt_df = new_expt_df
 
-
     @property
     def datatype(self):
-        """OrderedDict {(column1: datatype1), ...)} column name keys for datatype."""
+        """
+        OrderedDict {(column1: datatype1), ...)} column name keys for datatype.
+        """
         return self._datatype
+
     @datatype.setter
     def datatype(self, new_dict):
         self._datatype_has_changed = (self._datatype == new_dict)
         self._datatype = new_dict
 
-
     @property
     def calculated_results_datatype(self):
-        """OrderedDict {(column1: datatype1), ...)} column name keys for Calculated Results datatype."""
+        """
+        OrderedDict {(column1: datatype1), ...)} column name keys for
+        Calculated Results datatype.
+        """
         return self._datatype
+
     @calculated_results_datatype.setter
     def calculated_results_datatype(self, new_dict):
         self._datatype_has_changed = (self._datatype == new_dict)
         self._datatype = new_dict
 
 
 class Generic(AbstractExperiment):
     """
     Class to represent a Generic ACAS experiment file.
+
     Logical units (meta data, datatype, and calculated_results) are
     represented as separate data members.  There is some internal
     tracking to detect if the original data content is altered, but
     the datatype changes need to be updated by the caller.
+
     calculated_results_datatype - Datatype endpoint mapping.
     calculated_results_df - Calculated Results dataframe.
+
     Common formats are supported for both input and output:  csv,
     and excel
+
     API examples:
     # Read an existing file, change the 'Project' metadata and save.
     import datateam.fileio.acas as acas
     expt = acas.Generic('35250_FG_acas.csv')
     expt.project = 'Test Project'
     expt.saveAs('35250_FG_modified.xlsx')
+
     # Change the experimental values and save.
     import pandas as pd
     new_results = pd.read_csv('new_data.csv')
     expt.calculated_results_df = new_results
     expt.saveAs('replaced_data.csv')
+
     # Create new, completely empty handle, and populate it.
     expt = acas.Generic()
     expt.protocol_name = 'my super cool protocol'
     expt.experiment_name = 'ATP-Glo Assay 2020-05-19'
     expt.scientist = 'Jackson'
     expt.notebook = 'results_2020-05-19.pdf'
     expt.page = 'page 19'
@@ -469,36 +512,39 @@
     expt.calculated_results_datatype = {
         'Corporate ID': 'Datatype',
         'IC50 (nM)': 'Numeric',
         'Hill Slope': 'Numeric',
         'Assay Comment': 'Text'
     }
     expt.saveAs('my_expt.csv')
+
     """
 
     def __init__(self, file_name=None):
         """
         :param file_name: Path to the ACAS Generic Experiment file to load.
         :type file_name:  str
+
         """
 
         super().__init__(file_name)
         self._format = GENERIC
 
     def _parse(self, read_func):
         raw_df = read_func(
             self.file_name,
             header=None
         )
-        self._parseMeta(raw_df.iloc[0:self._meta_rows, [0,1]])
+        self._parseMeta(raw_df.iloc[0:self._meta_rows, [0, 1]])
 
         # Slice the 'calculated results'.
         self._expt_df = raw_df.iloc[self.RESULTS_HEADER['Datatype']+1:, :]
         self._expt_df.columns = self._expt_df.iloc[0]
         self._expt_df = self._expt_df.drop(self._expt_df.index[0])
+        self._expt_df = self._expt_df.dropna(axis='index', how='all') 
 
         # Do datatype after determining expt_df so the df.columns can be zipped.
         dt_rows = [self.RESULTS_HEADER['Datatype'], self.RESULTS_HEADER['Datatype']+1]
         datatype = raw_df.iloc[dt_rows, :]
         self._datatype = self._parseDataType(datatype)
 
         # Change tracking vars.
@@ -510,15 +556,15 @@
         meta = collections.OrderedDict([(x, '') for x in self.META_HEADER])
         for idx, row in meta_df.iterrows():
             if row[0] in meta:
                 meta[row[0]] = row[1]
             if row[0] in self.RESULTS_HEADER:
                 self.RESULTS_HEADER[row[0]] = idx
         self._experimental_meta_data = meta['Experiment Meta Data']
-        self._format = meta['Format']
+        self._format = meta['Format'].strip()
         self._protocol_name = meta['Protocol Name']
         self._experiment_name = meta['Experiment Name']
         self._scientist = meta['Scientist']
         self._notebook = meta['Notebook']
         self._page = meta['Page']
         self._assay_date = meta['Assay Date']
         self._project = meta['Project']
@@ -549,15 +595,15 @@
         meta_values = [
             self.experimental_meta_data, self.format, self.protocol_name,
             self.experiment_name, self.scientist, self.notebook, self.page,
             self.assay_date, self.project
         ]
         blanks = [self.blank, self.blank, self.blank]
         # Use zero-based numeric column name for all the logical
-        # units so they df.append() nicely.
+        # units so they df.concat() nicely.
         df_meta = pd.DataFrame(
             {
                 0: self.META_HEADER+blanks[0:2]+['Calculated Results'],
                 1: meta_values+blanks
             }
         )
         df_datatype = pd.DataFrame(
@@ -566,31 +612,38 @@
                 1: self.expt_df.columns
             }
         )
         df_expt = self.expt_df
         df_expt.columns = range(0, len(df_expt.columns))
 
         # Append the components into one output df.
-        df_out = df_meta.append(df_datatype.T, sort=True)
-        df_out = df_out.append(df_expt, ignore_index=True, sort=True)
+        df_out = pd.concat([df_meta, df_datatype.T], sort=True)
+        df_out = pd.concat([df_out, df_expt], ignore_index=True, sort=True)
 
     
         if file_type == CSV:
             output = df_out.to_csv(file_name, header=None, index=False)
         elif file_type in [XLS, XLSX]:
-            output = df_out.to_excel(file_name, header=None, index=False)
+            if file_name is None:
+                # Create excel writer object.
+                bio = io.BytesIO()
+                file_name = pd.ExcelWriter(bio, engine='openpyxl')
+            df_out.to_excel(file_name, header=None, index=False)
+            file_name.save()
+            output = bio.getvalue()
         else:
             raise ValueError(f'Unknown file type {file_type}')
         return output
 
     def validate(self):
         """
         Return True if:
             Format is 'Generic'
             expt_df.columns have a valid datatype.
+
         """
         if self.format != GENERIC:
             msg = f"Verify Format. {self.format} != {GENERIC}"
             logger.warning(msg)
             return False
         if self._datatype_has_changed or self._expt_has_changed:
             missing_datatype = []
@@ -605,28 +658,33 @@
 
 
 class DoseResponse(AbstractExperiment):
     """
     Class to represent a Dose Response ACAS experiment file, which
     has 'raw results' that describe the 'dose-response' titration
     observations.
+
     Logical units (meta data, datatype, and calculated_results,
     raw_results and raw_results_datatype) are represented as separate
     data members.  There is some internal tracking to detect if the
     original data content is altered, but the datatype changes need
     to be updated by the caller.  The 'Raw Results' string is treated
     as a dummy/spacer.
+
     Common formats are supported for both input and output:  csv,
     and excel
+
     API examples:
     import datateam.fileio.acas as acas
     expt = acas.DoseResponse('DoseResponse_Fit_Pre-Fit.xlsx')
     expt.project = 'Test Project'
     expt.saveAs('DoseResponse_Fit_Pre-Fit-out.csv')
+
     See Generic for more API examples.
+
     """
 
     RESULTS_HEADER = {
         'Calculated Results': None,
         'Datatype': None,
         'Raw Results': None,
     }
@@ -639,79 +697,106 @@
         'Michaelis-Menten',
         'Substrate Inhibition',
         'Scatter',
         'Scatter Log-x',
         'Scatter Log-y',
         'Scatter Log-x,y'
     ]
+
+    _datatype = {
+        'curve id': 'temp id',
+        'Concentration (nM)': 'x',
+        'Response': 'y',
+        'flag': 'flag'
+    }
     _meta_rows = 300  # Scan this many rows for the start of 'raw results'.
     _raw_has_changed = None
     _raw_expt_df = None
 
-
     @property
     def raw_expt_df(self):
-        """pd.DataFrame container for the experimental raw results data.  Also aliased as raw_results_df"""
+        """
+        pd.DataFrame container for the experimental raw results data.  Also
+        aliased as raw_results_df
+        """
         return self._raw_expt_df.copy()
+
     @raw_expt_df.setter
     def raw_expt_df(self, new_raw_expt_df):
         self._raw_expt_has_changed = self._raw_expt_df.equals(new_raw_expt_df)
         self._raw_expt_df = new_raw_expt_df
 
     @property
     def raw_results_df(self):
         """
         pd.DataFrame container for the experimental Raw Results data.
-        :note:  The df.columns are just the 'curve id', 'dose (units)', 'response' and 'flag', rows represent the values to register.  See raw_results_datatype for the 'temp id'  mapping of the endpoints to type.
+
+        :note:  The df.columns are just the 'curve id', 'dose (units)',
+        'response' and 'flag', rows represent the values to register.  See
+        raw_results_datatype for the 'temp id'  mapping of the endpoints to
+        type.
+
         """
         return self._raw_expt_df.copy()
+
     @raw_results_df.setter
     def raw_results_df(self, new_raw_expt_df):
-        self._raw_expt_has_changed = self._raw_expt_df.equals(new_raw_expt_df)
-        self._raw_expt_df = new_raw_expt_df
+        if self._raw_expt_df:
+            self._raw_expt_has_changed = self._raw_expt_df.equals(new_raw_expt_df)
+            self._raw_expt_df = new_raw_expt_df
+        else:
+            self._raw_expt_has_changed = True
+            self._raw_expt_df = new_raw_expt_df
+
 
     @property
     def raw_results(self):
         """OrderedDict {(column1: temp_id1), ...)} column name keys for raw results data."""
-        return self._raw_results
+        if hasattr(self, '_raw_results'):
+            return self._raw_results
+        else:
+            return self._datatype
+
     @raw_results.setter
     def raw_results(self, new_dict):
         self._raw_results_has_changed = (self._raw_results == new_dict)
         self._raw_results = new_dict
 
     @property
     def raw_results_datatype(self):
         """OrderedDict {(column1: temp_id1), ...)} column name keys for raw results data."""
         return self._raw_results
-    @raw_results.setter
-    def raw_results(self, new_dict):
-        self._raw_results_has_changed = (self._raw_results == new_dict)
+
+    @raw_results_datatype.setter
+    def raw_results_datatype(self, new_dict):
         self._raw_results = new_dict
 
     def __init__(self, file_name=None):
         """
         :param file_name: Path to the ACAS Dose Response Experiment file to load.
         :type file_name:  str
+
         """
 
         super().__init__(file_name)
         self._format = DOSE_RESPONSE
 
     def _parse(self, read_func):
         raw_df = read_func(
             self.file_name,
             header=None,
         )
-        self._parseMeta(raw_df.iloc[0:self._meta_rows, [0,1]])
+        self._parseMeta(raw_df.iloc[0:self._meta_rows, [0, 1]])
 
         # Slice the 'calculated results'.
         self._expt_df = raw_df.iloc[self.RESULTS_HEADER['Datatype']+1:self.RESULTS_HEADER['Raw Results'], :]
         self._expt_df.columns = self._expt_df.iloc[0]
         self._expt_df = self._expt_df.drop(self._expt_df.index[0])
         self._expt_df = self._expt_df.loc[:, self._expt_df.columns.notna()]
+        self._expt_df = self._expt_df.dropna(axis='index', how='all') 
 
         # Do datatype after determining expt_df so the df.columns can be zipped.
         dt_rows = [self.RESULTS_HEADER['Datatype'], self.RESULTS_HEADER['Datatype']+1]
         datatype = raw_df.iloc[dt_rows, :]
         self._datatype = self._parseDataType(datatype)
 
         # 'Raw results' row is just treated as a spacer and ignored.
@@ -737,15 +822,15 @@
         meta = collections.OrderedDict([(x, '') for x in self.META_HEADER])
         for idx, row in meta_df.iterrows():
             if row[0] in meta:
                 meta[row[0]] = row[1]
             if row[0] in self.RESULTS_HEADER:
                 self.RESULTS_HEADER[row[0]] = idx
         self._experimental_meta_data = meta['Experiment Meta Data']
-        self._format = meta['Format']
+        self._format = meta['Format'].strip()
         self._protocol_name = meta['Protocol Name']
         self._experiment_name = meta['Experiment Name']
         self._scientist = meta['Scientist']
         self._notebook = meta['Notebook']
         self._page = meta['Page']
         self._assay_date = meta['Assay Date']
         self._project = meta['Project']
@@ -760,31 +845,40 @@
         raw_results = list(raw_results.T.to_dict().values())
         raw_results = list(raw_results[0].values())
         raw_results = collections.OrderedDict(
             zip(self.raw_expt_df.columns, raw_results)
         )
         return raw_results
 
-    def saveAs(self, file_name):
+    def saveAs(self, file_name=None, file_type=None):
         """
         :param file_name: Path to output file to save record.
         :type file_name: str
+
         """
 
+        # Must provide either a file_name or a file_type but not both.
+        if file_name and file_type:
+            raise ValueError('Must provide either a file_name or a file_type but not both.')
+
+        # If file_name is provided, use it.
+        if file_name:
+            file_type = get_file_type(file_name)
+
         # Placeholder for better validation.
         self.validate()
 
         meta_values = [
             self.experimental_meta_data, self.format, self.protocol_name,
             self.experiment_name, self.scientist, self.notebook, self.page,
             self.assay_date, self.project
         ]
         blanks = [self.blank, self.blank, self.blank]
         # Use zero-based numeric column name for all the logical
-        # units so they df.append() nicely.
+        # units so they pd.concat() nicely.
         df_meta = pd.DataFrame(
             {
                 0: self.META_HEADER+blanks[0:2]+['Calculated Results'],
                 1: meta_values+blanks
             }
         )
         df_datatype = pd.DataFrame(
@@ -794,43 +888,52 @@
             }
         )
         df_expt = self.expt_df
         df_expt.columns = range(0, len(df_expt.columns))
 
         df_raw_results_header = pd.DataFrame(
             {
-                0: ['Raw Results'],
+                0: [self.blank],
+                1: ['Raw Results'],
             }
         )
         df_raw_results = pd.DataFrame(
             {
                 0: [self.raw_results.get(x) for x in self.raw_expt_df.columns],
                 1: self.raw_expt_df.columns
             }
         )
         df_raw_expt = self.raw_expt_df
         df_raw_expt.columns = range(0, len(df_raw_expt.columns))
 
         # Append the components into one output df.
-        df_out = df_meta.append(df_datatype.T, sort=True)
-        df_out = df_out.append(df_expt, ignore_index=True, sort=True)
-        df_out = df_out.append(
-            df_raw_results_header.T,
+        df_out = pd.concat([df_meta, df_datatype.T], sort=True)
+        df_out = pd.concat([df_out, df_expt], ignore_index=True, sort=True)
+        df_out = pd.concat(
+            [df_out, df_raw_results_header.T],
             ignore_index=True,
             sort=True
         )
-        df_out = df_out.append(df_raw_results.T, ignore_index=True, sort=True)
-        df_out = df_out.append(df_raw_expt, ignore_index=True, sort=True)
-        file_type = get_file_type(file_name)
+        df_out = pd.concat([df_out, df_raw_results.T], ignore_index=True, sort=True)
+        df_out = pd.concat([df_out, df_raw_expt], ignore_index=True, sort=True)
         if file_type == CSV:
-            df_out.to_csv(file_name, header=None, index=False)
+            output = df_out.to_csv(file_name, header=None, index=False)
         elif file_type in [XLS, XLSX]:
-            df_out.to_excel(file_name, header=None, index=False)
+            if file_name is None:
+                # Create excel writer object.
+                bio = io.BytesIO()
+                file_name = pd.ExcelWriter(bio, engine='openpyxl')
+                df_out.to_excel(file_name, header=None, index=False)
+                file_name.save()
+                output = bio.getvalue()
+            else:
+                output = df_out.to_excel(file_name, header=None, index=False)
         else:
-            raise ValueError(f'Unknown file type {file_name}')
+            raise ValueError(f'Unknown file type {file_type}')
+        return output
 
     def validate(self):
         """
         Return True if:
             Format is 'Dose Response'
             expt_df.columns have a valid datatype.
             TBD
```

### Comparing `acasclient-2023.1.0/acasclient/validation.py` & `acasclient-2023.2.0/acasclient/validation.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/acasclient.egg-info/PKG-INFO` & `acasclient-2023.2.0/acasclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acasclient
-Version: 2023.1.0
+Version: 2023.2.0
 Summary: ACAS API Client
 Home-page: https://github.com/mcneilco/acasclient
 Author: Brian Bolt
 Author-email: brian.bolt@boltengineered.com
 License: GNU General Public License v3
 Keywords: acasclient
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acasclient-2023.1.0/acasclient.egg-info/SOURCES.txt` & `acasclient-2023.2.0/acasclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
 tests/project_thing.py
 tests/test_acasclient.py
 tests/test_lsthing.py
+tests/test_acasclient/12_1_MultipleImage.csv
+tests/test_acasclient/12_2_MultipleImage.zip
 tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls
 tests/test_acasclient/1_1_Generic.xls
 tests/test_acasclient/1_1_Generic.xlsx
 tests/test_acasclient/1_1_Generic_empty_column.xlsx
 tests/test_acasclient/4 parameter D-R-validation-no-flags.csv
 tests/test_acasclient/4 parameter D-R-validation.csv
 tests/test_acasclient/4 parameter D-R.csv
```

### Comparing `acasclient-2023.1.0/docs/Makefile` & `acasclient-2023.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/docs/conf.py` & `acasclient-2023.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/docs/installation.rst` & `acasclient-2023.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/docs/make.bat` & `acasclient-2023.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/setup.py` & `acasclient-2023.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='acasclient',
     name='acasclient',
     packages=find_packages(include=['acasclient', 'acasclient.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mcneilco/acasclient',
-    version='2023.1.0',
+    version='2023.2.0',
     zip_safe=False,
 )
```

### Comparing `acasclient-2023.1.0/tests/project_thing.py` & `acasclient-2023.2.0/tests/project_thing.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls` & `acasclient-2023.2.0/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/1_1_Generic.xls` & `acasclient-2023.2.0/tests/test_acasclient/1_1_Generic.xls`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/1_1_Generic.xlsx` & `acasclient-2023.2.0/tests/test_acasclient/1_1_Generic.xlsx`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/1_1_Generic_empty_column.xlsx` & `acasclient-2023.2.0/tests/test_acasclient/1_1_Generic_empty_column.xlsx`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv` & `acasclient-2023.2.0/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/4 parameter D-R-validation.csv` & `acasclient-2023.2.0/tests/test_acasclient/4 parameter D-R-validation.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/4 parameter D-R.csv` & `acasclient-2023.2.0/tests/test_acasclient/4 parameter D-R.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/50k-lines.csv` & `acasclient-2023.2.0/tests/test_acasclient/50k-lines.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/blob_test.png` & `acasclient-2023.2.0/tests/test_acasclient/blob_test.png`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/dummy.pdf` & `acasclient-2023.2.0/tests/test_acasclient/dummy.pdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/dummy2.pdf` & `acasclient-2023.2.0/tests/test_acasclient/dummy2.pdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/escaped_quotes.csv` & `acasclient-2023.2.0/tests/test_acasclient/escaped_quotes.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/escaped_quotes.xls` & `acasclient-2023.2.0/tests/test_acasclient/escaped_quotes.xls`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/ibuprofen_big_lot_number.sdf` & `acasclient-2023.2.0/tests/test_acasclient/ibuprofen_big_lot_number.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/ibuprofen_methyl_ester.sdf` & `acasclient-2023.2.0/tests/test_acasclient/ibuprofen_methyl_ester.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/nci1000.sdf` & `acasclient-2023.2.0/tests/test_acasclient/nci1000.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_005_swap_parent_structures.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_005_swap_parent_structures.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_012_register_sdf.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_012_register_sdf.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_047_register_sdf_with_salts.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_047_register_sdf_with_salts.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf` & `acasclient-2023.2.0/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json` & `acasclient-2023.2.0/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json` & `acasclient-2023.2.0/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient/text_010_partial_parent_aliases.sdf` & `acasclient-2023.2.0/tests/test_acasclient/text_010_partial_parent_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.1.0/tests/test_acasclient.py` & `acasclient-2023.2.0/tests/test_acasclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 import uuid
 import json
 import operator
 import signal
 import requests
 from typing import List, Dict, Any, Optional
 from csv import DictReader
+from acasclient.experiment import Experiment
+from acasclient.acasclient import (get_entity_value_by_state_type_kind_value_type_kind)
+import zipfile
+from acasclient.selfile import Generic
 
 # Import project ls thing
 from datetime import datetime
 # Constants
 from tests.project_thing import (
     NAME_KEY, IS_RESTRICTED_KEY, STATUS_KEY, START_DATE_KEY, ACTIVE, PROJECT_NAME,
     Project
@@ -430,29 +434,138 @@
             'password': password,
             'url': self.client.url
         }
         user_client = acasclient.client(user_creds)
         return user_client
 
     # Helper for testing an experiment upload was successful
-    def experiment_load_test(self, data_file_to_upload, dry_run_mode, expect_failure=False):
+    def experiment_load_test(self, data_file_to_upload, dry_run_mode, expect_failure=False, report_file_to_upload=None, images_file_to_upload=None):
         response = self.client.\
-            experiment_loader(data_file_to_upload, "bob", dry_run_mode)
+            experiment_loader(data_file_to_upload, "bob", dry_run_mode, report_file_to_upload, images_file_to_upload)
         self.assertIn('results', response)
         self.assertIn('htmlSummary', response['results'])
         self.assertIn('errorMessages', response)
         self.assertIn('hasError', response)
         self.assertIn('hasWarning', response)
         self.assertIn('transactionId', response)
         if response['hasError'] and not expect_failure:
             raise ValueError(f"Experiment load failed unexpectedly with errorMessages: {response['errorMessages']}")
         if dry_run_mode:
             self.assertIsNone(response['transactionId'])
         else:
             self.assertIsNotNone(response['transactionId'])
+            self.assertIsNotNone(response['results']['experimentCode'])
+            experimentCode = response['results']['experimentCode']
+            experiment_dict = self.client.get_experiment_by_code(experimentCode)
+            experiment = Experiment(experiment_dict, self.client)
+
+            # Make sure the file was moved to the experiment folder by checking the file path
+            self.assertIn(experimentCode, experiment.source_file)
+
+            # Get the experiment source file
+            # Compare the source file['content'] to the data_file_to_upload content
+            # If the file['content'] is bytes then read the data_file_to_upload as bytes
+            # If the file['content'] is string then read the data_file_to_upload as string
+            source_file = experiment.get_source_file()
+            if isinstance(source_file['content'], bytes):
+                with open(data_file_to_upload, 'rb') as f:
+                    upload_bytes = f.read()
+                    self.assertEqual(source_file['content'], upload_bytes)
+            else:
+                with open(data_file_to_upload, 'r') as f:
+                    self.assertEqual(source_file['content'], f.read())
+
+            if report_file_to_upload is not None:
+                report_file = experiment.get_report_file()
+
+                # Make sure the file was moved to the experiment folder by checking the file path
+                self.assertIn(experimentCode, experiment.report_file)
+                
+                if isinstance(report_file['content'], bytes):
+                    with open(report_file_to_upload, 'rb') as f:
+                        upload_bytes = f.read()
+                        self.assertEqual(report_file['content'], upload_bytes)
+                else:
+                    with open(report_file_to_upload, 'r') as f:
+                        self.assertEqual(report_file['content'], f.read())
+
+            if images_file_to_upload is not None:
+                # The images file isn't saved as a file in the experiment, but rather each image file is saved as an analysis group value
+                # So we need to get the analysis group values and compare them to the images files
+                # Get the full experiment
+                experiment_dict = self.client.get_experiment_by_code(experimentCode, full=True)
+    
+                # Use simple experiment to read the file we uploaded
+                simple_experiment = Generic()
+                simple_experiment.loadFile(data_file_to_upload)
+                
+                # Loop through the simple_experiment._datatype  and if the value is "Image File" then get the key of the image file (lsType)
+                image_file_kinds = [k for k, v in simple_experiment._datatype.items() if v == "Image File"]
+                image_values_to_match = []
+                for image_file_kind in image_file_kinds:
+                    image_file_values = simple_experiment.calculated_results_df[image_file_kind]
+                    image_values_to_match.extend(image_file_values)
+                
+                # Now we verify that each of the imagesToMatch is in the experiment and that we can fetch the image file and it matches what we uploaded
+                experiment_value_matches = 0
+                image_zip_reconstruction_matches = 0
+                with zipfile.ZipFile(images_file_to_upload, 'r') as original_zip_ref:
+                    # We also want to verify we can reconstruct the zip from using experiment.get_images_file()
+                    saved_images_zip = experiment.get_images_file()
+                    with zipfile.ZipFile(saved_images_zip, 'r') as saved_zip_ref:
+                        # First match the experiment images to the zip file and compare the bytes and ls kinds
+                        original_zip_images = [f for f in original_zip_ref.namelist() if f.endswith(".png")]
+                        # Get all analysis group values where there is an lsType "inlineFileValue" using get_entity_value_by_state_type_kind_value_type_kind
+                        analysis_groups = experiment_dict["analysisGroups"]
+                        for ag in analysis_groups:
+                            for image_file_kind in image_file_kinds:
+                                inline_file_value = get_entity_value_by_state_type_kind_value_type_kind(ag, "data", "results", "inlineFileValue", image_file_kind)
+                                if inline_file_value is not None:
+                                    file_path = inline_file_value['fileValue']
+
+                                    # Assert that the experiment code name is in the file path to make sure it was uploaded correctly
+                                    self.assertIn(experimentCode, file_path)
+                                    
+                                    # Fetch the file from the API
+                                    file = self.client.get_file("/dataFiles/{}"
+                                                        .format(file_path))
+                                    
+                                    # Match the file name to the zip file name by file name and compare the bytes
+                                    baseName = Path(file_path).name
+                                    # Get the matching zip file
+                                    zipFile = [f for f in original_zip_images if f.endswith(baseName)]
+                                    if len(zipFile) == 0:
+                                        raise AssertionError("Could not find file {} in zip file".format(baseName))
+                                    
+                                    # Read the zipFile bytes
+                                    with original_zip_ref.open(zipFile[0]) as f:
+                                        zip_bytes = f.read()
+                                        self.assertEqual(file['content'], zip_bytes)
+                                        experiment_value_matches += 1
+                        
+                        # Now verify we can reconstruct the image zip from the experiment and make sure the zip images match the original zip images
+                        saved_zip_images = saved_zip_ref.namelist()
+                        for original_image_to_match in original_zip_images:
+                            for saved_image in saved_zip_images:
+                                if Path(original_image_to_match).name.upper() == saved_image.upper():
+                                    # Verify that the bytes match
+                                    with original_zip_ref.open(original_image_to_match) as f:
+                                        zip_bytes = f.read()
+                                        with saved_zip_ref.open(saved_image) as saved_f:
+                                            saved_zip_bytes = saved_f.read()
+                                            self.assertEqual(zip_bytes, saved_zip_bytes)
+                                            image_zip_reconstruction_matches += 1
+                                            break
+                
+                # Here we make sure we match the experiment values to the image values in the upload (which may contain multiple references to the same file)
+                self.assertEqual(experiment_value_matches, len(image_values_to_match))
+
+                # Here we match the unique set of image values as we are constructing a unique set of files in the zip
+                self.assertEqual(image_zip_reconstruction_matches, len(set(image_values_to_match)))
+
         return response
 
     def delete_all_experiments(self):
         """ Deletes all experiments """
         # Currently search is the only way to get all protocols
         self.basic_experiment_load_code = None
         protocols = self.client.protocol_search("*")
@@ -2713,33 +2826,75 @@
         sdf_string = self.client.\
             get_sdf_by_bulk_load_file(files[0]["id"])
         
         self.assertIn('<Parent Stereo Category>', sdf_string)
         self.assertIn('CMPD-0000001-001', sdf_string)
         self.assertIn('$$$$', sdf_string)
 
+    @requires_basic_cmpd_reg_load
+    def test_056_additional_assay_scientists(self):
+        """Testing additional assay scientists."""
+
+        # Test getting the current assay scientists
+        assay_scientists = self.client.get_assay_scientists()
+
+        # Verify bob is in the list
+        self.assertEqual(1, len([x for x in assay_scientists if x['code'] == 'bob']))
+
+        # Create a new assay scientist code and name using uuid
+        new_assay_scientist_code = str(uuid.uuid4())
+        new_assay_scientist_name = str(uuid.uuid4())
+
+        # Test create new scientist
+        resp = self.client.create_assay_scientist(new_assay_scientist_code, new_assay_scientist_name)
+        self.assertEqual(resp['code'], new_assay_scientist_code)
+        self.assertEqual(resp['name'], new_assay_scientist_name)
 
-def get_basic_experiment_load_file_with_project(project_code, tempdir, corp_name = None, file_name = None):
+        # Verify that the new assay scientist is in the list
+        assay_scientists = self.client.get_assay_scientists()
+        self.assertEqual(1, len([x for x in assay_scientists if x['code'] == new_assay_scientist_code]))
+
+        # Verify we can load an experiment file with the new assay scientist
+        data_file_to_upload = get_basic_experiment_load_file(self.tempdir, scientist=new_assay_scientist_code)
+
+        # This uploads the experiment and verifies the upload was successful
+        result = self.experiment_load_test(data_file_to_upload, False)
+        
+        # Fetch the experiment
+        experiment_code = result['results']['experimentCode']
+        experiment_dict = self.client.get_experiment_by_code(experiment_code)
+
+        # Verify the scientist is the same as we specified
+        experiment = Experiment(experiment_dict)
+        self.assertEqual(experiment.scientist, new_assay_scientist_code)
+
+
+def get_basic_experiment_load_file(tempdir, project_code=None, corp_name=None, file_name=None, scientist=None):
     if file_name is None:
         file_name = 'uniform-commas-with-quoted-text.csv'
     data_file_to_upload = Path(__file__).resolve()\
                         .parent.joinpath('test_acasclient', file_name)
     # Read the data file and replace the project code with the one we want
     with open(data_file_to_upload, 'r') as f:
         data_file_contents = f.read()
 
     # Replace the project code
-    data_file_contents = data_file_contents.replace('Global', project_code)
+    if project_code is not None:
+        data_file_contents = data_file_contents.replace('Global', project_code)
 
     # If corp name is specified, replace the corp name
     if corp_name is not None:
         data_file_contents = data_file_contents.replace('CMPD-0000001-001', corp_name)
 
+    # If scientist is specified, replace the scientist
+    if scientist is not None:
+        data_file_contents = data_file_contents.replace('bob', scientist)
+
     # Write the data file to the temp dir
-    file_name = f'basic-experiment-with-project-{project_code}.csv'
+    file_name = f'basic-experiment-{ str(uuid.uuid4())}.csv'
     data_file_to_upload = Path(tempdir).joinpath(file_name)
     with open(data_file_to_upload, 'w') as f:
         f.write(data_file_contents)
 
     return data_file_to_upload
 
 def csv_to_txt(data_file_to_upload, dir):
@@ -2847,29 +3002,42 @@
         # Verify we can turn off the linked lots checking
         meta_lot_dependencies = self.client.get_lot_dependencies("CMPD-0000001-001", include_linked_lots=False)
         self.assertNotIn('linkedLots', meta_lot_dependencies)
         
         # Verify that the experiment code name is in the linkedExperiments list
         self.assertIn(experiment['codeName'], [e['code'] for e in meta_lot_dependencies['linkedExperiments']])
 
+        # Verify the protocol information
+        self.assertEqual(len(meta_lot_dependencies['linkedExperiments']), 1)
+        protocol = meta_lot_dependencies['linkedExperiments'][0]['protocol']
+        self.assertIn('code', protocol)
+        self.assertEqual(protocol['name'], 'BLAH')
+
+        # Verify the analysis group information
+        self.assertEqual(len(meta_lot_dependencies['linkedExperiments']), 1)
+        item = meta_lot_dependencies['linkedExperiments'][0]['analysisGroups'][0]
+        self.assertIn('code', item)
+        self.assertIn('values', item)
+        self.assertEqual(len(item['values']), 3)
+
         # Delete the experiment and then check the meta lot dependencies again, this time the experiment should be removed from the linkedExperiments list
         self.client.delete_experiment(experiment['id'])
         meta_lot_dependencies = self.client.get_lot_dependencies("CMPD-0000001-001")
         self.assertNotIn(experiment['codeName'], [e['code'] for e in meta_lot_dependencies['linkedExperiments']])
 
         # Setup for further tests
         # Create a restricted project 
         project = self.create_basic_project_with_roles()
 
         # Bulk load a compound to the restricted project
         self.basic_cmpd_reg_load(project.code_name)
         all_lots = self.client.get_all_lots()
 
         # Load an experiment to the newly created restricted project using the global project lots
-        file_to_upload = get_basic_experiment_load_file_with_project(project.names[PROJECT_NAME], self.tempdir)
+        file_to_upload = get_basic_experiment_load_file(self.tempdir, project.names[PROJECT_NAME])
         response = self.client.\
             experiment_loader(file_to_upload, "bob", False)
         restricted_experiment_code_name = response['results']['experimentCode']
 
         # Sort lots by id and get the latest corp id
         # This is because we dont' get the corp id in the response from the bulkload
         all_lots = sorted(all_lots, key=lambda lot: lot['id'])
@@ -3123,15 +3291,15 @@
         self.assertIsNone(meta_lot)
 
         # Create a restricted lot
         restricted_lot_corp_name = self.create_restricted_lot(project.code_name)
 
         # Load an experiment to the newly created restricted project using the restricted lot
         restricted_lot_corp_name = self.create_restricted_lot(project.code_name)
-        file_to_upload = get_basic_experiment_load_file_with_project(project.names[PROJECT_NAME], self.tempdir, restricted_lot_corp_name, file_name = '4 parameter D-R.csv')
+        file_to_upload = get_basic_experiment_load_file(self.tempdir, project.names[PROJECT_NAME], restricted_lot_corp_name, file_name='4 parameter D-R.csv')
         response = self.client.\
             experiment_loader(file_to_upload, "bob", False)
         self.assertTrue(check_lot_exists_in_experiment(self, restricted_lot_corp_name, response['results']['experimentCode']))
                         
         # Deny rule: Creg admin is not an acas user
         self.assertFalse(can_delete_lot(self, cmpdreg_admin, restricted_lot_corp_name, set_owner_first=True))
  
@@ -3178,15 +3346,15 @@
 
         # # Allow Rule: Owns lot by chemist rule, has access to restricted lot project
         # restricted_lot_corp_name = self.create_restricted_lot(project.code_name)
         # self.assertTrue(can_delete_lot(self, cmpdreg_user_with_restricted_project_acls, restricted_lot_corp_name, set_owner_first=True))
 
         # # Load an experiment to the newly created restricted project using the global project lots
         # restricted_lot_corp_name = self.create_restricted_lot(project.code_name)
-        # file_to_upload = get_basic_experiment_load_file_with_project(project.names[PROJECT_NAME], self.tempdir, restricted_lot_corp_name, file_name = '4 parameter D-R.csv')
+        # file_to_upload = get_basic_experiment_load_file(self.tempdir, project.names[PROJECT_NAME], restricted_lot_corp_name, file_name = '4 parameter D-R.csv')
         # response = self.client.\
         #     experiment_loader(file_to_upload, "bob", False)
         # restricted_experiment_code_name = response['results']['experimentCode']
 
         # # Update the lot and make the cmpdreg_user_with_restricted_project_acls the chemist of the lot
         # meta_lot = self.client.get_meta_lot(restricted_lot_corp_name)
         # meta_lot["lot"]["chemist"] = cmpdreg_user_with_restricted_project_acls.username
@@ -3445,28 +3613,42 @@
         file = Path(__file__).resolve().parent.joinpath(
             'test_acasclient', 'test_005_swap_parent_structures.sdf')
         self.basic_cmpd_reg_load(file=file)
 
         # Setup constants
         corp_name = "CMPD-0000001"
         alias_1 = "alias-1"
-        test_alias = "TEST-00001"
+        test_alias = str(uuid.uuid4())
 
         # Get aliases
         aliases = self.client.get_parent_aliases(corp_name)
         self.assertEqual(len(aliases), 1)
         self.assertEquals(aliases[0], alias_1)
 
+        # Get parent alias kinds
+        parent_alias_kinds = self.client.get_parent_alias_kinds()
+        self.assertGreater(len(parent_alias_kinds), 0)
+        alias_type = parent_alias_kinds[0]["kindName"]
+        alias_kind = parent_alias_kinds[0]["lsType"]['typeName']
+
         # Add an alias
-        self.client.add_parent_alias(corp_name, test_alias)
+        meta_lot = self.client.add_parent_alias(corp_name, test_alias, alias_type, alias_kind)
         aliases = self.client.get_parent_aliases(corp_name)
         self.assertEqual(len(aliases), 2)
         self.assertIn(alias_1, aliases)
         self.assertIn(test_alias, aliases)
 
+        # Check the metalot and verify that the test_alias with the same type and kind was added
+        parent_aliases = meta_lot["lot"]['saltForm']['parent']['parentAliases']
+        has_test_alias = False
+        for parent_alias in parent_aliases:
+            if parent_alias["aliasName"] == test_alias and parent_alias["lsType"] == alias_type and parent_alias["lsKind"] == alias_kind:
+                has_test_alias = True
+        self.assertTrue(has_test_alias)
+
         # Set the aliases to only the test alias
         self.client.set_parent_aliases(corp_name, [test_alias])
         aliases = self.client.get_parent_aliases(corp_name)
         self.assertEqual(len(aliases), 1)
         self.assertEquals(aliases[0], test_alias)
     
     @requires_absent_basic_cmpd_reg_load
@@ -4345,7 +4527,26 @@
         accepted_results_analysis_groups = anonymize_experiment_dict(accepted_results_experiment)["analysisGroups"]
         new_results_analysis_groups = experiment["analysisGroups"]
 
         # Verify that the analysis groups are the same as the accepted results analysis groups
         # Groups should have been sorted by the "Key" analysis group value uploaded in the dose response file
         for i in range(len(accepted_results_analysis_groups)):
             self.assertDictEqual(accepted_results_analysis_groups[i], new_results_analysis_groups[i])
+
+    @requires_basic_cmpd_reg_load
+    def test_017_report_file(self):
+        """Test experiment loader with report file."""
+        data_file_to_upload = Path(__file__).resolve()\
+            .parent.joinpath('test_acasclient', 'uniform-commas-with-quoted-text.csv')
+        report_file_path = Path(__file__).resolve().parent\
+            .joinpath('test_acasclient', 'dummy.pdf')
+        self.experiment_load_test(data_file_to_upload, True, report_file_to_upload=report_file_path)
+        self.experiment_load_test(data_file_to_upload, False, report_file_to_upload=report_file_path)
+
+    @requires_basic_cmpd_reg_load
+    def test_018_image_file(self):
+        """Test experiment loader with image file."""
+        data_file_to_upload = Path(__file__).resolve()\
+            .parent.joinpath('test_acasclient', '12_1_MultipleImage.csv')
+        image_file_path = Path(__file__).resolve().parent\
+            .joinpath('test_acasclient', '12_2_MultipleImage.zip')
+        self.experiment_load_test(data_file_to_upload, False, images_file_to_upload=image_file_path)
```

### Comparing `acasclient-2023.1.0/tests/test_lsthing.py` & `acasclient-2023.2.0/tests/test_lsthing.py`

 * *Files identical despite different names*

