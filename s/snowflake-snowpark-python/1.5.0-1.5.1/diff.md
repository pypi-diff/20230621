# Comparing `tmp/snowflake-snowpark-python-1.5.0.tar.gz` & `tmp/snowflake-snowpark-python-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-snowpark-python-1.5.0.tar", last modified: Tue Jun 13 23:22:15 2023, max compression
+gzip compressed data, was "snowflake-snowpark-python-1.5.1.tar", last modified: Wed Jun 21 18:14:55 2023, max compression
```

## Comparing `snowflake-snowpark-python-1.5.0.tar` & `snowflake-snowpark-python-1.5.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:15.360362 snowflake-snowpark-python-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    30994 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-06-13 23:22:15.360362 snowflake-snowpark-python-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:22:15.360362 snowflake-snowpark-python-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:15.336362 snowflake-snowpark-python-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:15.336362 snowflake-snowpark-python-1.5.0/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:15.352362 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:15.352362 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:15.356362 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42766 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)    40138 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/table_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    26737 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/code_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/server_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27689 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/udf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/async_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/context.py
--rw-r--r--   0 runner    (1001) docker     (123)   150984 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_na_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28130 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_stat_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/file_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/files.py
--rw-r--r--   0 runner    (1001) docker     (123)   269192 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/query_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/relational_grouped_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/row.py
--rw-r--r--   0 runner    (1001) docker     (123)    93056 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    39467 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/stored_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)    29592 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/table_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    45769 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/udf.py
--rw-r--r--   0 runner    (1001) docker     (123)    35699 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/udtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-06-13 23:22:02.000000 snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:22:15.360362 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-06-13 23:22:15.000000 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-13 23:22:15.000000 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:22:15.000000 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 23:22:15.000000 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:22:15.000000 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-13 23:22:15.000000 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 23:22:15.000000 snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:55.864706 snowflake-snowpark-python-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    31093 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    37741 2023-06-21 18:14:55.864706 snowflake-snowpark-python-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:14:55.864706 snowflake-snowpark-python-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:55.852706 snowflake-snowpark-python-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:55.852706 snowflake-snowpark-python-1.5.1/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:55.856706 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:55.860706 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:55.864706 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/binary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/grouping_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42766 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/select_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40138 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/sort_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/table_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/unary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/window_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26737 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/server_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27689 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/udf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/async_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150984 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_na_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28130 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_stat_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/file_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)   269192 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/query_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/relational_grouped_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93056 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39467 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/stored_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29592 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/table_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45807 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/udf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35699 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/udtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-06-21 18:14:44.000000 snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:14:55.864706 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37741 2023-06-21 18:14:55.000000 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-21 18:14:55.000000 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:14:55.000000 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 18:14:55.000000 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:14:55.000000 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-21 18:14:55.000000 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 18:14:55.000000 snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/top_level.txt
```

### Comparing `snowflake-snowpark-python-1.5.0/CHANGELOG.md` & `snowflake-snowpark-python-1.5.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 1.5.1 (2023-06-20)
+
+### New Features
+
+- Added support for the Python 3.10 runtime environment.
+
 ## 1.5.0 (2023-06-09)
 
 ### Behavior Changes
 
 - Aggregation results, from functions such as `DataFrame.agg` and `DataFrame.describe`, no longer strip away non-printing characters from column names.
 
 ### New Features
```

### Comparing `snowflake-snowpark-python-1.5.0/LICENSE.txt` & `snowflake-snowpark-python-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/PKG-INFO` & `snowflake-snowpark-python-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-snowpark-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: Snowflake Snowpark for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/developer-guide/snowpark/python/index.html
 Project-URL: Source, https://github.com/snowflakedb/snowpark-python
@@ -20,21 +20,22 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8, <3.10
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: secure-local-storage
 Provides-Extra: development
 License-File: LICENSE.txt
 
 # Snowflake Snowpark Python API
@@ -52,16 +53,16 @@
 
 ## Getting started
 
 ### Have your Snowflake account ready
 If you don't have a Snowflake account yet, you can [sign up for a 30-day free trial account][sign up trial].
 
 ### Create a Python virtual environment
-Python 3.8 is required. You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
-to create a Python 3.8 virtual environment.
+You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
+to create a Python 3.8, 3.9 or 3.10 virtual environment.
 
 To have the best experience when using it with UDFs, [creating a local conda environment with the Snowflake channel][use snowflake channel] is recommended.
 
 ### Install the library to the Python virtual environment
 ```bash
 pip install snowflake-snowpark-python
 ```
@@ -131,14 +132,20 @@
 [snowflake lab sample code]: https://github.com/Snowflake-Labs/snowpark-python-demos
 [samples]: https://github.com/snowflakedb/snowpark-python/blob/main/README.md#samples
 [contributing]: https://github.com/snowflakedb/snowpark-python/blob/main/CONTRIBUTING.md
 
 
 # Release History
 
+## 1.5.1 (2023-06-20)
+
+### New Features
+
+- Added support for the Python 3.10 runtime environment.
+
 ## 1.5.0 (2023-06-09)
 
 ### Behavior Changes
 
 - Aggregation results, from functions such as `DataFrame.agg` and `DataFrame.describe`, no longer strip away non-printing characters from column names.
 
 ### New Features
```

### Comparing `snowflake-snowpark-python-1.5.0/README.md` & `snowflake-snowpark-python-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 ## Getting started
 
 ### Have your Snowflake account ready
 If you don't have a Snowflake account yet, you can [sign up for a 30-day free trial account][sign up trial].
 
 ### Create a Python virtual environment
-Python 3.8 is required. You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
-to create a Python 3.8 virtual environment.
+You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
+to create a Python 3.8, 3.9 or 3.10 virtual environment.
 
 To have the best experience when using it with UDFs, [creating a local conda environment with the Snowflake channel][use snowflake channel] is recommended.
 
 ### Install the library to the Python virtual environment
 ```bash
 pip install snowflake-snowpark-python
 ```
```

### Comparing `snowflake-snowpark-python-1.5.0/setup.py` & `snowflake-snowpark-python-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 SRC_DIR = os.path.join(THIS_DIR, "src")
 SNOWPARK_SRC_DIR = os.path.join(SRC_DIR, "snowflake", "snowpark")
 CONNECTOR_DEPENDENCY_VERSION = ">=2.7.12, <4.0.0"
-REQUIRED_PYTHON_VERSION = ">=3.8, <3.10"
+REQUIRED_PYTHON_VERSION = ">=3.8, <3.11"
 if os.getenv("SNOWFLAKE_IS_PYTHON_RUNTIME_TEST", False):
     REQUIRED_PYTHON_VERSION = ">=3.8"
 
 # read the version
 VERSION = ()
 with open(os.path.join(SNOWPARK_SRC_DIR, "version.py"), encoding="utf-8") as f:
     exec(f.read())
@@ -91,14 +91,15 @@
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: SQL",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Database",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Scientific/Engineering :: Information Analysis",
     ],
```

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/__init__.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/binary_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/expression.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/grouping_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/schema_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/select_statement.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/sort_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/table_function.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/table_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/unary_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/analyzer/window_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/code_generation.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/code_generation.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/error_message.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/error_message.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/server_connection.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/server_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/telemetry.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/type_utils.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/type_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/udf_utils.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/udf_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/_internal/utils.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/async_job.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/async_job.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/column.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/column.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/context.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/context.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_na_functions.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_na_functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_reader.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_stat_functions.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_stat_functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/dataframe_writer.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/dataframe_writer.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/exceptions.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/file_operation.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/file_operation.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/files.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/files.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/functions.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/query_history.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/query_history.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/relational_grouped_dataframe.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/relational_grouped_dataframe.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/row.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/row.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/session.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/session.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/stored_procedure.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/stored_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/table.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/table.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/table_function.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/table_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/types.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
             and self.length == StringType._MAX_LENGTH
         ):
             return True
 
         return False
 
     def __hash__(self):
+        if self.length == StringType._MAX_LENGTH:
+            return StringType().__hash__()
         return super().__hash__()
 
 
 class _NumericType(_AtomicType):
     pass
```

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/udf.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,17 +203,18 @@
     inefficient, a vectorized UDF allows vectorized operations on a dataframe, with the input as a
     `Pandas DataFrame <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html>`_
     or `Pandas Series <https://pandas.pydata.org/docs/reference/api/pandas.Series.html>`_. In a
     vectorized UDF, you can operate on a batches of rows by handling Pandas DataFrame or Pandas
     Series. You can use :func:`~snowflake.snowpark.functions.udf`, :meth:`register` or
     :func:`~snowflake.snowpark.functions.pandas_udf` to create a vectorized UDF by providing
     appropriate return and input types. If you would like to use :meth:`register_from_file` to
-    create a vectorized UDF, you should follow the guide of
-    `Python UDF Batch API <https://docs.snowflake.com/en/developer-guide/udf/python/udf-python-batch.html>`_ in
-    your Python source files. See Example 9, 10 and 11 here for registering a vectorized UDF.
+    create a vectorized UDF, you would need to explicitly mark the handler function as vectorized using
+    either the `vectorized` Decorator or a function attribute. Please see
+    `Python UDF Batch API <https://docs.snowflake.com/en/developer-guide/udf/python/udf-python-batch.html>`
+    for examples.
 
     Snowflake supports the following data types for the parameters for a UDF:
 
     =============================================  ======================================================= ============
     Python Type                                    Snowpark Type                                           SQL Type
     =============================================  ======================================================= ============
     ``int``                                        :class:`~snowflake.snowpark.types.LongType`             NUMBER
```

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/udtf.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/udtf.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake/snowpark/window.py` & `snowflake-snowpark-python-1.5.1/src/snowflake/snowpark/window.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/PKG-INFO` & `snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-snowpark-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: Snowflake Snowpark for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/developer-guide/snowpark/python/index.html
 Project-URL: Source, https://github.com/snowflakedb/snowpark-python
@@ -20,21 +20,22 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8, <3.10
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: secure-local-storage
 Provides-Extra: development
 License-File: LICENSE.txt
 
 # Snowflake Snowpark Python API
@@ -52,16 +53,16 @@
 
 ## Getting started
 
 ### Have your Snowflake account ready
 If you don't have a Snowflake account yet, you can [sign up for a 30-day free trial account][sign up trial].
 
 ### Create a Python virtual environment
-Python 3.8 is required. You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
-to create a Python 3.8 virtual environment.
+You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
+to create a Python 3.8, 3.9 or 3.10 virtual environment.
 
 To have the best experience when using it with UDFs, [creating a local conda environment with the Snowflake channel][use snowflake channel] is recommended.
 
 ### Install the library to the Python virtual environment
 ```bash
 pip install snowflake-snowpark-python
 ```
@@ -131,14 +132,20 @@
 [snowflake lab sample code]: https://github.com/Snowflake-Labs/snowpark-python-demos
 [samples]: https://github.com/snowflakedb/snowpark-python/blob/main/README.md#samples
 [contributing]: https://github.com/snowflakedb/snowpark-python/blob/main/CONTRIBUTING.md
 
 
 # Release History
 
+## 1.5.1 (2023-06-20)
+
+### New Features
+
+- Added support for the Python 3.10 runtime environment.
+
 ## 1.5.0 (2023-06-09)
 
 ### Behavior Changes
 
 - Aggregation results, from functions such as `DataFrame.agg` and `DataFrame.describe`, no longer strip away non-printing characters from column names.
 
 ### New Features
```

### Comparing `snowflake-snowpark-python-1.5.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt` & `snowflake-snowpark-python-1.5.1/src/snowflake_snowpark_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

