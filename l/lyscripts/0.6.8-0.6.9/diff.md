# Comparing `tmp/lyscripts-0.6.8.tar.gz` & `tmp/lyscripts-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyscripts-0.6.8.tar", last modified: Tue May 30 08:43:50 2023, max compression
+gzip compressed data, was "lyscripts-0.6.9.tar", last modified: Wed Jun 21 08:33:34 2023, max compression
```

## Comparing `lyscripts-0.6.8.tar` & `lyscripts-0.6.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.431637 lyscripts-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-30 08:43:34.000000 lyscripts-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-30 08:43:34.000000 lyscripts-0.6.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 08:43:34.000000 lyscripts-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-30 08:43:50.439637 lyscripts-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-30 08:43:34.000000 lyscripts-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-30 08:43:34.000000 lyscripts-0.6.8/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   105407 2023-05-30 08:43:34.000000 lyscripts-0.6.8/github-social-card.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts/app/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/app/prevalence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/enhance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/join.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/lyproxify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/lyscripts/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/corner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/histograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/thermo_int.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/lyscripts/predict/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/prevalences.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/risks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/predict/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/temp_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-05-30 08:43:34.000000 lyscripts-0.6.8/lyscripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.435637 lyscripts-0.6.8/lyscripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 08:43:50.000000 lyscripts-0.6.8/lyscripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 08:43:34.000000 lyscripts-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:43:50.439637 lyscripts-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:43:34.000000 lyscripts-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/plot/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/sine.png
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/sine.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/sine_svg.png
--rw-r--r--   0 runner    (1001) docker     (123)    36976 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/baseline/test_draw.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/plot/data/
--rw-r--r--   0 runner    (1001) docker     (123)    86144 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/data/beta_samples.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/plot/plot_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:50.439637 lyscripts-0.6.8/tests/predict/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/predict/predict_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/predict/prevalences_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/run_doctests.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/test_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 08:43:34.000000 lyscripts-0.6.8/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.435683 lyscripts-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.427682 lyscripts-0.6.9/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-06-21 08:33:17.000000 lyscripts-0.6.9/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-06-21 08:33:17.000000 lyscripts-0.6.9/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.423683 lyscripts-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.427682 lyscripts-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 08:33:17.000000 lyscripts-0.6.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-21 08:33:17.000000 lyscripts-0.6.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 08:33:17.000000 lyscripts-0.6.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-21 08:33:17.000000 lyscripts-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-21 08:33:17.000000 lyscripts-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-21 08:33:17.000000 lyscripts-0.6.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 08:33:17.000000 lyscripts-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-21 08:33:34.435683 lyscripts-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-21 08:33:17.000000 lyscripts-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-06-21 08:33:17.000000 lyscripts-0.6.9/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105407 2023-06-21 08:33:17.000000 lyscripts-0.6.9/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.427682 lyscripts-0.6.9/lyscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 08:33:34.000000 lyscripts-0.6.9/lyscripts/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.427682 lyscripts-0.6.9/lyscripts/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/app/prevalence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.431683 lyscripts-0.6.9/lyscripts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/lyproxify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.431683 lyscripts-0.6.9/lyscripts/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/plot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/plot/corner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/plot/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/plot/thermo_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.431683 lyscripts-0.6.9/lyscripts/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/predict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/predict/prevalences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/predict/risks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/predict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/temp_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-06-21 08:33:17.000000 lyscripts-0.6.9/lyscripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.427682 lyscripts-0.6.9/lyscripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-21 08:33:34.000000 lyscripts-0.6.9/lyscripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-21 08:33:34.000000 lyscripts-0.6.9/lyscripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:33:34.000000 lyscripts-0.6.9/lyscripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 08:33:34.000000 lyscripts-0.6.9/lyscripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-21 08:33:34.000000 lyscripts-0.6.9/lyscripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 08:33:34.000000 lyscripts-0.6.9/lyscripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-21 08:33:17.000000 lyscripts-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:33:34.435683 lyscripts-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:33:17.000000 lyscripts-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.431683 lyscripts-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.431683 lyscripts-0.6.9/tests/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.431683 lyscripts-0.6.9/tests/plot/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/plot/baseline/sine.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/plot/baseline/sine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/plot/baseline/sine_svg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36976 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/plot/baseline/test_draw.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.435683 lyscripts-0.6.9/tests/plot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    86144 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/plot/data/beta_samples.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/plot/plot_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:33:34.435683 lyscripts-0.6.9/tests/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/predict/predict_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/predict/prevalences_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/run_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/test_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-21 08:33:17.000000 lyscripts-0.6.9/tests/utils_test.py
```

### Comparing `lyscripts-0.6.8/.chglog/CHANGELOG.tpl.md` & `lyscripts-0.6.9/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/.chglog/config.yml` & `lyscripts-0.6.9/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/.github/workflows/build.yml` & `lyscripts-0.6.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/.github/workflows/docs.yml` & `lyscripts-0.6.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/.github/workflows/tests.yml` & `lyscripts-0.6.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/.gitignore` & `lyscripts-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/.pre-commit-config.yaml` & `lyscripts-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/CHANGELOG.md` & `lyscripts-0.6.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+<a name="0.6.9"></a>
+## [0.6.9] - 2023-06-21
+
+### Bug Fixes
+- change the indentation length in the generated markdown data documentation to 4 spaces. Fixes [#41].
+
+
 <a name="0.6.8"></a>
 ## [0.6.8] - 2023-05-30
 
 ### Bug Fixes
 - flattening error in `lyproxify`
 - more robust lyproxify working again
 
@@ -253,15 +260,16 @@
 - set up git-chglog for creating changelogs
 - add pre-commit hook to check commit msg
 
 
 <a name="0.5.3"></a>
 ## [0.5.3] - 2022-08-22
 
-[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/0.6.8...HEAD
+[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/0.6.9...HEAD
+[0.6.9]: https://github.com/rmnldwg/lyscripts/compare/0.6.8...0.6.9
 [0.6.8]: https://github.com/rmnldwg/lyscripts/compare/0.6.7...0.6.8
 [0.6.7]: https://github.com/rmnldwg/lyscripts/compare/0.6.6...0.6.7
 [0.6.6]: https://github.com/rmnldwg/lyscripts/compare/0.6.5...0.6.6
 [0.6.5]: https://github.com/rmnldwg/lyscripts/compare/0.6.4...0.6.5
 [0.6.4]: https://github.com/rmnldwg/lyscripts/compare/0.6.3...0.6.4
 [0.6.3]: https://github.com/rmnldwg/lyscripts/compare/0.6.2...0.6.3
 [0.6.2]: https://github.com/rmnldwg/lyscripts/compare/0.6.1...0.6.2
@@ -287,12 +295,13 @@
 [#20]: https://github.com/rmnldwg/lyscripts/issues/20
 [#21]: https://github.com/rmnldwg/lyscripts/issues/21
 [#23]: https://github.com/rmnldwg/lyscripts/issues/23
 [#25]: https://github.com/rmnldwg/lyscripts/issues/25
 [#30]: https://github.com/rmnldwg/lyscripts/issues/30
 [#31]: https://github.com/rmnldwg/lyscripts/issues/31
 [#33]: https://github.com/rmnldwg/lyscripts/issues/33
+[#41]: https://github.com/rmnldwg/lyscripts/issues/41
 
 [`emcee`]: https://emcee.readthedocs.io/en/stable/
 [`rich`]: https://rich.readthedocs.io/en/latest/
 [`rich_argparse`]: https://github.com/hamdanal/rich_argparse
 [LyProX]: https://lyprox.org
```

### Comparing `lyscripts-0.6.8/LICENSE` & `lyscripts-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/PKG-INFO` & `lyscripts-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.6.8
+Version: 0.6.9
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lyscripts-0.6.8/README.md` & `lyscripts-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/favicon.png` & `lyscripts-0.6.9/favicon.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/github-social-card.png` & `lyscripts-0.6.9/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/__init__.py` & `lyscripts-0.6.9/lyscripts/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/app/__init__.py` & `lyscripts-0.6.9/lyscripts/app/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/app/prevalence.py` & `lyscripts-0.6.9/lyscripts/app/prevalence.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/__init__.py` & `lyscripts-0.6.9/lyscripts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/__main__.py` & `lyscripts-0.6.9/lyscripts/data/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/clean.py` & `lyscripts-0.6.9/lyscripts/data/clean.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/enhance.py` & `lyscripts-0.6.9/lyscripts/data/enhance.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/generate.py` & `lyscripts-0.6.9/lyscripts/data/generate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/join.py` & `lyscripts-0.6.9/lyscripts/data/join.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/lyproxify.py` & `lyscripts-0.6.9/lyscripts/data/lyproxify.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
             "Leaf of column map must be a dictionary with 'func' or 'default' key."
         )
 
 
 def generate_markdown_docs(
     nested_column_map: Dict[Tuple, Dict[str, Any]],
     depth: int = 0,
+    indent_len: int = 4,
 ) -> str:
     """
     Generate a markdown nested, ordered list as documentation for the column map.
 
     A key in the doctionary is supposed to be documented, when its value is a dictionary
     containing a `"__doc__"` key.
 
@@ -154,25 +155,26 @@
     ...             "__doc__": "age of the patient",
     ...             "func": int,
     ...             "columns": ["age"],
     ...         },
     ...     },
     ... }
     >>> generate_markdown_docs(nested_column_map)
-    '1. **`patient`**: some patient info\\n   1. **`age`**: age of the patient\\n'
+    '1. **`patient:`** some patient info\\n    1. **`age:`** age of the patient\\n'
     """
     md_docs = ""
+    indent = " " * indent_len * depth
     i = 1
     for key, value in nested_column_map.items():
         if isinstance(value, dict):
             if "__doc__" in value:
-                md_docs += f"{'   ' * depth}{i}. **`{key}`**: {value['__doc__']}\n"
+                md_docs += f"{indent}{i}. **`{key}:`** {value['__doc__']}\n"
                 i += 1
 
-            md_docs += generate_markdown_docs(value, depth + 1)
+            md_docs += generate_markdown_docs(value, depth + 1, indent_len)
 
     return md_docs
 
 
 @report_state(
     status_msg="Transform raw data to LyProX style table...",
     success_msg="Transformed raw data to LyProX style table.",
```

### Comparing `lyscripts-0.6.8/lyscripts/data/split.py` & `lyscripts-0.6.9/lyscripts/data/split.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/data/utils.py` & `lyscripts-0.6.9/lyscripts/data/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/evaluate.py` & `lyscripts-0.6.9/lyscripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/plot/__init__.py` & `lyscripts-0.6.9/lyscripts/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/plot/__main__.py` & `lyscripts-0.6.9/lyscripts/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/plot/corner.py` & `lyscripts-0.6.9/lyscripts/plot/corner.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/plot/histograms.py` & `lyscripts-0.6.9/lyscripts/plot/histograms.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/plot/thermo_int.py` & `lyscripts-0.6.9/lyscripts/plot/thermo_int.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/plot/utils.py` & `lyscripts-0.6.9/lyscripts/plot/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/predict/__init__.py` & `lyscripts-0.6.9/lyscripts/predict/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/predict/__main__.py` & `lyscripts-0.6.9/lyscripts/predict/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/predict/prevalences.py` & `lyscripts-0.6.9/lyscripts/predict/prevalences.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/predict/risks.py` & `lyscripts-0.6.9/lyscripts/predict/risks.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/predict/utils.py` & `lyscripts-0.6.9/lyscripts/predict/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/sample.py` & `lyscripts-0.6.9/lyscripts/sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/temp_schedule.py` & `lyscripts-0.6.9/lyscripts/temp_schedule.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts/utils.py` & `lyscripts-0.6.9/lyscripts/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/lyscripts.egg-info/PKG-INFO` & `lyscripts-0.6.9/lyscripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.6.8
+Version: 0.6.9
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lyscripts-0.6.8/lyscripts.egg-info/SOURCES.txt` & `lyscripts-0.6.9/lyscripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/pyproject.toml` & `lyscripts-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/_sample.py` & `lyscripts-0.6.9/tests/_sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/plot/baseline/sine.png` & `lyscripts-0.6.9/tests/plot/baseline/sine.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/plot/baseline/sine.svg` & `lyscripts-0.6.9/tests/plot/baseline/sine.svg`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/plot/baseline/sine_svg.png` & `lyscripts-0.6.9/tests/plot/baseline/sine_svg.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/plot/baseline/test_draw.png` & `lyscripts-0.6.9/tests/plot/baseline/test_draw.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/plot/data/beta_samples.hdf5` & `lyscripts-0.6.9/tests/plot/data/beta_samples.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/plot/plot_utils_test.py` & `lyscripts-0.6.9/tests/plot/plot_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/predict/predict_utils_test.py` & `lyscripts-0.6.9/tests/predict/predict_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/predict/prevalences_test.py` & `lyscripts-0.6.9/tests/predict/prevalences_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/test_params.yaml` & `lyscripts-0.6.9/tests/test_params.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.8/tests/utils_test.py` & `lyscripts-0.6.9/tests/utils_test.py`

 * *Files identical despite different names*

