# Comparing `tmp/soam-0.9.3.tar.gz` & `tmp/soam-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soam-0.9.3.tar", last modified: Fri Aug 13 23:03:26 2021, max compression
+gzip compressed data, was "dist/soam-0.9.4.tar", last modified: Tue Aug 31 23:47:21 2021, max compression
```

## Comparing `soam-0.9.3.tar` & `soam-0.9.4.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.986267 soam-0.9.3/
--rw-r--r--   0 root         (0) root         (0)    14152 2021-08-13 23:03:26.986267 soam-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11294 2021-08-13 23:01:44.000000 soam-0.9.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      589 2021-08-13 23:01:44.000000 soam-0.9.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1325 2021-08-13 23:03:26.987267 soam-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3171 2021-08-13 23:01:44.000000 soam-0.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.911260 soam-0.9.3/soam/
--rw-rw-rw-   0 root         (0) root         (0)       38 2021-08-13 23:01:44.000000 soam-0.9.3/soam/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4471 2021-08-13 23:01:44.000000 soam-0.9.3/soam/cfg.py
--rw-rw-rw-   0 root         (0) root         (0)     3793 2021-08-13 23:01:44.000000 soam-0.9.3/soam/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.915260 soam-0.9.3/soam/core/
--rw-rw-rw-   0 root         (0) root         (0)       88 2021-08-13 23:01:44.000000 soam-0.9.3/soam/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2897 2021-08-13 23:01:44.000000 soam-0.9.3/soam/core/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2021-08-13 23:01:44.000000 soam-0.9.3/soam/core/step.py
--rw-rw-rw-   0 root         (0) root         (0)     4699 2021-08-13 23:01:44.000000 soam-0.9.3/soam/data_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.920260 soam-0.9.3/soam/models/
--rw-rw-rw-   0 root         (0) root         (0)      138 2021-08-13 23:01:44.000000 soam-0.9.3/soam/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3360 2021-08-13 23:01:44.000000 soam-0.9.3/soam/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3785 2021-08-13 23:01:44.000000 soam-0.9.3/soam/models/exponential.py
--rw-rw-rw-   0 root         (0) root         (0)     4170 2021-08-13 23:01:44.000000 soam-0.9.3/soam/models/orbit.py
--rw-rw-rw-   0 root         (0) root         (0)     4157 2021-08-13 23:01:44.000000 soam-0.9.3/soam/models/prophet.py
--rw-rw-rw-   0 root         (0) root         (0)     4035 2021-08-13 23:01:44.000000 soam-0.9.3/soam/models/sarimax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.923261 soam-0.9.3/soam/plotting/
--rw-rw-rw-   0 root         (0) root         (0)       21 2021-08-13 23:01:44.000000 soam-0.9.3/soam/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2021-08-13 23:01:44.000000 soam-0.9.3/soam/plotting/forecast_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)     8469 2021-08-13 23:01:44.000000 soam-0.9.3/soam/plotting/plot_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.927261 soam-0.9.3/soam/reporting/
--rw-rw-rw-   0 root         (0) root         (0)      149 2021-08-13 23:01:44.000000 soam-0.9.3/soam/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2021-08-13 23:01:44.000000 soam-0.9.3/soam/reporting/gsheets_report.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2021-08-13 23:01:44.000000 soam-0.9.3/soam/reporting/mail_report.py
--rw-rw-rw-   0 root         (0) root         (0)     3624 2021-08-13 23:01:44.000000 soam-0.9.3/soam/reporting/pdf_report.py
--rw-rw-rw-   0 root         (0) root         (0)    11381 2021-08-13 23:01:44.000000 soam-0.9.3/soam/reporting/slack_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.930261 soam-0.9.3/soam/savers/
--rw-rw-rw-   0 root         (0) root         (0)       19 2021-08-13 23:01:44.000000 soam-0.9.3/soam/savers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2021-08-13 23:01:44.000000 soam-0.9.3/soam/savers/csv_saver.py
--rw-rw-rw-   0 root         (0) root         (0)     4332 2021-08-13 23:01:44.000000 soam-0.9.3/soam/savers/db_saver.py
--rw-rw-rw-   0 root         (0) root         (0)     1786 2021-08-13 23:01:44.000000 soam-0.9.3/soam/savers/savers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.933261 soam-0.9.3/soam/utilities/
--rw-rw-rw-   0 root         (0) root         (0)       22 2021-08-13 23:01:44.000000 soam-0.9.3/soam/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7556 2021-08-13 23:01:44.000000 soam-0.9.3/soam/utilities/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     9320 2021-08-13 23:01:44.000000 soam-0.9.3/soam/utilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.966265 soam-0.9.3/soam/workflow/
--rw-rw-rw-   0 root         (0) root         (0)      484 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/anomalies.py
--rw-rw-rw-   0 root         (0) root         (0)    14254 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/backtester.py
--rw-rw-rw-   0 root         (0) root         (0)     3609 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/forecaster.py
--rw-rw-rw-   0 root         (0) root         (0)     2397 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/merge_concat.py
--rw-rw-rw-   0 root         (0) root         (0)     5416 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/slicer.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/store.py
--rw-rw-rw-   0 root         (0) root         (0)    20165 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/time_series_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     5684 2021-08-13 23:01:44.000000 soam-0.9.3/soam/workflow/transformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.913260 soam-0.9.3/soam.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14152 2021-08-13 23:03:26.000000 soam-0.9.3/soam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1869 2021-08-13 23:03:26.000000 soam-0.9.3/soam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-13 23:03:26.000000 soam-0.9.3/soam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2021-08-13 23:03:26.000000 soam-0.9.3/soam.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1515 2021-08-13 23:03:26.000000 soam-0.9.3/soam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-08-13 23:03:26.000000 soam-0.9.3/soam.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.968265 soam-0.9.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)       18 2021-08-13 23:01:44.000000 soam-0.9.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2021-08-13 23:01:44.000000 soam-0.9.3/tests/db_test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2021-08-13 23:01:44.000000 soam-0.9.3/tests/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.970265 soam-0.9.3/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)       30 2021-08-13 23:01:44.000000 soam-0.9.3/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7489 2021-08-13 23:01:44.000000 soam-0.9.3/tests/integration/test_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.971265 soam-0.9.3/tests/mlflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-13 23:01:44.000000 soam-0.9.3/tests/mlflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2021-08-13 23:01:44.000000 soam-0.9.3/tests/mlflow/test_mlflow_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.975266 soam-0.9.3/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)       25 2021-08-13 23:01:44.000000 soam-0.9.3/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2021-08-13 23:01:44.000000 soam-0.9.3/tests/models/test_exponential.py
--rw-rw-rw-   0 root         (0) root         (0)     2198 2021-08-13 23:01:44.000000 soam-0.9.3/tests/models/test_orbit.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2021-08-13 23:01:44.000000 soam-0.9.3/tests/models/test_sarimax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.976266 soam-0.9.3/tests/plotting/
--rw-rw-rw-   0 root         (0) root         (0)       31 2021-08-13 23:01:44.000000 soam-0.9.3/tests/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2460 2021-08-13 23:01:44.000000 soam-0.9.3/tests/plotting/test_forecast_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.978266 soam-0.9.3/tests/utilities/
--rw-rw-rw-   0 root         (0) root         (0)       28 2021-08-13 23:01:44.000000 soam-0.9.3/tests/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9265 2021-08-13 23:01:44.000000 soam-0.9.3/tests/utilities/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-13 23:03:26.985267 soam-0.9.3/tests/workflow/
--rw-rw-rw-   0 root         (0) root         (0)       27 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2791 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_anomalies.py
--rw-rw-rw-   0 root         (0) root         (0)    16775 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_backtester.py
--rw-rw-rw-   0 root         (0) root         (0)     3054 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_forecaster.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_mergeconcat.py
--rw-rw-rw-   0 root         (0) root         (0)     5294 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_slicer.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_store.py
--rw-rw-rw-   0 root         (0) root         (0)    28691 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_time_series_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2021-08-13 23:01:44.000000 soam-0.9.3/tests/workflow/test_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.881109 soam-0.9.4/
+-rw-r--r--   0 root         (0) root         (0)    14700 2021-08-31 23:47:21.881109 soam-0.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11786 2021-08-31 23:45:39.000000 soam-0.9.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      589 2021-08-31 23:45:39.000000 soam-0.9.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2021-08-31 23:47:21.882109 soam-0.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3087 2021-08-31 23:45:39.000000 soam-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.800102 soam-0.9.4/soam/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2021-08-31 23:45:39.000000 soam-0.9.4/soam/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4471 2021-08-31 23:45:39.000000 soam-0.9.4/soam/cfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2021-08-31 23:45:39.000000 soam-0.9.4/soam/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.804102 soam-0.9.4/soam/core/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2021-08-31 23:45:39.000000 soam-0.9.4/soam/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2897 2021-08-31 23:45:39.000000 soam-0.9.4/soam/core/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2021-08-31 23:45:39.000000 soam-0.9.4/soam/core/step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4699 2021-08-31 23:45:39.000000 soam-0.9.4/soam/data_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.811103 soam-0.9.4/soam/models/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2021-08-31 23:45:39.000000 soam-0.9.4/soam/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2021-08-31 23:45:39.000000 soam-0.9.4/soam/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3785 2021-08-31 23:45:39.000000 soam-0.9.4/soam/models/exponential.py
+-rw-rw-rw-   0 root         (0) root         (0)     4170 2021-08-31 23:45:39.000000 soam-0.9.4/soam/models/orbit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4157 2021-08-31 23:45:39.000000 soam-0.9.4/soam/models/prophet.py
+-rw-rw-rw-   0 root         (0) root         (0)     4035 2021-08-31 23:45:39.000000 soam-0.9.4/soam/models/sarimax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.814103 soam-0.9.4/soam/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2021-08-31 23:45:39.000000 soam-0.9.4/soam/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2021-08-31 23:45:39.000000 soam-0.9.4/soam/plotting/forecast_plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)     8469 2021-08-31 23:45:39.000000 soam-0.9.4/soam/plotting/plot_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.820104 soam-0.9.4/soam/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2021-08-31 23:45:39.000000 soam-0.9.4/soam/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2021-08-31 23:45:39.000000 soam-0.9.4/soam/reporting/gsheets_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2021-08-31 23:45:39.000000 soam-0.9.4/soam/reporting/mail_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     3624 2021-08-31 23:45:39.000000 soam-0.9.4/soam/reporting/pdf_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    11381 2021-08-31 23:45:39.000000 soam-0.9.4/soam/reporting/slack_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.824104 soam-0.9.4/soam/savers/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2021-08-31 23:45:39.000000 soam-0.9.4/soam/savers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2021-08-31 23:45:39.000000 soam-0.9.4/soam/savers/csv_saver.py
+-rw-rw-rw-   0 root         (0) root         (0)     4332 2021-08-31 23:45:39.000000 soam-0.9.4/soam/savers/db_saver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2021-08-31 23:45:39.000000 soam-0.9.4/soam/savers/savers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.827104 soam-0.9.4/soam/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2021-08-31 23:45:39.000000 soam-0.9.4/soam/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7556 2021-08-31 23:45:39.000000 soam-0.9.4/soam/utilities/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     9320 2021-08-31 23:45:39.000000 soam-0.9.4/soam/utilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.836105 soam-0.9.4/soam/workflow/
+-rw-rw-rw-   0 root         (0) root         (0)      484 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/anomalies.py
+-rw-rw-rw-   0 root         (0) root         (0)    14254 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/backtester.py
+-rw-rw-rw-   0 root         (0) root         (0)     3609 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/forecaster.py
+-rw-rw-rw-   0 root         (0) root         (0)     2397 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/merge_concat.py
+-rw-rw-rw-   0 root         (0) root         (0)     5416 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/slicer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/store.py
+-rw-rw-rw-   0 root         (0) root         (0)    20165 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/time_series_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2021-08-31 23:45:39.000000 soam-0.9.4/soam/workflow/transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.802102 soam-0.9.4/soam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14700 2021-08-31 23:47:21.000000 soam-0.9.4/soam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1838 2021-08-31 23:47:21.000000 soam-0.9.4/soam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-31 23:47:21.000000 soam-0.9.4/soam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1509 2021-08-31 23:47:21.000000 soam-0.9.4/soam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2021-08-31 23:47:21.000000 soam-0.9.4/soam.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.839105 soam-0.9.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2021-08-31 23:45:39.000000 soam-0.9.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2021-08-31 23:45:39.000000 soam-0.9.4/tests/db_test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2748 2021-08-31 23:45:39.000000 soam-0.9.4/tests/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.841106 soam-0.9.4/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2021-08-31 23:45:39.000000 soam-0.9.4/tests/integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7489 2021-08-31 23:45:39.000000 soam-0.9.4/tests/integration/test_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.842106 soam-0.9.4/tests/mlflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 23:45:39.000000 soam-0.9.4/tests/mlflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2021-08-31 23:45:39.000000 soam-0.9.4/tests/mlflow/test_mlflow_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.846106 soam-0.9.4/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2021-08-31 23:45:39.000000 soam-0.9.4/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2021-08-31 23:45:39.000000 soam-0.9.4/tests/models/test_exponential.py
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2021-08-31 23:45:39.000000 soam-0.9.4/tests/models/test_orbit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2021-08-31 23:45:39.000000 soam-0.9.4/tests/models/test_sarimax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.848106 soam-0.9.4/tests/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2021-08-31 23:45:39.000000 soam-0.9.4/tests/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2460 2021-08-31 23:45:39.000000 soam-0.9.4/tests/plotting/test_forecast_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.850107 soam-0.9.4/tests/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2021-08-31 23:45:39.000000 soam-0.9.4/tests/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9265 2021-08-31 23:45:39.000000 soam-0.9.4/tests/utilities/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 23:47:21.880109 soam-0.9.4/tests/workflow/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_anomalies.py
+-rw-rw-rw-   0 root         (0) root         (0)    16775 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_backtester.py
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_forecaster.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_mergeconcat.py
+-rw-rw-rw-   0 root         (0) root         (0)     5294 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_slicer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    28691 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_time_series_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2021-08-31 23:45:39.000000 soam-0.9.4/tests/workflow/test_transformer.py
```

### Comparing `soam-0.9.3/PKG-INFO` & `soam-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soam
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tools for time series analysis, plotting and reporting.
 Home-page: UNKNOWN
 Author: Mutt Data
 Author-email: info@muttdata.ai
 License: UNKNOWN
 Description: # SoaM
         
@@ -12,51 +12,55 @@
         
         SoaM is a [Prefect](https://docs.prefect.io/) based library created by [Mutt](https://muttdata.ai/).
         Its goal is to create a forecasting framework, this tool is developed with conjunctions of experience on previous
         projects. There come the name: Son of a Mutt = SoaM
         
         ## SoaM pipeline
         
-        ```mermaid
+        <!-- gfmd-start -->
+        ![Mermaid diagram](https://kroki.io/mermaid/svg/eNpljbEOgjAURXe_4o0wEBQQnJzUxEQSIm6EocITmwAlrx1MCP-uloIkdnu959xbEeuecLmu4PN4uc6sA1PsziTC2c4dZ89LL3NTwWK48QYhReIo4fhSxAolyM2NuVmas2pCT1_-VESslQ9BDf50XxOBIU6CsGBSLYBt30-_vK0gFiXWwzBaBgn0FWaW7kgIS14oLlppTyWhJqK_FUhqoZZrI7gz4BU7Qd_ZOY_G_A05RWCs)
+        
+        <details>
+        <summary><sup><sub>Diagram source code</sub></sup></summary>
         
-           graph LR
+        ```mermaid
+        graph LR
             id0[(Database I)]-->id2[/SoaM Time Series Extractor/]
             id1[(Database II)]-->id2
             id2-->id3[/SoaM Transformer/]
             id3-->id4[/SoaM Forecaster/]
             id5{{Forecasting Model}}-->id4
             id4-->id6[(SoaM Predictions)]
             id6-->id7[/SoaM Forecaster Plotter/]
             id6-->id8[/SoaM Reporting/]
             id7-->id8
         ```
-        
+        </details>
+        <!-- gfmd-end -->
         This library pipeline supports any data source.
         The process is structured in different stages:
         * Extraction: manages the granularity and aggregation of the input data.
         * Preprocessing: lets select among out of the box tools to perform standard tasks as normalization or fill nan values.
         * Forecasting: fits a model and predict results.
         * Postprocessing: modifies the results based on business/real information or create analysis with the predicted values,
-         such as an anomaly detection.
+        such as an anomaly detection.
         
         ## Overview of the Steps Run in SoaM
         
         ### Extraction
         This stage extracts data from the needed sources to build the condensed dataset for the next steps. This tends to be
         project dependent. Then it converts the full dataset to the desired time granularity and aggregation level by some categorical attribute/s.
         
         ### Preprocessing
         This step implements functions to further cleanup and prepare the data for the following steps, such as:
         * Add feature/transformation
         * Fill nan values
         * Apply value normalizations
         * Shift values
         
-        [//comment]: # (the preprocessing supports custom transformations?)
-        
         ### Forecasting
         This stage receives the clean data, performs the forecast and store the predicted values in the defined storages.
         Currently there are implementations to store in CSV files and SQL databases.
         A variety of models are currently supported to fit and predict data. They can be extended to create custom ones.
         * [Exponential Smoothing](https://www.statsmodels.org/stable/examples/notebooks/generated/exponential_smoothing.html)
         * [Orbit DLT Full](https://orbit-ml.readthedocs.io/en/latest/tutorials/dlt.html)
         * [Prophet](https://pypi.org/project/fbprophet)
@@ -67,34 +71,45 @@
         To do backtesting the data is splited in train and validation, there are two spliting methods:
         - Sliding: create a fixed size window for the training data that ends at the beginning of the validation data.
         - Expanding: create the training data from remaining data since the start of the series until the validation data.
         
         For more information review this document: [backtesting at scale](https://eng.uber.com/backtesting-at-scale/)
         
         ### Postprocessing
-        [//comment]: # (TODO: explain postprocessing stage chaining)
         This last stage is prepared to work on the forecasts generated by the pipeline. For example:
         * Clip/Cleanup the predictions.
         * Perform further analyses (such as anomaly detection).
         * Export reports.
         
-        [//comment]: # (does the postprocessing support custom outputs?)
-        
         ## Table of Contents
-        - [Installation](#installation)
-        - [Quick start](#quick-start)
-        - [Usage](#usage)
-        - [Soam CLI](#soam-cli)
-        - [Database Management](#database-management)
-        - [Developers Guide](#developers-guide)
-        - [Testing](#testing)
-        - [Contributing](#contributing)
-        - [Rules of Thumb](#rules-of-thumb)
-        - [Credits](#contributing)
-        - [License](#license)
+        - [SoaM](#soam)
+          - [SoaM pipeline](#soam-pipeline)
+          - [Overview of the Steps Run in SoaM](#overview-of-the-steps-run-in-soam)
+            - [Extraction](#extraction)
+            - [Preprocessing](#preprocessing)
+            - [Forecasting](#forecasting)
+            - [Backtesting](#backtesting)
+              - [Window policies](#window-policies)
+            - [Postprocessing](#postprocessing)
+          - [Table of Contents](#table-of-contents)
+          - [Installation](#installation)
+            - [Install extras](#install-extras)
+          - [Quick start](#quick-start)
+          - [Usage](#usage)
+          - [Database management](#database-management)
+            - [Alembic](#alembic)
+          - [Developers guide](#developers-guide)
+          - [Testing](#testing)
+            - [Testing data extraction](#testing-data-extraction)
+            - [Testing plots](#testing-plots)
+          - [Contributing](#contributing)
+          - [CI](#ci)
+          - [Rules of Thumb](#rules-of-thumb)
+          - [Credits](#credits)
+          - [License](#license)
         
         ## Installation
         Install the base lib via [pipy](https://pypi.org/project/soam/) by executing:
         ```bash
         pip install soam
         ```
         Or clone this repository:
@@ -113,17 +128,17 @@
         pip install -e ".[prophet]"
         pip install -e ".[pdf_report]"
         pip install -e ".[gsheets_report]"
         pip install -e ".[report]" # slack and *_report extras
         pip install -e ".[all]" # all previous
         ```
         
-        _Note_: The `pdf_report` extra might need to run the following command before installation ([More info](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex))
+        *Note*: The `pdf_report` extra might need to run the following command before installation ([More info](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex))
         
-          $ `apt-get install texlive-xetex texlive-fonts-recommended libpoppler-cpp-dev`
+        $ `apt-get install texlive-xetex texlive-fonts-recommended libpoppler-cpp-dev`
         
         ## Quick start
         [Here](https://gitlab.com/mutt_data/soam/-/blob/master/notebook/examples/quickstart.ipynb) is an example for a quick start into SoaM. In it a time series with AAPL stock prices is loaded, processed and forecasted. As well, there's [other example](https://gitlab.com/mutt_data/soam/-/blob/master/notebook/examples/soamflowrun.ipynb) with the same steps, but exploding the power of flows.
         
         ## Usage
         For further info check our [end to end](https://mutt_data.gitlab.io/soam/end2end.html) example where we explained how SoaM will interact with Airflow and Cookiecutter on a generic project.
         
@@ -155,18 +170,14 @@
         the python file with the necessary changes.
         It is always necessary to manually review and correct the candidate migrations that autogenerate produces.
         
         The second command will use this file to impact the changes in the database.
         
         For more alembic commands visit the [documentation](https://alembic.sqlalchemy.org/en/latest/)
         
-        [//comment]: # (TODO: add documentation about parameter and step logging.)
-        [//comment]: # (TODO: split and reorder documentation.)
-        
-        
         ## Developers guide
         If you are going to develop SoaM, you should checkout the documentation directory before adding code,
         you can start in the [project structure document](https://mutt_data.gitlab.io/soam/project_structure.html).
         
         ## Testing
         To run the default testsuite run this:
         ```
@@ -195,15 +206,14 @@
         To run a specific test file:
         ```bash
         TEST_DB_CONNSTR="postgresql://soam:soam@localhost/soam" pytest -v tests/test_file.py
         ```
         
         Note that even though the example has a DB name during the tests a new database is created and dropped to ensure that no state is maintened between runs.
         
-        
         ### Testing plots
         To generate images for testing we use [pytest-mpl](https://github.com/matplotlib/pytest-mpl) as follows:
         
         ```
         pytest --mpl-generate-path=tests/plotting/baseline
         ```
         
@@ -218,44 +228,40 @@
         ## CI
         
         To run the CI jobs locally you have to run it with [nox](https://nox.thea.codes/en/stable/):
         In the project root directory, there is a noxfile.py file defining all the jobs, these jobs will be executed when calling from CI or you can call them locally.
         
         You can run all the jobs with the command `nox`, from the project root directory or run just one job with `nox --session test` command, for example.
         
-        [//comment]: # (TODO: Link or explain how to run test and check locally)
-        [//comment]: # (TODO: Review the following CI explanation)
-        
         The .gitlab-ci.yml file configures the gitlab CI to run nox.
         Nox let us execute some test and checks before making the commit.
         We are using:
         * Linting job:
-            * [isort](https://pycqa.github.io/isort/) to reorder imports
-            * [pylint](https://github.com/PyCQA/pylint) to be pep8 compliant
-            * [black](https://github.com/psf/black) to format for code conventions
-            * [mypy](http://mypy-lang.org/) for static type checking
+          * [isort](https://pycqa.github.io/isort/) to reorder imports
+          * [pylint](https://github.com/PyCQA/pylint) to be pep8 compliant
+          * [black](https://github.com/psf/black) to format for code conventions
+          * [mypy](http://mypy-lang.org/) for static type checking
         * [bandit](https://bandit.readthedocs.io/en/latest/) for security checks
         * [pytest](https://docs.pytest.org/) to run all the tests in the test folder.
         * [pyreverse](https://pythonhosted.org/theape/documentation/developer/explorations/explore_graphs/explore_pyreverse.html) to create diagrams of the project
         
         This runs on a gitlab machine after every commit.
         
         We are caching the environments for each job on each branch.
         On every first commit of a branch, you will have to change the policy also if you add dependencies or a new package to the project.
         Gitlab cache policy:
         * `pull`: pull the cached files from the cloud.
         * `push`: push the created files to the cloud.
         * `pull-push`: pull the cached files and push the newly created files.
         
-        
         ## Rules of Thumb
         This section contains some recommendations when working with SoaM to avoid common mistakes:
         
         * When possible reuse objects to preserve their configuration.
-          Eg: Transformations, forecasters, etc.
+        Eg: Transformations, forecasters, etc.
         * Use the same train-test windows when backtesting and training to deploy and on later usage.
         
         ## Credits
         Alejandro Rusi <br>
         Diego Leguizamón <br>
         Diego Lizondo <br>
         Eugenio Scafati <br>
@@ -266,14 +272,15 @@
         Juan Martin Pampliega <br>
         Pablo Andres Lorenzatto <br>
         Wenceslao Villegas
         
         ## License
         `soam` is licensed under the [Apache License 2.0](https://gitlab.com/mutt_data/muttlib/-/blob/master/LICENCE).
         
+        
 Keywords: anomalies forecasting reporting
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
```

### Comparing `soam-0.9.3/README.md` & `soam-0.9.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,51 +4,55 @@
 
 SoaM is a [Prefect](https://docs.prefect.io/) based library created by [Mutt](https://muttdata.ai/).
 Its goal is to create a forecasting framework, this tool is developed with conjunctions of experience on previous
 projects. There come the name: Son of a Mutt = SoaM
 
 ## SoaM pipeline
 
-```mermaid
+<!-- gfmd-start -->
+![Mermaid diagram](https://kroki.io/mermaid/svg/eNpljbEOgjAURXe_4o0wEBQQnJzUxEQSIm6EocITmwAlrx1MCP-uloIkdnu959xbEeuecLmu4PN4uc6sA1PsziTC2c4dZ89LL3NTwWK48QYhReIo4fhSxAolyM2NuVmas2pCT1_-VESslQ9BDf50XxOBIU6CsGBSLYBt30-_vK0gFiXWwzBaBgn0FWaW7kgIS14oLlppTyWhJqK_FUhqoZZrI7gz4BU7Qd_ZOY_G_A05RWCs)
+
+<details>
+<summary><sup><sub>Diagram source code</sub></sup></summary>
 
-   graph LR
+```mermaid
+graph LR
     id0[(Database I)]-->id2[/SoaM Time Series Extractor/]
     id1[(Database II)]-->id2
     id2-->id3[/SoaM Transformer/]
     id3-->id4[/SoaM Forecaster/]
     id5{{Forecasting Model}}-->id4
     id4-->id6[(SoaM Predictions)]
     id6-->id7[/SoaM Forecaster Plotter/]
     id6-->id8[/SoaM Reporting/]
     id7-->id8
 ```
-
+</details>
+<!-- gfmd-end -->
 This library pipeline supports any data source.
 The process is structured in different stages:
 * Extraction: manages the granularity and aggregation of the input data.
 * Preprocessing: lets select among out of the box tools to perform standard tasks as normalization or fill nan values.
 * Forecasting: fits a model and predict results.
 * Postprocessing: modifies the results based on business/real information or create analysis with the predicted values,
- such as an anomaly detection.
+such as an anomaly detection.
 
 ## Overview of the Steps Run in SoaM
 
 ### Extraction
 This stage extracts data from the needed sources to build the condensed dataset for the next steps. This tends to be
 project dependent. Then it converts the full dataset to the desired time granularity and aggregation level by some categorical attribute/s.
 
 ### Preprocessing
 This step implements functions to further cleanup and prepare the data for the following steps, such as:
 * Add feature/transformation
 * Fill nan values
 * Apply value normalizations
 * Shift values
 
-[//comment]: # (the preprocessing supports custom transformations?)
-
 ### Forecasting
 This stage receives the clean data, performs the forecast and store the predicted values in the defined storages.
 Currently there are implementations to store in CSV files and SQL databases.
 A variety of models are currently supported to fit and predict data. They can be extended to create custom ones.
 * [Exponential Smoothing](https://www.statsmodels.org/stable/examples/notebooks/generated/exponential_smoothing.html)
 * [Orbit DLT Full](https://orbit-ml.readthedocs.io/en/latest/tutorials/dlt.html)
 * [Prophet](https://pypi.org/project/fbprophet)
@@ -59,34 +63,45 @@
 To do backtesting the data is splited in train and validation, there are two spliting methods:
 - Sliding: create a fixed size window for the training data that ends at the beginning of the validation data.
 - Expanding: create the training data from remaining data since the start of the series until the validation data.
 
 For more information review this document: [backtesting at scale](https://eng.uber.com/backtesting-at-scale/)
 
 ### Postprocessing
-[//comment]: # (TODO: explain postprocessing stage chaining)
 This last stage is prepared to work on the forecasts generated by the pipeline. For example:
 * Clip/Cleanup the predictions.
 * Perform further analyses (such as anomaly detection).
 * Export reports.
 
-[//comment]: # (does the postprocessing support custom outputs?)
-
 ## Table of Contents
-- [Installation](#installation)
-- [Quick start](#quick-start)
-- [Usage](#usage)
-- [Soam CLI](#soam-cli)
-- [Database Management](#database-management)
-- [Developers Guide](#developers-guide)
-- [Testing](#testing)
-- [Contributing](#contributing)
-- [Rules of Thumb](#rules-of-thumb)
-- [Credits](#contributing)
-- [License](#license)
+- [SoaM](#soam)
+  - [SoaM pipeline](#soam-pipeline)
+  - [Overview of the Steps Run in SoaM](#overview-of-the-steps-run-in-soam)
+    - [Extraction](#extraction)
+    - [Preprocessing](#preprocessing)
+    - [Forecasting](#forecasting)
+    - [Backtesting](#backtesting)
+      - [Window policies](#window-policies)
+    - [Postprocessing](#postprocessing)
+  - [Table of Contents](#table-of-contents)
+  - [Installation](#installation)
+    - [Install extras](#install-extras)
+  - [Quick start](#quick-start)
+  - [Usage](#usage)
+  - [Database management](#database-management)
+    - [Alembic](#alembic)
+  - [Developers guide](#developers-guide)
+  - [Testing](#testing)
+    - [Testing data extraction](#testing-data-extraction)
+    - [Testing plots](#testing-plots)
+  - [Contributing](#contributing)
+  - [CI](#ci)
+  - [Rules of Thumb](#rules-of-thumb)
+  - [Credits](#credits)
+  - [License](#license)
 
 ## Installation
 Install the base lib via [pipy](https://pypi.org/project/soam/) by executing:
 ```bash
 pip install soam
 ```
 Or clone this repository:
@@ -105,17 +120,17 @@
 pip install -e ".[prophet]"
 pip install -e ".[pdf_report]"
 pip install -e ".[gsheets_report]"
 pip install -e ".[report]" # slack and *_report extras
 pip install -e ".[all]" # all previous
 ```
 
-_Note_: The `pdf_report` extra might need to run the following command before installation ([More info](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex))
+*Note*: The `pdf_report` extra might need to run the following command before installation ([More info](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex))
 
-  $ `apt-get install texlive-xetex texlive-fonts-recommended libpoppler-cpp-dev`
+$ `apt-get install texlive-xetex texlive-fonts-recommended libpoppler-cpp-dev`
 
 ## Quick start
 [Here](https://gitlab.com/mutt_data/soam/-/blob/master/notebook/examples/quickstart.ipynb) is an example for a quick start into SoaM. In it a time series with AAPL stock prices is loaded, processed and forecasted. As well, there's [other example](https://gitlab.com/mutt_data/soam/-/blob/master/notebook/examples/soamflowrun.ipynb) with the same steps, but exploding the power of flows.
 
 ## Usage
 For further info check our [end to end](https://mutt_data.gitlab.io/soam/end2end.html) example where we explained how SoaM will interact with Airflow and Cookiecutter on a generic project.
 
@@ -147,18 +162,14 @@
 the python file with the necessary changes.
 It is always necessary to manually review and correct the candidate migrations that autogenerate produces.
 
 The second command will use this file to impact the changes in the database.
 
 For more alembic commands visit the [documentation](https://alembic.sqlalchemy.org/en/latest/)
 
-[//comment]: # (TODO: add documentation about parameter and step logging.)
-[//comment]: # (TODO: split and reorder documentation.)
-
-
 ## Developers guide
 If you are going to develop SoaM, you should checkout the documentation directory before adding code,
 you can start in the [project structure document](https://mutt_data.gitlab.io/soam/project_structure.html).
 
 ## Testing
 To run the default testsuite run this:
 ```
@@ -187,15 +198,14 @@
 To run a specific test file:
 ```bash
 TEST_DB_CONNSTR="postgresql://soam:soam@localhost/soam" pytest -v tests/test_file.py
 ```
 
 Note that even though the example has a DB name during the tests a new database is created and dropped to ensure that no state is maintened between runs.
 
-
 ### Testing plots
 To generate images for testing we use [pytest-mpl](https://github.com/matplotlib/pytest-mpl) as follows:
 
 ```
 pytest --mpl-generate-path=tests/plotting/baseline
 ```
 
@@ -210,44 +220,40 @@
 ## CI
 
 To run the CI jobs locally you have to run it with [nox](https://nox.thea.codes/en/stable/):
 In the project root directory, there is a noxfile.py file defining all the jobs, these jobs will be executed when calling from CI or you can call them locally.
 
 You can run all the jobs with the command `nox`, from the project root directory or run just one job with `nox --session test` command, for example.
 
-[//comment]: # (TODO: Link or explain how to run test and check locally)
-[//comment]: # (TODO: Review the following CI explanation)
-
 The .gitlab-ci.yml file configures the gitlab CI to run nox.
 Nox let us execute some test and checks before making the commit.
 We are using:
 * Linting job:
-    * [isort](https://pycqa.github.io/isort/) to reorder imports
-    * [pylint](https://github.com/PyCQA/pylint) to be pep8 compliant
-    * [black](https://github.com/psf/black) to format for code conventions
-    * [mypy](http://mypy-lang.org/) for static type checking
+  * [isort](https://pycqa.github.io/isort/) to reorder imports
+  * [pylint](https://github.com/PyCQA/pylint) to be pep8 compliant
+  * [black](https://github.com/psf/black) to format for code conventions
+  * [mypy](http://mypy-lang.org/) for static type checking
 * [bandit](https://bandit.readthedocs.io/en/latest/) for security checks
 * [pytest](https://docs.pytest.org/) to run all the tests in the test folder.
 * [pyreverse](https://pythonhosted.org/theape/documentation/developer/explorations/explore_graphs/explore_pyreverse.html) to create diagrams of the project
 
 This runs on a gitlab machine after every commit.
 
 We are caching the environments for each job on each branch.
 On every first commit of a branch, you will have to change the policy also if you add dependencies or a new package to the project.
 Gitlab cache policy:
 * `pull`: pull the cached files from the cloud.
 * `push`: push the created files to the cloud.
 * `pull-push`: pull the cached files and push the newly created files.
 
-
 ## Rules of Thumb
 This section contains some recommendations when working with SoaM to avoid common mistakes:
 
 * When possible reuse objects to preserve their configuration.
-  Eg: Transformations, forecasters, etc.
+Eg: Transformations, forecasters, etc.
 * Use the same train-test windows when backtesting and training to deploy and on later usage.
 
 ## Credits
 Alejandro Rusi <br>
 Diego Leguizamón <br>
 Diego Lizondo <br>
 Eugenio Scafati <br>
@@ -257,7 +263,8 @@
 Hugo Daniel Viotti <br>
 Juan Martin Pampliega <br>
 Pablo Andres Lorenzatto <br>
 Wenceslao Villegas
 
 ## License
 `soam` is licensed under the [Apache License 2.0](https://gitlab.com/mutt_data/muttlib/-/blob/master/LICENCE).
+
```

### Comparing `soam-0.9.3/pyproject.toml` & `soam-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/setup.cfg` & `soam-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/setup.py` & `soam-0.9.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,18 +89,16 @@
         "Cython<0.29.18,>=0.29",
         "sqlalchemy<1.4.0,>=1.3.0",
         "sqlalchemy_utils",
         "alembic",
         "python-decouple",
         "prefect==0.14.17",
         "filelock",
-        "click",
         "wheel",
         "muttlib>=1.1.2,<2",
         "numpy>=1.19,<1.20",
         "matplotlib==3.3.4",
     ],
     extras_require=extra_dependencies,
     python_requires="~=3.6",
-    entry_points={'console_scripts': ['soam = soam.console:cli']},
 )
 # TODO: check why 'python setup.py develop' is failing to obtain muttlib, but 'pip install -e .' is working
```

### Comparing `soam-0.9.3/soam/cfg.py` & `soam-0.9.4/soam/cfg.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/constants.py` & `soam-0.9.4/soam/constants.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/core/runner.py` & `soam-0.9.4/soam/core/runner.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/core/step.py` & `soam-0.9.4/soam/core/step.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/data_models.py` & `soam-0.9.4/soam/data_models.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/models/base.py` & `soam-0.9.4/soam/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""Wrapping functions for SkLearn API."""
+"""
+Wrapping functions for SkLearn API.
+
+This is inspired by wrappers developed in https://github.com/heidelbergcement/hcrystalball.
+"""
 import abc
 from abc import abstractmethod
 import inspect
 from types import FunctionType
 from typing import Callable, List
 
 from sklearn.base import BaseEstimator
```

### Comparing `soam-0.9.3/soam/models/exponential.py` & `soam-0.9.4/soam/models/exponential.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/models/orbit.py` & `soam-0.9.4/soam/models/orbit.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/models/prophet.py` & `soam-0.9.4/soam/models/prophet.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/models/sarimax.py` & `soam-0.9.4/soam/models/sarimax.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/plotting/forecast_plotter.py` & `soam-0.9.4/soam/plotting/forecast_plotter.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/plotting/plot_utils.py` & `soam-0.9.4/soam/plotting/plot_utils.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/reporting/gsheets_report.py` & `soam-0.9.4/soam/reporting/gsheets_report.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/reporting/mail_report.py` & `soam-0.9.4/soam/reporting/mail_report.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/reporting/pdf_report.py` & `soam-0.9.4/soam/reporting/pdf_report.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/reporting/slack_report.py` & `soam-0.9.4/soam/reporting/slack_report.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/savers/csv_saver.py` & `soam-0.9.4/soam/savers/csv_saver.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/savers/db_saver.py` & `soam-0.9.4/soam/savers/db_saver.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/savers/savers.py` & `soam-0.9.4/soam/savers/savers.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/utilities/helpers.py` & `soam-0.9.4/soam/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/utilities/utils.py` & `soam-0.9.4/soam/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/anomalies.py` & `soam-0.9.4/soam/workflow/anomalies.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/backtester.py` & `soam-0.9.4/soam/workflow/backtester.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/forecaster.py` & `soam-0.9.4/soam/workflow/forecaster.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/merge_concat.py` & `soam-0.9.4/soam/workflow/merge_concat.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/slicer.py` & `soam-0.9.4/soam/workflow/slicer.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/store.py` & `soam-0.9.4/soam/workflow/store.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/time_series_extractor.py` & `soam-0.9.4/soam/workflow/time_series_extractor.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam/workflow/transformer.py` & `soam-0.9.4/soam/workflow/transformer.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/soam.egg-info/PKG-INFO` & `soam-0.9.4/soam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soam
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tools for time series analysis, plotting and reporting.
 Home-page: UNKNOWN
 Author: Mutt Data
 Author-email: info@muttdata.ai
 License: UNKNOWN
 Description: # SoaM
         
@@ -12,51 +12,55 @@
         
         SoaM is a [Prefect](https://docs.prefect.io/) based library created by [Mutt](https://muttdata.ai/).
         Its goal is to create a forecasting framework, this tool is developed with conjunctions of experience on previous
         projects. There come the name: Son of a Mutt = SoaM
         
         ## SoaM pipeline
         
-        ```mermaid
+        <!-- gfmd-start -->
+        ![Mermaid diagram](https://kroki.io/mermaid/svg/eNpljbEOgjAURXe_4o0wEBQQnJzUxEQSIm6EocITmwAlrx1MCP-uloIkdnu959xbEeuecLmu4PN4uc6sA1PsziTC2c4dZ89LL3NTwWK48QYhReIo4fhSxAolyM2NuVmas2pCT1_-VESslQ9BDf50XxOBIU6CsGBSLYBt30-_vK0gFiXWwzBaBgn0FWaW7kgIS14oLlppTyWhJqK_FUhqoZZrI7gz4BU7Qd_ZOY_G_A05RWCs)
+        
+        <details>
+        <summary><sup><sub>Diagram source code</sub></sup></summary>
         
-           graph LR
+        ```mermaid
+        graph LR
             id0[(Database I)]-->id2[/SoaM Time Series Extractor/]
             id1[(Database II)]-->id2
             id2-->id3[/SoaM Transformer/]
             id3-->id4[/SoaM Forecaster/]
             id5{{Forecasting Model}}-->id4
             id4-->id6[(SoaM Predictions)]
             id6-->id7[/SoaM Forecaster Plotter/]
             id6-->id8[/SoaM Reporting/]
             id7-->id8
         ```
-        
+        </details>
+        <!-- gfmd-end -->
         This library pipeline supports any data source.
         The process is structured in different stages:
         * Extraction: manages the granularity and aggregation of the input data.
         * Preprocessing: lets select among out of the box tools to perform standard tasks as normalization or fill nan values.
         * Forecasting: fits a model and predict results.
         * Postprocessing: modifies the results based on business/real information or create analysis with the predicted values,
-         such as an anomaly detection.
+        such as an anomaly detection.
         
         ## Overview of the Steps Run in SoaM
         
         ### Extraction
         This stage extracts data from the needed sources to build the condensed dataset for the next steps. This tends to be
         project dependent. Then it converts the full dataset to the desired time granularity and aggregation level by some categorical attribute/s.
         
         ### Preprocessing
         This step implements functions to further cleanup and prepare the data for the following steps, such as:
         * Add feature/transformation
         * Fill nan values
         * Apply value normalizations
         * Shift values
         
-        [//comment]: # (the preprocessing supports custom transformations?)
-        
         ### Forecasting
         This stage receives the clean data, performs the forecast and store the predicted values in the defined storages.
         Currently there are implementations to store in CSV files and SQL databases.
         A variety of models are currently supported to fit and predict data. They can be extended to create custom ones.
         * [Exponential Smoothing](https://www.statsmodels.org/stable/examples/notebooks/generated/exponential_smoothing.html)
         * [Orbit DLT Full](https://orbit-ml.readthedocs.io/en/latest/tutorials/dlt.html)
         * [Prophet](https://pypi.org/project/fbprophet)
@@ -67,34 +71,45 @@
         To do backtesting the data is splited in train and validation, there are two spliting methods:
         - Sliding: create a fixed size window for the training data that ends at the beginning of the validation data.
         - Expanding: create the training data from remaining data since the start of the series until the validation data.
         
         For more information review this document: [backtesting at scale](https://eng.uber.com/backtesting-at-scale/)
         
         ### Postprocessing
-        [//comment]: # (TODO: explain postprocessing stage chaining)
         This last stage is prepared to work on the forecasts generated by the pipeline. For example:
         * Clip/Cleanup the predictions.
         * Perform further analyses (such as anomaly detection).
         * Export reports.
         
-        [//comment]: # (does the postprocessing support custom outputs?)
-        
         ## Table of Contents
-        - [Installation](#installation)
-        - [Quick start](#quick-start)
-        - [Usage](#usage)
-        - [Soam CLI](#soam-cli)
-        - [Database Management](#database-management)
-        - [Developers Guide](#developers-guide)
-        - [Testing](#testing)
-        - [Contributing](#contributing)
-        - [Rules of Thumb](#rules-of-thumb)
-        - [Credits](#contributing)
-        - [License](#license)
+        - [SoaM](#soam)
+          - [SoaM pipeline](#soam-pipeline)
+          - [Overview of the Steps Run in SoaM](#overview-of-the-steps-run-in-soam)
+            - [Extraction](#extraction)
+            - [Preprocessing](#preprocessing)
+            - [Forecasting](#forecasting)
+            - [Backtesting](#backtesting)
+              - [Window policies](#window-policies)
+            - [Postprocessing](#postprocessing)
+          - [Table of Contents](#table-of-contents)
+          - [Installation](#installation)
+            - [Install extras](#install-extras)
+          - [Quick start](#quick-start)
+          - [Usage](#usage)
+          - [Database management](#database-management)
+            - [Alembic](#alembic)
+          - [Developers guide](#developers-guide)
+          - [Testing](#testing)
+            - [Testing data extraction](#testing-data-extraction)
+            - [Testing plots](#testing-plots)
+          - [Contributing](#contributing)
+          - [CI](#ci)
+          - [Rules of Thumb](#rules-of-thumb)
+          - [Credits](#credits)
+          - [License](#license)
         
         ## Installation
         Install the base lib via [pipy](https://pypi.org/project/soam/) by executing:
         ```bash
         pip install soam
         ```
         Or clone this repository:
@@ -113,17 +128,17 @@
         pip install -e ".[prophet]"
         pip install -e ".[pdf_report]"
         pip install -e ".[gsheets_report]"
         pip install -e ".[report]" # slack and *_report extras
         pip install -e ".[all]" # all previous
         ```
         
-        _Note_: The `pdf_report` extra might need to run the following command before installation ([More info](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex))
+        *Note*: The `pdf_report` extra might need to run the following command before installation ([More info](https://nbconvert.readthedocs.io/en/latest/install.html#installing-tex))
         
-          $ `apt-get install texlive-xetex texlive-fonts-recommended libpoppler-cpp-dev`
+        $ `apt-get install texlive-xetex texlive-fonts-recommended libpoppler-cpp-dev`
         
         ## Quick start
         [Here](https://gitlab.com/mutt_data/soam/-/blob/master/notebook/examples/quickstart.ipynb) is an example for a quick start into SoaM. In it a time series with AAPL stock prices is loaded, processed and forecasted. As well, there's [other example](https://gitlab.com/mutt_data/soam/-/blob/master/notebook/examples/soamflowrun.ipynb) with the same steps, but exploding the power of flows.
         
         ## Usage
         For further info check our [end to end](https://mutt_data.gitlab.io/soam/end2end.html) example where we explained how SoaM will interact with Airflow and Cookiecutter on a generic project.
         
@@ -155,18 +170,14 @@
         the python file with the necessary changes.
         It is always necessary to manually review and correct the candidate migrations that autogenerate produces.
         
         The second command will use this file to impact the changes in the database.
         
         For more alembic commands visit the [documentation](https://alembic.sqlalchemy.org/en/latest/)
         
-        [//comment]: # (TODO: add documentation about parameter and step logging.)
-        [//comment]: # (TODO: split and reorder documentation.)
-        
-        
         ## Developers guide
         If you are going to develop SoaM, you should checkout the documentation directory before adding code,
         you can start in the [project structure document](https://mutt_data.gitlab.io/soam/project_structure.html).
         
         ## Testing
         To run the default testsuite run this:
         ```
@@ -195,15 +206,14 @@
         To run a specific test file:
         ```bash
         TEST_DB_CONNSTR="postgresql://soam:soam@localhost/soam" pytest -v tests/test_file.py
         ```
         
         Note that even though the example has a DB name during the tests a new database is created and dropped to ensure that no state is maintened between runs.
         
-        
         ### Testing plots
         To generate images for testing we use [pytest-mpl](https://github.com/matplotlib/pytest-mpl) as follows:
         
         ```
         pytest --mpl-generate-path=tests/plotting/baseline
         ```
         
@@ -218,44 +228,40 @@
         ## CI
         
         To run the CI jobs locally you have to run it with [nox](https://nox.thea.codes/en/stable/):
         In the project root directory, there is a noxfile.py file defining all the jobs, these jobs will be executed when calling from CI or you can call them locally.
         
         You can run all the jobs with the command `nox`, from the project root directory or run just one job with `nox --session test` command, for example.
         
-        [//comment]: # (TODO: Link or explain how to run test and check locally)
-        [//comment]: # (TODO: Review the following CI explanation)
-        
         The .gitlab-ci.yml file configures the gitlab CI to run nox.
         Nox let us execute some test and checks before making the commit.
         We are using:
         * Linting job:
-            * [isort](https://pycqa.github.io/isort/) to reorder imports
-            * [pylint](https://github.com/PyCQA/pylint) to be pep8 compliant
-            * [black](https://github.com/psf/black) to format for code conventions
-            * [mypy](http://mypy-lang.org/) for static type checking
+          * [isort](https://pycqa.github.io/isort/) to reorder imports
+          * [pylint](https://github.com/PyCQA/pylint) to be pep8 compliant
+          * [black](https://github.com/psf/black) to format for code conventions
+          * [mypy](http://mypy-lang.org/) for static type checking
         * [bandit](https://bandit.readthedocs.io/en/latest/) for security checks
         * [pytest](https://docs.pytest.org/) to run all the tests in the test folder.
         * [pyreverse](https://pythonhosted.org/theape/documentation/developer/explorations/explore_graphs/explore_pyreverse.html) to create diagrams of the project
         
         This runs on a gitlab machine after every commit.
         
         We are caching the environments for each job on each branch.
         On every first commit of a branch, you will have to change the policy also if you add dependencies or a new package to the project.
         Gitlab cache policy:
         * `pull`: pull the cached files from the cloud.
         * `push`: push the created files to the cloud.
         * `pull-push`: pull the cached files and push the newly created files.
         
-        
         ## Rules of Thumb
         This section contains some recommendations when working with SoaM to avoid common mistakes:
         
         * When possible reuse objects to preserve their configuration.
-          Eg: Transformations, forecasters, etc.
+        Eg: Transformations, forecasters, etc.
         * Use the same train-test windows when backtesting and training to deploy and on later usage.
         
         ## Credits
         Alejandro Rusi <br>
         Diego Leguizamón <br>
         Diego Lizondo <br>
         Eugenio Scafati <br>
@@ -266,14 +272,15 @@
         Juan Martin Pampliega <br>
         Pablo Andres Lorenzatto <br>
         Wenceslao Villegas
         
         ## License
         `soam` is licensed under the [Apache License 2.0](https://gitlab.com/mutt_data/muttlib/-/blob/master/LICENCE).
         
+        
 Keywords: anomalies forecasting reporting
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
```

### Comparing `soam-0.9.3/soam.egg-info/SOURCES.txt` & `soam-0.9.4/soam.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 soam/__init__.py
 soam/cfg.py
 soam/constants.py
 soam/data_models.py
 soam.egg-info/PKG-INFO
 soam.egg-info/SOURCES.txt
 soam.egg-info/dependency_links.txt
-soam.egg-info/entry_points.txt
 soam.egg-info/requires.txt
 soam.egg-info/top_level.txt
 soam/core/__init__.py
 soam/core/runner.py
 soam/core/step.py
 soam/models/__init__.py
 soam/models/base.py
```

### Comparing `soam-0.9.3/soam.egg-info/requires.txt` & `soam-0.9.4/soam.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Cython<0.29.18,>=0.29
 sqlalchemy<1.4.0,>=1.3.0
 sqlalchemy_utils
 alembic
 python-decouple
 prefect==0.14.17
 filelock
-click
 wheel
 muttlib<2,>=1.1.2
 numpy<1.20,>=1.19
 matplotlib==3.3.4
 
 [all]
 flake8-bugbear
```

### Comparing `soam-0.9.3/tests/db_test_case.py` & `soam-0.9.4/tests/db_test_case.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/helpers.py` & `soam-0.9.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/integration/test_integration.py` & `soam-0.9.4/tests/integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/mlflow/test_mlflow_logging.py` & `soam-0.9.4/tests/mlflow/test_mlflow_logging.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/models/test_exponential.py` & `soam-0.9.4/tests/models/test_exponential.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/models/test_orbit.py` & `soam-0.9.4/tests/models/test_orbit.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/models/test_sarimax.py` & `soam-0.9.4/tests/models/test_sarimax.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/plotting/test_forecast_plotter.py` & `soam-0.9.4/tests/plotting/test_forecast_plotter.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/utilities/test_utils.py` & `soam-0.9.4/tests/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_anomalies.py` & `soam-0.9.4/tests/workflow/test_anomalies.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_backtester.py` & `soam-0.9.4/tests/workflow/test_backtester.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_forecaster.py` & `soam-0.9.4/tests/workflow/test_forecaster.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_mergeconcat.py` & `soam-0.9.4/tests/workflow/test_mergeconcat.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_slicer.py` & `soam-0.9.4/tests/workflow/test_slicer.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_store.py` & `soam-0.9.4/tests/workflow/test_store.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_time_series_extractor.py` & `soam-0.9.4/tests/workflow/test_time_series_extractor.py`

 * *Files identical despite different names*

### Comparing `soam-0.9.3/tests/workflow/test_transformer.py` & `soam-0.9.4/tests/workflow/test_transformer.py`

 * *Files identical despite different names*

