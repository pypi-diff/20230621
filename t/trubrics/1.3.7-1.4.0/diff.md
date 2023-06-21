# Comparing `tmp/trubrics-1.3.7.tar.gz` & `tmp/trubrics-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.3.7.tar", last modified: Sun May  7 11:02:28 2023, max compression
+gzip compressed data, was "trubrics-1.4.0.tar", last modified: Wed Jun 21 11:21:46 2023, max compression
```

## Comparing `trubrics-1.3.7.tar` & `trubrics-1.4.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-07 11:02:18.000000 trubrics-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-07 11:02:28.611936 trubrics-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-07 11:02:18.000000 trubrics-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.599936 trubrics-1.3.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/examples/classification_titanic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/custom_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/custom_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 11:02:18.000000 trubrics-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 11:02:18.000000 trubrics-1.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-07 11:02:28.611936 trubrics-1.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-07 11:02:18.000000 trubrics-1.3.7/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/app_titanic_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/app_titanic_gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/app_titanic_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/feedback/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-21 11:21:32.000000 trubrics-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 11:21:46.137231 trubrics-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-21 11:21:32.000000 trubrics-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/examples/classification_titanic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/custom_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/custom_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/slicing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 11:21:32.000000 trubrics-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 11:21:32.000000 trubrics-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 11:21:46.137231 trubrics-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-21 11:21:32.000000 trubrics-1.4.0/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/app_titanic_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/app_titanic_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/app_titanic_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/save_to_trubrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/trubrics_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.3.7/LICENSE` & `trubrics-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/examples/classification_titanic/custom_validator.py` & `trubrics-1.4.0/examples/classification_titanic/custom_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/setup.cfg` & `trubrics-1.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trubrics
-version = 1.3.7
+version = 1.4.0
 description = Combine data science knowledge with business user feedback to validate machine learning.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
 
@@ -24,15 +24,15 @@
 [flake8]
 max-line-length = 120
 
 [isort]
 profile = black
 
 [options.extras_require]
-streamlit = streamlit>=1.18.0
+streamlit = streamlit>=1.20.0
 dash = dash>=2.6.2; dash-bootstrap-components>=1.2.1
 gradio = gradio>=3.8.1
 mlflow = mlflow>=2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trubrics-1.3.7/tests/test_context.py` & `trubrics-1.4.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/cli/run.py` & `trubrics-1.4.0/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/context.py` & `trubrics-1.4.0/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/example/app_titanic_streamlit.py` & `trubrics-1.4.0/trubrics/example/app_titanic_streamlit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import os
 from typing import Optional
 
 import streamlit as st
 import typer
 
-from trubrics.cli.main import init
 from trubrics.context import DataContext
 from trubrics.example import get_titanic_data_and_model
 from trubrics.example import titanic_config as tc
 from trubrics.integrations.streamlit import (
     FeedbackCollector,
     generate_what_if_streamlit,
 )
 
 cli = typer.Typer()
 
 
 @st.cache_resource
 def init_trubrics(trubrics_platform_auth):
-    if trubrics_platform_auth:
-        with st.spinner("Connecting to the Trubrics platform..."):
-            project_name = os.environ.get("TRUBRICS_PROJECT_NAME")
-            if project_name is None:
-                raise KeyError("Environment variable TRUBRICS_PROJECT_NAME is not set.")
-            init(project_name=project_name)
+    # if trubrics_platform_auth:
+    #     with st.spinner("Connecting to the Trubrics platform..."):
+    #         project_name = os.environ.get("TRUBRICS_PROJECT_NAME")
+    #         if project_name is None:
+    #             raise KeyError("Environment variable TRUBRICS_PROJECT_NAME is not set.")
+    #         init(project_name=project_name)
     _, test_df, model = get_titanic_data_and_model()
 
     data_context = DataContext(
         testing_data=test_df,
         target="Survived",
         categorical_columns=tc.CATEGORICAL_COLUMNS,
         business_columns=tc.BUSINESS_COLUMNS,
     )
 
     collector = FeedbackCollector(
-        data="trubrics data_context",
+        component_name="test",
+        data=["trubrics data_context"],
         model="rf_model",
         trubrics_platform_auth=trubrics_platform_auth,
     )
     return model, data_context, collector
 
 
 def feedback_example(feedback_type, collector, metadata, open_feedback_label=None, user_response=None):
```

### Comparing `trubrics-1.3.7/trubrics/example/my_first_trubric.json` & `trubrics-1.4.0/trubrics/example/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/example/titanic.py` & `trubrics-1.4.0/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/example/titanic_data.csv` & `trubrics-1.4.0/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/example/trubric_run.py` & `trubrics-1.4.0/trubrics/example/trubric_run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/exceptions.py` & `trubrics-1.4.0/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/feedback/config.py` & `trubrics-1.4.0/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/integrations/dash/collect.py` & `trubrics-1.4.0/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/integrations/gradio/collect.py` & `trubrics-1.4.0/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.4.0/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/integrations/streamlit/collect.py` & `trubrics-1.4.0/trubrics/integrations/streamlit/collect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,286 +1,233 @@
-from typing import Any, Dict, List, Optional, Tuple, Union
+from datetime import datetime
+from typing import Optional
 
 import streamlit as st
 
 from trubrics.feedback import config
-from trubrics.feedback.dataclass import Feedback
-from trubrics.ui.auth import expire_after_n_seconds, get_trubrics_auth_token
-from trubrics.ui.trubrics_config import load_trubrics_config
+from trubrics.feedback.dataclass import Feedback, Response
+from trubrics.feedback.save_to_trubrics import save_to_trubrics as save
+from trubrics.trubrics_platform.auth import init
 
 
 class FeedbackCollector:
     def __init__(
         self,
-        data: Optional[str] = None,
-        model: Optional[str] = None,
-        trubrics_platform_auth: Optional[str] = None,
+        component_name: str,
+        email: Optional[str],
+        password: Optional[str],
+        firebase_api_key: Optional[str] = None,
+        firebase_project_id: Optional[str] = None,
     ):
         """
         The FeedbackCollector allows Data Scientists to collect feedback from within their app.
 
         Args:
-            data: a reference to the data that was used to collect the feedback (e.g. a link to a dataset)
-            model: a reference to the model that was used to collect the feedback (e.g. a link to a model)
-            trubrics_platform_auth: option to save the feedback to the trubrics platform
-
-                - *None*: save feedback locally to .json
-                - *single_user*: save feedback directly to the Trubrics platform,
-                    using auth credentials of the app owner
-                - *multiple_users*: save feedback directly to the Trubrics platform, with full user auth
+            TODO
         """
-        self.data = data
-        self.model = model
-        if trubrics_platform_auth in [None, "single_user", "multiple_users"]:
-            self.trubrics_platform_auth = trubrics_platform_auth
-        else:
-            raise ValueError(
-                f"trubrics_platform_auth={trubrics_platform_auth} not recognised. Must be one of [None, 'single_user',"
-                " 'multiple_users']."
-            )
-
-        self.email = ""
-        self.password = ""
-        self.authenticated = False
-
-    def st_trubrics_auth(self):
-        if self.trubrics_platform_auth is None:
-            raise ValueError(
-                "The `.st_trubrics_auth()` method is reserved for usage with the Trubrics platform. See the"
-                " 'trubrics_platform_auth' argument for authentication options."
+        self.component_name = component_name
+        if email and password:
+            self.trubrics_config = init(
+                email=email,
+                password=password,
+                firebase_api_key=firebase_api_key,
+                firebase_project_id=firebase_project_id,
             )
 
-        trubrics_config = load_trubrics_config()
-        if self.authenticated:
-            st.write(self.email + " signed in.")
-            if st.button("Sign out"):
-                self.authenticated = False
-                self.st_trubrics_auth()
-        else:
-            with st.form("auth form"):
-                self.email = st.text_input(
-                    label=config.USER_EMAIL,
-                    placeholder=config.USER_EMAIL,
-                    label_visibility="collapsed",
-                    key="email",
-                )
-                self.password = st.text_input(
-                    label=config.USER_PASSWORD,
-                    placeholder=config.USER_PASSWORD,
-                    label_visibility="collapsed",
-                    key="password",
-                    type="password",
-                )
-                submitted = st.form_submit_button("Sign In")
-                if submitted:
-                    # check auth
-                    auth = get_trubrics_auth_token(
-                        trubrics_config.firebase_auth_api_url, self.email, self.password, rerun=expire_after_n_seconds()
-                    )
-                    if "error" in auth:
-                        st.error(f"Error authenticating user {self.email}. Try again or contact your admin team.")
-                    else:
-                        st.success(f"{self.email} successfully signed in.")
-                        self.authenticated = True
-
     def st_feedback(
         self,
-        feedback_type: str = "issue",
-        user_response: Optional[Dict[str, Union[float, int, str, bool]]] = None,
-        path: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-        tags: Optional[List[str]] = None,
+        feedback_type: str,
+        model: str,
+        tags: list = [],
+        metadata: dict = {},
+        response: Optional[Response] = None,
+        user_id: Optional[str] = None,
         key: Optional[str] = None,
         open_feedback_label: Optional[str] = None,
-    ) -> Optional[Feedback]:
+        save_to_trubrics: bool = True,
+    ) -> Optional[dict]:
         """
         Collect user feedback within a Streamlit web application.
 
         Args:
+            TODO
             feedback_type: type of feedback to be collected
 
-                - issue: issue with a open text title and description fields
+                - textbox: open textbox feedback
                 - thumbs: positive or negative feedback with thumbs emojis
                 - faces: a scale of 1 to 5 with face emojis
                 - custom: a customisable feedback type that allows users to specify the user_response dict
-            user_response: a dict of user responses to save with your feedback for feedback_type='custom'
-            path: path to save feedback local .json. Defaults to "./*timestamp*_feedback.json"
+            response: a dict of user responses to save with your feedback for feedback_type='custom'
             metadata: data to save with your feedback
             tags: a list of tags for your feedback
             key: a key for each streamlit component
             open_feedback_label: label of optional text_input for "faces" or "thumbs" feedback_type
         """
         if key is None:
             key = feedback_type
-        if feedback_type == "issue":
-            if user_response or open_feedback_label:
-                raise ValueError("For feedback_type='issue', title, description and open_feedback_label must be None.")
-            issue_data = self.st_issue_ui(key)
-            if issue_data:
+        if feedback_type == "textbox":
+            if response:
+                raise ValueError("For feedback_type='textbox', user_response must be None.")
+            text = self.st_textbox_ui(key, label=open_feedback_label)
+            if text:
+                response = Response(type=feedback_type, score=None, text=text)
                 return self._save_feedback(
-                    feedback_type=feedback_type,
-                    path=path,
-                    metadata=metadata,
-                    user_response={issue_data[0]: issue_data[1]},
+                    model=model,
+                    response=response,
+                    user_id=user_id,
                     tags=tags,
+                    metadata=metadata,
+                    save_to_trubrics=save_to_trubrics,
                 )
         elif feedback_type in ("thumbs", "faces"):
-            if user_response:
+            if response:
                 raise ValueError(
-                    f"For feedback_type='{feedback_type}', user_response is set inside the component (must be None)."
+                    f"For feedback_type='{feedback_type}', response is set inside the component (must be None)."
                 )
             return self._save_quantitative_feedback(
+                model=model,
                 feedback_type=feedback_type,
-                path=path,
+                user_id=user_id,
                 metadata=metadata,
                 tags=tags,
                 key=key,
                 open_feedback_label=open_feedback_label,
+                save_to_trubrics=save_to_trubrics,
             )
-        elif feedback_type == "custom":
-            if user_response:
-                return self._save_feedback(
-                    feedback_type=feedback_type,
-                    user_response=user_response,
-                    path=path,
-                    metadata=metadata,
-                    tags=tags,
-                )
-            else:
-                raise ValueError("For feedback_type='custom', title and description parameters must be specified.")
+        # elif feedback_type == "custom":
+        #     if user_response:
+        #         return self._save_feedback(
+        #             feedback_type=feedback_type,
+        #             user_response=user_response,
+        #             path=path,
+        #             metadata=metadata,
+        #             tags=tags,
+        #         )
+        #     else:
+        #         raise ValueError("For feedback_type='custom', title and description parameters must be specified.")
         else:
-            raise ValueError("feedback_type must be one of ['issue', 'faces', 'thumbs', 'custom'].")
+            raise ValueError("feedback_type must be one of ['textbox', 'faces', 'thumbs', 'custom'].")
         return None
 
     def _save_feedback(
         self,
-        feedback_type: str,
-        user_response: Dict[str, Union[float, int, str, bool]],
-        path: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-        tags: Optional[List[str]] = None,
-    ) -> Optional[Feedback]:
+        model: str,
+        response: Response,
+        user_id: Optional[str] = None,
+        tags: list = [],
+        metadata: dict = {},
+        save_to_trubrics: bool = True,
+    ) -> Optional[dict]:
         feedback = Feedback(
-            feedback_type=feedback_type,
-            user_response=user_response,
-            data=self.data,
-            model=self.model,
+            component_name=self.component_name,
+            response=response,
+            model=model,
             metadata=metadata,
             tags=tags,
+            user_id=user_id,
+            created_on=datetime.now(),
         )
-        if self.trubrics_platform_auth is None:
-            feedback.save_local(path=path)
-            st.success(config.LOCAL_SAVE)
-        elif self.trubrics_platform_auth == "multiple_users":
-            if self.authenticated:
-                feedback.save_ui(self.email, self.password)
-                st.success(config.PLATFORM_SAVE)
+        if save_to_trubrics:
+            res = save(trubrics_config=self.trubrics_config, feedback=feedback)
+            if "error" in res:
+                error_msg = f"Error in pushing feedback issue to Trubrics: {res}"
+                st.error(error_msg)
             else:
-                st.error("User is not authenticated. Please try again or contact your admin.")
-        elif self.trubrics_platform_auth == "single_user":
-            feedback.save_ui(None, None)
-            st.success(config.PLATFORM_SAVE)
-        else:
-            raise ValueError(
-                f"trubrics_platform_auth={self.trubrics_platform_auth} not recognised. Must be one of [None,"
-                " 'single_user', 'multiple_users']."
-            )
-        return feedback
+                st.success(config.PLATFORM_SAVE)
+        return feedback.dict()
 
     def _save_quantitative_feedback(
         self,
-        feedback_type,
-        key,
+        feedback_type: str,
+        key: str,
         open_feedback_label: Optional[str],
-        path: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-        tags: Optional[List[str]] = None,
-    ) -> Optional[Feedback]:
+        model: str,
+        user_id: Optional[str] = None,
+        tags: list = [],
+        metadata: dict = {},
+        save_to_trubrics: bool = True,
+    ) -> Optional[dict]:
         if f"{key}_state" not in st.session_state:
             st.session_state[f"{key}_state"] = ""
         if f"{key}_save_button" not in st.session_state:
             st.session_state[f"{key}_save_button"] = False
         if f"previous_{key}_state" not in st.session_state:
             st.session_state[f"previous_{key}_state"] = ""
 
-        title = f"User satisfaction: {feedback_type}"
-
-        def feedback_handler(open_feedback_label):
-            user_response = {
-                title: st.session_state[f"{key}_state"],
-                open_feedback_label: st.session_state[f"{feedback_type}_open_feedback"].rstrip(),
-            }
-            st.session_state[f"previous_{key}_state"] = user_response
+        def feedback_handler():
+            response = Response(
+                type=feedback_type,
+                score=st.session_state[f"{key}_state"],
+                text=st.session_state[f"{feedback_type}_open_feedback_{key}"].rstrip(),
+            )
+            st.session_state[f"previous_{key}_state"] = response
             st.session_state[f"{key}_state"] = ""
 
             self._enable_all_buttons(feedback_type=feedback_type)
 
         ui_state = getattr(self, f"st_{feedback_type}_ui")(
             key=key, disable_on_click=True if open_feedback_label else False
         )
         if ui_state:
             st.session_state[f"{key}_state"] = ui_state
 
         if open_feedback_label:
             if st.session_state.get(f"{key}_state_clicked", "") != "":
-                st.text_input(open_feedback_label, key=f"{feedback_type}_open_feedback")
+                st.text_input(open_feedback_label, key=f"{feedback_type}_open_feedback_{key}")
                 st.button(
                     config.FEEDBACK_SAVE_BUTTON,
                     on_click=feedback_handler,
-                    args=(open_feedback_label,),
                     key=f"{key}_save_button",
                 )
         else:
             if ui_state:
-                user_response = {title: ui_state}
+                response = Response(
+                    type=feedback_type,
+                    score=ui_state,
+                    text=None,
+                )
                 return self._save_feedback(
-                    user_response=user_response, feedback_type=feedback_type, metadata=metadata, path=path, tags=tags
+                    model=model,
+                    response=response,
+                    user_id=user_id,
+                    tags=tags,
+                    metadata=metadata,
+                    save_to_trubrics=save_to_trubrics,
                 )
         if st.session_state[f"{key}_save_button"]:
-            user_response = {title: ui_state}
             return self._save_feedback(
-                user_response=st.session_state[f"previous_{key}_state"],
-                feedback_type=feedback_type,
-                metadata=metadata,
-                path=path,
+                model=model,
+                response=st.session_state[f"previous_{key}_state"],
+                user_id=user_id,
                 tags=tags,
+                metadata=metadata,
+                save_to_trubrics=save_to_trubrics,
             )
         return None
 
     @staticmethod
-    def st_issue_ui(key: Optional[str] = None) -> Optional[Tuple[str, str]]:
+    def st_textbox_ui(key: Optional[str] = None, label: Optional[str] = None) -> Optional[str]:
         if key is None:
-            key = "issue"
+            key = "textbox"
 
         if f"{key}_save_button" not in st.session_state:
             st.session_state[f"{key}_save_button"] = False
 
         if f"previous_{key}_state" not in st.session_state:
             st.session_state[f"previous_{key}_state"] = ""
 
         def clear_session_state():
-            st.session_state[f"previous_{key}_state"] = (
-                st.session_state[f"{key}_title"],
-                st.session_state[f"{key}_description"],
-            )
+            st.session_state[f"previous_{key}_state"] = st.session_state[f"{key}_title"]
             st.session_state[f"{key}_title"] = ""
-            st.session_state[f"{key}_description"] = ""
 
         title = st.text_input(
-            label=config.TITLE,
-            help=config.TITLE_EXPLAIN,
+            label=label or "Provide some feedback",
             key=f"{key}_title",
         )
-        description = st.text_input(
-            label=config.DESCRIPTION,
-            help=config.DESCRIPTION_EXPLAIN,
-            key=f"{key}_description",
-        )
-        enabled = title and description
-        if enabled:
+        if title:
             st.button(config.FEEDBACK_SAVE_BUTTON, on_click=clear_session_state, key=f"{key}_save_button")
         if st.session_state[f"{key}_save_button"]:
             return st.session_state[f"previous_{key}_state"]
         else:
             return None
 
     def st_thumbs_ui(self, disable_on_click: bool = False, key: Optional[str] = None) -> Optional[str]:
@@ -291,17 +238,17 @@
         col1, col2 = st.columns([1, 15])
         with col1:
             up = self._emoji_button("👍", key, disable_on_click, button_states, 1)
         with col2:
             down = self._emoji_button("👎", key, disable_on_click, button_states, 2)
 
         if up:
-            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 1, "thumbs up")
+            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 1, "👍")
         elif down:
-            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 2, "thumbs down")
+            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 2, "👎")
         else:
             return None
 
     def st_faces_ui(self, disable_on_click: bool = False, key: Optional[str] = None) -> Optional[str]:
         if key is None:
             key = "faces"
 
@@ -315,35 +262,35 @@
             three = self._emoji_button("😐", key, disable_on_click, button_states, 3)
         with col4:
             four = self._emoji_button("🙂", key, disable_on_click, button_states, 4)
         with col5:
             five = self._emoji_button("😀", key, disable_on_click, button_states, 5)
 
         if one:
-            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 1, "very negative")
+            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 1, "😞")
         elif two:
-            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 2, "negative")
+            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 2, "🙁")
         elif three:
-            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 3, "neutral")
+            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 3, "😐")
         elif four:
-            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 4, "positive")
+            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 4, "🙂")
         elif five:
-            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 5, "very positive")
+            return self._return_quantitative_ui_button(key, disable_on_click, button_states, 5, "😀")
         else:
             return None
 
     @staticmethod
-    def _return_quantitative_ui_button(ui_type, disable_on_click, button_states, index, output_str):
+    def _return_quantitative_ui_button(ui_type, disable_on_click, button_states, index, output):
         if disable_on_click:
             if st.session_state[f"{ui_type}_state_clicked"] == button_states[index - 1]:
-                return f":{index} - {output_str}:"
+                return output
             else:
                 return None
         else:
-            return f":{index} - {output_str}:"
+            return output
 
     def _emoji_button(self, emoji, key, disable_on_click, button_states, index):
         return st.button(
             emoji,
             key=f"{key}_{index}",
             on_click=self._disable_buttons,
             args=(key, disable_on_click, index, button_states),
```

### Comparing `trubrics-1.3.7/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.4.0/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/ui/firestore.py` & `trubrics-1.4.0/trubrics/trubrics_platform/firestore.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,45 +3,48 @@
 """
 import json
 from datetime import datetime
 
 import requests  # type: ignore
 
 
-def json_to_firestore_document(json_object):
-    python_dict = json.loads(json_object)
+def dict_to_firestore_document(python_dict):
     firestore_compatible = {"fields": {}}
     for key, value in python_dict.items():
-        if isinstance(value, str):
+        if value is None:
+            firestore_compatible["fields"][key] = {"nullValue": value}
+        elif isinstance(value, str):
             firestore_compatible["fields"][key] = {"stringValue": value}
         elif isinstance(value, bool):
             firestore_compatible["fields"][key] = {"booleanValue": value}
         elif isinstance(value, int):
             firestore_compatible["fields"][key] = {"integerValue": value}
         elif isinstance(value, float):
             firestore_compatible["fields"][key] = {"doubleValue": value}
         elif isinstance(value, datetime):
             firestore_compatible["fields"][key] = {"timestampValue": value.isoformat() + "Z"}
         elif isinstance(value, dict):
-            firestore_compatible["fields"][key] = {"mapValue": json_to_firestore_document(json.dumps(value))}
+            firestore_compatible["fields"][key] = {"mapValue": dict_to_firestore_document(value)}
         elif isinstance(value, list):
             array_values = []
             for item in value:
-                if isinstance(item, str):
+                if value is None:
+                    array_values.append({"nullValue": item})
+                elif isinstance(item, str):
                     array_values.append({"stringValue": item})
                 elif isinstance(item, bool):
                     array_values.append({"booleanValue": item})
                 elif isinstance(item, int):
                     array_values.append({"integerValue": item})
                 elif isinstance(item, float):
                     array_values.append({"doubleValue": item})
                 elif isinstance(item, datetime):
                     array_values.append({"timestampValue": item.isoformat() + "Z"})
                 elif isinstance(item, dict):
-                    array_values.append({"mapValue": json_to_firestore_document(json.dumps(item))})
+                    array_values.append({"mapValue": dict_to_firestore_document(item)})
             firestore_compatible["fields"][key] = {"arrayValue": {"values": array_values}}
     return firestore_compatible
 
 
 def get_trubrics_firestore_api_url(auth, project_id):
     structured_query = {
         "structuredQuery": {
@@ -63,33 +66,61 @@
             headers={"Content-Type": "application/json", "Authorization": f"Bearer {auth['idToken']}"},
             data=json.dumps(structured_query),
         ).text
     )[0]["document"]["name"]
     return f"https://firestore.googleapis.com/v1/{organisation_route}"
 
 
-def list_projects_in_organisation(firestore_api_url, auth):
+def list_components_in_organisation(firestore_api_url, auth):
     r = requests.get(
-        firestore_api_url + "/projects" + "?pageSize=50",
+        firestore_api_url + "/feedback" + "?pageSize=50",
         headers={"Content-Type": "application/json", "Authorization": f"Bearer {auth['idToken']}"},
     )
     r.raise_for_status()
-    projects_res = json.loads(r.text)
+    components_res = json.loads(r.text)
 
-    all_projects = []
-    if len(projects_res) != 0:
-        for project in projects_res["documents"]:
-            if project.get("fields", {}).get("archived", {}).get("booleanValue", {}) is False:
-                all_projects.append(project["name"].split("/")[-1])
-    return all_projects
+    all_components = []
+    if len(components_res) != 0:
+        for component in components_res["documents"]:
+            if component.get("fields", {}).get("archived", {}).get("booleanValue", {}) is False:
+                all_components.append(component["name"].split("/")[-1])
+    return all_components
+
+
+def record_feedback(auth, firestore_api_url, document_dict):
+    url = firestore_api_url + f"/feedback/{document_dict['component_name']}/responses"
+    res = json.loads(
+        requests.post(
+            url,
+            headers={"Content-Type": "application/json", "Authorization": f"Bearer {auth['idToken']}"},
+            data=json.dumps(dict_to_firestore_document(document_dict)),
+        ).text
+    )
+    return res
 
 
-def add_document_to_project_subcollection(auth, firestore_api_url, project, subcollection, document_id, document_json):
+def add_document_to_project_subcollection(auth, firestore_api_url, project, subcollection, document_id, document_dict):
     url = firestore_api_url + f"/projects/{project}/{subcollection}/?documentId={document_id}"
     res = json.loads(
         requests.post(
             url,
             headers={"Content-Type": "application/json", "Authorization": f"Bearer {auth['idToken']}"},
-            data=json.dumps(json_to_firestore_document(document_json)),
+            data=json.dumps(dict_to_firestore_document(document_dict)),
         ).text
     )
     return res
+
+
+def list_projects_in_organisation(firestore_api_url, auth):
+    r = requests.get(
+        firestore_api_url + "/projects" + "?pageSize=50",
+        headers={"Content-Type": "application/json", "Authorization": f"Bearer {auth['idToken']}"},
+    )
+    r.raise_for_status()
+    projects_res = json.loads(r.text)
+
+    all_projects = []
+    if len(projects_res) != 0:
+        for project in projects_res["documents"]:
+            if project.get("fields", {}).get("archived", {}).get("booleanValue", {}) is False:
+                all_projects.append(project["name"].split("/")[-1])
+    return all_projects
```

### Comparing `trubrics-1.3.7/trubrics/ui/trubrics_config.py` & `trubrics-1.4.0/trubrics/trubrics_platform/trubrics_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import os
 
 from pydantic import BaseModel, SecretStr
 
 
 class TrubricsDefaults(BaseModel):
     # no stress, this is not a secret api key
-    firebase_api_key: str = "AIzaSyAWGOaN7_sL98irVM2g5O2RULK4yj9Tdvs"
-    firebase_project_id: str = "trubrics-ea-prod"
-    trubrics_url: str = "https://ea.trubrics.com/"
-    demo_sign_up_url: str = "https://trubrics.com/demo/"
+    firebase_api_key: str = "AIzaSyB6WPIVzMaRCnlL1ZmRosrQsbQYYagZARQ"
+    firebase_project_id: str = "trubrics-streamlit"
+    trubrics_url: str = "https://trubrics.streamlit.com/"
+    demo_sign_up_url: str = "https://trubrics.com/sign-up/"
 
 
 class TrubricsConfig(BaseModel):
-    firebase_auth_api_url: str
-    firestore_api_url: str
-    username: str
     email: str
     password: SecretStr
-    project: str
+    username: str
+    firebase_api_key: str
+    firestore_api_url: str
 
     class Config:
         json_encoders = {SecretStr: lambda v: v.get_secret_value() if v else None}
 
     def save(self):
         config_path = os.path.join(os.path.expanduser("~"), ".trubrics_config.json")
         with open(config_path, "w") as file:
```

### Comparing `trubrics-1.3.7/trubrics/validations/dataclass.py` & `trubrics-1.4.0/trubrics/validations/dataclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 from git import InvalidGitRepositoryError
 from git.repo import Repo
 from loguru import logger
 from pydantic import BaseModel, validator
 
 from trubrics.exceptions import TrubricValidationError
-from trubrics.ui.auth import expire_after_n_seconds, get_trubrics_auth_token
-from trubrics.ui.firestore import add_document_to_project_subcollection
-from trubrics.ui.trubrics_config import load_trubrics_config
+from trubrics.trubrics_platform.auth import (
+    expire_after_n_seconds,
+    get_trubrics_auth_token,
+)
+from trubrics.trubrics_platform.firestore import add_document_to_project_subcollection
+from trubrics.trubrics_platform.trubrics_config import load_trubrics_config
 
 
 def _validation_context_example():
     return {
         "example": {
             "validation_type": "validate_performance_against_threshold",
             "validation_kwargs": {"args": [], "kwargs": {"threshold": 0.8}},
@@ -121,30 +124,30 @@
 
         if raise_on_failure:
             self.raise_trubric_failure()
 
     def save_ui(self, raise_on_failure: bool = False):
         trubrics_config = load_trubrics_config()
         auth = get_trubrics_auth_token(
-            trubrics_config.firebase_auth_api_url,
+            trubrics_config.firebase_api_key,
             trubrics_config.email,
             trubrics_config.password.get_secret_value(),
             rerun=expire_after_n_seconds(),
         )
 
         self.run_by = {"email": trubrics_config.email, "displayName": trubrics_config.username}
         self.set_dynamic_fields()
 
         res = add_document_to_project_subcollection(
             auth,
             firestore_api_url=trubrics_config.firestore_api_url,
             project=trubrics_config.project,
             subcollection="trubrics",
             document_id=self.timestamp,
-            document_json=self.json(),
+            document_dict=self.dict(),
         )
         if "error" in res:
             error_msg = f"Error in pushing trubric to the Trubrics UI: {res}"
             logger.error(error_msg)
             raise Exception(error_msg)
         else:
             logger.info("Trubric saved to the Trubrics UI.")
```

### Comparing `trubrics-1.3.7/trubrics/validations/model/base.py` & `trubrics-1.4.0/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/validations/run.py` & `trubrics-1.4.0/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics/validations/validation_output.py` & `trubrics-1.4.0/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.7/trubrics.egg-info/SOURCES.txt` & `trubrics-1.4.0/trubrics.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -30,28 +30,29 @@
 trubrics/example/titanic.py
 trubrics/example/titanic_config.py
 trubrics/example/titanic_data.csv
 trubrics/example/trubric_run.py
 trubrics/feedback/__init__.py
 trubrics/feedback/config.py
 trubrics/feedback/dataclass.py
+trubrics/feedback/save_to_trubrics.py
 trubrics/integrations/__init__.py
 trubrics/integrations/dash/__init__.py
 trubrics/integrations/dash/collect.py
 trubrics/integrations/gradio/__init__.py
 trubrics/integrations/gradio/collect.py
 trubrics/integrations/mlflow/__init__.py
 trubrics/integrations/mlflow/trubrics_validator.py
 trubrics/integrations/streamlit/__init__.py
 trubrics/integrations/streamlit/collect.py
 trubrics/integrations/streamlit/experiment.py
-trubrics/ui/__init__.py
-trubrics/ui/auth.py
-trubrics/ui/firestore.py
-trubrics/ui/trubrics_config.py
+trubrics/trubrics_platform/__init__.py
+trubrics/trubrics_platform/auth.py
+trubrics/trubrics_platform/firestore.py
+trubrics/trubrics_platform/trubrics_config.py
 trubrics/utils/__init__.py
 trubrics/utils/pandas.py
 trubrics/validations/__init__.py
 trubrics/validations/dataclass.py
 trubrics/validations/run.py
 trubrics/validations/validation_output.py
 trubrics/validations/model/__init__.py
```

