# Comparing `tmp/dbt-athena-community-1.5.0.tar.gz` & `tmp/dbt-athena-community-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-athena-community-1.5.0.tar", last modified: Mon May 15 13:38:15 2023, max compression
+gzip compressed data, was "dbt-athena-community-1.5.1.tar", last modified: Wed Jun 21 10:38:18 2023, max compression
```

## Comparing `dbt-athena-community-1.5.0.tar` & `dbt-athena-community-1.5.1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.826985 dbt-athena-community-1.5.0/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36236 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.818985 dbt-athena-community-1.5.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.830985 dbt-athena-community-1.5.0/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.830985 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.822985 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.818985 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.834986 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.838986 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 13:38:15.000000 dbt-athena-community-1.5.0/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:38:15.842986 dbt-athena-community-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-15 13:38:04.000000 dbt-athena-community-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.397674 dbt-athena-community-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-06-21 10:38:18.397674 dbt-athena-community-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.385674 dbt-athena-community-1.5.1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.385674 dbt-athena-community-1.5.1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.385674 dbt-athena-community-1.5.1/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36007 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/lakeformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.381674 dbt-athena-community-1.5.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.389674 dbt-athena-community-1.5.1/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.381674 dbt-athena-community-1.5.1/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.389674 dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.381674 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.381674 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.389674 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.389674 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.389674 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.393674 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.393674 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.393674 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:18.397674 dbt-athena-community-1.5.1/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-06-21 10:38:18.000000 dbt-athena-community-1.5.1/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-21 10:38:18.000000 dbt-athena-community-1.5.1/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:38:18.000000 dbt-athena-community-1.5.1/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 10:38:18.000000 dbt-athena-community-1.5.1/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-21 10:38:18.000000 dbt-athena-community-1.5.1/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:38:18.397674 dbt-athena-community-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-21 10:38:06.000000 dbt-athena-community-1.5.1/setup.py
```

### Comparing `dbt-athena-community-1.5.0/LICENSE.txt` & `dbt-athena-community-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/PKG-INFO` & `dbt-athena-community-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,13 @@
-Metadata-Version: 2.1
-Name: dbt-athena-community
-Version: 1.5.0
-Summary: The athena adapter plugin for dbt (data build tool)
-Home-page: https://github.com/dbt-athena/dbt-athena
-License: Apache License 2.0
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
+    <a href="https://github.com/python/mypy"><img src="https://www.mypy-lang.org/static/mypy_badge.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
 * Supports dbt version `1.5.*`
 * Supports [seeds][seeds]
@@ -99,15 +80,14 @@
 | database              | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                           |
 | poll_interval         | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                        |
 | aws_access_key_id     | Access key ID of the user performing requests.                                 | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
 | aws_secret_access_key | Secret access key of the user performing requests                              | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
 | aws_profile_name      | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                               |
 | work_group            | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                      |
 | num_retries           | Number of times to retry a failing query                                       | Optional  | `3`                                        |
-| lf_tags               | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}`   |
 
 **Example profiles.yml entry:**
 ```yaml
 athena:
   target: dev
   outputs:
     dev:
@@ -116,17 +96,14 @@
       s3_data_dir: s3://your_s3_bucket/dbt/
       s3_data_naming: schema_table
       region_name: eu-west-1
       schema: dbt
       database: awsdatacatalog
       aws_profile_name: my-profile
       work_group: my-workgroup
-      lf_tags:
-        origin: dbt
-        team: analytics
 ```
 
 _Additional information_
 * `threads` is supported
 * `database` and `catalog` can be used interchangeably
 
 
@@ -154,20 +131,82 @@
   * The data format for the table
   * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE`
 * `write_compression` (`default=none`)
   * The compression type to use for any storage format that allows compression to be specified. To see which options are available, check out [CREATE TABLE AS][create-table-as]
 * `field_delimiter` (`default=none`)
   * Custom field delimiter, for when format is set to `TEXTFILE`
 * `table_properties`: table properties to add to the table, valid for Iceberg only
-* `lf_tags` (`default=none`)
-  * lf tags to associate with the table
-  * format: `{"tag1": "value1", "tag2": "value2"}`
-* `lf_tags_columns` (`default=none`)
-  * lf tags to associate with the table columns
-  * format: `{"tag1": {"value1": ["column1": "column2"]}}`
++ `native_drop`: Relation drop operations will be performed with SQL, not direct Glue API calls. No S3 calls will be made to manage data in S3. Data in S3 will only be cleared up for Iceberg tables [see AWS docs](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html). Note that Iceberg DROP TABLE operations may timeout if they take longer than 60 seconds.
++ `seed_by_insert` (`default=false`)
+  + default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
+  + large seed files cannot use `seed_by_insert`, as the SQL insert statement would exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/latest/ug/service-limits.html)
+* `lf_tags_config` (`default=none`)
+  * [AWS lakeformation](#aws-lakeformation-integration) tags to associate with the table and columns
+  * format for model config:
+```sql
+{{
+  config(
+    materialized='incremental',
+    incremental_strategy='append',
+    on_schema_change='append_new_columns',
+    table_type='iceberg',
+    schema='test_schema',
+    lf_tags_config={
+          'enabled': true,
+          'tags': {
+            'tag1': 'value1',
+            'tag2': 'value2'
+          },
+          'tags_columns': {
+            'tag1': {
+              'value1': ['column1', 'column2'],
+              'value2': ['column3', 'column4']
+            }
+          }
+    }
+  )
+}}
+```
+* format for `dbt_project.yml`:
+```yaml
+  +lf_tags_config:
+    enabled: true
+    tags:
+      tag1: value1
+      tag2: value2
+    tags_columns:
+      tag1:
+        value1: [ column1, column2 ]
+```
+* `lf_grants` (`default=none`)
+  * lakeformation grants config for data_cell filters
+  * format:
+  ```python
+  lf_grants={
+          'data_cell_filters': {
+              'enabled': True | False,
+              'filters': {
+                  'filter_name': {
+                      'row_filter': '<filter_condition>',
+                      'principals': ['principal_arn1', 'principal_arn2']
+                  }
+              }
+          }
+      }
+  ```
+
+> Notes:  
+> - `lf_tags` and `lf_tags_columns` configs support only attaching lf tags to corresponding resources.
+> We recommend managing LF Tags permissions somewhere outside dbt. For example, you may use
+> [terraform](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions) or
+> [aws cdk](https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for such purpose.
+> - `data_cell_filters` management can't be automated outside dbt because the filter can't be attached to the table
+> which doesn't exist. Once you `enable` this config, dbt will set all filters and their permissions during every
+> dbt run. Such approach keeps the actual state of row level security configuration actual after every dbt run and
+> apply changes if they occur: drop, create, update filters and their permissions.
 
 [create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 
 ### Table location
 
 The location in which a table is saved is determined by:
 
@@ -239,28 +278,28 @@
 ```
 
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
 It is possible to use Iceberg in an incremental fashion, specifically two strategies are supported:
-* `append`: new records are appended to the table, this can lead to duplicates
-* `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
-   It performs an upsert, new record are added, and record already existing are updated. If
-   `delete_condition` is provided in the model config, it can also delete records based on the
-   provided condition (SQL condition). You can use any column of the incremental table (`src`) or
-   the final table (`target`). You must prefix the column by the name of the table to prevent
-   `Column is ambiguous` error.
+* `append`: New records are appended to the table, this can lead to duplicates.
+* `merge`: Performs an upsert (and optional delete), where new records are added and existing records are updated. Only available with Athena engine version 3.
+    - `unique_key` **(required)**: columns that define a unique record in the source and target tables.
+    - `incremental_predicates` (optional): SQL conditions that enable custom join clauses in the merge statement. This can be useful for improving performance via predicate pushdown on the target table.
+    - `delete_condition` (optional): SQL condition used to identify records that should be deleted.
+      - `delete_condition` and `incremental_predicates` can include any column of the incremental table (`src`) or the final table (`target`). Column names must be prefixed by either `src` or `target` to prevent a `Column is ambiguous` error.
 
 ```sql
 {{ config(
     materialized='incremental',
     table_type='iceberg',
     incremental_strategy='merge',
     unique_key='user_id',
+    incremental_predicates=["src.quantity > 1", "target.my_date >= now() - interval '4' year"],
     delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year",
     format='parquet'
 ) }}
 
 select
 	'A' as user_id,
 	'pi' as name,
@@ -280,15 +319,15 @@
 
 ```sql
 {{ config(
     materialized='table',
     ha=true,
     format='parquet',
     table_type='hive',
-    partition_by=['status'],
+    partitioned_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
 select
   'a' as user_id,
   'pi' as user_name,
   'active' as status
@@ -321,14 +360,32 @@
 
 To use the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy)
 
 ### Hard-deletes
 
 The materialization also supports invalidating hard deletes. Check the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to understand usage.
 
+### AWS Lakeformation integration
+
+The adapter implements AWS Lakeformation tags management in the following way:
+- you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
+- once you enable the feature, lf-tags will be updated on every dbt run
+- first, all lf-tags for columns are removed to avoid inheritance issues
+- then all redundant lf-tags are removed from table and actual tags from config are applied
+- finally, lf-tags for columns are applied
+
+It's important to understand the following points:
+- dbt does not manage lf-tags for database
+- dbt does not manage lakeformation permissions
+
+That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.  
+You may find the following links useful to manage that:
+- [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
+- [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
+
 ### Working example
 
 seed file - employent_indicators_november_2022_csv_tables.csv
 ```
 Series_reference,Period,Data_value,Suppressed
 MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803,
```

#### html2text {}

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.5.0 Summary: The
-athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
-dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
- code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
-                                    month]
+       code%20style-black-000000.svg] [https://www.mypy-lang.org/static/
+     mypy_badge.svg] [https://pepy.tech/badge/dbt-athena-community/month]
 ## Features * Supports dbt version `1.5.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
 [table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
 * Hive tables are supported by both Athena engines. * Supports [incremental
 models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
 only with the `merge` strategy * Supports the `append` strategy * On Hive
@@ -64,45 +53,72 @@
 results in Athena | Optional | `5` | | aws_access_key_id | Access key ID of the
 user performing requests. | Optional | `AKIAIOSFODNN7EXAMPLE` | |
 aws_secret_access_key | Secret access key of the user performing requests |
 Optional | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` | | aws_profile_name |
 Profile to use from your AWS shared credentials file. | Optional | `my-profile`
 | | work_group | Identifier of Athena workgroup | Optional | `my-custom-
 workgroup` | | num_retries | Number of times to retry a failing query |
-Optional | `3` | | lf_tags | Default lf tags to apply to any database created
-by dbt | Optional | `{"origin": "dbt", "team": "analytics"}` | **Example
-profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
-s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
-your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
-dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
-workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
-`threads` is supported * `database` and `catalog` can be used interchangeably
-## Models ### Table Configuration * `external_location` (`default=none`) * If
-set, the full S3 path in which the table will be saved. * Does not work with
-Iceberg table or Hive table with `ha` set to true. * `partitioned_by`
-(`default=none`) * An array list of columns by which the table will be
-partitioned * Limited to creation of 100 partitions (_currently_) *
-`bucketed_by` (`default=none`) * An array list of columns to bucket data,
-ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
-buckets for bucketing your data, ignored if using Iceberg * `table_type`
-(`default='hive'`) * The type of table * Supports `hive` or `iceberg` * `ha`
-(`default=false`) * If the table should be built using the high-availability
-method. This option is only available for Hive tables since it is by default
-for Iceberg tables (see the section [below](#highly-available-table)) *
-`format` (`default='parquet'`) * The data format for the table * Supports
-`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
-(`default=none`) * The compression type to use for any storage format that
-allows compression to be specified. To see which options are available, check
-out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
-Custom field delimiter, for when format is set to `TEXTFILE` *
-`table_properties`: table properties to add to the table, valid for Iceberg
-only * `lf_tags` (`default=none`) * lf tags to associate with the table *
-format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
-(`default=none`) * lf tags to associate with the table columns * format: `
-{"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
+Optional | `3` | **Example profiles.yml entry:** ```yaml athena: target: dev
+outputs: dev: type: athena s3_staging_dir: s3://athena-query-results/dbt/
+s3_data_dir: s3://your_s3_bucket/dbt/ s3_data_naming: schema_table region_name:
+eu-west-1 schema: dbt database: awsdatacatalog aws_profile_name: my-profile
+work_group: my-workgroup ``` _Additional information_ * `threads` is supported
+* `database` and `catalog` can be used interchangeably ## Models ### Table
+Configuration * `external_location` (`default=none`) * If set, the full S3 path
+in which the table will be saved. * Does not work with Iceberg table or Hive
+table with `ha` set to true. * `partitioned_by` (`default=none`) * An array
+list of columns by which the table will be partitioned * Limited to creation of
+100 partitions (_currently_) * `bucketed_by` (`default=none`) * An array list
+of columns to bucket data, ignored if using Iceberg * `bucket_count`
+(`default=none`) * The number of buckets for bucketing your data, ignored if
+using Iceberg * `table_type` (`default='hive'`) * The type of table * Supports
+`hive` or `iceberg` * `ha` (`default=false`) * If the table should be built
+using the high-availability method. This option is only available for Hive
+tables since it is by default for Iceberg tables (see the section [below]
+(#highly-available-table)) * `format` (`default='parquet'`) * The data format
+for the table * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` *
+`write_compression` (`default=none`) * The compression type to use for any
+storage format that allows compression to be specified. To see which options
+are available, check out [CREATE TABLE AS][create-table-as] * `field_delimiter`
+(`default=none`) * Custom field delimiter, for when format is set to `TEXTFILE`
+* `table_properties`: table properties to add to the table, valid for Iceberg
+only + `native_drop`: Relation drop operations will be performed with SQL, not
+direct Glue API calls. No S3 calls will be made to manage data in S3. Data in
+S3 will only be cleared up for Iceberg tables [see AWS docs](https://
+docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html).
+Note that Iceberg DROP TABLE operations may timeout if they take longer than 60
+seconds. + `seed_by_insert` (`default=false`) + default behaviour uploads seed
+data to S3. This flag will create seeds using an SQL insert statement + large
+seed files cannot use `seed_by_insert`, as the SQL insert statement would
+exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/
+latest/ug/service-limits.html) * `lf_tags_config` (`default=none`) * [AWS
+lakeformation](#aws-lakeformation-integration) tags to associate with the table
+and columns * format for model config: ```sql {{ config
+( materialized='incremental', incremental_strategy='append',
+on_schema_change='append_new_columns', table_type='iceberg',
+schema='test_schema', lf_tags_config={ 'enabled': true, 'tags': { 'tag1':
+'value1', 'tag2': 'value2' }, 'tags_columns': { 'tag1': { 'value1': ['column1',
+'column2'], 'value2': ['column3', 'column4'] } } } ) }} ``` * format for
+`dbt_project.yml`: ```yaml +lf_tags_config: enabled: true tags: tag1: value1
+tag2: value2 tags_columns: tag1: value1: [ column1, column2 ] ``` * `lf_grants`
+(`default=none`) * lakeformation grants config for data_cell filters * format:
+```python lf_grants={ 'data_cell_filters': { 'enabled': True | False,
+'filters': { 'filter_name': { 'row_filter': '', 'principals':
+['principal_arn1', 'principal_arn2'] } } } } ``` > Notes: > - `lf_tags` and
+`lf_tags_columns` configs support only attaching lf tags to corresponding
+resources. > We recommend managing LF Tags permissions somewhere outside dbt.
+For example, you may use > [terraform](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) or > [aws cdk]
+(https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for
+such purpose. > - `data_cell_filters` management can't be automated outside dbt
+because the filter can't be attached to the table > which doesn't exist. Once
+you `enable` this config, dbt will set all filters and their permissions during
+every > dbt run. Such approach keeps the actual state of row level security
+configuration actual after every dbt run and > apply changes if they occur:
+drop, create, update filters and their permissions. [create-table-as]: https://
 docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 ### Table location The location in which a table is saved is determined by: 1.
 If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
 defined, the path is determined by that and `s3_data_naming` 3. If
 `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
 ` Here all the options available for `s3_data_naming`: * `unique`: `
 {s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
@@ -133,37 +149,43 @@
 table_type='iceberg', format='parquet', partitioned_by=['bucket(user_id, 5)'],
 table_properties={ 'optimize_rewrite_delete_file_threshold': '2' } ) }} select
 'A' as user_id, 'pi' as name, 'active' as status, 17.89 as cost, 1 as quantity,
 100000000 as quantity_big, current_date as my_date ``` Iceberg supports
 bucketing as hidden partitions, therefore use the `partitioned_by` config to
 add specific bucketing conditions. Iceberg supports several table formats for
 data : `PARQUET`, `AVRO` and `ORC`. It is possible to use Iceberg in an
-incremental fashion, specifically two strategies are supported: * `append`: new
-records are appended to the table, this can lead to duplicates * `merge`: must
-be used in combination with `unique_key` and it's only available with Engine
-version 3. It performs an upsert, new record are added, and record already
-existing are updated. If `delete_condition` is provided in the model config, it
-can also delete records based on the provided condition (SQL condition). You
-can use any column of the incremental table (`src`) or the final table
-(`target`). You must prefix the column by the name of the table to prevent
-`Column is ambiguous` error. ```sql {{ config( materialized='incremental',
-table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
+incremental fashion, specifically two strategies are supported: * `append`: New
+records are appended to the table, this can lead to duplicates. * `merge`:
+Performs an upsert (and optional delete), where new records are added and
+existing records are updated. Only available with Athena engine version 3. -
+`unique_key` **(required)**: columns that define a unique record in the source
+and target tables. - `incremental_predicates` (optional): SQL conditions that
+enable custom join clauses in the merge statement. This can be useful for
+improving performance via predicate pushdown on the target table. -
+`delete_condition` (optional): SQL condition used to identify records that
+should be deleted. - `delete_condition` and `incremental_predicates` can
+include any column of the incremental table (`src`) or the final table
+(`target`). Column names must be prefixed by either `src` or `target` to
+prevent a `Column is ambiguous` error. ```sql {{ config
+( materialized='incremental', table_type='iceberg',
+incremental_strategy='merge', unique_key='user_id', incremental_predicates=
+["src.quantity > 1", "target.my_date >= now() - interval '4' year"],
 delete_condition="src.status != 'active' and target.my_date < now() - interval
 '2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
 as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
 current_date as my_date ``` ### Highly available table The current
 implementation of the table materialization can lead to downtime, as target
 table is dropped and re-created. To have the less destructive behavior it's
 possible to use the `ha` config on your `table` materialized models. It
 leverages the table versions feature of glue catalog, creating a tmp table and
 swapping the target table to the location of the tmp table. This
 materialization is only available for `table_type=hive` and requires using
 unique locations. For iceberg, high availability is by default. ```sql {
 { config( materialized='table', ha=true, format='parquet', table_type='hive',
-partition_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
+partitioned_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
 user_id, 'pi' as user_name, 'active' as status union all select 'b' as user_id,
 'sh' as user_name, 'disabled' as status ``` By default, the materialization
 keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions * By default, Glue "duplicates" the versions internally,
@@ -176,16 +198,30 @@
 snapshot create a snapshot file in the snapshots directory. If the directory
 does not exist create one. ### Timestamp strategy To use the timestamp strategy
 refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
 strategy-recommended) ### Check strategy To use the check strategy refer to the
 [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
 Hard-deletes The materialization also supports invalidating hard deletes. Check
 the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
-understand usage. ### Working example seed file -
-employent_indicators_november_2022_csv_tables.csv ```
+understand usage. ### AWS Lakeformation integration The adapter implements AWS
+Lakeformation tags management in the following way: - you can enable or disable
+lf-tags management via [config](#table-configuration) (disabled by default) -
+once you enable the feature, lf-tags will be updated on every dbt run - first,
+all lf-tags for columns are removed to avoid inheritance issues - then all
+redundant lf-tags are removed from table and actual tags from config are
+applied - finally, lf-tags for columns are applied It's important to understand
+the following points: - dbt does not manage lf-tags for database - dbt does not
+manage lakeformation permissions That's why you should handle this by yourself
+manually or using some automation tools like terraform, AWS CDK etc. You may
+find the following links useful to manage that: - [terraform
+aws_lakeformation_permissions](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) - [terraform
+aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ### Working
+example seed file - employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
```

### Comparing `dbt-athena-community-1.5.0/README.md` & `dbt-athena-community-1.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: dbt-athena-community
+Version: 1.5.1
+Summary: The athena adapter plugin for dbt (data build tool)
+Home-page: https://github.com/dbt-athena/dbt-athena
+License: Apache License 2.0
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
+    <a href="https://github.com/python/mypy"><img src="https://www.mypy-lang.org/static/mypy_badge.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
 * Supports dbt version `1.5.*`
 * Supports [seeds][seeds]
@@ -79,15 +100,14 @@
 | database              | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                           |
 | poll_interval         | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                        |
 | aws_access_key_id     | Access key ID of the user performing requests.                                 | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
 | aws_secret_access_key | Secret access key of the user performing requests                              | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
 | aws_profile_name      | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                               |
 | work_group            | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                      |
 | num_retries           | Number of times to retry a failing query                                       | Optional  | `3`                                        |
-| lf_tags               | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}`   |
 
 **Example profiles.yml entry:**
 ```yaml
 athena:
   target: dev
   outputs:
     dev:
@@ -96,17 +116,14 @@
       s3_data_dir: s3://your_s3_bucket/dbt/
       s3_data_naming: schema_table
       region_name: eu-west-1
       schema: dbt
       database: awsdatacatalog
       aws_profile_name: my-profile
       work_group: my-workgroup
-      lf_tags:
-        origin: dbt
-        team: analytics
 ```
 
 _Additional information_
 * `threads` is supported
 * `database` and `catalog` can be used interchangeably
 
 
@@ -134,20 +151,82 @@
   * The data format for the table
   * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE`
 * `write_compression` (`default=none`)
   * The compression type to use for any storage format that allows compression to be specified. To see which options are available, check out [CREATE TABLE AS][create-table-as]
 * `field_delimiter` (`default=none`)
   * Custom field delimiter, for when format is set to `TEXTFILE`
 * `table_properties`: table properties to add to the table, valid for Iceberg only
-* `lf_tags` (`default=none`)
-  * lf tags to associate with the table
-  * format: `{"tag1": "value1", "tag2": "value2"}`
-* `lf_tags_columns` (`default=none`)
-  * lf tags to associate with the table columns
-  * format: `{"tag1": {"value1": ["column1": "column2"]}}`
++ `native_drop`: Relation drop operations will be performed with SQL, not direct Glue API calls. No S3 calls will be made to manage data in S3. Data in S3 will only be cleared up for Iceberg tables [see AWS docs](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html). Note that Iceberg DROP TABLE operations may timeout if they take longer than 60 seconds.
++ `seed_by_insert` (`default=false`)
+  + default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
+  + large seed files cannot use `seed_by_insert`, as the SQL insert statement would exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/latest/ug/service-limits.html)
+* `lf_tags_config` (`default=none`)
+  * [AWS lakeformation](#aws-lakeformation-integration) tags to associate with the table and columns
+  * format for model config:
+```sql
+{{
+  config(
+    materialized='incremental',
+    incremental_strategy='append',
+    on_schema_change='append_new_columns',
+    table_type='iceberg',
+    schema='test_schema',
+    lf_tags_config={
+          'enabled': true,
+          'tags': {
+            'tag1': 'value1',
+            'tag2': 'value2'
+          },
+          'tags_columns': {
+            'tag1': {
+              'value1': ['column1', 'column2'],
+              'value2': ['column3', 'column4']
+            }
+          }
+    }
+  )
+}}
+```
+* format for `dbt_project.yml`:
+```yaml
+  +lf_tags_config:
+    enabled: true
+    tags:
+      tag1: value1
+      tag2: value2
+    tags_columns:
+      tag1:
+        value1: [ column1, column2 ]
+```
+* `lf_grants` (`default=none`)
+  * lakeformation grants config for data_cell filters
+  * format:
+  ```python
+  lf_grants={
+          'data_cell_filters': {
+              'enabled': True | False,
+              'filters': {
+                  'filter_name': {
+                      'row_filter': '<filter_condition>',
+                      'principals': ['principal_arn1', 'principal_arn2']
+                  }
+              }
+          }
+      }
+  ```
+
+> Notes:  
+> - `lf_tags` and `lf_tags_columns` configs support only attaching lf tags to corresponding resources.
+> We recommend managing LF Tags permissions somewhere outside dbt. For example, you may use
+> [terraform](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions) or
+> [aws cdk](https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for such purpose.
+> - `data_cell_filters` management can't be automated outside dbt because the filter can't be attached to the table
+> which doesn't exist. Once you `enable` this config, dbt will set all filters and their permissions during every
+> dbt run. Such approach keeps the actual state of row level security configuration actual after every dbt run and
+> apply changes if they occur: drop, create, update filters and their permissions.
 
 [create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 
 ### Table location
 
 The location in which a table is saved is determined by:
 
@@ -219,28 +298,28 @@
 ```
 
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
 It is possible to use Iceberg in an incremental fashion, specifically two strategies are supported:
-* `append`: new records are appended to the table, this can lead to duplicates
-* `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
-   It performs an upsert, new record are added, and record already existing are updated. If
-   `delete_condition` is provided in the model config, it can also delete records based on the
-   provided condition (SQL condition). You can use any column of the incremental table (`src`) or
-   the final table (`target`). You must prefix the column by the name of the table to prevent
-   `Column is ambiguous` error.
+* `append`: New records are appended to the table, this can lead to duplicates.
+* `merge`: Performs an upsert (and optional delete), where new records are added and existing records are updated. Only available with Athena engine version 3.
+    - `unique_key` **(required)**: columns that define a unique record in the source and target tables.
+    - `incremental_predicates` (optional): SQL conditions that enable custom join clauses in the merge statement. This can be useful for improving performance via predicate pushdown on the target table.
+    - `delete_condition` (optional): SQL condition used to identify records that should be deleted.
+      - `delete_condition` and `incremental_predicates` can include any column of the incremental table (`src`) or the final table (`target`). Column names must be prefixed by either `src` or `target` to prevent a `Column is ambiguous` error.
 
 ```sql
 {{ config(
     materialized='incremental',
     table_type='iceberg',
     incremental_strategy='merge',
     unique_key='user_id',
+    incremental_predicates=["src.quantity > 1", "target.my_date >= now() - interval '4' year"],
     delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year",
     format='parquet'
 ) }}
 
 select
 	'A' as user_id,
 	'pi' as name,
@@ -260,15 +339,15 @@
 
 ```sql
 {{ config(
     materialized='table',
     ha=true,
     format='parquet',
     table_type='hive',
-    partition_by=['status'],
+    partitioned_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
 select
   'a' as user_id,
   'pi' as user_name,
   'active' as status
@@ -301,14 +380,32 @@
 
 To use the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy)
 
 ### Hard-deletes
 
 The materialization also supports invalidating hard deletes. Check the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to understand usage.
 
+### AWS Lakeformation integration
+
+The adapter implements AWS Lakeformation tags management in the following way:
+- you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
+- once you enable the feature, lf-tags will be updated on every dbt run
+- first, all lf-tags for columns are removed to avoid inheritance issues
+- then all redundant lf-tags are removed from table and actual tags from config are applied
+- finally, lf-tags for columns are applied
+
+It's important to understand the following points:
+- dbt does not manage lf-tags for database
+- dbt does not manage lakeformation permissions
+
+That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.  
+You may find the following links useful to manage that:
+- [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
+- [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
+
 ### Working example
 
 seed file - employent_indicators_november_2022_csv_tables.csv
 ```
 Series_reference,Period,Data_value,Suppressed
 MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803,
```

#### html2text {}

```diff
@@ -1,13 +1,24 @@
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.5.1 Summary: The
+athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
+dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
- code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
-                                    month]
+       code%20style-black-000000.svg] [https://www.mypy-lang.org/static/
+     mypy_badge.svg] [https://pepy.tech/badge/dbt-athena-community/month]
 ## Features * Supports dbt version `1.5.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
 [table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
 * Hive tables are supported by both Athena engines. * Supports [incremental
 models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
 only with the `merge` strategy * Supports the `append` strategy * On Hive
@@ -53,45 +64,72 @@
 results in Athena | Optional | `5` | | aws_access_key_id | Access key ID of the
 user performing requests. | Optional | `AKIAIOSFODNN7EXAMPLE` | |
 aws_secret_access_key | Secret access key of the user performing requests |
 Optional | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` | | aws_profile_name |
 Profile to use from your AWS shared credentials file. | Optional | `my-profile`
 | | work_group | Identifier of Athena workgroup | Optional | `my-custom-
 workgroup` | | num_retries | Number of times to retry a failing query |
-Optional | `3` | | lf_tags | Default lf tags to apply to any database created
-by dbt | Optional | `{"origin": "dbt", "team": "analytics"}` | **Example
-profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
-s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
-your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
-dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
-workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
-`threads` is supported * `database` and `catalog` can be used interchangeably
-## Models ### Table Configuration * `external_location` (`default=none`) * If
-set, the full S3 path in which the table will be saved. * Does not work with
-Iceberg table or Hive table with `ha` set to true. * `partitioned_by`
-(`default=none`) * An array list of columns by which the table will be
-partitioned * Limited to creation of 100 partitions (_currently_) *
-`bucketed_by` (`default=none`) * An array list of columns to bucket data,
-ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
-buckets for bucketing your data, ignored if using Iceberg * `table_type`
-(`default='hive'`) * The type of table * Supports `hive` or `iceberg` * `ha`
-(`default=false`) * If the table should be built using the high-availability
-method. This option is only available for Hive tables since it is by default
-for Iceberg tables (see the section [below](#highly-available-table)) *
-`format` (`default='parquet'`) * The data format for the table * Supports
-`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
-(`default=none`) * The compression type to use for any storage format that
-allows compression to be specified. To see which options are available, check
-out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
-Custom field delimiter, for when format is set to `TEXTFILE` *
-`table_properties`: table properties to add to the table, valid for Iceberg
-only * `lf_tags` (`default=none`) * lf tags to associate with the table *
-format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
-(`default=none`) * lf tags to associate with the table columns * format: `
-{"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
+Optional | `3` | **Example profiles.yml entry:** ```yaml athena: target: dev
+outputs: dev: type: athena s3_staging_dir: s3://athena-query-results/dbt/
+s3_data_dir: s3://your_s3_bucket/dbt/ s3_data_naming: schema_table region_name:
+eu-west-1 schema: dbt database: awsdatacatalog aws_profile_name: my-profile
+work_group: my-workgroup ``` _Additional information_ * `threads` is supported
+* `database` and `catalog` can be used interchangeably ## Models ### Table
+Configuration * `external_location` (`default=none`) * If set, the full S3 path
+in which the table will be saved. * Does not work with Iceberg table or Hive
+table with `ha` set to true. * `partitioned_by` (`default=none`) * An array
+list of columns by which the table will be partitioned * Limited to creation of
+100 partitions (_currently_) * `bucketed_by` (`default=none`) * An array list
+of columns to bucket data, ignored if using Iceberg * `bucket_count`
+(`default=none`) * The number of buckets for bucketing your data, ignored if
+using Iceberg * `table_type` (`default='hive'`) * The type of table * Supports
+`hive` or `iceberg` * `ha` (`default=false`) * If the table should be built
+using the high-availability method. This option is only available for Hive
+tables since it is by default for Iceberg tables (see the section [below]
+(#highly-available-table)) * `format` (`default='parquet'`) * The data format
+for the table * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` *
+`write_compression` (`default=none`) * The compression type to use for any
+storage format that allows compression to be specified. To see which options
+are available, check out [CREATE TABLE AS][create-table-as] * `field_delimiter`
+(`default=none`) * Custom field delimiter, for when format is set to `TEXTFILE`
+* `table_properties`: table properties to add to the table, valid for Iceberg
+only + `native_drop`: Relation drop operations will be performed with SQL, not
+direct Glue API calls. No S3 calls will be made to manage data in S3. Data in
+S3 will only be cleared up for Iceberg tables [see AWS docs](https://
+docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html).
+Note that Iceberg DROP TABLE operations may timeout if they take longer than 60
+seconds. + `seed_by_insert` (`default=false`) + default behaviour uploads seed
+data to S3. This flag will create seeds using an SQL insert statement + large
+seed files cannot use `seed_by_insert`, as the SQL insert statement would
+exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/
+latest/ug/service-limits.html) * `lf_tags_config` (`default=none`) * [AWS
+lakeformation](#aws-lakeformation-integration) tags to associate with the table
+and columns * format for model config: ```sql {{ config
+( materialized='incremental', incremental_strategy='append',
+on_schema_change='append_new_columns', table_type='iceberg',
+schema='test_schema', lf_tags_config={ 'enabled': true, 'tags': { 'tag1':
+'value1', 'tag2': 'value2' }, 'tags_columns': { 'tag1': { 'value1': ['column1',
+'column2'], 'value2': ['column3', 'column4'] } } } ) }} ``` * format for
+`dbt_project.yml`: ```yaml +lf_tags_config: enabled: true tags: tag1: value1
+tag2: value2 tags_columns: tag1: value1: [ column1, column2 ] ``` * `lf_grants`
+(`default=none`) * lakeformation grants config for data_cell filters * format:
+```python lf_grants={ 'data_cell_filters': { 'enabled': True | False,
+'filters': { 'filter_name': { 'row_filter': '', 'principals':
+['principal_arn1', 'principal_arn2'] } } } } ``` > Notes: > - `lf_tags` and
+`lf_tags_columns` configs support only attaching lf tags to corresponding
+resources. > We recommend managing LF Tags permissions somewhere outside dbt.
+For example, you may use > [terraform](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) or > [aws cdk]
+(https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for
+such purpose. > - `data_cell_filters` management can't be automated outside dbt
+because the filter can't be attached to the table > which doesn't exist. Once
+you `enable` this config, dbt will set all filters and their permissions during
+every > dbt run. Such approach keeps the actual state of row level security
+configuration actual after every dbt run and > apply changes if they occur:
+drop, create, update filters and their permissions. [create-table-as]: https://
 docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 ### Table location The location in which a table is saved is determined by: 1.
 If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
 defined, the path is determined by that and `s3_data_naming` 3. If
 `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
 ` Here all the options available for `s3_data_naming`: * `unique`: `
 {s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
@@ -122,37 +160,43 @@
 table_type='iceberg', format='parquet', partitioned_by=['bucket(user_id, 5)'],
 table_properties={ 'optimize_rewrite_delete_file_threshold': '2' } ) }} select
 'A' as user_id, 'pi' as name, 'active' as status, 17.89 as cost, 1 as quantity,
 100000000 as quantity_big, current_date as my_date ``` Iceberg supports
 bucketing as hidden partitions, therefore use the `partitioned_by` config to
 add specific bucketing conditions. Iceberg supports several table formats for
 data : `PARQUET`, `AVRO` and `ORC`. It is possible to use Iceberg in an
-incremental fashion, specifically two strategies are supported: * `append`: new
-records are appended to the table, this can lead to duplicates * `merge`: must
-be used in combination with `unique_key` and it's only available with Engine
-version 3. It performs an upsert, new record are added, and record already
-existing are updated. If `delete_condition` is provided in the model config, it
-can also delete records based on the provided condition (SQL condition). You
-can use any column of the incremental table (`src`) or the final table
-(`target`). You must prefix the column by the name of the table to prevent
-`Column is ambiguous` error. ```sql {{ config( materialized='incremental',
-table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
+incremental fashion, specifically two strategies are supported: * `append`: New
+records are appended to the table, this can lead to duplicates. * `merge`:
+Performs an upsert (and optional delete), where new records are added and
+existing records are updated. Only available with Athena engine version 3. -
+`unique_key` **(required)**: columns that define a unique record in the source
+and target tables. - `incremental_predicates` (optional): SQL conditions that
+enable custom join clauses in the merge statement. This can be useful for
+improving performance via predicate pushdown on the target table. -
+`delete_condition` (optional): SQL condition used to identify records that
+should be deleted. - `delete_condition` and `incremental_predicates` can
+include any column of the incremental table (`src`) or the final table
+(`target`). Column names must be prefixed by either `src` or `target` to
+prevent a `Column is ambiguous` error. ```sql {{ config
+( materialized='incremental', table_type='iceberg',
+incremental_strategy='merge', unique_key='user_id', incremental_predicates=
+["src.quantity > 1", "target.my_date >= now() - interval '4' year"],
 delete_condition="src.status != 'active' and target.my_date < now() - interval
 '2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
 as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
 current_date as my_date ``` ### Highly available table The current
 implementation of the table materialization can lead to downtime, as target
 table is dropped and re-created. To have the less destructive behavior it's
 possible to use the `ha` config on your `table` materialized models. It
 leverages the table versions feature of glue catalog, creating a tmp table and
 swapping the target table to the location of the tmp table. This
 materialization is only available for `table_type=hive` and requires using
 unique locations. For iceberg, high availability is by default. ```sql {
 { config( materialized='table', ha=true, format='parquet', table_type='hive',
-partition_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
+partitioned_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
 user_id, 'pi' as user_name, 'active' as status union all select 'b' as user_id,
 'sh' as user_name, 'disabled' as status ``` By default, the materialization
 keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions * By default, Glue "duplicates" the versions internally,
@@ -165,16 +209,30 @@
 snapshot create a snapshot file in the snapshots directory. If the directory
 does not exist create one. ### Timestamp strategy To use the timestamp strategy
 refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
 strategy-recommended) ### Check strategy To use the check strategy refer to the
 [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
 Hard-deletes The materialization also supports invalidating hard deletes. Check
 the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
-understand usage. ### Working example seed file -
-employent_indicators_november_2022_csv_tables.csv ```
+understand usage. ### AWS Lakeformation integration The adapter implements AWS
+Lakeformation tags management in the following way: - you can enable or disable
+lf-tags management via [config](#table-configuration) (disabled by default) -
+once you enable the feature, lf-tags will be updated on every dbt run - first,
+all lf-tags for columns are removed to avoid inheritance issues - then all
+redundant lf-tags are removed from table and actual tags from config are
+applied - finally, lf-tags for columns are applied It's important to understand
+the following points: - dbt does not manage lf-tags for database - dbt does not
+manage lakeformation permissions That's why you should handle this by yourself
+manually or using some automation tools like terraform, AWS CDK etc. You may
+find the following links useful to manage that: - [terraform
+aws_lakeformation_permissions](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) - [terraform
+aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ### Working
+example seed file - employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
```

### Comparing `dbt-athena-community-1.5.0/dbt/adapters/athena/__init__.py` & `dbt-athena-community-1.5.1/dbt/adapters/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/adapters/athena/column.py` & `dbt-athena-community-1.5.1/dbt/adapters/athena/column.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,23 +33,21 @@
         if self.is_iceberg():
             return "timestamp(6)"
         return "timestamp"
 
     def string_size(self) -> int:
         if not self.is_string():
             raise DbtRuntimeError("Called string_size() on non-string field!")
-        if not self.char_size:
-            # Handle error: '>' not supported between instances of 'NoneType' and 'NoneType' for union relations macro
-            return 0
-        return self.char_size
+        # Handle error: '>' not supported between instances of 'NoneType' and 'NoneType' for union relations macro
+        return self.char_size or 0
 
     @property
     def data_type(self) -> str:
         if self.is_string():
             return self.string_type(self.string_size())
         elif self.is_numeric():
-            return self.numeric_type(self.dtype, self.numeric_precision, self.numeric_scale)
+            return self.numeric_type(self.dtype, self.numeric_precision, self.numeric_scale)  # type: ignore
         elif self.is_binary():
             return self.binary_type()
         elif self.is_timestamp():
             return self.timestamp_type()
-        return self.dtype
+        return self.dtype  # type: ignore
```

### Comparing `dbt-athena-community-1.5.0/dbt/adapters/athena/connections.py` & `dbt-athena-community-1.5.1/dbt/adapters/athena/connections.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
+import time
 from concurrent.futures.thread import ThreadPoolExecutor
 from contextlib import contextmanager
 from copy import deepcopy
 from dataclasses import dataclass
 from decimal import Decimal
-from typing import Any, ContextManager, Dict, List, Optional, Tuple, Union
+from typing import Any, ContextManager, Dict, List, Optional, Tuple
 
 import tenacity
 from pyathena.connection import Connection as AthenaConnection
 from pyathena.cursor import Cursor
 from pyathena.error import OperationalError, ProgrammingError
 
 # noinspection PyProtectedMember
@@ -46,22 +47,21 @@
     aws_access_key_id: Optional[str] = None
     aws_secret_access_key: Optional[str] = None
     poll_interval: float = 1.0
     _ALIASES = {"catalog": "database"}
     num_retries: Optional[int] = 5
     s3_data_dir: Optional[str] = None
     s3_data_naming: Optional[str] = "schema_table_unique"
-    lf_tags: Optional[Dict[str, str]] = None
 
     @property
     def type(self) -> str:
         return "athena"
 
     @property
-    def unique_field(self):
+    def unique_field(self) -> str:
         return f"athena-{hashlib.md5(self.s3_staging_dir.encode()).hexdigest()}"
 
     def _connection_keys(self) -> Tuple[str, ...]:
         return (
             "s3_staging_dir",
             "work_group",
             "region_name",
@@ -75,40 +75,65 @@
             "s3_data_dir",
             "s3_data_naming",
             "lf_tags",
         )
 
 
 class AthenaCursor(Cursor):
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:  # type: ignore
         super().__init__(**kwargs)
         self._executor = ThreadPoolExecutor()
 
     def _collect_result_set(self, query_id: str) -> AthenaResultSet:
         query_execution = self._poll(query_id)
         return self._result_set_class(
             connection=self._connection,
             converter=self._converter,
             query_execution=query_execution,
             arraysize=self._arraysize,
             retry_config=self._retry_config,
         )
 
-    def execute(
+    def _poll(self, query_id: str) -> AthenaQueryExecution:
+        try:
+            query_execution = self.__poll(query_id)
+        except KeyboardInterrupt as e:
+            if self._kill_on_interrupt:
+                logger.warning("Query canceled by user.")
+                self._cancel(query_id)
+                query_execution = self.__poll(query_id)
+            else:
+                raise e
+        return query_execution
+
+    def __poll(self, query_id: str) -> AthenaQueryExecution:
+        while True:
+            query_execution = self._get_query_execution(query_id)
+            if query_execution.state in [
+                AthenaQueryExecution.STATE_SUCCEEDED,
+                AthenaQueryExecution.STATE_FAILED,
+                AthenaQueryExecution.STATE_CANCELLED,
+            ]:
+                return query_execution
+            else:
+                logger.debug(f"Query state is: {query_execution.state}. Sleeping for {self._poll_interval}...")
+                time.sleep(self._poll_interval)
+
+    def execute(  # type: ignore
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         endpoint_url: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
         **kwargs,
     ):
-        def inner():
+        def inner() -> AthenaCursor:
             query_id = self._execute(
                 operation,
                 parameters=parameters,
                 work_group=work_group,
                 s3_staging_dir=s3_staging_dir,
                 cache_size=cache_size,
                 cache_expiration_time=cache_expiration_time,
@@ -140,25 +165,25 @@
         return retry(inner)
 
 
 class AthenaConnectionManager(SQLConnectionManager):
     TYPE = "athena"
 
     @classmethod
-    def data_type_code_to_name(cls, type_code: Union[int, str]) -> str:
+    def data_type_code_to_name(cls, type_code: str) -> str:
         """
         Get the string representation of the data type from the Athena metadata. Dbt performs a
         query to retrieve the types of the columns in the SQL query. Then these types are compared
         to the types in the contract config, simplified because they need to match what is returned
         by Athena metadata (we are only interested in the broader type, without subtypes nor granularity).
         """
         return type_code.split("(")[0].split("<")[0].upper()
 
-    @contextmanager
-    def exception_handler(self, sql: str) -> ContextManager:
+    @contextmanager  # type: ignore
+    def exception_handler(self, sql: str) -> ContextManager:  # type: ignore
         try:
             yield
         except Exception as e:
             logger.debug(f"Error running SQL: {sql}")
             raise DbtRuntimeError(str(e)) from e
 
     @classmethod
@@ -177,19 +202,15 @@
                 work_group=creds.work_group,
                 cursor_class=AthenaCursor,
                 formatter=AthenaParameterFormatter(),
                 poll_interval=creds.poll_interval,
                 session=get_boto3_session(connection),
                 retry_config=RetryConfig(
                     attempt=creds.num_retries,
-                    exceptions=(
-                        "ThrottlingException",
-                        "TooManyRequestsException",
-                        "InternalServerException",
-                    ),
+                    exceptions=("ThrottlingException", "TooManyRequestsException", "InternalServerException"),
                 ),
                 config=get_boto3_config(),
             )
 
             connection.state = ConnectionState.OPEN
             connection.handle = handle
 
@@ -198,31 +219,31 @@
             connection.handle = None
             connection.state = ConnectionState.FAIL
             raise ConnectionError(str(exc))
 
         return connection
 
     @classmethod
-    def get_response(cls, cursor) -> AdapterResponse:
+    def get_response(cls, cursor: AthenaCursor) -> AdapterResponse:
         code = "OK" if cursor.state == AthenaQueryExecution.STATE_SUCCEEDED else "ERROR"
         return AdapterResponse(_message=f"{code} {cursor.rowcount}", rows_affected=cursor.rowcount, code=code)
 
-    def cancel(self, connection: Connection):
+    def cancel(self, connection: Connection) -> None:
         connection.handle.cancel()
 
-    def add_begin_query(self):
+    def add_begin_query(self) -> None:
         pass
 
-    def add_commit_query(self):
+    def add_commit_query(self) -> None:
         pass
 
-    def begin(self):
+    def begin(self) -> None:
         pass
 
-    def commit(self):
+    def commit(self) -> None:
         pass
 
 
 class AthenaParameterFormatter(Formatter):
     def __init__(self) -> None:
         super().__init__(mappings=deepcopy(_DEFAULT_FORMATTERS), default=None)
```

### Comparing `dbt-athena-community-1.5.0/dbt/adapters/athena/impl.py` & `dbt-athena-community-1.5.1/dbt/adapters/athena/impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,42 +8,58 @@
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
 from urllib.parse import urlparse
 from uuid import uuid4
 
 import agate
 from botocore.exceptions import ClientError
 from mypy_boto3_athena.type_defs import DataCatalogTypeDef
+from mypy_boto3_glue.type_defs import (
+    ColumnTypeDef,
+    GetTableResponseTypeDef,
+    TableTypeDef,
+    TableVersionTypeDef,
+)
 
 from dbt.adapters.athena import AthenaConnectionManager
 from dbt.adapters.athena.column import AthenaColumn
 from dbt.adapters.athena.config import get_boto3_config
 from dbt.adapters.athena.constants import LOGGER
 from dbt.adapters.athena.exceptions import (
     S3LocationException,
     SnapshotMigrationRequired,
 )
+from dbt.adapters.athena.lakeformation import (
+    LfGrantsConfig,
+    LfPermissions,
+    LfTagsConfig,
+    LfTagsManager,
+)
 from dbt.adapters.athena.relation import (
     RELATION_TYPE_MAP,
     AthenaRelation,
     AthenaSchemaSearchMap,
+    TableType,
     get_table_type,
 )
 from dbt.adapters.athena.s3 import S3DataNaming
-from dbt.adapters.athena.utils import clean_sql_comment, get_catalog_id
+from dbt.adapters.athena.utils import clean_sql_comment, get_catalog_id, get_chunks
 from dbt.adapters.base import ConstraintSupport, available
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
 from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import CompiledNode, ConstraintType
 from dbt.exceptions import DbtRuntimeError
 
 boto3_client_lock = Lock()
 
 
 class AthenaAdapter(SQLAdapter):
+    BATCH_CREATE_PARTITION_API_LIMIT = 100
+    BATCH_DELETE_PARTITION_API_LIMIT = 25
+
     ConnectionManager = AthenaConnectionManager
     Relation = AthenaRelation
 
     # There is no such concept as constraints in Athena
     CONSTRAINT_SUPPORT = {
         ConstraintType.check: ConstraintSupport.NOT_SUPPORTED,
         ConstraintType.not_null: ConstraintSupport.NOT_SUPPORTED,
@@ -65,92 +81,40 @@
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
         return "double" if decimals else "integer"
 
     @classmethod
     def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "timestamp"
 
-    @classmethod
-    def parse_lf_response(
-        cls,
-        response: Dict[str, Any],
-        database: str,
-        table: Optional[str],
-        columns: Optional[List[str]],
-        lf_tags: Dict[str, str],
-    ) -> str:
-        failures = response.get("Failures", [])
-        tbl_appendix = f".{table}" if table else ""
-        columns_appendix = f" for columns {columns}" if columns else ""
-        msg_appendix = tbl_appendix + columns_appendix
-        if failures:
-            base_msg = f"Failed to add LF tags: {lf_tags} to {database}" + msg_appendix
-            for failure in failures:
-                tag = failure.get("LFTag", {}).get("TagKey")
-                error = failure.get("Error", {}).get("ErrorMessage")
-                LOGGER.error(f"Failed to set {tag} for {database}" + msg_appendix + f" - {error}")
-            raise DbtRuntimeError(base_msg)
-        return f"Added LF tags: {lf_tags} to {database}" + msg_appendix
-
-    @classmethod
-    def lf_tags_columns_is_valid(cls, lf_tags_columns: Dict[str, Dict[str, List[str]]]) -> Optional[bool]:
-        if not lf_tags_columns:
-            return False
-        for tag_key, tag_config in lf_tags_columns.items():
-            if isinstance(tag_config, Dict):
-                for tag_value, columns in tag_config.items():
-                    if not isinstance(columns, List):
-                        raise DbtRuntimeError(f"Not a list: {columns}. " + "Expected format: ['c1', 'c2']")
-            else:
-                raise DbtRuntimeError(f"Not a dict: {tag_config}. " + "Expected format: {'tag_value': ['c1', 'c2']}")
-        return True
-
-    # TODO: Add more lf-tag unit tests when moto supports lakeformation
-    # moto issue: https://github.com/getmoto/moto/issues/5964
     @available
-    def add_lf_tags(
-        self,
-        database: str,
-        table: str = None,
-        lf_tags: Optional[Dict[str, str]] = None,
-        lf_tags_columns: Optional[Dict[str, Dict[str, List[str]]]] = None,
-    ):
-        conn = self.connections.get_thread_connection()
-        client = conn.handle
-
-        lf_tags = lf_tags or conn.credentials.lf_tags
-
-        if not lf_tags and not lf_tags_columns:
-            LOGGER.debug("No LF tags configured")
-        else:
+    def add_lf_tags(self, relation: AthenaRelation, lf_tags_config: Dict[str, Any]) -> None:
+        config = LfTagsConfig(**lf_tags_config)
+        if config.enabled:
+            conn = self.connections.get_thread_connection()
+            client = conn.handle
             with boto3_client_lock:
-                lf_client = client.session.client(
-                    "lakeformation", region_name=client.region_name, config=get_boto3_config()
-                )
-
-            if lf_tags:
-                resource = {"Database": {"Name": database}}
-                if table:
-                    resource = {"Table": {"DatabaseName": database, "Name": table}}
+                lf_client = client.session.client("lakeformation", client.region_name, config=get_boto3_config())
+            manager = LfTagsManager(lf_client, relation, config)
+            manager.process_lf_tags()
+            return
+        LOGGER.debug(f"Lakeformation is disabled for {relation}")
 
-                response = lf_client.add_lf_tags_to_resource(
-                    Resource=resource, LFTags=[{"TagKey": key, "TagValues": [value]} for key, value in lf_tags.items()]
-                )
-                LOGGER.debug(self.parse_lf_response(response, database, table, None, lf_tags))
-
-            if self.lf_tags_columns_is_valid(lf_tags_columns):
-                for tag_key, tag_config in lf_tags_columns.items():
-                    for tag_value, columns in tag_config.items():
-                        response = lf_client.add_lf_tags_to_resource(
-                            Resource={
-                                "TableWithColumns": {"DatabaseName": database, "Name": table, "ColumnNames": columns}
-                            },
-                            LFTags=[{"TagKey": tag_key, "TagValues": [tag_value]}],
-                        )
-                        LOGGER.debug(self.parse_lf_response(response, database, table, columns, {tag_key: tag_value}))
+    @available
+    def apply_lf_grants(self, relation: AthenaRelation, lf_grants_config: Dict[str, Any]) -> None:
+        lf_config = LfGrantsConfig(**lf_grants_config)
+        if lf_config.data_cell_filters.enabled:
+            conn = self.connections.get_thread_connection()
+            client = conn.handle
+            with boto3_client_lock:
+                lf = client.session.client("lakeformation", region_name=client.region_name, config=get_boto3_config())
+            catalog = self._get_data_catalog(relation.database)
+            catalog_id = get_catalog_id(catalog)
+            lf_permissions = LfPermissions(catalog_id, relation, lf)  # type: ignore
+            lf_permissions.process_filters(lf_config)
+            lf_permissions.process_permissions(lf_config)
 
     @available
     def is_work_group_output_location_enforced(self) -> bool:
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         client = conn.handle
 
@@ -185,15 +149,15 @@
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         if s3_data_dir is not None:
             return s3_data_dir
 
         return path.join(creds.s3_staging_dir, "tables")
 
-    def _s3_data_naming(self, s3_data_naming: Optional[str]) -> Optional[S3DataNaming]:
+    def _s3_data_naming(self, s3_data_naming: Optional[str]) -> S3DataNaming:
         """
         Returns the s3 data naming strategy if provided, otherwise the value from the connection.
         """
         conn = self.connections.get_thread_connection()
         creds = conn.credentials
         if s3_data_naming is not None:
             return S3DataNaming(s3_data_naming)
@@ -214,61 +178,82 @@
         depending on the value of s3_table
         """
         if external_location and not is_temporary_table:
             return external_location.rstrip("/")
 
         s3_path_table_part = relation.s3_path_table_part or relation.identifier
         schema_name = relation.schema
-        s3_data_naming = self._s3_data_naming(s3_data_naming)
         table_prefix = self._s3_table_prefix(s3_data_dir)
 
         mapping = {
             S3DataNaming.UNIQUE: path.join(table_prefix, str(uuid4())),
             S3DataNaming.TABLE: path.join(table_prefix, s3_path_table_part),
             S3DataNaming.TABLE_UNIQUE: path.join(table_prefix, s3_path_table_part, str(uuid4())),
             S3DataNaming.SCHEMA_TABLE: path.join(table_prefix, schema_name, s3_path_table_part),
             S3DataNaming.SCHEMA_TABLE_UNIQUE: path.join(table_prefix, schema_name, s3_path_table_part, str(uuid4())),
         }
 
-        return mapping[s3_data_naming]
+        return mapping[self._s3_data_naming(s3_data_naming)]
 
     @available
-    def get_glue_table_location(self, relation: AthenaRelation) -> Optional[str]:
+    def get_glue_table(self, relation: AthenaRelation) -> Optional[GetTableResponseTypeDef]:
         """
-        Helper function to get location of a relation in S3.
-        Will return None if the table does not exist or does not have a location (views)
+        Helper function to get a relation via Glue
         """
         conn = self.connections.get_thread_connection()
         client = conn.handle
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         try:
             table = glue_client.get_table(DatabaseName=relation.schema, Name=relation.identifier)
         except ClientError as e:
             if e.response["Error"]["Code"] == "EntityNotFoundException":
                 LOGGER.debug(f"Table {relation.render()} does not exists - Ignoring")
                 return None
             raise e
+        return table
+
+    @available
+    def get_glue_table_type(self, relation: AthenaRelation) -> Optional[TableType]:
+        """
+        Get the table type of the relation from Glue
+        """
+        table = self.get_glue_table(relation)
+        if not table:
+            LOGGER.debug(f"Table {relation.render()} does not exist - Ignoring")
+            return None
+
+        return get_table_type(table["Table"])
+
+    @available
+    def get_glue_table_location(self, relation: AthenaRelation) -> Optional[str]:
+        """
+        Helper function to get location of a relation in S3.
+        Will return None if the table does not exist or does not have a location (views)
+        """
+        table = self.get_glue_table(relation)
+        if not table:
+            LOGGER.debug(f"Table {relation.render()} does not exist - Ignoring")
+            return None
 
         table_type = get_table_type(table["Table"])
         table_location = table["Table"].get("StorageDescriptor", {}).get("Location")
         if table_type.is_physical():
             if not table_location:
                 raise S3LocationException(
                     f"Relation {relation.render()} is of type '{table_type.value}' which requires a location, "
                     f"but no location returned by Glue."
                 )
             LOGGER.debug(f"{relation.render()} is stored in {table_location}")
-            return table_location
-
+            return str(table_location)
         return None
 
     @available
-    def clean_up_partitions(self, relation: AthenaRelation, where_condition: str):
+    def clean_up_partitions(self, relation: AthenaRelation, where_condition: str) -> None:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
         paginator = glue_client.get_paginator("get_partitions")
         partition_params = {
@@ -279,25 +264,25 @@
         }
         partition_pg = paginator.paginate(**partition_params)
         partitions = partition_pg.build_full_result().get("Partitions")
         for partition in partitions:
             self.delete_from_s3(partition["StorageDescriptor"]["Location"])
 
     @available
-    def clean_up_table(self, relation: AthenaRelation):
+    def clean_up_table(self, relation: AthenaRelation) -> None:
         table_location = self.get_glue_table_location(relation)
 
-        # this check avoid issues for when the table location is an empty string
-        # or when the table do not exist and table location is None
+        # this check avoids issues for when the table location is an empty string
+        # or when the table does not exist and table location is None
         if table_location:
             self.delete_from_s3(table_location)
 
     @available
     def quote_seed_column(self, column: str, quote_config: Optional[bool]) -> str:
-        return super().quote_seed_column(column, False)
+        return str(super().quote_seed_column(column, False))
 
     @available
     def upload_seed_to_s3(
         self,
         relation: AthenaRelation,
         table: agate.Table,
         s3_data_dir: Optional[str] = None,
@@ -320,18 +305,18 @@
             s3_client = client.session.client("s3", region_name=client.region_name, config=get_boto3_config())
             # This ensures cross-platform support, tempfile.NamedTemporaryFile does not
             tmpfile = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
             table.to_csv(tmpfile, quoting=csv.QUOTE_NONNUMERIC)
             s3_client.upload_file(tmpfile, bucket, object_name)
             os.remove(tmpfile)
 
-        return s3_location
+        return str(s3_location)
 
     @available
-    def delete_from_s3(self, s3_path: str):
+    def delete_from_s3(self, s3_path: str) -> None:
         """
         Deletes files from s3 given a s3 path in the format: s3://my_bucket/prefix
         Additionally, parses the response from the s3 delete request and raises
         a DbtRuntimeError in case it included errors.
         """
         conn = self.connections.get_thread_connection()
         client = conn.handle
@@ -398,15 +383,15 @@
         join_keys = ["table_database", "table_schema", "table_name"]
         return table.join(
             right_table=owners_table,
             left_key=join_keys,
             right_key=join_keys,
         )
 
-    def _get_one_table_for_catalog(self, table: dict, database: str) -> list:
+    def _get_one_table_for_catalog(self, table: TableTypeDef, database: str) -> List[Dict[str, Any]]:
         table_catalog = {
             "table_database": database,
             "table_schema": table["DatabaseName"],
             "table_name": table["Name"],
             "table_type": RELATION_TYPE_MAP[table.get("TableType", "EXTERNAL_TABLE")].value,
             "table_comment": table.get("Parameters", {}).get("comment", table.get("Description", "")),
         }
@@ -445,15 +430,15 @@
             }
             # If the catalog is `awsdatacatalog` we don't need to pass CatalogId as boto3 infers it from the account Id.
             if catalog_id:
                 kwargs["CatalogId"] = catalog_id
 
             for page in paginator.paginate(**kwargs):
                 for table in page["TableList"]:
-                    if table["Name"] in relations:
+                    if relations and table["Name"] in relations:
                         catalog.extend(self._get_one_table_for_catalog(table, information_schema.path.database))
 
         table = agate.Table.from_object(catalog)
         filtered_table = self._catalog_filter_table(table, manifest)
         return self._join_catalog_table_owners(filtered_table, manifest)
 
     def _get_catalog_schemas(self, manifest: Manifest) -> AthenaSchemaSearchMap:
@@ -472,25 +457,25 @@
             conn = self.connections.get_thread_connection()
             client = conn.handle
             if database.lower() == "awsdatacatalog":
                 with boto3_client_lock:
                     sts = client.session.client("sts", region_name=client.region_name, config=get_boto3_config())
                 catalog_id = sts.get_caller_identity()["Account"]
                 return {"Name": database, "Type": "GLUE", "Parameters": {"catalog-id": catalog_id}}
-            else:
-                with boto3_client_lock:
-                    athena = client.session.client("athena", region_name=client.region_name, config=get_boto3_config())
-                return athena.get_data_catalog(Name=database)["DataCatalog"]
+            with boto3_client_lock:
+                athena = client.session.client("athena", region_name=client.region_name, config=get_boto3_config())
+            return athena.get_data_catalog(Name=database)["DataCatalog"]
+        return None
 
     def list_relations_without_caching(self, schema_relation: AthenaRelation) -> List[BaseRelation]:
         data_catalog = self._get_data_catalog(schema_relation.database)
         catalog_id = get_catalog_id(data_catalog)
         if data_catalog and data_catalog["Type"] != "GLUE":
             # For non-Glue Data Catalogs, use the original Athena query against INFORMATION_SCHEMA approach
-            return super().list_relations_without_caching(schema_relation)
+            return super().list_relations_without_caching(schema_relation)  # type: ignore
 
         conn = self.connections.get_thread_connection()
         client = conn.handle
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
         paginator = glue_client.get_paginator("get_tables")
 
@@ -531,15 +516,15 @@
             # don't error out when schema doesn't exist
             # this allows dbt to create and manage schemas/databases
             LOGGER.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
 
         return relations
 
     @available
-    def swap_table(self, src_relation: AthenaRelation, target_relation: AthenaRelation):
+    def swap_table(self, src_relation: AthenaRelation, target_relation: AthenaRelation) -> None:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         src_table = glue_client.get_table(DatabaseName=src_relation.schema, Name=src_relation.identifier).get("Table")
@@ -564,31 +549,37 @@
         glue_client.update_table(DatabaseName=target_relation.schema, TableInput=target_table_version)
         LOGGER.debug(f"Table {target_relation.render()} swapped with the content of {src_relation.render()}")
 
         # we delete the target table partitions in any case
         # if source table has partitions we need to delete and add partitions
         # it source table hasn't any partitions we need to delete target table partitions
         if target_table_partitions:
-            glue_client.batch_delete_partition(
-                DatabaseName=target_relation.schema,
-                TableName=target_relation.identifier,
-                PartitionsToDelete=[{"Values": i["Values"]} for i in target_table_partitions],
-            )
+            for partition_batch in get_chunks(target_table_partitions, AthenaAdapter.BATCH_DELETE_PARTITION_API_LIMIT):
+                glue_client.batch_delete_partition(
+                    DatabaseName=target_relation.schema,
+                    TableName=target_relation.identifier,
+                    PartitionsToDelete=[{"Values": partition["Values"]} for partition in partition_batch],
+                )
 
         if src_table_partitions:
-            glue_client.batch_create_partition(
-                DatabaseName=target_relation.schema,
-                TableName=target_relation.identifier,
-                PartitionInputList=[
-                    {"Values": p["Values"], "StorageDescriptor": p["StorageDescriptor"], "Parameters": p["Parameters"]}
-                    for p in src_table_partitions
-                ],
-            )
+            for partition_batch in get_chunks(src_table_partitions, AthenaAdapter.BATCH_CREATE_PARTITION_API_LIMIT):
+                glue_client.batch_create_partition(
+                    DatabaseName=target_relation.schema,
+                    TableName=target_relation.identifier,
+                    PartitionInputList=[
+                        {
+                            "Values": partition["Values"],
+                            "StorageDescriptor": partition["StorageDescriptor"],
+                            "Parameters": partition["Parameters"],
+                        }
+                        for partition in partition_batch
+                    ],
+                )
 
-    def _get_glue_table_versions_to_expire(self, relation: AthenaRelation, to_keep: int):
+    def _get_glue_table_versions_to_expire(self, relation: AthenaRelation, to_keep: int) -> List[TableVersionTypeDef]:
         """
         Given a table and the amount of its version to keep, it returns the versions to delete
         """
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
@@ -603,15 +594,17 @@
         )
         table_versions = response_iterator.build_full_result().get("TableVersions")
         LOGGER.debug(f"Total table versions: {[v['VersionId'] for v in table_versions]}")
         table_versions_ordered = sorted(table_versions, key=lambda i: int(i["Table"]["VersionId"]), reverse=True)
         return table_versions_ordered[int(to_keep) :]
 
     @available
-    def expire_glue_table_versions(self, relation: AthenaRelation, to_keep: int, delete_s3: bool):
+    def expire_glue_table_versions(
+        self, relation: AthenaRelation, to_keep: int, delete_s3: bool
+    ) -> List[TableVersionTypeDef]:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         versions_to_delete = self._get_glue_table_versions_to_expire(relation, to_keep)
@@ -639,15 +632,15 @@
     @available
     def persist_docs_to_glue(
         self,
         relation: AthenaRelation,
         model: Dict[str, Any],
         persist_relation_docs: bool = False,
         persist_column_docs: bool = False,
-    ):
+    ) -> None:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         table = glue_client.get_table(DatabaseName=relation.schema, Name=relation.name).get("Table")
@@ -684,17 +677,17 @@
         paginator = glue_client.get_paginator("get_databases")
         result = []
         for page in paginator.paginate():
             result.extend([schema["Name"] for schema in page["DatabaseList"]])
         return result
 
     @staticmethod
-    def _is_current_column(col: dict) -> bool:
+    def _is_current_column(col: ColumnTypeDef) -> bool:
         """
-        Check if a column is explicit set as not current. If not, it is considered as current.
+        Check if a column is explicitly set as not current. If not, it is considered as current.
         """
         if col.get("Parameters", {}).get("iceberg.field.current") == "false":
             return False
         return True
 
     @available
     def get_columns_in_relation(self, relation: AthenaRelation) -> List[AthenaColumn]:
@@ -722,15 +715,15 @@
         LOGGER.debug(f"Columns in relation {relation.identifier}: {columns + partition_keys}")
 
         return [
             AthenaColumn(column=c["Name"], dtype=c["Type"], table_type=table_type) for c in columns + partition_keys
         ]
 
     @available
-    def delete_from_glue_catalog(self, relation: AthenaRelation):
+    def delete_from_glue_catalog(self, relation: AthenaRelation) -> None:
         schema_name = relation.schema
         table_name = relation.identifier
 
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         with boto3_client_lock:
@@ -754,39 +747,39 @@
         names = {c.name.lower() for c in columns}
 
         table_columns = [col for col in names if not col.startswith("dbt_") and col != "is_current_record"]
 
         if "dbt_unique_key" in names:
             sql = self._generate_snapshot_migration_sql(relation=relation, table_columns=table_columns)
             msg = (
-                f"{'!'*90}\n"
+                f"{'!' * 90}\n"
                 "The snapshot logic of dbt-athena has changed in an incompatible way to be more consistent "
                 "with the dbt-core implementation.\nYou will need to migrate your existing snapshot tables to be "
                 "able to keep using them with the latest dbt-athena version.\nYou can find more information "
                 "in the release notes:\nhttps://github.com/dbt-athena/dbt-athena/releases\n"
-                f"{'!'*90}\n\n"
+                f"{'!' * 90}\n\n"
                 "You can use the example query below as a baseline to perform the migration:\n\n"
-                f"{'-'*90}\n"
+                f"{'-' * 90}\n"
                 f"{sql}\n"
-                f"{'-'*90}\n\n"
+                f"{'-' * 90}\n\n"
             )
             LOGGER.error(msg)
             raise SnapshotMigrationRequired("Look into 1.5 dbt-athena docs for the complete migration procedure")
 
     def _generate_snapshot_migration_sql(self, relation: AthenaRelation, table_columns: List[str]) -> str:
         """Generate a sequence of queries that can be used to migrate the existing table to the new format.
 
         The queries perform the following steps:
         - Backup the existing table
         - Make the necessary modifications and store the results in a staging table
         - Delete the target table (users might have to delete the S3 files manually)
         - Copy the content of the staging table to the final table
         - Delete the staging table
         """
-        col_csv = f",\n{' '*16}".join(table_columns)
+        col_csv = f",\n{' ' * 16}".join(table_columns)
         staging_relation = relation.incorporate(
             path={"identifier": relation.identifier + "__dbt_tmp_migration_staging"}
         )
         ctas = dedent(
             f"""\
             select
                 {col_csv},
@@ -828,7 +821,15 @@
                 drop_target_sql.strip(),
                 "\n\n-- Copy staging to target",
                 copy_to_target_sql.strip(),
                 "\n\n-- Drop staging table",
                 drop_staging_sql.strip(),
             ]
         )
+
+    @available
+    def is_list(self, value: Any) -> bool:
+        """
+        This function is intended to test whether a Jinja object is
+        a list since this is complicated with purely Jinja syntax.
+        """
+        return isinstance(value, list)
```

### Comparing `dbt-athena-community-1.5.0/dbt/adapters/athena/query_headers.py` & `dbt-athena-community-1.5.1/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/adapters/athena/relation.py` & `dbt-athena-community-1.5.1/dbt/adapters/athena/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,52 +28,51 @@
 
 @dataclass(frozen=True, eq=False, repr=False)
 class AthenaRelation(BaseRelation):
     quote_character: str = '"'  # Presto quote character
     include_policy: Policy = field(default_factory=lambda: AthenaIncludePolicy())
     s3_path_table_part: Optional[str] = None
 
-    def render_hive(self):
+    def render_hive(self) -> str:
         """
-        Render relation with Hive format. Athena uses Hive format for some DDL statements.
+        Render relation with Hive format. Athena uses a Hive format for some DDL statements.
 
         See:
         - https://aws.amazon.com/athena/faqs/ "Q: How do I create tables and schemas for my data on Amazon S3?"
         - https://cwiki.apache.org/confluence/display/Hive/LanguageManual+DDL
         """
 
         old_value = self.quote_character
         object.__setattr__(self, "quote_character", "`")  # Hive quote char
         rendered = self.render()
         object.__setattr__(self, "quote_character", old_value)
-        return rendered
+        return str(rendered)
 
-    def render_pure(self):
+    def render_pure(self) -> str:
         """
         Render relation without quotes characters.
         This is needed for not standard executions like optimize and vacuum
         """
         old_value = self.quote_character
         object.__setattr__(self, "quote_character", "")
         rendered = self.render()
         object.__setattr__(self, "quote_character", old_value)
-        return rendered
+        return str(rendered)
 
 
 class AthenaSchemaSearchMap(Dict[InformationSchema, Dict[str, Set[Optional[str]]]]):
     """A utility class to keep track of what information_schema tables to
     search for what schemas and relations. The schema and relation values are all
-    lowercased to avoid duplication.
+    lowercase to avoid duplication.
     """
 
-    def add(self, relation: AthenaRelation):
+    def add(self, relation: AthenaRelation) -> None:
         key = relation.information_schema_only()
         if key not in self:
             self[key] = {}
-        schema: Optional[str] = None
         if relation.schema is not None:
             schema = relation.schema.lower()
             relation_name = relation.name.lower()
             if schema not in self[key]:
                 self[key][schema] = set()
             self[key][schema].add(relation_name)
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/columns.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/adapters/relation.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/adapters/relation.sql`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,38 @@
 {% macro athena__drop_relation(relation) -%}
+  {%- set native_drop = config.get('native_drop', default=false) -%}
+  {%- set rel_type_object = adapter.get_glue_table_type(relation) -%}
+  {%- set rel_type = none if rel_type_object == none else rel_type_object.value -%}
+  {%- set natively_droppable = rel_type == 'iceberg_table' or relation.type == 'view' -%}
+
+  {%- if native_drop and natively_droppable -%}
+    {%- do drop_relation_sql(relation) -%}
+  {%- else -%}
+    {%- do drop_relation_glue(relation) -%}
+  {%- endif -%}
+{% endmacro %}
+
+{% macro drop_relation_glue(relation) -%}
+  {%- do log('Dropping relation via Glue and S3 APIs') -%}
   {%- do adapter.clean_up_table(relation) -%}
   {%- do adapter.delete_from_glue_catalog(relation) -%}
 {% endmacro %}
 
+{% macro drop_relation_sql(relation) -%}
+
+  {%- do log('Dropping relation via SQL only') -%}
+  {% call statement('drop_relation', auto_begin=False) -%}
+    {%- if relation.type == 'view' -%}
+      drop {{ relation.type }} if exists {{ relation.render() }}
+    {%- else -%}
+      drop {{ relation.type }} if exists {{ relation.render_hive() }}
+    {% endif %}
+  {%- endcall %}
+{% endmacro %}
+
 {% macro set_table_classification(relation) -%}
   {%- set format = config.get('format', default='parquet') -%}
   {% call statement('set_table_classification', auto_begin=False) -%}
     alter table {{ relation.render_hive() }} set tblproperties ('classification' = '{{ format }}')
   {%- endcall %}
 {%- endmacro %}
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% materialization incremental, adapter='athena' -%}
 
   {% set raw_strategy = config.get('incremental_strategy') or 'insert_overwrite' %}
   {% set table_type = config.get('table_type', default='hive') | lower %}
   {% set strategy = validate_get_incremental_strategy(raw_strategy, table_type) %}
   {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
 
-  {% set lf_tags = config.get('lf_tags', default=none) %}
-  {% set lf_tags_columns = config.get('lf_tags_columns', default=none) %}
+  {% set lf_tags_config = config.get('lf_tags_config') %}
+  {% set lf_grants = config.get('lf_grants') %}
   {% set partitioned_by = config.get('partitioned_by', default=none) %}
   {% set target_relation = this.incorporate(type='table') %}
   {% set existing_relation = load_relation(this) %}
   {% set tmp_relation = make_temp_relation(this) %}
 
   -- If no partitions are used with insert_overwrite, we fall back to append mode.
   {% if partitioned_by is none and strategy == 'insert_overwrite' %}
@@ -43,28 +43,36 @@
       {% do drop_relation(tmp_relation) %}
     {% endif %}
     {% do run_query(create_table_as(True, tmp_relation, sql)) %}
     {% set build_sql = incremental_insert(on_schema_change, tmp_relation, target_relation, existing_relation) %}
     {% do to_drop.append(tmp_relation) %}
   {% elif strategy == 'merge' and table_type == 'iceberg' %}
     {% set unique_key = config.get('unique_key') %}
+    {% set incremental_predicates = config.get('incremental_predicates') %}
     {% set delete_condition = config.get('delete_condition') %}
     {% set empty_unique_key -%}
       Merge strategy must implement unique_key as a single column or a list of columns.
     {%- endset %}
     {% if unique_key is none %}
       {% do exceptions.raise_compiler_error(empty_unique_key) %}
     {% endif %}
-
+    {% if incremental_predicates is not none %}
+      {% set inc_predicates_not_list -%}
+        Merge strategy must implement incremental_predicates as a list of predicates.
+      {%- endset %}
+      {% if not adapter.is_list(incremental_predicates) %}
+        {% do exceptions.raise_compiler_error(inc_predicates_not_list) %}
+      {% endif %}
+    {% endif %}
     {% set tmp_relation = make_temp_relation(target_relation) %}
     {% if tmp_relation is not none %}
       {% do drop_relation(tmp_relation) %}
     {% endif %}
     {% do run_query(create_table_as(True, tmp_relation, sql)) %}
-    {% set build_sql = iceberg_merge(on_schema_change, tmp_relation, target_relation, unique_key, existing_relation, delete_condition) %}
+    {% set build_sql = iceberg_merge(on_schema_change, tmp_relation, target_relation, unique_key, incremental_predicates, existing_relation, delete_condition) %}
     {% do to_drop.append(tmp_relation) %}
   {% endif %}
 
   {% call statement("main") %}
     {{ build_sql }}
   {% endcall %}
 
@@ -80,16 +88,20 @@
 
   {% for rel in to_drop %}
     {% do drop_relation(rel) %}
   {% endfor %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
-  {% if lf_tags is not none or lf_tags_columns is not none %}
-    {{ adapter.add_lf_tags(target_relation.schema, target_relation.identifier, lf_tags, lf_tags_columns) }}
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
   {% endif %}
 
   {% do persist_docs(target_relation, model) %}
 
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization %}
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         {{ col.quoted }} = {{ 'src.' + col.quoted }}
     {%- else -%}
         {{ col.quoted }} = {{ rule | replace("_new_", 'src.' + col.quoted) | replace("_old_", 'target.' + col.quoted) }}
     {%- endif -%}
     {{ "," if not is_last }}
 {%- endmacro -%}
 
-{% macro iceberg_merge(on_schema_change, tmp_relation, target_relation, unique_key, existing_relation, delete_condition, statement_name="main") %}
+{% macro iceberg_merge(on_schema_change, tmp_relation, target_relation, unique_key, incremental_predicates, existing_relation, delete_condition, statement_name="main") %}
     {%- set merge_update_columns = config.get('merge_update_columns') -%}
     {%- set merge_exclude_columns = config.get('merge_exclude_columns') -%}
     {%- set merge_update_columns_default_rule = config.get('merge_update_columns_default_rule', 'replace') -%}
     {%- set merge_update_columns_rules = config.get('merge_update_columns_rules') -%}
 
     {% set dest_columns = process_schema_changes(on_schema_change, tmp_relation, existing_relation) %}
     {% if not dest_columns %}
@@ -75,14 +75,21 @@
     {%- set src_cols_csv = src_columns_quoted | join(', ') -%}
     merge into {{ target_relation }} as target using {{ tmp_relation }} as src
     on (
       {%- for key in unique_key_cols %}
         target.{{ key }} = src.{{ key }} {{ "and " if not loop.last }}
       {%- endfor %}
     )
+    {% if incremental_predicates is not none -%}
+    and (
+      {%- for inc_predicate in incremental_predicates %}
+        {{ inc_predicate }} {{ "and " if not loop.last }}
+      {%- endfor %}
+    )
+    {%- endif %}
     {% if delete_condition is not none -%}
     when matched and ({{ delete_condition }})
       then delete
     {%- endif %}
     when matched
       then update set
         {%- for col in update_columns %}
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   {%- set partition_property = 'partitioned_by' -%}
   {%- set work_group_output_location_enforced = adapter.is_work_group_output_location_enforced() -%}
   {%- set location = adapter.generate_s3_location(relation,
                                                  s3_data_dir,
                                                  s3_data_naming,
                                                  external_location,
                                                  temporary) -%}
+  {%- set native_drop = config.get('native_drop', default=false) -%}
 
   {%- set contract_config = config.get('contract') -%}
   {%- if contract_config.enforced -%}
     {{ get_assert_columns_equivalent(sql) }}
   {%- endif -%}
 
   {%- if table_type == 'iceberg' -%}
@@ -43,15 +44,19 @@
         You need to have an unique table location when creating Iceberg table since we use the RENAME feature
         to have near-zero downtime.
       {%- endset -%}
       {% do exceptions.raise_compiler_error(error_unique_location_iceberg) %}
     {%- endif -%}
   {%- endif %}
 
-  {% do adapter.delete_from_s3(location) %}
+  {%- if native_drop and table_type == 'iceberg' -%}
+    {% do log('Config native_drop enabled, skipping direct S3 delete') %}
+  {%- else -%}
+    {% do adapter.delete_from_s3(location) %}
+  {%- endif -%}
 
   create table {{ relation }}
   with (
     table_type='{{ table_type }}',
     is_external={%- if table_type == 'iceberg' -%}false{%- else -%}true{%- endif %},
   {%- if not work_group_output_location_enforced or table_type == 'iceberg' -%}
     {{ location_property }}='{{ location }}',
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 -- TODO create a drop_relation_with_versions, to be sure to remove all historical versions of a table
 {% materialization table, adapter='athena' -%}
   {%- set identifier = model['alias'] -%}
 
-  {%- set lf_tags = config.get('lf_tags', default=none) -%}
-  {%- set lf_tags_columns = config.get('lf_tags_columns', default=none) -%}
+  {%- set lf_tags_config = config.get('lf_tags_config') -%}
+  {%- set lf_grants = config.get('lf_grants') -%}
+
   {%- set table_type = config.get('table_type', default='hive') | lower -%}
   {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
   {%- set is_ha = config.get('ha', default=false) -%}
   {%- set s3_data_dir = config.get('s3_data_dir', default=target.s3_data_dir) -%}
   {%- set s3_data_naming = config.get('s3_data_naming', default='table_unique') -%}
   {%- set full_refresh_config = config.get('full_refresh', default=False) -%}
   {%- set is_full_refresh_mode = (flags.FULL_REFRESH == True or full_refresh_config == True) -%}
@@ -104,16 +105,20 @@
       {{ drop_relation(old_relation_bkp) }}
     {%- endif -%}
 
   {%- endif -%}
 
   {{ run_hooks(post_hooks) }}
 
-  {% if lf_tags is not none or lf_tags_columns is not none %}
-    {{ adapter.add_lf_tags(target_relation.schema, identifier, lf_tags, lf_tags_columns) }}
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
   {% endif %}
 
   {% do persist_docs(target_relation, model) %}
 
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 {% macro create_or_replace_view(run_outside_transaction_hooks=True) %}
   {%- set identifier = model['alias'] -%}
 
-  {%- set lf_tags = config.get('lf_tags', default=none) -%}
-  {%- set lf_tags_columns = config.get('lf_tags_columns', default=none) -%}
+  {%- set lf_tags_config = config.get('lf_tags_config') -%}
+  {%- set lf_grants = config.get('lf_grants') -%}
+
   {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
   {%- set exists_as_view = (old_relation is not none and old_relation.is_view) -%}
   {%- set target_relation = api.Relation.create(
       identifier=identifier,
       schema=schema,
       database=database,
       type='view',
@@ -26,16 +27,20 @@
   {%- endif -%}
 
   -- build model
   {% call statement('main') -%}
     {{ create_view_as(target_relation, sql) }}
   {%- endcall %}
 
-  {% if lf_tags is not none or lf_tags_columns is not none %}
-    {{ adapter.add_lf_tags(target_relation.schema, identifier, lf_tags, lf_tags_columns) }}
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
   {% endif %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
   {{ adapter.commit() }}
 
   {% if run_outside_transaction_hooks %}
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files 3% similar despite different names*

```diff
@@ -119,19 +119,20 @@
     {% do return(temp_relation) %}
 {% endmacro %}
 
 {% materialization snapshot, adapter='athena' %}
   {%- set config = model['config'] -%}
 
   {%- set target_table = model.get('alias', model.get('name')) -%}
-
   {%- set strategy_name = config.get('strategy') -%}
   {%- set file_format = config.get('file_format', 'parquet') -%}
   {%- set table_type = config.get('table_type', 'hive') -%}
 
+  {%- set lf_tags_config = config.get('lf_tags_config') -%}
+  {%- set lf_grants = config.get('lf_grants') -%}
 
   {{ log('Checking if target table exists') }}
   {% set target_relation_exists, target_relation = get_or_create_relation(
           database=model.database,
           schema=model.schema,
           identifier=target_table,
           type='table') -%}
@@ -229,12 +230,20 @@
 
   {% if new_snapshot_table is defined %}
       {% do adapter.drop_relation(new_snapshot_table) %}
   {% endif %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
+  {% endif %}
+
   {% do persist_docs(target_relation, model) %}
 
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
```

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/datediff.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/ddl_dml_data_type.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/macros/utils/timestamps.sql` & `dbt-athena-community-1.5.1/dbt/include/athena/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt/include/athena/profile_template.yml` & `dbt-athena-community-1.5.1/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/dbt_athena_community.egg-info/PKG-INFO` & `dbt-athena-community-1.5.1/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.5.0
+Version: 1.5.1
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -19,14 +19,15 @@
 License-File: LICENSE.txt
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
+    <a href="https://github.com/python/mypy"><img src="https://www.mypy-lang.org/static/mypy_badge.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
 * Supports dbt version `1.5.*`
 * Supports [seeds][seeds]
@@ -99,15 +100,14 @@
 | database              | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                           |
 | poll_interval         | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                        |
 | aws_access_key_id     | Access key ID of the user performing requests.                                 | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
 | aws_secret_access_key | Secret access key of the user performing requests                              | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
 | aws_profile_name      | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                               |
 | work_group            | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                      |
 | num_retries           | Number of times to retry a failing query                                       | Optional  | `3`                                        |
-| lf_tags               | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}`   |
 
 **Example profiles.yml entry:**
 ```yaml
 athena:
   target: dev
   outputs:
     dev:
@@ -116,17 +116,14 @@
       s3_data_dir: s3://your_s3_bucket/dbt/
       s3_data_naming: schema_table
       region_name: eu-west-1
       schema: dbt
       database: awsdatacatalog
       aws_profile_name: my-profile
       work_group: my-workgroup
-      lf_tags:
-        origin: dbt
-        team: analytics
 ```
 
 _Additional information_
 * `threads` is supported
 * `database` and `catalog` can be used interchangeably
 
 
@@ -154,20 +151,82 @@
   * The data format for the table
   * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE`
 * `write_compression` (`default=none`)
   * The compression type to use for any storage format that allows compression to be specified. To see which options are available, check out [CREATE TABLE AS][create-table-as]
 * `field_delimiter` (`default=none`)
   * Custom field delimiter, for when format is set to `TEXTFILE`
 * `table_properties`: table properties to add to the table, valid for Iceberg only
-* `lf_tags` (`default=none`)
-  * lf tags to associate with the table
-  * format: `{"tag1": "value1", "tag2": "value2"}`
-* `lf_tags_columns` (`default=none`)
-  * lf tags to associate with the table columns
-  * format: `{"tag1": {"value1": ["column1": "column2"]}}`
++ `native_drop`: Relation drop operations will be performed with SQL, not direct Glue API calls. No S3 calls will be made to manage data in S3. Data in S3 will only be cleared up for Iceberg tables [see AWS docs](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html). Note that Iceberg DROP TABLE operations may timeout if they take longer than 60 seconds.
++ `seed_by_insert` (`default=false`)
+  + default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
+  + large seed files cannot use `seed_by_insert`, as the SQL insert statement would exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/latest/ug/service-limits.html)
+* `lf_tags_config` (`default=none`)
+  * [AWS lakeformation](#aws-lakeformation-integration) tags to associate with the table and columns
+  * format for model config:
+```sql
+{{
+  config(
+    materialized='incremental',
+    incremental_strategy='append',
+    on_schema_change='append_new_columns',
+    table_type='iceberg',
+    schema='test_schema',
+    lf_tags_config={
+          'enabled': true,
+          'tags': {
+            'tag1': 'value1',
+            'tag2': 'value2'
+          },
+          'tags_columns': {
+            'tag1': {
+              'value1': ['column1', 'column2'],
+              'value2': ['column3', 'column4']
+            }
+          }
+    }
+  )
+}}
+```
+* format for `dbt_project.yml`:
+```yaml
+  +lf_tags_config:
+    enabled: true
+    tags:
+      tag1: value1
+      tag2: value2
+    tags_columns:
+      tag1:
+        value1: [ column1, column2 ]
+```
+* `lf_grants` (`default=none`)
+  * lakeformation grants config for data_cell filters
+  * format:
+  ```python
+  lf_grants={
+          'data_cell_filters': {
+              'enabled': True | False,
+              'filters': {
+                  'filter_name': {
+                      'row_filter': '<filter_condition>',
+                      'principals': ['principal_arn1', 'principal_arn2']
+                  }
+              }
+          }
+      }
+  ```
+
+> Notes:  
+> - `lf_tags` and `lf_tags_columns` configs support only attaching lf tags to corresponding resources.
+> We recommend managing LF Tags permissions somewhere outside dbt. For example, you may use
+> [terraform](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions) or
+> [aws cdk](https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for such purpose.
+> - `data_cell_filters` management can't be automated outside dbt because the filter can't be attached to the table
+> which doesn't exist. Once you `enable` this config, dbt will set all filters and their permissions during every
+> dbt run. Such approach keeps the actual state of row level security configuration actual after every dbt run and
+> apply changes if they occur: drop, create, update filters and their permissions.
 
 [create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 
 ### Table location
 
 The location in which a table is saved is determined by:
 
@@ -239,28 +298,28 @@
 ```
 
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
 It is possible to use Iceberg in an incremental fashion, specifically two strategies are supported:
-* `append`: new records are appended to the table, this can lead to duplicates
-* `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
-   It performs an upsert, new record are added, and record already existing are updated. If
-   `delete_condition` is provided in the model config, it can also delete records based on the
-   provided condition (SQL condition). You can use any column of the incremental table (`src`) or
-   the final table (`target`). You must prefix the column by the name of the table to prevent
-   `Column is ambiguous` error.
+* `append`: New records are appended to the table, this can lead to duplicates.
+* `merge`: Performs an upsert (and optional delete), where new records are added and existing records are updated. Only available with Athena engine version 3.
+    - `unique_key` **(required)**: columns that define a unique record in the source and target tables.
+    - `incremental_predicates` (optional): SQL conditions that enable custom join clauses in the merge statement. This can be useful for improving performance via predicate pushdown on the target table.
+    - `delete_condition` (optional): SQL condition used to identify records that should be deleted.
+      - `delete_condition` and `incremental_predicates` can include any column of the incremental table (`src`) or the final table (`target`). Column names must be prefixed by either `src` or `target` to prevent a `Column is ambiguous` error.
 
 ```sql
 {{ config(
     materialized='incremental',
     table_type='iceberg',
     incremental_strategy='merge',
     unique_key='user_id',
+    incremental_predicates=["src.quantity > 1", "target.my_date >= now() - interval '4' year"],
     delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year",
     format='parquet'
 ) }}
 
 select
 	'A' as user_id,
 	'pi' as name,
@@ -280,15 +339,15 @@
 
 ```sql
 {{ config(
     materialized='table',
     ha=true,
     format='parquet',
     table_type='hive',
-    partition_by=['status'],
+    partitioned_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
 select
   'a' as user_id,
   'pi' as user_name,
   'active' as status
@@ -321,14 +380,32 @@
 
 To use the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy)
 
 ### Hard-deletes
 
 The materialization also supports invalidating hard deletes. Check the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to understand usage.
 
+### AWS Lakeformation integration
+
+The adapter implements AWS Lakeformation tags management in the following way:
+- you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
+- once you enable the feature, lf-tags will be updated on every dbt run
+- first, all lf-tags for columns are removed to avoid inheritance issues
+- then all redundant lf-tags are removed from table and actual tags from config are applied
+- finally, lf-tags for columns are applied
+
+It's important to understand the following points:
+- dbt does not manage lf-tags for database
+- dbt does not manage lakeformation permissions
+
+That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.  
+You may find the following links useful to manage that:
+- [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
+- [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
+
 ### Working example
 
 seed file - employent_indicators_november_2022_csv_tables.csv
 ```
 Series_reference,Period,Data_value,Suppressed
 MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803,
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.5.0 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.5.1 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
- code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
-                                    month]
+       code%20style-black-000000.svg] [https://www.mypy-lang.org/static/
+     mypy_badge.svg] [https://pepy.tech/badge/dbt-athena-community/month]
 ## Features * Supports dbt version `1.5.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
 [table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
 * Hive tables are supported by both Athena engines. * Supports [incremental
 models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
 only with the `merge` strategy * Supports the `append` strategy * On Hive
@@ -64,45 +64,72 @@
 results in Athena | Optional | `5` | | aws_access_key_id | Access key ID of the
 user performing requests. | Optional | `AKIAIOSFODNN7EXAMPLE` | |
 aws_secret_access_key | Secret access key of the user performing requests |
 Optional | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` | | aws_profile_name |
 Profile to use from your AWS shared credentials file. | Optional | `my-profile`
 | | work_group | Identifier of Athena workgroup | Optional | `my-custom-
 workgroup` | | num_retries | Number of times to retry a failing query |
-Optional | `3` | | lf_tags | Default lf tags to apply to any database created
-by dbt | Optional | `{"origin": "dbt", "team": "analytics"}` | **Example
-profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
-s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
-your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
-dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
-workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
-`threads` is supported * `database` and `catalog` can be used interchangeably
-## Models ### Table Configuration * `external_location` (`default=none`) * If
-set, the full S3 path in which the table will be saved. * Does not work with
-Iceberg table or Hive table with `ha` set to true. * `partitioned_by`
-(`default=none`) * An array list of columns by which the table will be
-partitioned * Limited to creation of 100 partitions (_currently_) *
-`bucketed_by` (`default=none`) * An array list of columns to bucket data,
-ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
-buckets for bucketing your data, ignored if using Iceberg * `table_type`
-(`default='hive'`) * The type of table * Supports `hive` or `iceberg` * `ha`
-(`default=false`) * If the table should be built using the high-availability
-method. This option is only available for Hive tables since it is by default
-for Iceberg tables (see the section [below](#highly-available-table)) *
-`format` (`default='parquet'`) * The data format for the table * Supports
-`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
-(`default=none`) * The compression type to use for any storage format that
-allows compression to be specified. To see which options are available, check
-out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
-Custom field delimiter, for when format is set to `TEXTFILE` *
-`table_properties`: table properties to add to the table, valid for Iceberg
-only * `lf_tags` (`default=none`) * lf tags to associate with the table *
-format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
-(`default=none`) * lf tags to associate with the table columns * format: `
-{"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
+Optional | `3` | **Example profiles.yml entry:** ```yaml athena: target: dev
+outputs: dev: type: athena s3_staging_dir: s3://athena-query-results/dbt/
+s3_data_dir: s3://your_s3_bucket/dbt/ s3_data_naming: schema_table region_name:
+eu-west-1 schema: dbt database: awsdatacatalog aws_profile_name: my-profile
+work_group: my-workgroup ``` _Additional information_ * `threads` is supported
+* `database` and `catalog` can be used interchangeably ## Models ### Table
+Configuration * `external_location` (`default=none`) * If set, the full S3 path
+in which the table will be saved. * Does not work with Iceberg table or Hive
+table with `ha` set to true. * `partitioned_by` (`default=none`) * An array
+list of columns by which the table will be partitioned * Limited to creation of
+100 partitions (_currently_) * `bucketed_by` (`default=none`) * An array list
+of columns to bucket data, ignored if using Iceberg * `bucket_count`
+(`default=none`) * The number of buckets for bucketing your data, ignored if
+using Iceberg * `table_type` (`default='hive'`) * The type of table * Supports
+`hive` or `iceberg` * `ha` (`default=false`) * If the table should be built
+using the high-availability method. This option is only available for Hive
+tables since it is by default for Iceberg tables (see the section [below]
+(#highly-available-table)) * `format` (`default='parquet'`) * The data format
+for the table * Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` *
+`write_compression` (`default=none`) * The compression type to use for any
+storage format that allows compression to be specified. To see which options
+are available, check out [CREATE TABLE AS][create-table-as] * `field_delimiter`
+(`default=none`) * Custom field delimiter, for when format is set to `TEXTFILE`
+* `table_properties`: table properties to add to the table, valid for Iceberg
+only + `native_drop`: Relation drop operations will be performed with SQL, not
+direct Glue API calls. No S3 calls will be made to manage data in S3. Data in
+S3 will only be cleared up for Iceberg tables [see AWS docs](https://
+docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html).
+Note that Iceberg DROP TABLE operations may timeout if they take longer than 60
+seconds. + `seed_by_insert` (`default=false`) + default behaviour uploads seed
+data to S3. This flag will create seeds using an SQL insert statement + large
+seed files cannot use `seed_by_insert`, as the SQL insert statement would
+exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/
+latest/ug/service-limits.html) * `lf_tags_config` (`default=none`) * [AWS
+lakeformation](#aws-lakeformation-integration) tags to associate with the table
+and columns * format for model config: ```sql {{ config
+( materialized='incremental', incremental_strategy='append',
+on_schema_change='append_new_columns', table_type='iceberg',
+schema='test_schema', lf_tags_config={ 'enabled': true, 'tags': { 'tag1':
+'value1', 'tag2': 'value2' }, 'tags_columns': { 'tag1': { 'value1': ['column1',
+'column2'], 'value2': ['column3', 'column4'] } } } ) }} ``` * format for
+`dbt_project.yml`: ```yaml +lf_tags_config: enabled: true tags: tag1: value1
+tag2: value2 tags_columns: tag1: value1: [ column1, column2 ] ``` * `lf_grants`
+(`default=none`) * lakeformation grants config for data_cell filters * format:
+```python lf_grants={ 'data_cell_filters': { 'enabled': True | False,
+'filters': { 'filter_name': { 'row_filter': '', 'principals':
+['principal_arn1', 'principal_arn2'] } } } } ``` > Notes: > - `lf_tags` and
+`lf_tags_columns` configs support only attaching lf tags to corresponding
+resources. > We recommend managing LF Tags permissions somewhere outside dbt.
+For example, you may use > [terraform](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) or > [aws cdk]
+(https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for
+such purpose. > - `data_cell_filters` management can't be automated outside dbt
+because the filter can't be attached to the table > which doesn't exist. Once
+you `enable` this config, dbt will set all filters and their permissions during
+every > dbt run. Such approach keeps the actual state of row level security
+configuration actual after every dbt run and > apply changes if they occur:
+drop, create, update filters and their permissions. [create-table-as]: https://
 docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 ### Table location The location in which a table is saved is determined by: 1.
 If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
 defined, the path is determined by that and `s3_data_naming` 3. If
 `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
 ` Here all the options available for `s3_data_naming`: * `unique`: `
 {s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
@@ -133,37 +160,43 @@
 table_type='iceberg', format='parquet', partitioned_by=['bucket(user_id, 5)'],
 table_properties={ 'optimize_rewrite_delete_file_threshold': '2' } ) }} select
 'A' as user_id, 'pi' as name, 'active' as status, 17.89 as cost, 1 as quantity,
 100000000 as quantity_big, current_date as my_date ``` Iceberg supports
 bucketing as hidden partitions, therefore use the `partitioned_by` config to
 add specific bucketing conditions. Iceberg supports several table formats for
 data : `PARQUET`, `AVRO` and `ORC`. It is possible to use Iceberg in an
-incremental fashion, specifically two strategies are supported: * `append`: new
-records are appended to the table, this can lead to duplicates * `merge`: must
-be used in combination with `unique_key` and it's only available with Engine
-version 3. It performs an upsert, new record are added, and record already
-existing are updated. If `delete_condition` is provided in the model config, it
-can also delete records based on the provided condition (SQL condition). You
-can use any column of the incremental table (`src`) or the final table
-(`target`). You must prefix the column by the name of the table to prevent
-`Column is ambiguous` error. ```sql {{ config( materialized='incremental',
-table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
+incremental fashion, specifically two strategies are supported: * `append`: New
+records are appended to the table, this can lead to duplicates. * `merge`:
+Performs an upsert (and optional delete), where new records are added and
+existing records are updated. Only available with Athena engine version 3. -
+`unique_key` **(required)**: columns that define a unique record in the source
+and target tables. - `incremental_predicates` (optional): SQL conditions that
+enable custom join clauses in the merge statement. This can be useful for
+improving performance via predicate pushdown on the target table. -
+`delete_condition` (optional): SQL condition used to identify records that
+should be deleted. - `delete_condition` and `incremental_predicates` can
+include any column of the incremental table (`src`) or the final table
+(`target`). Column names must be prefixed by either `src` or `target` to
+prevent a `Column is ambiguous` error. ```sql {{ config
+( materialized='incremental', table_type='iceberg',
+incremental_strategy='merge', unique_key='user_id', incremental_predicates=
+["src.quantity > 1", "target.my_date >= now() - interval '4' year"],
 delete_condition="src.status != 'active' and target.my_date < now() - interval
 '2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
 as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
 current_date as my_date ``` ### Highly available table The current
 implementation of the table materialization can lead to downtime, as target
 table is dropped and re-created. To have the less destructive behavior it's
 possible to use the `ha` config on your `table` materialized models. It
 leverages the table versions feature of glue catalog, creating a tmp table and
 swapping the target table to the location of the tmp table. This
 materialization is only available for `table_type=hive` and requires using
 unique locations. For iceberg, high availability is by default. ```sql {
 { config( materialized='table', ha=true, format='parquet', table_type='hive',
-partition_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
+partitioned_by=['status'], s3_data_naming='table_unique' ) }} select 'a' as
 user_id, 'pi' as user_name, 'active' as status union all select 'b' as user_id,
 'sh' as user_name, 'disabled' as status ``` By default, the materialization
 keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions * By default, Glue "duplicates" the versions internally,
@@ -176,16 +209,30 @@
 snapshot create a snapshot file in the snapshots directory. If the directory
 does not exist create one. ### Timestamp strategy To use the timestamp strategy
 refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
 strategy-recommended) ### Check strategy To use the check strategy refer to the
 [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
 Hard-deletes The materialization also supports invalidating hard deletes. Check
 the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
-understand usage. ### Working example seed file -
-employent_indicators_november_2022_csv_tables.csv ```
+understand usage. ### AWS Lakeformation integration The adapter implements AWS
+Lakeformation tags management in the following way: - you can enable or disable
+lf-tags management via [config](#table-configuration) (disabled by default) -
+once you enable the feature, lf-tags will be updated on every dbt run - first,
+all lf-tags for columns are removed to avoid inheritance issues - then all
+redundant lf-tags are removed from table and actual tags from config are
+applied - finally, lf-tags for columns are applied It's important to understand
+the following points: - dbt does not manage lf-tags for database - dbt does not
+manage lakeformation permissions That's why you should handle this by yourself
+manually or using some automation tools like terraform, AWS CDK etc. You may
+find the following links useful to manage that: - [terraform
+aws_lakeformation_permissions](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) - [terraform
+aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ### Working
+example seed file - employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
```

### Comparing `dbt-athena-community-1.5.0/dbt_athena_community.egg-info/SOURCES.txt` & `dbt-athena-community-1.5.1/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dbt/adapters/athena/__version__.py
 dbt/adapters/athena/column.py
 dbt/adapters/athena/config.py
 dbt/adapters/athena/connections.py
 dbt/adapters/athena/constants.py
 dbt/adapters/athena/exceptions.py
 dbt/adapters/athena/impl.py
+dbt/adapters/athena/lakeformation.py
 dbt/adapters/athena/query_headers.py
 dbt/adapters/athena/relation.py
 dbt/adapters/athena/s3.py
 dbt/adapters/athena/session.py
 dbt/adapters/athena/utils.py
 dbt/include/athena/__init__.py
 dbt/include/athena/dbt_project.yml
```

### Comparing `dbt-athena-community-1.5.0/pyproject.toml` & `dbt-athena-community-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.5.0/setup.py` & `dbt-athena-community-1.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #!/usr/bin/env python
 import os
 import re
+from typing import Any, Dict
 
 from setuptools import find_namespace_packages, setup
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 package_name = "dbt-athena-community"
 
 
 # get version from a separate file
-def _get_plugin_version_dict():
+def _get_plugin_version_dict() -> Dict[str, Any]:
     _version_path = os.path.join(this_directory, "dbt", "adapters", "athena", "__version__.py")
     _semver = r"""(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)"""
     _pre = r"""((?P<prekind>a|b|rc)(?P<pre>\d+))?"""
     _version_pattern = rf"""version\s*=\s*["']{_semver}{_pre}["']"""
     with open(_version_path) as f:
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
             raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
-def _get_package_version():
+def _get_package_version() -> str:
     parts = _get_plugin_version_dict()
     return f'{parts["major"]}.{parts["minor"]}.{parts["patch"]}'
 
 
 dbt_version = "1.5"
 package_version = _get_package_version()
 description = "The athena adapter plugin for dbt (data build tool)"
@@ -52,14 +53,15 @@
     include_package_data=True,
     install_requires=[
         # In order to control dbt-core version and package version
         "boto3~=1.26",
         "boto3-stubs[athena,glue,lakeformation,sts]~=1.26",
         "dbt-core~=1.5.0",
         "pyathena>=2.25,<4.0",
+        "pydantic~=1.10",
         "tenacity~=8.2",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

