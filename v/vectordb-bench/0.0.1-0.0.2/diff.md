# Comparing `tmp/vectordb-bench-0.0.1-1.tar.gz` & `tmp/vectordb-bench-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb-bench-0.0.1.tar", last modified: Wed Jun 14 11:05:52 2023, max compression
+gzip compressed data, was "vectordb-bench-0.0.2.tar", last modified: Wed Jun 21 12:43:37 2023, max compression
```

## Comparing `vectordb-bench-0.0.1-1.tar` & `vectordb-bench-0.0.2.tar`

### file list

```diff
@@ -1,85 +1,102 @@
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1067 2023-06-14 02:27:58.000000 vectordb-bench-0.0.1/LICENSE
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14689 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13797 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/README.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1642 2023-06-14 11:04:59.000000 vectordb-bench-0.0.1/pyproject.toml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/setup.cfg
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/tests/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1841 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/tests/test_bench_runner.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1776 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/tests/test_dataset.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2753 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/tests/test_elasticsearch_cloud.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1977 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/tests/test_models.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1079 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/tests/test_utils.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      837 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      848 2023-06-14 11:04:59.000000 vectordb-bench-0.0.1/vectordb_bench/__main__.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1734 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/assembler.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3965 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/cases.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/clients/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1255 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5168 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/api.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/clients/elastic_cloud/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1612 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/elastic_cloud/config.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5037 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/clients/milvus/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3171 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/milvus/config.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5830 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/milvus/milvus.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/clients/pinecone/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      434 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/pinecone/config.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3854 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/pinecone/pinecone.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/clients/qdrant_cloud/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      420 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/qdrant_cloud/config.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5250 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/clients/weaviate_cloud/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1331 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/weaviate_cloud/config.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5111 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/clients/zilliz_cloud/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      865 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/zilliz_cloud/config.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      973 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    12865 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/dataset.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      435 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/result_collector.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench/backend/runner/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      230 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/runner/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4406 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/runner/mp_runner.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6327 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/runner/serial_runner.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9134 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/task_runner.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2563 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/backend/utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      130 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/base.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/vectordb_bench/frontend/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.053520 vectordb-bench-0.0.1/vectordb_bench/frontend/components/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5340 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/charts.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2828 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/data.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3214 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/filters.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      399 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/headerIcon.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      592 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/nav.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1299 2023-06-14 11:04:59.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/priceTable.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      281 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/autoRefresh.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3451 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/caseSelector.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1642 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/dbConfigSetting.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1184 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/dbSelector.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      706 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/generateTasks.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      281 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/hideSidebar.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2116 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/submitTask.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13175 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/const.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/vectordb_bench/frontend/pages/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2034 2023-06-14 11:04:59.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/pages/qps_with_price.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1929 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/pages/run_test.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      162 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/frontend/vdb_benchmark.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8671 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/interface.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2907 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/log_util.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1018 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/metric.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7683 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/models.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.061520 vectordb-bench-0.0.1/vectordb_bench/results/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    80276 2023-06-14 09:23:16.000000 vectordb-bench-0.0.1/vectordb_bench/results/result_20230609_standard.json
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-14 11:05:52.057520 vectordb-bench-0.0.1/vectordb_bench.egg-info/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14689 2023-06-14 11:05:52.000000 vectordb-bench-0.0.1/vectordb_bench.egg-info/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2720 2023-06-14 11:05:52.000000 vectordb-bench-0.0.1/vectordb_bench.egg-info/SOURCES.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-06-14 11:05:52.000000 vectordb-bench-0.0.1/vectordb_bench.egg-info/dependency_links.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       60 2023-06-14 11:05:52.000000 vectordb-bench-0.0.1/vectordb_bench.egg-info/entry_points.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      246 2023-06-14 11:05:52.000000 vectordb-bench-0.0.1/vectordb_bench.egg-info/requires.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       15 2023-06-14 11:05:52.000000 vectordb-bench-0.0.1/vectordb_bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.874934 vectordb-bench-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.886934 vectordb-bench-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.github/workflows/publish_package_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.890935 vectordb-bench-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_bench_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_elasticsearch_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/tests/ut_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.894935 vectordb-bench-0.0.2/vectordb_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/pinecone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.898934 vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/result_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/backend/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/runner/mp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/runner/serial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/backend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.882934 vectordb-bench-0.0.2/vectordb_bench/frontend/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/expanderStyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/headerIcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/priceTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/stPageConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.902935 vectordb-bench-0.0.2/vectordb_bench/frontend/components/get_results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/get_results/saveAsImage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/autoRefresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/caseSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbConfigSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/generateTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/hideSidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/submitTask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/frontend/const/
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/const/dbCaseConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/const/dbPrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/const/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/frontend/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/pages/quries_per_dollar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/pages/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/frontend/vdb_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/log_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.906935 vectordb-bench-0.0.2/vectordb_bench/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    86206 2023-06-21 12:43:21.000000 vectordb-bench-0.0.2/vectordb_bench/results/result_20230609_standard.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:43:37.894935 vectordb-bench-0.0.2/vectordb_bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 12:43:37.000000 vectordb-bench-0.0.2/vectordb_bench.egg-info/top_level.txt
```

### Comparing `vectordb-bench-0.0.1/LICENSE` & `vectordb-bench-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/PKG-INFO` & `vectordb-bench-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: vectordb-bench
-Version: 0.0.1
+Version: 0.0.2
 Summary: VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 Author-email: XuanYang-cn <xuan.yang@zilliz.com>
 Project-URL: repository, https://github.com/zilliztech/VectorDBBench
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # VectorDBBench: A Benchmark Tool for VectorDB
 
+[![version](https://img.shields.io/pypi/v/vectordb-bench.svg?color=blue)](https://pypi.org/project/vectordb-bench/)
+[![Downloads](https://pepy.tech/badge/vectordb-bench)](https://pepy.tech/project/vectordb-bench)
+
 ## Quick Start
 ### Prerequirement
 ``` shell
 python >= 3.11
 ```
 ### Install
 ``` shell
@@ -30,15 +33,15 @@
 ```
 ## What is VectorDBBench
 VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 
 Understanding the importance of user experience, we provide an intuitive visual interface. This not only empowers users to initiate benchmarks at ease, but also to view comparative result reports, thereby reproducing benchmark results effortlessly.
 To add more relevance and practicality, we provide cost-effectiveness reports particularly for cloud services. This allows for a more realistic and applicable benchmarking process.
 
-Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as SIFT, GIST, Cohere, and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
+Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as [SIFT](http://corpus-texmex.irisa.fr/), [GIST](http://corpus-texmex.irisa.fr/), [Cohere](https://huggingface.co/datasets/Cohere/wikipedia-22-12/tree/main/en), and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
 
 Prepare to delve into the world of VectorDBBench, and let it guide you in uncovering your perfect vector database match.  
 
 ## Build on your own
 ### Install requirements
 ``` shell
 pip install -e '.[test]'
@@ -62,64 +65,58 @@
 
 ```shell
 $ ruff check vectordb_bench --fix
 ```
 
 ## How does it work?
 ### Result Page
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/a8418fb6-0822-4f04-a04d-ab9143815b3e)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/66ab83c4-656e-41a8-a643-d9790faccbeb)
 This is the main page of VectorDBBench, which displays the standard benchmark results we provide. Additionally, results of all tests performed by users themselves will also be shown here. We also offer the ability to select and compare results from multiple tests simultaneously.
 
-The standard benchmark results displayed here include all 12 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
+The standard benchmark results displayed here include all 9 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
 ### Run Test Page
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/364e2462-107e-4ce1-aabc-ff2b217ae9b7)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/a789099a-3707-4214-8052-b73463b8f2c6)
 This is the page to run a test:
 1. Initially, you select the systems to be tested - multiple selections are allowed. Once selected, corresponding forms will pop up to gather necessary information for using the chosen databases. The db_label is used to differentiate different instances of the same system. We recommend filling in the host size or instance type here (as we do in our standard results).
 2. The next step is to select the test cases you want to perform. You can select multiple cases at once, and a form to collect corresponding parameters will appear.
 3. Finally, you'll need to provide a task label to distinguish different test results. Using the same label for different tests will result in the previous results being overwritten.
 Now we can only run one task at the same time. 
 
 ## Module
 ### Code Structure
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/8d65c8b4-b9a3-4405-9db8-d27bf1ffda4b)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/8c06512e-5419-4381-b084-9c93aed59639)
 ### Client
 Our client module is designed with flexibility and extensibility in mind, aiming to integrate APIs from different systems seamlessly. As of now, it supports Milvus, Zilliz Cloud, Elastic Search, Pinecone, Qdrant, and Weaviate. Stay tuned for more options, as we are consistently working on extending our reach to other systems.
 ### Benchmark Cases
-We've developed an array of 12 comprehensive benchmark cases to test vector databases' various capabilities, each designed to give you a different piece of the puzzle. These cases are categorized into three main types:
+We've developed an array of 9 comprehensive benchmark cases to test vector databases' various capabilities, each designed to give you a different piece of the puzzle. These cases are categorized into three main types:
 #### Capacity Case
 - **Large Dim:** Tests the database's loading capacity by inserting large-dimension vectors (GIST 100K vectors, 960 dimensions) until fully loaded. The final number of inserted vectors is reported.
 - **Small Dim:** Similar to the Large Dim case but uses small-dimension vectors (SIFT 100K vectors, 128 dimensions).
 #### Search Performance Case
 - **XLarge Dataset:** Measures search performance with a massive dataset (LAION 100M vectors, 768 dimensions) at varying parallel levels. The results include index building time, recall, latency, and maximum QPS.
 - **Large Dataset:** Similar to the XLarge Dataset case, but uses a slightly smaller dataset (Cohere 10M vectors, 768 dimensions).
 - **Medium Dataset:** A case using a medium dataset (Cohere 1M vectors, 768 dimensions).
-- **Small Dataset:** This case uses a small dataset (Cohere 100K vectors, 768 dimensions).
 #### Filtering Search Performance Case
 - **Large Dataset, Low Filtering Rate:** Evaluates search performance with a large dataset (Cohere 10M vectors, 768 dimensions) under a low filtering rate (1% vectors) at different parallel levels.
 - **Medium Dataset, Low Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a similar low filtering rate.
-- **Small Dataset, Low Filtering Rate:** This case uses a small dataset (Cohere 100K vectors, 768 dimensions) with a low filtering rate.
 - **Large Dataset, High Filtering Rate:** It tests with a large dataset (Cohere 10M vectors, 768 dimensions) but under a high filtering rate (99% vectors).
 - **Medium Dataset, High Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a high filtering rate.
-- **Small Dataset, High Filtering Rate:** Finally, this case uses a small dataset (Cohere 100K vectors, 768 dimensions) under a high filtering rate.
 For a quick reference, here is a table summarizing the key aspects of each case:
 
 Case No. | Case Type | Dataset Size | Dataset Type | Filtering Rate | Results |
 |----------|-----------|--------------|--------------|----------------|---------|
 1 | Capacity Case | Large Dim | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
 2 | Capacity Case | Small Dim | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
 3 | Search Performance Case | XLarge Dataset | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
 4 | Search Performance Case | Large Dataset | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
 5 | Search Performance Case | Medium Dataset | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-6 | Search Performance Case | Small Dataset | Cohere 100K vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-7 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-8 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-9 | Filtering Search Performance Case | Small Dataset, Low Filtering Rate | Cohere 100K vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-10 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-11 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-12 | Filtering Search Performance Case | Small Dataset, High Filtering Rate | Cohere 100K vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+6 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+7 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+8 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+9 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
 
 Each case provides an in-depth examination of a vector database's abilities, providing you a comprehensive view of the database's performance.
 
 ## Goals
 Our goals of this benchmark are:
 ### Reproducibility & Usability
 One of the primary goals of VectorDBBench is to enable users to reproduce benchmark results swiftly and easily, or to test their customized scenarios. We believe that lowering the barriers to entry for conducting these tests will enhance the community's understanding and improvement of vector databases. We aim to create an environment where any user, regardless of their technical expertise, can quickly set up and run benchmarks, and view and analyze results in an intuitive manner.
@@ -132,15 +129,15 @@
 2. Adhere to coding conventions and formatting guidelines.
 3. Use clear commit messages to document the purpose of your changes.
 ### Adding New Clients
 **Step 1: Creating New Client Files**
 
 1. Navigate to the vectordb_bench/backend/clients directory.
 2. Create a new folder for your client, for example, "new_client".
-3. Inside the "new_client" folder, create two files: new_client.py and config.py. 
+3. Inside the "new_client" folder, create two files: new_client.py and config.py.
 
 **Step 2: Implement new_client.py and config.py**
 
 1. Open new_client.py and define the NewClient class, which should inherit from the clients/api.py file's VectorDB abstract class. The VectorDB class serves as the API for benchmarking, and all DB clients must implement this abstract class. 
 Example implementation in new_client.py:
 new_client.py
 ```python 
@@ -197,11 +194,9 @@
 ### Installation 
 The system under test can be installed in any form to achieve optimal performance. This includes but is not limited to binary deployment, Docker, and cloud services.
 ### Fine-Tuning
 For the system under test, we use the default server-side configuration to maintain the authenticity and representativeness of our results.
 For the Client, we welcome any parameter tuning to obtain better results.
 ### Incomplete Results
 Many databases may not be able to complete all test cases due to issues such as Out of Memory (OOM), crashes, or timeouts. In these scenarios, we will clearly state these occurrences in the test results.
-### Unpublishable Results
-Although we are trying to support as many clients as possible for benchmarking, due to the restrictions imposed by the [Dewitt Clause](https://cube.dev/blog/dewitt-clause-or-can-you-benchmark-a-database), we're unable to publish all benchmark results. This means that users may not be able to fully compare performance data for certain databases on our platform, despite the support we have integrated for these systems. 
 ### Mistake Or Misrepresentation 
 We strive for accuracy in learning and supporting various vector databases, yet there might be oversights or misapplications. For any such occurrences, feel free to [raise an issue](https://github.com/zilliztech/VectorDBBench/issues/new) or make amendments on our GitHub page.
```

### Comparing `vectordb-bench-0.0.1/README.md` & `vectordb-bench-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # VectorDBBench: A Benchmark Tool for VectorDB
 
+[![version](https://img.shields.io/pypi/v/vectordb-bench.svg?color=blue)](https://pypi.org/project/vectordb-bench/)
+[![Downloads](https://pepy.tech/badge/vectordb-bench)](https://pepy.tech/project/vectordb-bench)
+
 ## Quick Start
 ### Prerequirement
 ``` shell
 python >= 3.11
 ```
 ### Install
 ``` shell
@@ -16,15 +19,15 @@
 ```
 ## What is VectorDBBench
 VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 
 Understanding the importance of user experience, we provide an intuitive visual interface. This not only empowers users to initiate benchmarks at ease, but also to view comparative result reports, thereby reproducing benchmark results effortlessly.
 To add more relevance and practicality, we provide cost-effectiveness reports particularly for cloud services. This allows for a more realistic and applicable benchmarking process.
 
-Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as SIFT, GIST, Cohere, and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
+Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as [SIFT](http://corpus-texmex.irisa.fr/), [GIST](http://corpus-texmex.irisa.fr/), [Cohere](https://huggingface.co/datasets/Cohere/wikipedia-22-12/tree/main/en), and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
 
 Prepare to delve into the world of VectorDBBench, and let it guide you in uncovering your perfect vector database match.  
 
 ## Build on your own
 ### Install requirements
 ``` shell
 pip install -e '.[test]'
@@ -48,64 +51,58 @@
 
 ```shell
 $ ruff check vectordb_bench --fix
 ```
 
 ## How does it work?
 ### Result Page
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/a8418fb6-0822-4f04-a04d-ab9143815b3e)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/66ab83c4-656e-41a8-a643-d9790faccbeb)
 This is the main page of VectorDBBench, which displays the standard benchmark results we provide. Additionally, results of all tests performed by users themselves will also be shown here. We also offer the ability to select and compare results from multiple tests simultaneously.
 
-The standard benchmark results displayed here include all 12 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
+The standard benchmark results displayed here include all 9 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
 ### Run Test Page
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/364e2462-107e-4ce1-aabc-ff2b217ae9b7)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/a789099a-3707-4214-8052-b73463b8f2c6)
 This is the page to run a test:
 1. Initially, you select the systems to be tested - multiple selections are allowed. Once selected, corresponding forms will pop up to gather necessary information for using the chosen databases. The db_label is used to differentiate different instances of the same system. We recommend filling in the host size or instance type here (as we do in our standard results).
 2. The next step is to select the test cases you want to perform. You can select multiple cases at once, and a form to collect corresponding parameters will appear.
 3. Finally, you'll need to provide a task label to distinguish different test results. Using the same label for different tests will result in the previous results being overwritten.
 Now we can only run one task at the same time. 
 
 ## Module
 ### Code Structure
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/8d65c8b4-b9a3-4405-9db8-d27bf1ffda4b)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/8c06512e-5419-4381-b084-9c93aed59639)
 ### Client
 Our client module is designed with flexibility and extensibility in mind, aiming to integrate APIs from different systems seamlessly. As of now, it supports Milvus, Zilliz Cloud, Elastic Search, Pinecone, Qdrant, and Weaviate. Stay tuned for more options, as we are consistently working on extending our reach to other systems.
 ### Benchmark Cases
-We've developed an array of 12 comprehensive benchmark cases to test vector databases' various capabilities, each designed to give you a different piece of the puzzle. These cases are categorized into three main types:
+We've developed an array of 9 comprehensive benchmark cases to test vector databases' various capabilities, each designed to give you a different piece of the puzzle. These cases are categorized into three main types:
 #### Capacity Case
 - **Large Dim:** Tests the database's loading capacity by inserting large-dimension vectors (GIST 100K vectors, 960 dimensions) until fully loaded. The final number of inserted vectors is reported.
 - **Small Dim:** Similar to the Large Dim case but uses small-dimension vectors (SIFT 100K vectors, 128 dimensions).
 #### Search Performance Case
 - **XLarge Dataset:** Measures search performance with a massive dataset (LAION 100M vectors, 768 dimensions) at varying parallel levels. The results include index building time, recall, latency, and maximum QPS.
 - **Large Dataset:** Similar to the XLarge Dataset case, but uses a slightly smaller dataset (Cohere 10M vectors, 768 dimensions).
 - **Medium Dataset:** A case using a medium dataset (Cohere 1M vectors, 768 dimensions).
-- **Small Dataset:** This case uses a small dataset (Cohere 100K vectors, 768 dimensions).
 #### Filtering Search Performance Case
 - **Large Dataset, Low Filtering Rate:** Evaluates search performance with a large dataset (Cohere 10M vectors, 768 dimensions) under a low filtering rate (1% vectors) at different parallel levels.
 - **Medium Dataset, Low Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a similar low filtering rate.
-- **Small Dataset, Low Filtering Rate:** This case uses a small dataset (Cohere 100K vectors, 768 dimensions) with a low filtering rate.
 - **Large Dataset, High Filtering Rate:** It tests with a large dataset (Cohere 10M vectors, 768 dimensions) but under a high filtering rate (99% vectors).
 - **Medium Dataset, High Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a high filtering rate.
-- **Small Dataset, High Filtering Rate:** Finally, this case uses a small dataset (Cohere 100K vectors, 768 dimensions) under a high filtering rate.
 For a quick reference, here is a table summarizing the key aspects of each case:
 
 Case No. | Case Type | Dataset Size | Dataset Type | Filtering Rate | Results |
 |----------|-----------|--------------|--------------|----------------|---------|
 1 | Capacity Case | Large Dim | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
 2 | Capacity Case | Small Dim | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
 3 | Search Performance Case | XLarge Dataset | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
 4 | Search Performance Case | Large Dataset | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
 5 | Search Performance Case | Medium Dataset | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-6 | Search Performance Case | Small Dataset | Cohere 100K vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-7 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-8 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-9 | Filtering Search Performance Case | Small Dataset, Low Filtering Rate | Cohere 100K vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-10 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-11 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-12 | Filtering Search Performance Case | Small Dataset, High Filtering Rate | Cohere 100K vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+6 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+7 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+8 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+9 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
 
 Each case provides an in-depth examination of a vector database's abilities, providing you a comprehensive view of the database's performance.
 
 ## Goals
 Our goals of this benchmark are:
 ### Reproducibility & Usability
 One of the primary goals of VectorDBBench is to enable users to reproduce benchmark results swiftly and easily, or to test their customized scenarios. We believe that lowering the barriers to entry for conducting these tests will enhance the community's understanding and improvement of vector databases. We aim to create an environment where any user, regardless of their technical expertise, can quickly set up and run benchmarks, and view and analyze results in an intuitive manner.
@@ -118,15 +115,15 @@
 2. Adhere to coding conventions and formatting guidelines.
 3. Use clear commit messages to document the purpose of your changes.
 ### Adding New Clients
 **Step 1: Creating New Client Files**
 
 1. Navigate to the vectordb_bench/backend/clients directory.
 2. Create a new folder for your client, for example, "new_client".
-3. Inside the "new_client" folder, create two files: new_client.py and config.py. 
+3. Inside the "new_client" folder, create two files: new_client.py and config.py.
 
 **Step 2: Implement new_client.py and config.py**
 
 1. Open new_client.py and define the NewClient class, which should inherit from the clients/api.py file's VectorDB abstract class. The VectorDB class serves as the API for benchmarking, and all DB clients must implement this abstract class. 
 Example implementation in new_client.py:
 new_client.py
 ```python 
@@ -183,11 +180,9 @@
 ### Installation 
 The system under test can be installed in any form to achieve optimal performance. This includes but is not limited to binary deployment, Docker, and cloud services.
 ### Fine-Tuning
 For the system under test, we use the default server-side configuration to maintain the authenticity and representativeness of our results.
 For the Client, we welcome any parameter tuning to obtain better results.
 ### Incomplete Results
 Many databases may not be able to complete all test cases due to issues such as Out of Memory (OOM), crashes, or timeouts. In these scenarios, we will clearly state these occurrences in the test results.
-### Unpublishable Results
-Although we are trying to support as many clients as possible for benchmarking, due to the restrictions imposed by the [Dewitt Clause](https://cube.dev/blog/dewitt-clause-or-can-you-benchmark-a-database), we're unable to publish all benchmark results. This means that users may not be able to fully compare performance data for certain databases on our platform, despite the support we have integrated for these systems. 
 ### Mistake Or Misrepresentation 
 We strive for accuracy in learning and supporting various vector databases, yet there might be oversights or misapplications. For any such occurrences, feel free to [raise an issue](https://github.com/zilliztech/VectorDBBench/issues/new) or make amendments on our GitHub page.
```

### Comparing `vectordb-bench-0.0.1/pyproject.toml` & `vectordb-bench-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=67.0", "wheel"]
+requires = ["setuptools>=67.0", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
 "vectordb_bench.results" = ["*.json"]
 
 [project]
 name = "vectordb-bench"
@@ -34,20 +34,22 @@
     "plotly",
     "pydantic==v1.10.7", # for qdrant-client
     "environs",
     "scikit-learn",
     "s3fs",
     "psutil",
 ]
-version = "0.0.1"
+dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "ruff",
     "pytest",
 ]
 
 [project.urls]
 "repository" = "https://github.com/zilliztech/VectorDBBench"
 
 [project.scripts]
 init_bench = "vectordb_bench.__main__:main"
+
+[tool.setuptools_scm]
```

### Comparing `vectordb-bench-0.0.1/tests/test_bench_runner.py` & `vectordb-bench-0.0.2/tests/test_bench_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/tests/test_dataset.py` & `vectordb-bench-0.0.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/tests/test_elasticsearch_cloud.py` & `vectordb-bench-0.0.2/tests/test_elasticsearch_cloud.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/tests/test_models.py` & `vectordb-bench-0.0.2/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     @pytest.mark.skip("runs locally")
     def test_test_result(self):
         result = CaseResult(
             task_config=TaskConfig(
                 db=DB.Milvus,
                 db_config=DB.Milvus.config(),
                 db_case_config=DB.Milvus.case_config_cls(index=IndexType.Flat)(),
-                case_config=CaseConfig(case_id=CaseType.PerformanceLZero),
+                case_config=CaseConfig(case_id=CaseType.Performance10M),
             ),
             metrics=Metric(),
         )
 
         test_result = TestResult(run_id=10000, results=[result])
         test_result.write_file()
```

### Comparing `vectordb-bench-0.0.1/tests/test_utils.py` & `vectordb-bench-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/__init__.py` & `vectordb-bench-0.0.2/vectordb_bench/__init__.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/__main__.py` & `vectordb-bench-0.0.2/vectordb_bench/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/assembler.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/assembler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .cases import type2case, CaseLabel
+from .cases import CaseLabel
 from .task_runner import CaseRunner, RunningStatus, TaskRunner
 from ..models import TaskConfig
 from ..backend.clients import EmptyDBCaseConfig
 import logging
 
 
 log = logging.getLogger(__name__)
 
 
 class Assembler:
     @classmethod
     def assemble(cls, run_id , task: TaskConfig) -> CaseRunner:
-        c_cls = type2case.get(task.case_config.case_id)
+        c_cls = task.case_config.case_id.case_cls
 
         c = c_cls()
         if type(task.db_case_config) != EmptyDBCaseConfig:
             task.db_case_config.metric_type = c.dataset.data.metric_type
 
         runner = CaseRunner(
             run_id=run_id,
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/__init__.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/api.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Type
 from contextlib import contextmanager
 
-from pydantic import BaseModel
+from pydantic import BaseModel, validator, SecretStr
 
 
 class MetricType(str, Enum):
     L2 = "L2"
     COSINE = "COSINE"
     IP = "IP"
 
@@ -28,20 +28,28 @@
         db_label(str): label to distinguish different types of DB of the same database.
 
             MilvusConfig.db_label = 2c8g
             MilvusConfig.db_label = 16c64g
             ZillizCloudConfig.db_label = 1cu-perf
     """
 
-    db_label: str | None = None
+    db_label: str = ""
 
     @abstractmethod
     def to_dict(self) -> dict:
         raise NotImplementedError
 
+    @validator("*")
+    def not_empty_field(cls, v, field):
+        if field.name == "db_label":
+            return v
+        if isinstance(v, (str, SecretStr)) and len(v) == 0:
+            raise ValueError("Empty string!")
+        return v
+
 
 class DBCaseConfig(ABC):
     """Case specific vector database configs, usually uesed for index params like HNSW"""
     @abstractmethod
     def index_param(self) -> dict:
         raise NotImplementedError
 
@@ -119,15 +127,15 @@
 
     @abstractmethod
     def insert_embeddings(
         self,
         embeddings: list[list[float]],
         metadata: list[int],
         kwargs: Any,
-    ) -> int:
+    ) -> (int, Exception):
         """Insert the embeddings to the vector database. The default number of embeddings for
         each insert_embeddings is 5000.
 
         Args:
             embeddings(list[list[float]]): list of embedding to add to the vector database.
             metadatas(list[int]): metadata associated with the embeddings, for filtering.
             kwargs(Any): vector database specific parameters.
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/elastic_cloud/config.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from enum import Enum
 from pydantic import SecretStr, BaseModel
 
 from ..api import DBConfig, DBCaseConfig, MetricType, IndexType
 
 
-class ElasticsearchConfig(DBConfig, BaseModel):
+class ElasticCloudConfig(DBConfig, BaseModel):
     cloud_id: SecretStr
-    password: SecretStr | None = None
+    password: SecretStr
 
     def to_dict(self) -> dict:
         return {
             "cloud_id": self.cloud_id.get_secret_value(),
             "basic_auth": ("elastic", self.password.get_secret_value()),
         }
 
 
 class ESElementType(str, Enum):
     float = "float"  # 4 byte
     byte = "byte"  # 1 byte, -128 to 127
 
 
-class ElasticsearchIndexConfig(BaseModel, DBCaseConfig):
+class ElasticCloudIndexConfig(BaseModel, DBCaseConfig):
     element_type: ESElementType = ESElementType.float
     index: IndexType = IndexType.ES_HNSW  # ES only support 'hnsw'
 
     metric_type: MetricType | None = None
     efConstruction: int | None = None
     M: int | None = None
     num_candidates: int | None = None
@@ -41,16 +41,16 @@
             "type": "dense_vector",
             "index": True,
             "element_type": self.element_type.value,
             "similarity": self.parse_metric(),
             "index_options": {
                 "type": self.index.value,
                 "m": self.M,
-                "ef_construction": self.efConstruction
-            }
+                "ef_construction": self.efConstruction,
+            },
         }
         return params
 
     def search_param(self) -> dict:
         return {
             "num_candidates": self.num_candidates,
         }
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 from contextlib import contextmanager
 from typing import Iterable, Type
 from ..api import VectorDB, DBCaseConfig, DBConfig, IndexType
-from .config import ElasticsearchIndexConfig, ElasticsearchConfig
+from .config import ElasticCloudIndexConfig, ElasticCloudConfig
 from elasticsearch.helpers import bulk
 
 
 for logger in ("elasticsearch", "elastic_transport"):
     logging.getLogger(logger).setLevel(logging.WARNING)
 
 log = logging.getLogger(__name__)
 
 class ElasticCloud(VectorDB):
     def __init__(
         self,
         dim: int,
         db_config: dict,
-        db_case_config: ElasticsearchIndexConfig,
+        db_case_config: ElasticCloudIndexConfig,
         indice: str = "vdb_bench_indice",  # must be lowercase
         id_col_name: str = "id",
         vector_col_name: str = "vector",
         drop_old: bool = False,
     ):
         self.dim = dim
         self.db_config = db_config
@@ -39,20 +39,20 @@
             if is_existed_res.raw:
                 client.indices.delete(index=self.indice)
             self._create_indice(client)
 
 
     @classmethod
     def config_cls(cls) -> Type[DBConfig]:
-        return ElasticsearchConfig
+        return ElasticCloudConfig
 
 
     @classmethod
     def case_config_cls(cls, index_type: IndexType | None = None) -> Type[DBCaseConfig]:
-        return ElasticsearchIndexConfig
+        return ElasticCloudIndexConfig
 
 
     @contextmanager
     def init(self) -> None:
         """connect to elasticsearch"""
         from elasticsearch import Elasticsearch
         self.client = Elasticsearch(**self.db_config, request_timeout=30)
@@ -79,15 +79,15 @@
             log.warning(f"Failed to create indice: {self.indice} error: {str(e)}")
             raise e from None
 
     def insert_embeddings(
         self,
         embeddings: Iterable[list[float]],
         metadata: list[int],
-    ) -> int:
+    ) -> (int, Exception):
         """Insert the embeddings to the elasticsearch."""
         assert self.client is not None, "should self.init() first"
 
         insert_data = [
             {
                 "_index": self.indice,
                 "_source": {
@@ -95,18 +95,18 @@
                     self.vector_col_name: embeddings[i],
                 },
             }
             for i in range(len(embeddings))
         ]
         try:
             bulk_insert_res = bulk(self.client, insert_data)
-            return bulk_insert_res[0]
+            return (bulk_insert_res[0], None)
         except Exception as e:
             log.warning(f"Failed to insert data: {self.indice} error: {str(e)}")
-            raise e from None
+            return (0, e)
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
     ) -> list[int]:
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/milvus/config.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pydantic import BaseModel, SecretStr
 from ..api import DBConfig, DBCaseConfig, MetricType, IndexType
 
 
-class MilvusConfig(DBConfig, BaseModel):
-    uri: SecretStr | None = "http://localhost:19530"
+class MilvusConfig(DBConfig):
+    uri: SecretStr = "http://localhost:19530"
 
     def to_dict(self) -> dict:
         return {"uri": self.uri.get_secret_value()}
 
 
-
 class MilvusIndexConfig(BaseModel):
     """Base config for milvus"""
 
     index: IndexType
     metric_type: MetricType | None = None
 
     def parse_metric(self) -> str:
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/milvus/milvus.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/milvus/milvus.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from ..api import VectorDB, DBCaseConfig, DBConfig, IndexType
 from .config import MilvusConfig, _milvus_case_config
 
 
 log = logging.getLogger(__name__)
 
+MILVUS_LOAD_REQS_SIZE = 1.5 * 1024 *1024
 
 class Milvus(VectorDB):
     def __init__(
         self,
         dim: int,
         db_config: dict,
         db_case_config: DBCaseConfig,
@@ -25,14 +26,15 @@
         name: str = "Milvus",
     ):
         """Initialize wrapper around the milvus vector database."""
         self.name = name
         self.db_config = db_config
         self.case_config = db_case_config
         self.collection_name = collection_name
+        self.batch_size = int(MILVUS_LOAD_REQS_SIZE / (dim *4))
 
         self._primary_field = "pk"
         self._scalar_field = "id"
         self._vector_field = "vector"
         self._index_name = "vector_idx"
 
         from pymilvus import connections
@@ -135,30 +137,34 @@
         self._optimize()
 
     def insert_embeddings(
         self,
         embeddings: Iterable[list[float]],
         metadata: list[int],
         **kwargs: Any,
-    ) -> int:
+    ) -> (int, Exception):
         """Insert embeddings into Milvus. should call self.init() first"""
         # use the first insert_embeddings to init collection
         assert self.col is not None
-        insert_data = [
-                metadata,
-                metadata,
-                embeddings,
-        ]
-
+        assert len(embeddings) == len(metadata)
+        insert_count = 0
         try:
-            res = self.col.insert(insert_data, **kwargs)
-            return len(res.primary_keys)
+            for batch_start_offset in range(0, len(embeddings), self.batch_size):
+                batch_end_offset = min(batch_start_offset + self.batch_size, len(embeddings))
+                insert_data = [
+                        metadata[batch_start_offset : batch_end_offset],
+                        metadata[batch_start_offset : batch_end_offset],
+                        embeddings[batch_start_offset : batch_end_offset],
+                ]
+                res = self.col.insert(insert_data, **kwargs)
+                insert_count += len(res.primary_keys)
         except MilvusException as e:
             log.warning("Failed to insert data")
-            raise e from None
+            return (insert_count, e)
+        return (insert_count, None)
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/pinecone/pinecone.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/pinecone/pinecone.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,25 +72,30 @@
     def ready_to_search(self):
         pass
 
     def insert_embeddings(
         self,
         embeddings: list[list[float]],
         metadata: list[int],
-    ) -> list[str]:
+    ) -> (int, Exception):
         assert len(embeddings) == len(metadata)
-        for batch_start_offset in range(0, len(embeddings), self.batch_size):
-            batch_end_offset = min(batch_start_offset + self.batch_size, len(embeddings))
-            insert_datas = []
-            for i in range(batch_start_offset, batch_end_offset):
-                insert_data = (str(metadata[i]), embeddings[i], {
-                            self._metadata_key: metadata[i]})
-                insert_datas.append(insert_data)
-            self.index.upsert(insert_datas)
-        return len(embeddings)
+        insert_count = 0
+        try:
+            for batch_start_offset in range(0, len(embeddings), self.batch_size):
+                batch_end_offset = min(batch_start_offset + self.batch_size, len(embeddings))
+                insert_datas = []
+                for i in range(batch_start_offset, batch_end_offset):
+                    insert_data = (str(metadata[i]), embeddings[i], {
+                                self._metadata_key: metadata[i]})
+                    insert_datas.append(insert_data)
+                self.index.upsert(insert_datas)
+                insert_count += batch_end_offset - batch_start_offset
+        except Exception as e:
+            return (insert_count, e)
+        return (len(embeddings), None)
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,29 +113,28 @@
             raise e from None
 
     def insert_embeddings(
         self,
         embeddings: list[list[float]],
         metadata: list[int],
         **kwargs: Any,
-    ) -> list[str]:
+    ) -> (int, Exception):
         """Insert embeddings into Milvus. should call self.init() first"""
         assert self.qdrant_client is not None
         try:
             # TODO: counts
             _ = self.qdrant_client.upsert(
                 collection_name=self.collection_name,
                 wait=True,
                 points=Batch(ids=metadata, payloads=[{self._primary_field: v} for v in metadata], vectors=embeddings)
             )
-
-            return len(metadata)
+            return (len(metadata), None)
         except Exception as e:
             log.info(f"Failed to insert data, {e}")
-            raise e from None
+            return (0, e)
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/weaviate_cloud/config.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pydantic import BaseModel, SecretStr
 import weaviate
 
 from ..api import DBConfig, DBCaseConfig, MetricType
 
 
-class WeaviateConfig(DBConfig, BaseModel):
-    url: SecretStr | None = None
-    api_key: SecretStr | None = None
+class WeaviateConfig(DBConfig):
+    url: SecretStr
+    api_key: SecretStr
 
     def to_dict(self) -> dict:
         return {
             "url": self.url.get_secret_value(),
             "auth_client_secret": weaviate.AuthApiKey(api_key=self.api_key.get_secret_value()),
         }
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,33 +95,34 @@
                 raise e from None
 
     def insert_embeddings(
         self,
         embeddings: Iterable[list[float]],
         metadata: list[int],
         **kwargs: Any,
-    ) -> int:
+    ) -> (int, Exception):
         """Insert embeddings into Weaviate"""
         assert self.client.schema.exists(self.collection_name)
-
+        insert_count = 0
         try:
-            with self.client.batch as batch:
+            with self.client.batch as batch:               
                 batch.batch_size = len(metadata)
                 batch.dynamic = True
                 res = []
                 for i in range(len(metadata)):
                     res.append(batch.add_data_object(
                         {self._scalar_field: metadata[i]},
                         class_name=self.collection_name,
                         vector=embeddings[i]
                     ))
-                return len(res)
+                    insert_count += 1
+                return (len(res), None)
         except WeaviateBaseError as e:
             log.warning(f"Failed to insert data, error: {str(e)}")
-            raise e from None
+            return (insert_count, e)
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/dataset.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 log = logging.getLogger(__name__)
 
 @dataclass
 class LAION:
     name: str = "LAION"
     dim: int = 768
-    metric_type: MetricType = MetricType.COSINE
+    metric_type: MetricType = MetricType.L2
     use_shuffled: bool = False
 
     @property
     def dir_name(self) -> str:
         return f"{self.name}_{self.label}_{utils.numerize(self.size)}".lower()
 
 @dataclass
@@ -93,34 +93,24 @@
 
 @dataclass
 class GIST_M(GIST):
     label: str = "MEDIUM"
     size: int  = 1_000_000
 
 @dataclass
-class Cohere_S(Cohere):
-    label: str = "SMALL"
-    size: int  = 100_000
-
-@dataclass
 class Cohere_M(Cohere):
     label: str = "MEDIUM"
     size: int = 1_000_000
 
 @dataclass
 class Cohere_L(Cohere):
     label : str = "LARGE"
     size  : int = 10_000_000
 
 @dataclass
-class Glove_S(Glove):
-    label: str = "SMALL"
-    size : int = 100_000
-
-@dataclass
 class Glove_M(Glove):
     label: str = "MEDIUM"
     size : int = 1_000_000
 
 @dataclass
 class SIFT_S(SIFT):
     label: str = "SMALL"
@@ -367,20 +357,18 @@
 
 _global_ds_mapping = {
     Name.GIST: {
         Label.SMALL: DataSet(data=GIST_S()),
         Label.MEDIUM: DataSet(data=GIST_M()),
     },
     Name.Cohere: {
-        Label.SMALL: DataSet(data=Cohere_S()),
         Label.MEDIUM: DataSet(data=Cohere_M()),
         Label.LARGE: DataSet(data=Cohere_L()),
     },
     Name.Glove:{
-        Label.SMALL: DataSet(data=Glove_S()),
         Label.MEDIUM: DataSet(data=Glove_M()),
     },
     Name.SIFT: {
         Label.SMALL: DataSet(data=SIFT_S()),
         Label.MEDIUM: DataSet(data=SIFT_M()),
         Label.LARGE: DataSet(data=SIFT_L()),
     },
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/runner/mp_runner.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/runner/mp_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/runner/serial_runner.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/runner/serial_runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from ...metric import calc_recall
 from ...models import LoadTimeoutError
 from .. import utils
 from ... import config
 
 NUM_PER_BATCH = config.NUM_PER_BATCH
 LOAD_TIMEOUT = 24 * 60 * 60
+LOAD_MAX_TRY_COUNT = 10
+WAITTING_TIME = 60
 
 log = logging.getLogger(__name__)
 
 
 class SerialInsertRunner:
     def __init__(self, db: api.VectorDB, train_emb: list[list[float]], train_id: list[int]):
         log.debug(f"Dataset shape: {len(train_emb)}")
@@ -39,25 +41,67 @@
             log.info(f"({mp.current_process().name:16}) Start inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
             count = 0
             for batch_id in range(self.seq_batches):
                 metadata = all_metadata[batch_id*NUM_PER_BATCH: (batch_id+1)*NUM_PER_BATCH]
                 embeddings = all_embeddings[batch_id*NUM_PER_BATCH: (batch_id+1)*NUM_PER_BATCH]
 
                 log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Start inserting {len(metadata)} embeddings")
-                insert_count = self.db.insert_embeddings(
+                insert_count, error = self.db.insert_embeddings(
                     embeddings=embeddings,
                     metadata=metadata,
                 )
+                if error != None:
+                    raise error
                 log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Finish inserting {len(metadata)} embeddings")
 
                 assert insert_count == len(metadata)
                 count += insert_count
             log.info(f"({mp.current_process().name:16}) Finish inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
         return count
 
+    def endless_insert_data(self, left_id: int = 0) -> int:
+        with self.db.init():
+            all_embeddings = self.shared_emb
+
+            # unique id for endlessness insertion
+            all_metadata = [i+left_id for i in self.train_id]
+
+            num_conc_batches = math.ceil(len(all_embeddings)/NUM_PER_BATCH)
+            log.info(f"({mp.current_process().name:16}) Start inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
+            count = 0
+            for batch_id in range(self.seq_batches):
+                retry_count = 0
+                already_insert_count = 0
+                metadata = all_metadata[batch_id*NUM_PER_BATCH : (batch_id+1)*NUM_PER_BATCH]
+                embeddings = all_embeddings[batch_id*NUM_PER_BATCH : (batch_id+1)*NUM_PER_BATCH]
+
+                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Start inserting {len(metadata)} embeddings")
+                while retry_count < LOAD_MAX_TRY_COUNT:
+                    previous_beg, current_beg = 0, 0
+                    insert_count, error = self.db.insert_embeddings(
+                        embeddings=embeddings[already_insert_count :],
+                        metadata=metadata[already_insert_count :],
+                    )
+                    already_insert_count += insert_count
+                    if error != None:
+                        retry_count += 1
+                        time.sleep(WAITTING_TIME)
+                       
+                        log.info(f"Failed to insert data, try {retry_count} time")
+                        if retry_count >= LOAD_MAX_TRY_COUNT:
+                            raise error
+                    else:
+                        break
+                log.debug(f"({mp.current_process().name:16}) batch [{batch_id:3}/{num_conc_batches}], Finish inserting {len(metadata)} embeddings")
+
+                assert already_insert_count == len(metadata)
+                count += already_insert_count
+            log.info(f"({mp.current_process().name:16}) Finish inserting {len(all_embeddings)} embeddings in batch {NUM_PER_BATCH}")
+        return count
+
     @utils.time_it
     def _insert_all_batches(self) -> int:
         """Performance case only"""
         with concurrent.futures.ProcessPoolExecutor(mp_context=mp.get_context('spawn'), max_workers=1) as executor:
             future = executor.submit(self.insert_data)
             count = future.result()
             return count
@@ -66,15 +110,15 @@
         """run forever util DB raises exception or crash"""
         start_time = time.perf_counter()
         max_load_count, times = 0, 0
         try:
             with self.db.init():
                 self.db.ready_to_load()
             while time.perf_counter() - start_time < config.CASE_TIMEOUT_IN_SECOND:
-                count = self.insert_data(left_id=max_load_count)
+                count = self.endless_insert_data(left_id=max_load_count)
                 max_load_count += count
                 times += 1
                 log.info(f"Loaded {times} entire dataset, current max load counts={utils.numerize(max_load_count)}, {max_load_count}")
             raise LoadTimeoutError("capacity case load timeout and stop")
         except LoadTimeoutError as e:
             log.info("load timetout, stop the load case")
             raise e from None
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/task_runner.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/task_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/backend/utils.py` & `vectordb-bench-0.0.2/vectordb_bench/backend/utils.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/charts.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/charts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,23 @@
+from vectordb_bench.backend.cases import Case
+from vectordb_bench.frontend.components.check_results.expanderStyle import initMainExpanderStyle
 from vectordb_bench.metric import metricOrder, isLowerIsBetterMetric, metricUnitMap
-from vectordb_bench.frontend.const import *
+from vectordb_bench.frontend.const.styles import *
 from vectordb_bench.models import ResultLabel
 import plotly.express as px
 
 
-def drawCharts(st, allData, failedTasks, cases):
-    st.markdown(
-        "<style> .main .streamlit-expanderHeader p {font-size: 20px; font-weight: 600;} </style>",
-        unsafe_allow_html=True,
-    )
-    st.markdown(
-        """<style>
-            .main div[data-testid='stExpander'] {
-                background-color: #F6F8FA;
-                border: 1px solid #A9BDD140;
-                border-radius: 8px;
-            }
-        </style>""",
-        unsafe_allow_html=True,
-    )
+def drawCharts(st, allData, failedTasks, cases: list[Case]):
+    initMainExpanderStyle(st)
     for case in cases:
-        chartContainer = st.expander(case, True)
-        data = [data for data in allData if data["case"] == case]
+        chartContainer = st.expander(case.name, True)
+        data = [data for data in allData if data["case_name"] == case.name]
         drawChart(data, chartContainer)
 
-        errorDBs = failedTasks[case]
+        errorDBs = failedTasks[case.name]
         showFailedDBs(chartContainer, errorDBs)
 
 
 def showFailedDBs(st, errorDBs):
     failedDBs = [db for db, label in errorDBs.items() if label == ResultLabel.FAILED]
     timeoutDBs = [
         db for db, label in errorDBs.items() if label == ResultLabel.OUTOFRANGE
@@ -98,15 +87,15 @@
     # )
     chart = st.container()
 
     height = len(dataWithMetric) * 24 + 48
     xmin = 0
     xmax = max([d.get(metric, 0) for d in dataWithMetric])
     xpadding = (xmax - xmin) / 16
-    xpadding_multiplier = 1.6
+    xpadding_multiplier = 1.8
     xrange = [xmin, xmax + xpadding * xpadding_multiplier]
     unit = metricUnitMap.get(metric, "")
     labelToShapeMap = getLabelToShapeMap(dataWithMetric)
     categoryorder = (
         "total descending" if isLowerIsBetterMetric(metric) else "total ascending"
     )
     fig = px.bar(
@@ -132,15 +121,15 @@
     fig.update_yaxes(
         # showticklabels=False,
         # visible=False,
         title=dict(
             font=dict(
                 size=1,
             ),
-            # text="",
+            text="",
         )
     )
     fig.update_traces(
         textposition="outside",
         textfont=dict(
             color="#333",
             size=12,
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/data.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,82 @@
 from collections import defaultdict
 from dataclasses import asdict
+from vectordb_bench.backend.cases import Case
 from vectordb_bench.metric import isLowerIsBetterMetric
-from vectordb_bench.models import ResultLabel
+from vectordb_bench.models import CaseResult, ResultLabel
 
 
-def getChartData(tasks, dbNames, cases):
+def getChartData(
+    tasks: list[CaseResult],
+    dbNames: list[str],
+    cases: list[Case],
+):
     filterTasks = getFilterTasks(tasks, dbNames, cases)
     mergedTasks, failedTasks = mergeTasks(filterTasks)
     return mergedTasks, failedTasks
 
 
-def getFilterTasks(tasks, dbNames, cases):
+def getFilterTasks(
+    tasks: list[CaseResult],
+    dbNames: list[str],
+    cases: list[Case],
+) -> list[CaseResult]:
+    case_ids = [case.case_id for case in cases]
     filterTasks = [
         task
         for task in tasks
         if task.task_config.db_name in dbNames
-        and task.task_config.case_config.case_id.value in cases
+        and task.task_config.case_config.case_id in case_ids
     ]
     return filterTasks
 
 
-def mergeTasks(tasks):
+def mergeTasks(tasks: list[CaseResult]):
     dbCaseMetricsMap = defaultdict(lambda: defaultdict(dict))
     for task in tasks:
         db_name = task.task_config.db_name
         db = task.task_config.db.value
         db_label = task.task_config.db_config.db_label or ""
-        case = task.task_config.case_config.case_id.value
-        dbCaseMetricsMap[db_name][case] = {
+        case_id = task.task_config.case_config.case_id
+        dbCaseMetricsMap[db_name][case_id] = {
             "db": db,
             "db_label": db_label,
             "metrics": mergeMetrics(
-                dbCaseMetricsMap[db_name][case].get("metrics", {}), asdict(task.metrics)
+                dbCaseMetricsMap[db_name][case_id].get("metrics", {}),
+                asdict(task.metrics),
+            ),
+            "label": getBetterLabel(
+                dbCaseMetricsMap[db_name][case_id].get("label", ResultLabel.FAILED),
+                task.label,
             ),
-            "label": getBetterLabel(dbCaseMetricsMap[db_name][case].get("label", ResultLabel.FAILED), task.label)
         }
 
     mergedTasks = []
     failedTasks = defaultdict(lambda: defaultdict(str))
     for db_name, caseMetricsMap in dbCaseMetricsMap.items():
-        for case, metricInfo in caseMetricsMap.items():
+        for case_id, metricInfo in caseMetricsMap.items():
             metrics = metricInfo["metrics"]
             db = metricInfo["db"]
             db_label = metricInfo["db_label"]
             label = metricInfo["label"]
+            case_name = case_id.case_name
             if label == ResultLabel.NORMAL:
                 mergedTasks.append(
                     {
                         "db_name": db_name,
                         "db": db,
                         "db_label": db_label,
-                        "case": case,
+                        "case_name": case_name,
                         "metricsSet": set(metrics.keys()),
                         **metrics,
                     }
                 )
-            else: 
-                failedTasks[case][db_name] = label
-                
+            else:
+                failedTasks[case_name][db_name] = label
+
     return mergedTasks, failedTasks
 
 
 def mergeMetrics(metrics_1: dict, metrics_2: dict) -> dict:
     metrics = {**metrics_1}
     for key, value in metrics_2.items():
         metrics[key] = (
@@ -77,10 +92,11 @@
     if value_2 < 1e-7:
         return value_1
     return (
         min(value_1, value_2)
         if isLowerIsBetterMetric(metric)
         else max(value_1, value_2)
     )
-    
+
+
 def getBetterLabel(label_1: ResultLabel, label_2: ResultLabel):
     return label_2 if label_1 != ResultLabel.NORMAL else label_1
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/nav.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/nav.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from streamlit_extras.switch_page_button import switch_page
 
 
 def NavToRunTest(st):
-    st.header("Run your test")
+    st.subheader("Run your test")
     st.write("You can set the configs and run your own test.")
     navClick = st.button("Run Your Test &nbsp;&nbsp;>")
     if navClick:
         switch_page("run test")
         
         
-def NavToQPSWithPrice(st):
-    navClick = st.button("QPS with Price &nbsp;&nbsp;>")
+def NavToQuriesPerDollar(st):
+    st.subheader("Compare qps with price.")
+    navClick = st.button("QP$ (Quries per Dollar) &nbsp;&nbsp;>")
     if navClick:
-        switch_page("qps with price")
+        switch_page("quries_per_dollar")
         
         
-def NavToResults(st):
-    navClick = st.button("< &nbsp;&nbsp;Back to Results")
+def NavToResults(st, key="nav-to-results"):
+    navClick = st.button("< &nbsp;&nbsp;Back to Results", key=key)
     if navClick:
         switch_page("vdb benchmark")
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/check_results/priceTable.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/check_results/priceTable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from vectordb_bench.backend.clients import DB
-from vectordb_bench.frontend.const import DB_DBLABEL_TO_PRICE
 import pandas as pd
 from collections import defaultdict
 import streamlit as st
 
+from vectordb_bench.frontend.const.dbPrices import DB_DBLABEL_TO_PRICE
+
 
 def priceTable(container, data):
     dbAndLabelSet = {
         (d["db"], d["db_label"]) for d in data if d["db"] != DB.Milvus.value
     }
 
     dbAndLabelList = list(dbAndLabelSet)
@@ -21,15 +22,15 @@
                 "Price per hour": DB_DBLABEL_TO_PRICE.get(db, {}).get(db_label, 0),
             }
             for db, db_label in dbAndLabelList
         ]
     )
     height = len(table) * 35 + 38
 
-    expander = container.expander("You can edit the price.")
+    expander = container.expander("Price List (Editable).")
     editTable = expander.data_editor(
         table,
         use_container_width=True,
         hide_index=True,
         height=height,
         disabled=("DB", "Label"),
         column_config={
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/caseSelector.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/caseSelector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-from vectordb_bench.frontend.const import *
+from vectordb_bench.frontend.const.styles import *
+from vectordb_bench.backend.cases import CaseType
+from vectordb_bench.frontend.const.dbCaseConfigs import *
 
 
 def caseSelector(st, activedDbList):
     st.markdown(
         "<div style='height: 24px;'></div>",
         unsafe_allow_html=True,
     )
     st.subheader("STEP 2: Choose the case(s)")
     st.markdown(
         "<div style='color: #647489; margin-bottom: 24px; margin-top: -12px;'>Choose at least one case you want to run the test for. </div>",
         unsafe_allow_html=True,
     )
 
-    caseIsActived = {case["name"]: False for case in CASE_LIST}
-    allCaseConfigs = {db: {case["name"]: {} for case in CASE_LIST} for db in DB_LIST}
-    for case in CASE_LIST:
-        caseItemContainer = st.container()
-        caseIsActived[case["name"]] = caseItem(
-            caseItemContainer, allCaseConfigs, case, activedDbList
-        )
-        if case.get("divider"):
+    caseIsActived = {case: False for case in CASE_LIST}
+    allCaseConfigs = {db: {case: {} for case in CASE_LIST} for db in DB_LIST}
+    for caseOrDivider in CASE_LIST_WITH_DIVIDER:
+        if caseOrDivider == DIVIDER:
             caseItemContainer.markdown(
                 "<div style='border: 1px solid #cccccc60; margin-bottom: 24px;'></div>",
                 unsafe_allow_html=True,
             )
-    activedCaseList = [
-        case["name"] for case in CASE_LIST if caseIsActived[case["name"]]
-    ]
+        else:
+            case = caseOrDivider
+            caseItemContainer = st.container()
+            caseIsActived[case] = caseItem(
+                caseItemContainer, allCaseConfigs, case, activedDbList
+            )
+    activedCaseList = [case for case in CASE_LIST if caseIsActived[case]]
     return activedCaseList, allCaseConfigs
 
-def caseItem(st, allCaseConfigs, case, activedDbList):
-    selected = st.checkbox(case["name"].value)
+
+def caseItem(st, allCaseConfigs, case: CaseType, activedDbList):
+    selected = st.checkbox(case.case_name)
     st.markdown(
-        f"<div style='color: #1D2939; margin: -8px 0 20px {CHECKBOX_INDENT}px; font-size: 14px;'>{case['intro']}</div>",
+        f"<div style='color: #1D2939; margin: -8px 0 20px {CHECKBOX_INDENT}px; font-size: 14px;'>{case.case_description}</div>",
         unsafe_allow_html=True,
     )
 
     if selected:
         caseConfigSettingContainer = st.container()
         caseConfigSetting(
-            caseConfigSettingContainer, allCaseConfigs, case["name"], activedDbList
+            caseConfigSettingContainer, allCaseConfigs, case, activedDbList
         )
 
     return selected
 
 
 def caseConfigSetting(st, allCaseConfigs, case, activedDbList):
     for db in activedDbList:
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/dbConfigSetting.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbConfigSetting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-from vectordb_bench.frontend.const import *
+from pydantic import ValidationError
+from vectordb_bench.frontend.const.styles import *
 from vectordb_bench.frontend.utils import inputIsPassword
 
 
 def dbConfigSettings(st, activedDbList):
     st.markdown(
         "<style> .streamlit-expanderHeader p {font-size: 20px; font-weight: 600;}</style>",
         unsafe_allow_html=True,
     )
     expander = st.expander("Configurations for the selected databases", True)
 
     dbConfigs = {}
+    isAllValid = True
     for activeDb in activedDbList:
         dbConfigSettingItemContainer = expander.container()
         dbConfig = dbConfigSettingItem(dbConfigSettingItemContainer, activeDb)
-        dbConfigs[activeDb] = dbConfig
-        
-    return dbConfigs
+        try:
+            dbConfigs[activeDb] = activeDb.init_cls.config_cls()(**dbConfig)
+        except ValidationError as e:
+            isAllValid = False
+            errTexts = []
+            for err in e.raw_errors:
+                errLocs = err.loc_tuple()
+                errInfo = err.exc
+                errText = f"{', '.join(errLocs)} - {errInfo}"
+                errTexts.append(errText)
+
+            dbConfigSettingItemContainer.error(f"{'; '.join(errTexts)}")
+
+    return dbConfigs, isAllValid
+
 
 def dbConfigSettingItem(st, activeDb):
     st.markdown(
         f"<div style='font-weight: 600; font-size: 20px; margin-top: 16px;'>{activeDb.value}</div>",
         unsafe_allow_html=True,
     )
     columns = st.columns(DB_CONFIG_SETTING_COLUMNS)
@@ -35,13 +49,12 @@
         key, value = property
         dbConfig[key] = column.text_input(
             key,
             key="%s-%s" % (activeDb, key),
             value=value.get("default", ""),
             type="password" if inputIsPassword(key) else "default",
         )
-    return dbConfigClass(**dbConfig)
+    return dbConfig
 
 
 def moveDBLabelToLast(propertiesItems):
-    propertiesItems.sort(key=lambda x: 1 if x[0] == 'db_label' else 0)
-    
+    propertiesItems.sort(key=lambda x: 1 if x[0] == "db_label" else 0)
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/dbSelector.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/dbSelector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-
-from vectordb_bench.frontend.const import *
+from vectordb_bench.frontend.const.styles import *
+from vectordb_bench.frontend.const.dbCaseConfigs import DB_LIST
 
 
 def dbSelector(st):
     st.markdown(
         "<div style='height: 12px;'></div>",
         unsafe_allow_html=True,
     )
     st.subheader("STEP 1: Select the database(s)")
     st.markdown(
         "<div style='color: #647489; margin-bottom: 24px; margin-top: -12px;'>Choose at least one case you want to run the test for. </div>",
         unsafe_allow_html=True,
     )
-    
+
     dbContainerColumns = st.columns(DB_SELECTOR_COLUMNS, gap="small")
     dbIsActived = {db: False for db in DB_LIST}
-    
+
     # style - image; column gap; checkbox font;
     st.markdown(
         """
         <style>
             div[data-testid='stImage'] {margin: auto;}
             div[data-testid='stHorizontalBlock'] {gap: 8px;}
             .stCheckbox p { color: #000; font-size: 18px; font-weight: 600; }
@@ -28,9 +28,9 @@
         unsafe_allow_html=True,
     )
     for i, db in enumerate(DB_LIST):
         column = dbContainerColumns[i % DB_SELECTOR_COLUMNS]
         dbIsActived[db] = column.checkbox(db.name)
         column.image(DB_TO_ICON.get(db, ""))
     activedDbList = [db for db in DB_LIST if dbIsActived[db]]
-    
+
     return activedDbList
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/generateTasks.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/generateTasks.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/components/run_test/submitTask.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/components/run_test/submitTask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,75 @@
 from datetime import datetime
-from vectordb_bench.frontend.const import *
+from vectordb_bench.frontend.const.styles import *
 from vectordb_bench.interface import benchMarkRunner
 
 
-def submitTask(st, tasks):
+def submitTask(st, tasks, isAllValid):
     st.markdown(
         "<div style='height: 24px;'></div>",
         unsafe_allow_html=True,
     )
     st.subheader("STEP 3: Task Label")
     st.markdown(
         "<div style='color: #647489; margin-bottom: 20px; margin-top: -12px;'>This description is used to mark the result. </div>",
         unsafe_allow_html=True,
     )
 
     taskLabel = taskLabelInput(st)
-    
+
     st.markdown(
         "<div style='height: 24px;'></div>",
         unsafe_allow_html=True,
     )
 
     controlPanelContainer = st.container()
-    controlPanel(controlPanelContainer, tasks, taskLabel)
+    controlPanel(controlPanelContainer, tasks, taskLabel, isAllValid)
 
 
 def taskLabelInput(st):
     defaultTaskLabel = datetime.now().strftime("%Y%m%d%H")
     columns = st.columns(TASK_LABEL_INPUT_COLUMNS)
-    taskLabel = columns[0].text_input("task_label", defaultTaskLabel, label_visibility="collapsed")
+    taskLabel = columns[0].text_input(
+        "task_label", defaultTaskLabel, label_visibility="collapsed"
+    )
     return taskLabel
 
 
-def controlPanel(st, tasks, taskLabel):
+def controlPanel(st, tasks, taskLabel, isAllValid):
     isRunning = benchMarkRunner.has_running()
     runHandler = lambda: benchMarkRunner.run(tasks, taskLabel)
     stopHandler = lambda: benchMarkRunner.stop_running()
-    
+
     if isRunning:
         currentTaskId = benchMarkRunner.get_current_task_id()
         tasksCount = benchMarkRunner.get_tasks_count()
         text = f":running: Running Task {currentTaskId} / {tasksCount}"
         st.progress(currentTaskId / tasksCount, text=text)
-        
+
         columns = st.columns(6)
         columns[0].button(
             "Run Your Test",
             disabled=True,
             on_click=runHandler,
             type="primary",
         )
         columns[1].button(
             "Stop",
             on_click=stopHandler,
             type="primary",
         )
-        
+
     else:
         errorText = benchMarkRunner.latest_error or ""
         if len(errorText) > 0:
             st.error(errorText)
-        disabled = True if len(tasks) == 0 else False
+        disabled = True if len(tasks) == 0 or not isAllValid else False
+        if not isAllValid:
+            st.error("Make sure all config is valid.")
+        elif len(tasks) == 0:
+            st.warning("No tests to run.")
         st.button(
             "Run Your Test",
             disabled=disabled,
             on_click=runHandler,
             type="primary",
         )
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/pages/qps_with_price.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/pages/quries_per_dollar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 import streamlit as st
+from vectordb_bench.frontend.components.check_results.footer import footer
+from vectordb_bench.frontend.components.check_results.expanderStyle import initMainExpanderStyle
 from vectordb_bench.frontend.components.check_results.priceTable import priceTable
-from vectordb_bench.frontend.const import *
+from vectordb_bench.frontend.components.check_results.stPageConfig import initResultsPageConfig
 from vectordb_bench.frontend.components.check_results.headerIcon import drawHeaderIcon
 from vectordb_bench.frontend.components.check_results.nav import NavToResults, NavToRunTest
 from vectordb_bench.frontend.components.check_results.charts import drawMetricChart
 from vectordb_bench.frontend.components.check_results.filters import getshownData
+from vectordb_bench.frontend.components.get_results.saveAsImage import getResults
+from vectordb_bench.frontend.const.styles import *
 from vectordb_bench.interface import benchMarkRunner
+from vectordb_bench.metric import QURIES_PER_DOLLAR_METRIC
 
 
 def main():
-    st.set_page_config(
-        page_title="VectorDB Benchmark",
-        page_icon="https://assets.zilliz.com/favicon_f7f922fe27.png",
-        # layout="wide",
-        # initial_sidebar_state="collapsed",
-    )
-
+    # set page config
+    initResultsPageConfig(st)
+    
     # header
     drawHeaderIcon(st)
 
     allResults = benchMarkRunner.get_results()
 
-    st.title("Vector DB Benchmark (QPS / Price)")
-    st.subheader("Price List")
+    st.title("Vector DB Benchmark (QP$)")
 
     # results selector
     resultSelectorContainer = st.sidebar.container()
-    shownData, failedTasks, showCases = getshownData(allResults, resultSelectorContainer)
+    shownData, _, showCases = getshownData(allResults, resultSelectorContainer)
 
     resultSelectorContainer.divider()
 
     # nav
     navContainer = st.sidebar.container()
     NavToRunTest(navContainer)
     NavToResults(navContainer)
-    
+
+    # save or share
+    resultesContainer = st.sidebar.container()
+    getResults(resultesContainer, "vectordb_bench_qp$")
+
     # price table
+    initMainExpanderStyle(st)
     priceTableContainer = st.container()
     priceMap = priceTable(priceTableContainer, shownData)
 
     # charts
     for case in showCases:
-        chartContainer = st.container()
-        data = [data for data in shownData if data["case"] == case]
+        data = [data for data in shownData if data["case_name"] == case.name]
         dataWithMetric = []
-        metric = "qps_per_dollar (qps / price)"
+        metric = QURIES_PER_DOLLAR_METRIC
         for d in data:
             qps = d.get("qps", 0)
             price = priceMap.get(d["db"], {}).get(d["db_label"], 0)
             if qps > 0 and price > 0:
-                d[metric] = d["qps"] / price
+                d[metric] = d["qps"] / price * 3.6
                 dataWithMetric.append(d)
         if len(dataWithMetric) > 0:
-            chartContainer.subheader(case)
+            chartContainer = st.expander(case.name, True)
             drawMetricChart(data, metric, chartContainer)
 
+    # footer
+    footer(st.container())
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/pages/run_test.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/pages/run_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import streamlit as st
 from vectordb_bench.frontend.components.run_test.autoRefresh import autoRefresh
 from vectordb_bench.frontend.components.run_test.caseSelector import caseSelector
 from vectordb_bench.frontend.components.run_test.dbConfigSetting import dbConfigSettings
 from vectordb_bench.frontend.components.run_test.dbSelector import dbSelector
 from vectordb_bench.frontend.components.run_test.generateTasks import generate_tasks
-from vectordb_bench.frontend.components.check_results.headerIcon import drawHeaderIcon
 from vectordb_bench.frontend.components.run_test.hideSidebar import hideSidebar
-from vectordb_bench.frontend.components.check_results.nav import NavToResults
 from vectordb_bench.frontend.components.run_test.submitTask import submitTask
+from vectordb_bench.frontend.components.check_results.nav import NavToResults
+from vectordb_bench.frontend.components.check_results.headerIcon import drawHeaderIcon
+from vectordb_bench.frontend.components.check_results.stPageConfig import initRunTestPageConfig
 
 
 def main():
-    st.set_page_config(
-        page_title="VectorDB Benchmark",
-        page_icon="https://assets.zilliz.com/favicon_f7f922fe27.png",
-        # layout="wide",
-        initial_sidebar_state="collapsed",
-    )
+    # set page config
+    initRunTestPageConfig(st)
+    
     # header
     drawHeaderIcon(st)
 
     # hide sidebar
     hideSidebar(st)
 
     # nav to results
@@ -32,28 +30,36 @@
 
     # select db
     dbSelectorContainer = st.container()
     activedDbList = dbSelector(dbSelectorContainer)
 
     # db config setting
     dbConfigs = {}
+    isAllValid = True
     if len(activedDbList) > 0:
         dbConfigContainer = st.container()
-        dbConfigs = dbConfigSettings(dbConfigContainer, activedDbList)
+        dbConfigs, isAllValid = dbConfigSettings(dbConfigContainer, activedDbList)
 
     # select case and set db_case_config
     caseSelectorContainer = st.container()
     activedCaseList, allCaseConfigs = caseSelector(caseSelectorContainer, activedDbList)
 
     # generate tasks
-    tasks = generate_tasks(activedDbList, dbConfigs, activedCaseList, allCaseConfigs)
+    tasks = (
+        generate_tasks(activedDbList, dbConfigs, activedCaseList, allCaseConfigs)
+        if isAllValid
+        else []
+    )
 
     # submit
     submitContainer = st.container()
-    submitTask(submitContainer, tasks)
+    submitTask(submitContainer, tasks, isAllValid)
+
+    # nav to results
+    NavToResults(st, key="footer-nav-to-results")
 
     # autofresh
     autoRefresh()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/frontend/vdb_benchmark.py` & `vectordb-bench-0.0.2/vectordb_bench/frontend/vdb_benchmark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 import streamlit as st
-from vectordb_bench.frontend.const import *
+from vectordb_bench.frontend.components.check_results.footer import footer
+from vectordb_bench.frontend.components.check_results.stPageConfig import initResultsPageConfig
 from vectordb_bench.frontend.components.check_results.headerIcon import drawHeaderIcon
-from vectordb_bench.frontend.components.check_results.nav import NavToQPSWithPrice, NavToRunTest
+from vectordb_bench.frontend.components.check_results.nav import NavToQuriesPerDollar, NavToRunTest
 from vectordb_bench.frontend.components.check_results.charts import drawCharts
 from vectordb_bench.frontend.components.check_results.filters import getshownData
+from vectordb_bench.frontend.components.get_results.saveAsImage import getResults
+from vectordb_bench.frontend.const.styles import *
 from vectordb_bench.interface import benchMarkRunner
 
 
 def main():
-    st.set_page_config(
-        page_title="VectorDB Benchmark",
-        page_icon="https://assets.zilliz.com/favicon_f7f922fe27.png",
-        # layout="wide",
-        # initial_sidebar_state="collapsed",
-    )
+    # set page config
+    initResultsPageConfig(st)
 
     # header
     drawHeaderIcon(st)
 
     allResults = benchMarkRunner.get_results()
 
     st.title("Vector Database Benchmark")
-    # st.write("description [todo]")
 
-    # results selector
+    # results selector and filter
     resultSelectorContainer = st.sidebar.container()
-    shownData, failedTasks, showCases = getshownData(allResults, resultSelectorContainer)
+    shownData, failedTasks, showCases = getshownData(
+        allResults, resultSelectorContainer
+    )
 
     resultSelectorContainer.divider()
 
     # nav
     navContainer = st.sidebar.container()
     NavToRunTest(navContainer)
-    NavToQPSWithPrice(navContainer)
+    NavToQuriesPerDollar(navContainer)
+
+    # save or share
+    resultesContainer = st.sidebar.container()
+    getResults(resultesContainer, "vectordb_bench")
 
     # charts
     drawCharts(st, shownData, failedTasks, showCases)
 
+    # footer
+    footer(st.container())
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/interface.py` & `vectordb-bench-0.0.2/vectordb_bench/interface.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/log_util.py` & `vectordb-bench-0.0.2/vectordb_bench/log_util.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.1/vectordb_bench/models.py` & `vectordb-bench-0.0.2/vectordb_bench/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .backend.clients import (
     DB,
     DBConfig,
     DBCaseConfig,
     IndexType,
 )
+from .backend.cases import CaseType
 from .base import BaseModel
 from . import config
 from .metric import Metric
 
 
 log = logging.getLogger(__name__)
 
@@ -23,46 +24,14 @@
 class LoadTimeoutError(TimeoutError):
     pass
 
 class PerformanceTimeoutError(TimeoutError):
     pass
 
 
-class CaseType(Enum):
-    """
-    Value will be displayed in UI
-    """
-
-    CapacitySDim = "Capacity Test (Large-dim)"
-    CapacityLDim = "Capacity Test (Small-dim)"
-
-    Performance100M = "Search Performance Test (XLarge Dataset)"
-    PerformanceLZero = "Search Performance Test (Large Dataset)"
-    PerformanceMZero = "Search Performance Test (Medium Dataset)"
-    PerformanceSZero = "Search Performance Test (Small Dataset)"
-
-    PerformanceLLow = (
-        "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)"
-    )
-    PerformanceMLow = (
-        "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)"
-    )
-    PerformanceSLow = (
-        "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)"
-    )
-    PerformanceLHigh = (
-        "Filtering Search Performance Test (Large Dataset, High Filtering Rate)"
-    )
-    PerformanceMHigh = (
-        "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)"
-    )
-    PerformanceSHigh = (
-        "Filtering Search Performance Test (Small Dataset, High Filtering Rate)"
-    )
-
 
 class CaseConfigParamType(Enum):
     """
     Value will be the key of CaseConfig.params and displayed in UI
     """
 
     IndexType = "IndexType"
@@ -147,14 +116,15 @@
             if "task_label" not in test_result:
                 test_result["task_label"] = test_result["run_id"]
 
             for case_result in test_result["results"]:
                 task_config = case_result.get("task_config")
                 db = DB(task_config.get("db"))
                 dbcls = db.init_cls
+
                 task_config["db_config"] = dbcls.config_cls()(
                     **task_config["db_config"]
                 )
                 task_config["db_case_config"] = dbcls.case_config_cls(
                     index_type=task_config["db_case_config"].get("index", None),
                 )(**task_config["db_case_config"])
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench/results/result_20230609_standard.json` & `vectordb-bench-0.0.2/vectordb_bench/results/result_20230609_standard.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9524250922688423%*

 * *Differences: {"'results'": "{0: {'task_config': {'case_config': {'case_id': 2}}}, 1: {'task_config': "*

 * *              "{'case_config': {'case_id': 1}}}, 2: {'task_config': {'case_config': {'case_id': "*

 * *              "5}}}, 3: {'task_config': {'case_config': {'case_id': 7}}}, 4: {'task_config': "*

 * *              "{'case_config': {'case_id': 9}}}, 5: {'task_config': {'case_config': {'case_id': "*

 * *              "4}}}, 6: {'task_config': {'case_config': {'case_id': 6}}}, 7: {'task_config': "*

 * *              "{'case_config': {'cas […]*

```diff
@@ -7,15 +7,15 @@
                 "max_load_count": 3200000,
                 "qps": 0.0,
                 "recall": 0.0,
                 "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Large-dim)",
+                    "case_id": 2,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -37,15 +37,15 @@
                 "max_load_count": 8600000,
                 "qps": 0.0,
                 "recall": 0.0,
                 "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Small-dim)",
+                    "case_id": 1,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -59,113 +59,23 @@
                     "password": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2434.5387,
-                "max_load_count": 0,
-                "qps": 34.3911,
-                "recall": 0.9923,
-                "serial_latency_p99": 0.1734
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
-                    "custom_case": {}
-                },
-                "db": "ElasticCloud",
-                "db_case_config": {
-                    "M": 30,
-                    "efConstruction": 360,
-                    "element_type": "float",
-                    "index": "hnsw",
-                    "metric_type": "COSINE",
-                    "num_candidates": 100
-                },
-                "db_config": {
-                    "cloud_id": "**********",
-                    "db_label": "upTo2.5c8g",
-                    "password": "**********"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
-                "load_duration": 2434.5387,
-                "max_load_count": 0,
-                "qps": 31.5927,
-                "recall": 0.9924,
-                "serial_latency_p99": 0.1646
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
-                    "custom_case": {}
-                },
-                "db": "ElasticCloud",
-                "db_case_config": {
-                    "M": 30,
-                    "efConstruction": 360,
-                    "element_type": "float",
-                    "index": "hnsw",
-                    "metric_type": "COSINE",
-                    "num_candidates": 100
-                },
-                "db_config": {
-                    "cloud_id": "**********",
-                    "db_label": "upTo2.5c8g",
-                    "password": "**********"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
-                "load_duration": 2434.5387,
-                "max_load_count": 0,
-                "qps": 42.3405,
-                "recall": 0.9992,
-                "serial_latency_p99": 0.1383
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
-                    "custom_case": {}
-                },
-                "db": "ElasticCloud",
-                "db_case_config": {
-                    "M": 30,
-                    "efConstruction": 360,
-                    "element_type": "float",
-                    "index": "hnsw",
-                    "metric_type": "COSINE",
-                    "num_candidates": 100
-                },
-                "db_config": {
-                    "cloud_id": "**********",
-                    "db_label": "upTo2.5c8g",
-                    "password": "**********"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
                 "load_duration": 26412.1028,
                 "max_load_count": 0,
                 "qps": 15.2269,
                 "recall": 0.9888,
                 "serial_latency_p99": 0.8618
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -187,15 +97,15 @@
                 "max_load_count": 0,
                 "qps": 15.1749,
                 "recall": 0.989,
                 "serial_latency_p99": 0.7743
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -217,15 +127,15 @@
                 "max_load_count": 0,
                 "qps": 27.6181,
                 "recall": 0.9999,
                 "serial_latency_p99": 0.3055
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -247,15 +157,15 @@
                 "max_load_count": 0,
                 "qps": 0.0,
                 "recall": 0.0,
                 "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -277,15 +187,15 @@
                 "max_load_count": 0,
                 "qps": 0.0,
                 "recall": 0.0,
                 "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -307,15 +217,15 @@
                 "max_load_count": 0,
                 "qps": 0.0,
                 "recall": 0.0,
                 "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "ElasticCloud",
                 "db_case_config": {
                     "M": 30,
                     "efConstruction": 360,
                     "element_type": "float",
@@ -337,15 +247,15 @@
                 "max_load_count": 0,
                 "qps": 89.4473,
                 "recall": 0.9875,
                 "serial_latency_p99": 0.0219
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "index": "DISKANN",
                     "metric_type": "COSINE",
                     "search_list": 100
@@ -363,15 +273,15 @@
                 "max_load_count": 0,
                 "qps": 87.8616,
                 "recall": 0.9871,
                 "serial_latency_p99": 0.0215
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "index": "DISKANN",
                     "metric_type": "COSINE",
                     "search_list": 100
@@ -389,15 +299,15 @@
                 "max_load_count": 0,
                 "qps": 62.5257,
                 "recall": 1,
                 "serial_latency_p99": 0.0261
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "index": "DISKANN",
                     "metric_type": "COSINE",
                     "search_list": 100
@@ -405,265 +315,265 @@
                 "db_config": {
                     "db_label": "2c8g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 29829.7671,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 48.3866,
-                "recall": 0.9909,
-                "serial_latency_p99": 0.0443
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "index": "DISKANN",
                     "metric_type": "COSINE",
                     "search_list": 100
                 },
                 "db_config": {
-                    "db_label": "4c16g-disk",
+                    "db_label": "2c8g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 29829.7671,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 48.8021,
-                "recall": 0.9909,
-                "serial_latency_p99": 0.0347
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "index": "DISKANN",
                     "metric_type": "COSINE",
                     "search_list": 100
                 },
                 "db_config": {
-                    "db_label": "4c16g-disk",
+                    "db_label": "2c8g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 29829.7671,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 30.5848,
-                "recall": 1,
-                "serial_latency_p99": 0.0473
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "index": "DISKANN",
                     "metric_type": "COSINE",
                     "search_list": 100
                 },
                 "db_config": {
-                    "db_label": "4c16g-disk",
+                    "db_label": "2c8g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1455.573,
+                "load_duration": 29829.7671,
                 "max_load_count": 0,
-                "qps": 290.695,
-                "recall": 0.9801,
-                "serial_latency_p99": 0.0075
+                "qps": 48.3866,
+                "recall": 0.9909,
+                "serial_latency_p99": 0.0443
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "index": "DISKANN",
+                    "metric_type": "COSINE",
+                    "search_list": 100
                 },
                 "db_config": {
                     "db_label": "4c16g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1455.573,
+                "load_duration": 29829.7671,
                 "max_load_count": 0,
-                "qps": 284.9882,
-                "recall": 0.9803,
-                "serial_latency_p99": 0.0087
+                "qps": 48.8021,
+                "recall": 0.9909,
+                "serial_latency_p99": 0.0347
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "index": "DISKANN",
+                    "metric_type": "COSINE",
+                    "search_list": 100
                 },
                 "db_config": {
                     "db_label": "4c16g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 1455.573,
+                "load_duration": 29829.7671,
                 "max_load_count": 0,
-                "qps": 390.2579,
+                "qps": 30.5848,
                 "recall": 1,
-                "serial_latency_p99": 0.0073
+                "serial_latency_p99": 0.0473
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "index": "DISKANN",
+                    "metric_type": "COSINE",
+                    "search_list": 100
                 },
                 "db_config": {
                     "db_label": "4c16g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 398.5015,
+                "load_duration": 1455.573,
                 "max_load_count": 0,
-                "qps": 523.0791,
-                "recall": 0.9513,
-                "serial_latency_p99": 0.0063
+                "qps": 290.695,
+                "recall": 0.9801,
+                "serial_latency_p99": 0.0075
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
-                    "index": "DISKANN",
-                    "metric_type": "COSINE",
-                    "search_list": 100
+                    "M": 30,
+                    "ef": 100,
+                    "efConstruction": 360,
+                    "index": "HNSW",
+                    "metric_type": "COSINE"
                 },
                 "db_config": {
                     "db_label": "4c16g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 398.5015,
+                "load_duration": 1455.573,
                 "max_load_count": 0,
-                "qps": 487.4188,
-                "recall": 0.9503,
-                "serial_latency_p99": 0.0067
+                "qps": 284.9882,
+                "recall": 0.9803,
+                "serial_latency_p99": 0.0087
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
-                    "index": "DISKANN",
-                    "metric_type": "COSINE",
-                    "search_list": 100
+                    "M": 30,
+                    "ef": 100,
+                    "efConstruction": 360,
+                    "index": "HNSW",
+                    "metric_type": "COSINE"
                 },
                 "db_config": {
                     "db_label": "4c16g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 398.5015,
+                "load_duration": 1455.573,
                 "max_load_count": 0,
-                "qps": 473.241,
+                "qps": 390.2579,
                 "recall": 1,
-                "serial_latency_p99": 0.0045
+                "serial_latency_p99": 0.0073
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
-                    "index": "DISKANN",
-                    "metric_type": "COSINE",
-                    "search_list": 100
+                    "M": 30,
+                    "ef": 100,
+                    "efConstruction": 360,
+                    "index": "HNSW",
+                    "metric_type": "COSINE"
                 },
                 "db_config": {
                     "db_label": "4c16g-disk",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
                 "load_duration": 0,
-                "max_load_count": 4300000,
+                "max_load_count": 6700000,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Large-dim)",
+                    "case_id": 2,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "L2"
                 },
@@ -682,15 +592,15 @@
                 "max_load_count": 12700000,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Small-dim)",
+                    "case_id": 1,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "L2"
                 },
@@ -701,104 +611,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 752.1779,
-                "max_load_count": 0,
-                "qps": 228.6015,
-                "recall": 0.9491,
-                "serial_latency_p99": 0.0118
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
-                    "custom_case": {}
-                },
-                "db": "ZillizCloud",
-                "db_case_config": {
-                    "index": "AUTOINDEX",
-                    "metric_type": "COSINE"
-                },
-                "db_config": {
-                    "db_label": "1cu-cap",
-                    "password": "**********",
-                    "uri": "**********",
-                    "user": "root"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
-                "load_duration": 752.1779,
-                "max_load_count": 0,
-                "qps": 215.5243,
-                "recall": 0.9486,
-                "serial_latency_p99": 0.011
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
-                    "custom_case": {}
-                },
-                "db": "ZillizCloud",
-                "db_case_config": {
-                    "index": "AUTOINDEX",
-                    "metric_type": "COSINE"
-                },
-                "db_config": {
-                    "db_label": "1cu-cap",
-                    "password": "**********",
-                    "uri": "**********",
-                    "user": "root"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
-                "load_duration": 752.1779,
-                "max_load_count": 0,
-                "qps": 245.1032,
-                "recall": 1,
-                "serial_latency_p99": 0.0095
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
-                    "custom_case": {}
-                },
-                "db": "ZillizCloud",
-                "db_case_config": {
-                    "index": "AUTOINDEX",
-                    "metric_type": "COSINE"
-                },
-                "db_config": {
-                    "db_label": "1cu-cap",
-                    "password": "**********",
-                    "uri": "**********",
-                    "user": "root"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
                 "load_duration": 3478.7882,
                 "max_load_count": 0,
                 "qps": 164.3866,
                 "recall": 0.95,
                 "serial_latency_p99": 0.0131
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -817,15 +646,15 @@
                 "max_load_count": 0,
                 "qps": 139.0901,
                 "recall": 0.9669,
                 "serial_latency_p99": 0.0172
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -844,15 +673,15 @@
                 "max_load_count": 0,
                 "qps": 115.3193,
                 "recall": 1,
                 "serial_latency_p99": 0.0157
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -861,184 +690,106 @@
                     "password": "**********",
                     "uri": "**********",
                     "user": "root"
                 }
             }
         },
         {
-            "label": ":)",
-            "metrics": {
-                "load_duration": 752.1779,
-                "max_load_count": 0,
-                "qps": 233.6172,
-                "recall": 0.9494,
-                "serial_latency_p99": 0.011
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
-                    "custom_case": {}
-                },
-                "db": "Milvus",
-                "db_case_config": {
-                    "index": "DISKANN",
-                    "metric_type": "COSINE",
-                    "search_list": 100
-                },
-                "db_config": {
-                    "db_label": "2c8g-disk",
-                    "uri": "**********"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
-                "load_duration": 752.1779,
-                "max_load_count": 0,
-                "qps": 218.1513,
-                "recall": 0.9485,
-                "serial_latency_p99": 0.0104
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
-                    "custom_case": {}
-                },
-                "db": "Milvus",
-                "db_case_config": {
-                    "index": "DISKANN",
-                    "metric_type": "COSINE",
-                    "search_list": 100
-                },
-                "db_config": {
-                    "db_label": "2c8g-disk",
-                    "uri": "**********"
-                }
-            }
-        },
-        {
-            "label": ":)",
-            "metrics": {
-                "load_duration": 752.1779,
-                "max_load_count": 0,
-                "qps": 235.2801,
-                "recall": 1,
-                "serial_latency_p99": 0.009
-            },
-            "task_config": {
-                "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
-                    "custom_case": {}
-                },
-                "db": "Milvus",
-                "db_case_config": {
-                    "index": "DISKANN",
-                    "metric_type": "COSINE",
-                    "search_list": 100
-                },
-                "db_config": {
-                    "db_label": "2c8g-disk",
-                    "uri": "**********"
-                }
-            }
-        },
-        {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 427.2816,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 472.2174,
-                "recall": 0.9776,
-                "serial_latency_p99": 0.0084
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap",
+                    "db_label": "1cu-cap",
                     "password": "**********",
                     "uri": "**********",
                     "user": "root"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 427.2816,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 447.1405,
-                "recall": 0.9774,
-                "serial_latency_p99": 0.0071
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap",
+                    "db_label": "1cu-cap",
                     "password": "**********",
                     "uri": "**********",
                     "user": "root"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 427.2816,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 476.5357,
-                "recall": 1,
-                "serial_latency_p99": 0.0053
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap",
+                    "db_label": "1cu-cap",
                     "password": "**********",
                     "uri": "**********",
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 22201.8358,
+                "load_duration": 14485.1106,
                 "max_load_count": 0,
                 "qps": 100.23,
                 "recall": 0.972,
                 "serial_latency_p99": 0.0288
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1049,23 +800,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 22201.8358,
+                "load_duration": 14485.1106,
                 "max_load_count": 0,
                 "qps": 48.7675,
                 "recall": 0.9911,
                 "serial_latency_p99": 0.0352
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1076,23 +827,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 22201.8358,
+                "load_duration": 14485.1106,
                 "max_load_count": 0,
                 "qps": 30.5627,
                 "recall": 1,
                 "serial_latency_p99": 0.0471
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1111,15 +862,15 @@
                 "max_load_count": 0,
                 "qps": 352.1345,
                 "recall": 0.9213,
                 "serial_latency_p99": 0.0093
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1138,15 +889,15 @@
                 "max_load_count": 0,
                 "qps": 264.539,
                 "recall": 0.9684,
                 "serial_latency_p99": 0.0099
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1165,15 +916,15 @@
                 "max_load_count": 0,
                 "qps": 232.8041,
                 "recall": 1,
                 "serial_latency_p99": 0.0109
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1192,15 +943,15 @@
                 "max_load_count": 5800000,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Small-dim)",
+                    "case_id": 1,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1220,15 +971,15 @@
                 "max_load_count": 1800000,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Large-dim)",
+                    "case_id": 2,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1248,15 +999,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 4,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1276,15 +1027,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1304,15 +1055,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1332,15 +1083,15 @@
                 "max_load_count": 0,
                 "qps": 67.9121,
                 "recall": 0.9909,
                 "serial_latency_p99": 0.1795
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 5,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1360,15 +1111,15 @@
                 "max_load_count": 0,
                 "qps": 0.7636,
                 "recall": 0.9908,
                 "serial_latency_p99": 1.9213
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1388,15 +1139,15 @@
                 "max_load_count": 0,
                 "qps": 32,
                 "recall": 1.0,
                 "serial_latency_p99": 0.1245
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1408,107 +1159,107 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 251.0931,
-                "max_load_count": 0,
-                "qps": 101.6631,
-                "recall": 0.9977,
-                "serial_latency_p99": 0.03
+                "load_duration": 0,
+                "max_load_count": 1480000,
+                "qps": 0,
+                "recall": 0,
+                "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 1,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
                     "metric_type": "COSINE"
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "bus_crit",
+                    "db_label": "sandbox",
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 251.0931,
-                "max_load_count": 0,
-                "qps": 7.6,
-                "recall": 0.9977,
-                "serial_latency_p99": 0.583
+                "load_duration": 0,
+                "max_load_count": 455000,
+                "qps": 0,
+                "recall": 0,
+                "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 2,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
                     "metric_type": "COSINE"
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "bus_crit",
+                    "db_label": "sandbox",
                     "url": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 251.0931,
+                "load_duration": 0,
                 "max_load_count": 0,
-                "qps": 102,
-                "recall": 1.0,
-                "serial_latency_p99": 0.0292
+                "qps": 0,
+                "recall": 0,
+                "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 5,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
                     "metric_type": "COSINE"
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "bus_crit",
+                    "db_label": "sandbox",
                     "url": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
                 "load_duration": 0,
-                "max_load_count": 1480000,
+                "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Small-dim)",
+                    "case_id": 7,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1518,25 +1269,25 @@
                     "api_key": "**********",
                     "db_label": "sandbox",
                     "url": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
                 "load_duration": 0,
-                "max_load_count": 455000,
+                "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Large-dim)",
+                    "case_id": 9,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1556,15 +1307,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 4,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1584,15 +1335,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1612,15 +1363,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1632,51 +1383,51 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 283.6404,
-                "max_load_count": 0,
-                "qps": 113.661,
-                "recall": 0.9977,
-                "serial_latency_p99": 0.0489
+                "load_duration": 0,
+                "max_load_count": 5500000,
+                "qps": 0,
+                "recall": 0,
+                "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 1,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
                     "metric_type": "COSINE"
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "sandbox",
+                    "db_label": "standard",
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
                 "load_duration": 0,
-                "max_load_count": 5500000,
+                "max_load_count": 1800000,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Small-dim)",
+                    "case_id": 2,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1688,23 +1439,23 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 0,
-                "max_load_count": 1800000,
-                "qps": 0,
-                "recall": 0,
-                "serial_latency_p99": 0
+                "load_duration": 3580.7827,
+                "max_load_count": 0,
+                "qps": 63.1365,
+                "recall": 0.991,
+                "serial_latency_p99": 0.1457
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Large-dim)",
+                    "case_id": 5,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1716,58 +1467,58 @@
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 280.2736,
+                "load_duration": 3580.12,
                 "max_load_count": 0,
-                "qps": 73.0806,
-                "recall": 0.9977,
-                "serial_latency_p99": 0.0472
+                "qps": 0.7512,
+                "recall": 0.9908,
+                "serial_latency_p99": 1.9838
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
-                    "custom_case": null
+                    "case_id": 7,
+                    "custom_case": {}
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
-                    "efConstruction": null,
-                    "maxConnections": null,
+                    "efConstruction": 128,
+                    "maxConnections": 64,
                     "metric_type": "COSINE"
                 },
                 "db_config": {
                     "api_key": "**********",
                     "db_label": "standard",
                     "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 3580.7827,
+                "load_duration": 0,
                 "max_load_count": 0,
-                "qps": 63.1365,
-                "recall": 0.991,
-                "serial_latency_p99": 0.1457
+                "qps": 30.1358,
+                "recall": 1,
+                "serial_latency_p99": 0.1298
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
-                    "custom_case": null
+                    "case_id": 9,
+                    "custom_case": {}
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
-                    "efConstruction": null,
-                    "maxConnections": null,
+                    "efConstruction": 128,
+                    "maxConnections": 64,
                     "metric_type": "COSINE"
                 },
                 "db_config": {
                     "api_key": "**********",
                     "db_label": "standard",
                     "url": "**********"
                 }
@@ -1780,15 +1531,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 4,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1808,15 +1559,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1836,15 +1587,15 @@
                 "max_load_count": 0,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": null
                 },
                 "db": "WeaviateCloud",
                 "db_case_config": {
                     "ef": -1,
                     "efConstruction": null,
                     "maxConnections": null,
@@ -1864,15 +1615,15 @@
                 "max_load_count": 5000000,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Small-dim)",
+                    "case_id": 1,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1891,15 +1642,15 @@
                 "max_load_count": 1200000,
                 "qps": 0,
                 "recall": 0,
                 "serial_latency_p99": 0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Large-dim)",
+                    "case_id": 2,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1910,23 +1661,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2142.6913,
+                "load_duration": 1165.833,
                 "max_load_count": 0,
                 "qps": 457.3331,
                 "recall": 0.9473,
                 "serial_latency_p99": 0.0056
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1937,23 +1688,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2142.6913,
+                "load_duration": 1165.833,
                 "max_load_count": 0,
                 "qps": 308.5526,
                 "recall": 0.9805,
                 "serial_latency_p99": 0.0077
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1964,23 +1715,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2142.6913,
+                "load_duration": 1165.833,
                 "max_load_count": 0,
                 "qps": 408.1209,
                 "recall": 1,
                 "serial_latency_p99": 0.0057
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -1989,25 +1740,25 @@
                     "password": "**********",
                     "uri": "**********",
                     "user": "root"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 254.2501,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 1157.4606,
-                "recall": 0.958,
-                "serial_latency_p99": 0.0033
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2016,25 +1767,25 @@
                     "password": "**********",
                     "uri": "**********",
                     "user": "root"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 254.2501,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 1018.7988,
-                "recall": 0.958,
-                "serial_latency_p99": 0.0041
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2043,25 +1794,25 @@
                     "password": "**********",
                     "uri": "**********",
                     "user": "root"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 254.2501,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 1517.0827,
-                "recall": 1,
-                "serial_latency_p99": 0.0035
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2072,23 +1823,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2325.0144,
+                "load_duration": 1229.3664,
                 "max_load_count": 0,
                 "qps": 2867.9092,
                 "recall": 0.8769,
                 "serial_latency_p99": 0.0037
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2099,23 +1850,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2325.0144,
+                "load_duration": 1229.3664,
                 "max_load_count": 0,
                 "qps": 1689.5799,
                 "recall": 0.9486,
                 "serial_latency_p99": 0.0054
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2126,23 +1877,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2325.0144,
+                "load_duration": 1229.3664,
                 "max_load_count": 0,
                 "qps": 1371.0535,
                 "recall": 1,
                 "serial_latency_p99": 0.0079
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2153,23 +1904,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 221.5923,
+                "load_duration": 7772.641,
                 "max_load_count": 0,
-                "qps": 3676.5906,
-                "recall": 0.9567,
-                "serial_latency_p99": 0.0046
+                "qps": 723.9371,
+                "recall": 0.9285,
+                "serial_latency_p99": 0.0052
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2180,23 +1931,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 221.5923,
+                "load_duration": 7772.641,
                 "max_load_count": 0,
-                "qps": 3348.3574,
-                "recall": 0.957,
-                "serial_latency_p99": 0.0039
+                "qps": 315.5653,
+                "recall": 0.9757,
+                "serial_latency_p99": 0.0089
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2207,23 +1958,23 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 221.5923,
+                "load_duration": 7772.641,
                 "max_load_count": 0,
-                "qps": 5113.8498,
+                "qps": 147.6055,
                 "recall": 1,
-                "serial_latency_p99": 0.0041
+                "serial_latency_p99": 0.0132
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
@@ -2234,104 +1985,107 @@
                     "user": "root"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 15985.5509,
-                "max_load_count": 0,
-                "qps": 723.9371,
-                "recall": 0.9285,
-                "serial_latency_p99": 0.0052
+                "load_duration": 0.0,
+                "max_load_count": 9100000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 1,
                     "custom_case": {}
                 },
-                "db": "ZillizCloud",
+                "db": "Milvus",
                 "db_case_config": {
-                    "index": "AUTOINDEX",
+                    "M": 30,
+                    "ef": 100,
+                    "efConstruction": 360,
+                    "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf",
-                    "password": "**********",
-                    "uri": "**********",
-                    "user": "root"
+                    "db_label": "2c8g-hnsw",
+                    "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 15985.5509,
-                "max_load_count": 0,
-                "qps": 315.5653,
-                "recall": 0.9757,
-                "serial_latency_p99": 0.0089
+                "load_duration": 0.0,
+                "max_load_count": 1000000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 2,
                     "custom_case": {}
                 },
-                "db": "ZillizCloud",
+                "db": "Milvus",
                 "db_case_config": {
-                    "index": "AUTOINDEX",
+                    "M": 30,
+                    "ef": 100,
+                    "efConstruction": 360,
+                    "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf",
-                    "password": "**********",
-                    "uri": "**********",
-                    "user": "root"
+                    "db_label": "2c8g-hnsw",
+                    "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 15985.5509,
+                "load_duration": 2379.7118,
                 "max_load_count": 0,
-                "qps": 147.6055,
-                "recall": 1,
-                "serial_latency_p99": 0.0132
+                "qps": 274.5407,
+                "recall": 0.9807,
+                "serial_latency_p99": 0.0049
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
-                "db": "ZillizCloud",
+                "db": "Milvus",
                 "db_case_config": {
-                    "index": "AUTOINDEX",
+                    "M": 30,
+                    "ef": 100,
+                    "efConstruction": 360,
+                    "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf",
-                    "password": "**********",
-                    "uri": "**********",
-                    "user": "root"
+                    "db_label": "2c8g-hnsw",
+                    "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 0.0,
-                "max_load_count": 9100000,
-                "qps": 0.0,
-                "recall": 0.0,
-                "serial_latency_p99": 0.0
+                "load_duration": 2379.7118,
+                "max_load_count": 0,
+                "qps": 236.5672,
+                "recall": 0.981,
+                "serial_latency_p99": 0.0103
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Small-dim)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
@@ -2343,23 +2097,23 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 0.0,
-                "max_load_count": 1000000,
-                "qps": 0.0,
-                "recall": 0.0,
-                "serial_latency_p99": 0.0
+                "load_duration": 2379.7118,
+                "max_load_count": 0,
+                "qps": 309.4833,
+                "recall": 1,
+                "serial_latency_p99": 0.0043
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Capacity Test (Large-dim)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
@@ -2369,25 +2123,25 @@
                 "db_config": {
                     "db_label": "2c8g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 2379.5565,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 232.1813,
-                "recall": 0.9818,
-                "serial_latency_p99": 0.0363
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
@@ -2397,25 +2151,25 @@
                 "db_config": {
                     "db_label": "2c8g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 229.3619,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 1241.9402,
-                "recall": 0.9578,
-                "serial_latency_p99": 0.0031
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
@@ -2425,25 +2179,25 @@
                 "db_config": {
                     "db_label": "2c8g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
-            "label": ":)",
+            "label": "x",
             "metrics": {
-                "load_duration": 229.3619,
+                "load_duration": 0.0,
                 "max_load_count": 0,
-                "qps": 1090.1883,
-                "recall": 0.9579,
-                "serial_latency_p99": 0.003
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
@@ -2455,774 +2209,1577 @@
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 229.3619,
+                "load_duration": 5530.3545,
                 "max_load_count": 0,
-                "qps": 1610.7467,
-                "recall": 1,
-                "serial_latency_p99": 0.0025
+                "qps": 133.6633,
+                "recall": 0.9842,
+                "serial_latency_p99": 0.0133
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
                     "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2c8g-hnsw",
+                    "db_label": "16c64g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 218.1418,
+                "load_duration": 5530.3545,
                 "max_load_count": 0,
-                "qps": 1232.3202,
-                "recall": 0.9577,
-                "serial_latency_p99": 0.0025
+                "qps": 127.0729,
+                "recall": 0.9843,
+                "serial_latency_p99": 0.0154
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
                     "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2c8g-hnsw",
+                    "db_label": "16c64g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2379.7118,
+                "load_duration": 5530.3545,
                 "max_load_count": 0,
-                "qps": 274.5407,
-                "recall": 0.9807,
-                "serial_latency_p99": 0.0049
+                "qps": 182.826,
+                "recall": 1,
+                "serial_latency_p99": 0.0122
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
                     "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2c8g-hnsw",
+                    "db_label": "16c64g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2379.7118,
+                "load_duration": 607.0437,
                 "max_load_count": 0,
-                "qps": 236.5672,
-                "recall": 0.981,
-                "serial_latency_p99": 0.0103
+                "qps": 1118.5178,
+                "recall": 0.9796,
+                "serial_latency_p99": 0.0043
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
                     "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2c8g-hnsw",
+                    "db_label": "16c64g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2379.7118,
+                "load_duration": 607.0437,
                 "max_load_count": 0,
-                "qps": 309.4833,
-                "recall": 1,
-                "serial_latency_p99": 0.0043
+                "qps": 963.5486,
+                "recall": 0.9799,
+                "serial_latency_p99": 0.0048
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
                     "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2c8g-hnsw",
+                    "db_label": "16c64g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 4229.5853,
+                "load_duration": 607.0437,
                 "max_load_count": 0,
-                "qps": 120.3348,
-                "recall": 0.9819,
-                "serial_latency_p99": 0.0603
+                "qps": 1381.2118,
+                "recall": 1,
+                "serial_latency_p99": 0.0039
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "Milvus",
                 "db_case_config": {
                     "M": 30,
                     "ef": 100,
                     "efConstruction": 360,
                     "index": "HNSW",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1c8g-hnsw",
+                    "db_label": "16c64g-hnsw",
                     "uri": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 364.6594,
+                "load_duration": 2559.3758,
                 "max_load_count": 0,
-                "qps": 674.0372,
-                "recall": 0.9576,
-                "serial_latency_p99": 0.0027
+                "qps": 76.672,
+                "recall": 0.7964,
+                "serial_latency_p99": 0.0569
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "1c8g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 0,
+                "load_duration": 2519.4009,
                 "max_load_count": 0,
-                "qps": 118.9911,
-                "recall": 0.981,
-                "serial_latency_p99": 0.0607
+                "qps": 51.9266,
+                "recall": 0.7952,
+                "serial_latency_p99": 0.0535
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "1c8g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 370.4316,
+                "load_duration": 2528.1643,
                 "max_load_count": 0,
-                "qps": 646.3226,
-                "recall": 0.9578,
-                "serial_latency_p99": 0.0028
+                "qps": 128.3939,
+                "recall": 0.8613,
+                "serial_latency_p99": 0.0397
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "1c8g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "QdrantCloud",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "2c8g-1node",
+                    "prefer_grpc": true,
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 390.8309,
+                "load_duration": 2571.4912,
                 "max_load_count": 0,
-                "qps": 655.6607,
-                "recall": 0.9581,
-                "serial_latency_p99": 0.0027
+                "qps": 720.0978,
+                "recall": 0.7942,
+                "serial_latency_p99": 0.0347
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "1c8g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "4c16g-5node",
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 78.1565,
+                "load_duration": 2571.4912,
                 "max_load_count": 0,
-                "qps": 4380.5652,
-                "recall": 0.9581,
-                "serial_latency_p99": 0.0028
+                "qps": 553.2483,
+                "recall": 0.7942,
+                "serial_latency_p99": 0.0356
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "4c16g-5node",
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 78.1565,
+                "load_duration": 2571.4912,
                 "max_load_count": 0,
-                "qps": 4028.975,
-                "recall": 0.9582,
-                "serial_latency_p99": 0.0033
+                "qps": 796.9777,
+                "recall": 0.8587,
+                "serial_latency_p99": 0.035
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "4c16g-5node",
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 78.1565,
+                "load_duration": 25181.5505,
                 "max_load_count": 0,
-                "qps": 5740.1221,
-                "recall": 1,
-                "serial_latency_p99": 0.0026
+                "qps": 115.4696,
+                "recall": 0.7861,
+                "serial_latency_p99": 0.0677
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "4c16g-5node",
+                    "prefer_grpc": true,
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5530.3545,
+                "load_duration": 24106.79,
                 "max_load_count": 0,
-                "qps": 133.6633,
-                "recall": 0.9842,
-                "serial_latency_p99": 0.0133
+                "qps": 87.881,
+                "recall": 0.7836,
+                "serial_latency_p99": 0.0485
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 6,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "4c16g-5node",
+                    "prefer_grpc": true,
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5530.3545,
+                "load_duration": 24106.79,
                 "max_load_count": 0,
-                "qps": 127.0729,
-                "recall": 0.9843,
-                "serial_latency_p99": 0.0154
+                "qps": 130.1864,
+                "recall": 0.8412,
+                "serial_latency_p99": 0.0411
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 8,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "QdrantCloud",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "4c16g-5node",
+                    "prefer_grpc": true,
+                    "url": "**********"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 5530.3545,
+                "load_duration": 0.0,
+                "max_load_count": 5500000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 2,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 8300000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 1,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1259.961,
                 "max_load_count": 0,
-                "qps": 182.826,
-                "recall": 1,
-                "serial_latency_p99": 0.0122
+                "qps": 19.9197,
+                "recall": 0.8733,
+                "serial_latency_p99": 0.0697
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "Pinecone",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 607.0437,
+                "load_duration": 1259.961,
                 "max_load_count": 0,
-                "qps": 1118.5178,
-                "recall": 0.9796,
-                "serial_latency_p99": 0.0043
+                "qps": 19.358,
+                "recall": 0.8733,
+                "serial_latency_p99": 0.0697
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "Pinecone",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 607.0437,
+                "load_duration": 1259.961,
                 "max_load_count": 0,
-                "qps": 963.5486,
-                "recall": 0.9799,
-                "serial_latency_p99": 0.0048
+                "qps": 29.3414,
+                "recall": 0.9356,
+                "serial_latency_p99": 0.0706
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "Pinecone",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "s1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 607.0437,
+                "load_duration": 0.0,
+                "max_load_count": 1600000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 2,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 2700000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 1,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1450.5834,
                 "max_load_count": 0,
-                "qps": 1381.2118,
-                "recall": 1,
-                "serial_latency_p99": 0.0039
+                "qps": 237.946,
+                "recall": 0.9268,
+                "serial_latency_p99": 0.0204
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
-                "db": "Milvus",
+                "db": "Pinecone",
                 "db_case_config": {
-                    "M": 30,
-                    "ef": 100,
-                    "efConstruction": 360,
-                    "index": "HNSW",
-                    "metric_type": "COSINE"
+                    "null": null
                 },
                 "db_config": {
-                    "db_label": "16c64g-hnsw",
-                    "uri": "**********"
+                    "api_key": "**********",
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 468.3754,
+                "load_duration": 1450.5834,
                 "max_load_count": 0,
-                "qps": 78.9362,
-                "recall": 0.8197,
-                "serial_latency_p99": 0.0385
+                "qps": 207.6451,
+                "recall": 0.9268,
+                "serial_latency_p99": 0.0217
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Small Dataset)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "0.5c4g-1node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 518.1908,
+                "load_duration": 1450.5834,
                 "max_load_count": 0,
-                "qps": 75.0343,
-                "recall": 0.8122,
-                "serial_latency_p99": 0.042
+                "qps": 66.6749,
+                "recall": 0.9191,
+                "serial_latency_p99": 0.0322
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, Low Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "0.5c4g-1node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 700000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 2,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 4100000,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 1,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 599.7789,
+                "load_duration": 1235.8487,
                 "max_load_count": 0,
-                "qps": 240.455,
-                "recall": 0.9112,
-                "serial_latency_p99": 0.0349
+                "qps": 46.4164,
+                "recall": 0.8733,
+                "serial_latency_p99": 0.0348
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Small Dataset, High Filtering Rate)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "0.5c4g-1node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2559.3758,
+                "load_duration": 1235.8474,
                 "max_load_count": 0,
-                "qps": 76.672,
-                "recall": 0.7964,
-                "serial_latency_p99": 0.0569
+                "qps": 44.5978,
+                "recall": 0.8733,
+                "serial_latency_p99": 0.0394
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Medium Dataset)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "2c8g-1node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2519.4009,
+                "load_duration": 1235.8474,
                 "max_load_count": 0,
-                "qps": 51.9266,
-                "recall": 0.7952,
-                "serial_latency_p99": 0.0535
+                "qps": 127.9003,
+                "recall": 0.9356,
+                "serial_latency_p99": 0.0232
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, Low Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "2c8g-1node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1",
+                    "environment": "**********",
+                    "index_name": "test_index"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 2528.1643,
+                "load_duration": 1450.6205,
                 "max_load_count": 0,
-                "qps": 128.3939,
-                "recall": 0.8613,
-                "serial_latency_p99": 0.0397
+                "qps": 20.7437,
+                "recall": 0.9291,
+                "serial_latency_p99": 0.0758
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Medium Dataset, High Filtering Rate)",
+                    "case_id": 5,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "2c8g-1node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "s1.x1-2node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 25181.5505,
+                "load_duration": 1450.6205,
                 "max_load_count": 0,
-                "qps": 115.4696,
-                "recall": 0.7861,
-                "serial_latency_p99": 0.0677
+                "qps": 20.2993,
+                "recall": 0.9293,
+                "serial_latency_p99": 0.0765
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Search Performance Test (Large Dataset)",
+                    "case_id": 7,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "4c16g-5node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "s1.x1-2node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 24106.79,
+                "load_duration": 1450.6205,
                 "max_load_count": 0,
-                "qps": 87.881,
-                "recall": 0.7836,
-                "serial_latency_p99": 0.0485
+                "qps": 26.4719,
+                "recall": 1.0,
+                "serial_latency_p99": 0.067
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, Low Filtering Rate)",
+                    "case_id": 9,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "4c16g-5node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "s1.x1-2node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 24106.79,
+                "load_duration": 14991.9752,
                 "max_load_count": 0,
-                "qps": 130.1864,
-                "recall": 0.8412,
-                "serial_latency_p99": 0.0411
+                "qps": 8.2809,
+                "recall": 0.8369,
+                "serial_latency_p99": 0.1549
             },
             "task_config": {
                 "case_config": {
-                    "case_id": "Filtering Search Performance Test (Large Dataset, High Filtering Rate)",
+                    "case_id": 4,
                     "custom_case": {}
                 },
-                "db": "QdrantCloud",
+                "db": "Pinecone",
                 "db_case_config": {
                     "null": null
                 },
                 "db_config": {
                     "api_key": "**********",
-                    "db_label": "4c16g-5node",
-                    "prefer_grpc": true,
-                    "url": "**********"
+                    "db_label": "s1.x1-2node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 14991.9752,
+                "max_load_count": 0,
+                "qps": 7.6488,
+                "recall": 0.8369,
+                "serial_latency_p99": 0.1618
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "s1.x1-2node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 14991.9752,
+                "max_load_count": 0,
+                "qps": 16.5246,
+                "recall": 0.9814,
+                "serial_latency_p99": 0.0803
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "s1.x1-2node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1210.2139,
+                "max_load_count": 0,
+                "qps": 365.0835,
+                "recall": 0.945,
+                "serial_latency_p99": 0.0236
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 5,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1210.2139,
+                "max_load_count": 0,
+                "qps": 325.5271,
+                "recall": 0.9452,
+                "serial_latency_p99": 0.0251
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 7,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1210.2139,
+                "max_load_count": 0,
+                "qps": 596.7942,
+                "recall": 0.9693,
+                "serial_latency_p99": 0.0242
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 9,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 12658.5938,
+                "max_load_count": 0,
+                "qps": 283.5304,
+                "recall": 0.9246,
+                "serial_latency_p99": 0.0256
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 12658.5938,
+                "max_load_count": 0,
+                "qps": 136.1829,
+                "recall": 0.9245,
+                "serial_latency_p99": 0.029
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 12658.5938,
+                "max_load_count": 0,
+                "qps": 71.5744,
+                "recall": 0.963,
+                "serial_latency_p99": 0.0345
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p2.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1211.8883,
+                "max_load_count": 0,
+                "qps": 131.2549,
+                "recall": 0.9867,
+                "serial_latency_p99": 0.0302
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 5,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1211.8883,
+                "max_load_count": 0,
+                "qps": 127.9337,
+                "recall": 0.9869,
+                "serial_latency_p99": 0.0301
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 7,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": ":)",
+            "metrics": {
+                "load_duration": 1211.8883,
+                "max_load_count": 0,
+                "qps": 595.8462,
+                "recall": 1.0,
+                "serial_latency_p99": 0.0234
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 9,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "Pinecone",
+                "db_case_config": {
+                    "null": null
+                },
+                "db_config": {
+                    "api_key": "**********",
+                    "db_label": "p1.x1-8node",
+                    "environment": "**********",
+                    "index_name": "benchmark-test"
                 }
             }
         }
     ],
     "run_id": "5c1e8bd468224ffda1b39b08cdc342c3",
     "task_label": "standard"
 }
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench.egg-info/PKG-INFO` & `vectordb-bench-0.0.2/vectordb_bench.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: vectordb-bench
-Version: 0.0.1
+Version: 0.0.2
 Summary: VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 Author-email: XuanYang-cn <xuan.yang@zilliz.com>
 Project-URL: repository, https://github.com/zilliztech/VectorDBBench
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # VectorDBBench: A Benchmark Tool for VectorDB
 
+[![version](https://img.shields.io/pypi/v/vectordb-bench.svg?color=blue)](https://pypi.org/project/vectordb-bench/)
+[![Downloads](https://pepy.tech/badge/vectordb-bench)](https://pepy.tech/project/vectordb-bench)
+
 ## Quick Start
 ### Prerequirement
 ``` shell
 python >= 3.11
 ```
 ### Install
 ``` shell
@@ -30,15 +33,15 @@
 ```
 ## What is VectorDBBench
 VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 
 Understanding the importance of user experience, we provide an intuitive visual interface. This not only empowers users to initiate benchmarks at ease, but also to view comparative result reports, thereby reproducing benchmark results effortlessly.
 To add more relevance and practicality, we provide cost-effectiveness reports particularly for cloud services. This allows for a more realistic and applicable benchmarking process.
 
-Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as SIFT, GIST, Cohere, and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
+Closely mimicking real-world production environments, we've set up diverse testing scenarios including insertion, searching, and filtered searching. To provide you with credible and reliable data, we've included public datasets from actual production scenarios, such as [SIFT](http://corpus-texmex.irisa.fr/), [GIST](http://corpus-texmex.irisa.fr/), [Cohere](https://huggingface.co/datasets/Cohere/wikipedia-22-12/tree/main/en), and more. It's fascinating to discover how a relatively unknown open-source database might excel in certain circumstances!
 
 Prepare to delve into the world of VectorDBBench, and let it guide you in uncovering your perfect vector database match.  
 
 ## Build on your own
 ### Install requirements
 ``` shell
 pip install -e '.[test]'
@@ -62,64 +65,58 @@
 
 ```shell
 $ ruff check vectordb_bench --fix
 ```
 
 ## How does it work?
 ### Result Page
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/a8418fb6-0822-4f04-a04d-ab9143815b3e)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/66ab83c4-656e-41a8-a643-d9790faccbeb)
 This is the main page of VectorDBBench, which displays the standard benchmark results we provide. Additionally, results of all tests performed by users themselves will also be shown here. We also offer the ability to select and compare results from multiple tests simultaneously.
 
-The standard benchmark results displayed here include all 12 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
+The standard benchmark results displayed here include all 9 cases that we currently support for all our clients (Milvus, Zilliz Cloud, Elastic Search, Qdrant Cloud, and Weaviate Cloud). However, as some systems may not be able to complete all the tests successfully due to issues like Out of Memory (OOM) or timeouts, not all clients are included in every case.
 ### Run Test Page
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/364e2462-107e-4ce1-aabc-ff2b217ae9b7)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/a789099a-3707-4214-8052-b73463b8f2c6)
 This is the page to run a test:
 1. Initially, you select the systems to be tested - multiple selections are allowed. Once selected, corresponding forms will pop up to gather necessary information for using the chosen databases. The db_label is used to differentiate different instances of the same system. We recommend filling in the host size or instance type here (as we do in our standard results).
 2. The next step is to select the test cases you want to perform. You can select multiple cases at once, and a form to collect corresponding parameters will appear.
 3. Finally, you'll need to provide a task label to distinguish different test results. Using the same label for different tests will result in the previous results being overwritten.
 Now we can only run one task at the same time. 
 
 ## Module
 ### Code Structure
-![image](https://github.com/liliu-z/VectorDBBench/assets/105927039/8d65c8b4-b9a3-4405-9db8-d27bf1ffda4b)
+![image](https://github.com/zilliztech/VectorDBBench/assets/105927039/8c06512e-5419-4381-b084-9c93aed59639)
 ### Client
 Our client module is designed with flexibility and extensibility in mind, aiming to integrate APIs from different systems seamlessly. As of now, it supports Milvus, Zilliz Cloud, Elastic Search, Pinecone, Qdrant, and Weaviate. Stay tuned for more options, as we are consistently working on extending our reach to other systems.
 ### Benchmark Cases
-We've developed an array of 12 comprehensive benchmark cases to test vector databases' various capabilities, each designed to give you a different piece of the puzzle. These cases are categorized into three main types:
+We've developed an array of 9 comprehensive benchmark cases to test vector databases' various capabilities, each designed to give you a different piece of the puzzle. These cases are categorized into three main types:
 #### Capacity Case
 - **Large Dim:** Tests the database's loading capacity by inserting large-dimension vectors (GIST 100K vectors, 960 dimensions) until fully loaded. The final number of inserted vectors is reported.
 - **Small Dim:** Similar to the Large Dim case but uses small-dimension vectors (SIFT 100K vectors, 128 dimensions).
 #### Search Performance Case
 - **XLarge Dataset:** Measures search performance with a massive dataset (LAION 100M vectors, 768 dimensions) at varying parallel levels. The results include index building time, recall, latency, and maximum QPS.
 - **Large Dataset:** Similar to the XLarge Dataset case, but uses a slightly smaller dataset (Cohere 10M vectors, 768 dimensions).
 - **Medium Dataset:** A case using a medium dataset (Cohere 1M vectors, 768 dimensions).
-- **Small Dataset:** This case uses a small dataset (Cohere 100K vectors, 768 dimensions).
 #### Filtering Search Performance Case
 - **Large Dataset, Low Filtering Rate:** Evaluates search performance with a large dataset (Cohere 10M vectors, 768 dimensions) under a low filtering rate (1% vectors) at different parallel levels.
 - **Medium Dataset, Low Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a similar low filtering rate.
-- **Small Dataset, Low Filtering Rate:** This case uses a small dataset (Cohere 100K vectors, 768 dimensions) with a low filtering rate.
 - **Large Dataset, High Filtering Rate:** It tests with a large dataset (Cohere 10M vectors, 768 dimensions) but under a high filtering rate (99% vectors).
 - **Medium Dataset, High Filtering Rate:** This case uses a medium dataset (Cohere 1M vectors, 768 dimensions) with a high filtering rate.
-- **Small Dataset, High Filtering Rate:** Finally, this case uses a small dataset (Cohere 100K vectors, 768 dimensions) under a high filtering rate.
 For a quick reference, here is a table summarizing the key aspects of each case:
 
 Case No. | Case Type | Dataset Size | Dataset Type | Filtering Rate | Results |
 |----------|-----------|--------------|--------------|----------------|---------|
 1 | Capacity Case | Large Dim | GIST 100K vectors, 960 dimensions | N/A | Number of inserted vectors |
 2 | Capacity Case | Small Dim | SIFT 100K vectors, 128 dimensions | N/A | Number of inserted vectors |
 3 | Search Performance Case | XLarge Dataset | LAION 100M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
 4 | Search Performance Case | Large Dataset | Cohere 10M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
 5 | Search Performance Case | Medium Dataset | Cohere 1M vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-6 | Search Performance Case | Small Dataset | Cohere 100K vectors, 768 dimensions | N/A | Index building time, recall, latency, maximum QPS |
-7 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-8 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-9 | Filtering Search Performance Case | Small Dataset, Low Filtering Rate | Cohere 100K vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
-10 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-11 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
-12 | Filtering Search Performance Case | Small Dataset, High Filtering Rate | Cohere 100K vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+6 | Filtering Search Performance Case | Large Dataset, Low Filtering Rate | Cohere 10M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+7 | Filtering Search Performance Case | Medium Dataset, Low Filtering Rate | Cohere 1M vectors, 768 dimensions | 1% vectors | Index building time, recall, latency, maximum QPS |
+8 | Filtering Search Performance Case | Large Dataset, High Filtering Rate | Cohere 10M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
+9 | Filtering Search Performance Case | Medium Dataset, High Filtering Rate | Cohere 1M vectors, 768 dimensions | 99% vectors | Index building time, recall, latency, maximum QPS |
 
 Each case provides an in-depth examination of a vector database's abilities, providing you a comprehensive view of the database's performance.
 
 ## Goals
 Our goals of this benchmark are:
 ### Reproducibility & Usability
 One of the primary goals of VectorDBBench is to enable users to reproduce benchmark results swiftly and easily, or to test their customized scenarios. We believe that lowering the barriers to entry for conducting these tests will enhance the community's understanding and improvement of vector databases. We aim to create an environment where any user, regardless of their technical expertise, can quickly set up and run benchmarks, and view and analyze results in an intuitive manner.
@@ -132,15 +129,15 @@
 2. Adhere to coding conventions and formatting guidelines.
 3. Use clear commit messages to document the purpose of your changes.
 ### Adding New Clients
 **Step 1: Creating New Client Files**
 
 1. Navigate to the vectordb_bench/backend/clients directory.
 2. Create a new folder for your client, for example, "new_client".
-3. Inside the "new_client" folder, create two files: new_client.py and config.py. 
+3. Inside the "new_client" folder, create two files: new_client.py and config.py.
 
 **Step 2: Implement new_client.py and config.py**
 
 1. Open new_client.py and define the NewClient class, which should inherit from the clients/api.py file's VectorDB abstract class. The VectorDB class serves as the API for benchmarking, and all DB clients must implement this abstract class. 
 Example implementation in new_client.py:
 new_client.py
 ```python 
@@ -197,11 +194,9 @@
 ### Installation 
 The system under test can be installed in any form to achieve optimal performance. This includes but is not limited to binary deployment, Docker, and cloud services.
 ### Fine-Tuning
 For the system under test, we use the default server-side configuration to maintain the authenticity and representativeness of our results.
 For the Client, we welcome any parameter tuning to obtain better results.
 ### Incomplete Results
 Many databases may not be able to complete all test cases due to issues such as Out of Memory (OOM), crashes, or timeouts. In these scenarios, we will clearly state these occurrences in the test results.
-### Unpublishable Results
-Although we are trying to support as many clients as possible for benchmarking, due to the restrictions imposed by the [Dewitt Clause](https://cube.dev/blog/dewitt-clause-or-can-you-benchmark-a-database), we're unable to publish all benchmark results. This means that users may not be able to fully compare performance data for certain databases on our platform, despite the support we have integrated for these systems. 
 ### Mistake Or Misrepresentation 
 We strive for accuracy in learning and supporting various vector databases, yet there might be oversights or misapplications. For any such occurrences, feel free to [raise an issue](https://github.com/zilliztech/VectorDBBench/issues/new) or make amendments on our GitHub page.
```

### Comparing `vectordb-bench-0.0.1/vectordb_bench.egg-info/SOURCES.txt` & `vectordb-bench-0.0.2/vectordb_bench.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+.env.example
+.gitignore
+.ruff.toml
 LICENSE
 README.md
 pyproject.toml
+.github/workflows/publish_package_on_release.yml
+tests/conftest.py
+tests/pytest.ini
 tests/test_bench_runner.py
 tests/test_dataset.py
 tests/test_elasticsearch_cloud.py
 tests/test_models.py
 tests/test_utils.py
+tests/ut_cases.py
 vectordb_bench/__init__.py
 vectordb_bench/__main__.py
 vectordb_bench/base.py
 vectordb_bench/interface.py
 vectordb_bench/log_util.py
 vectordb_bench/metric.py
 vectordb_bench/models.py
@@ -39,26 +46,32 @@
 vectordb_bench/backend/clients/weaviate_cloud/config.py
 vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
 vectordb_bench/backend/clients/zilliz_cloud/config.py
 vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py
 vectordb_bench/backend/runner/__init__.py
 vectordb_bench/backend/runner/mp_runner.py
 vectordb_bench/backend/runner/serial_runner.py
-vectordb_bench/frontend/const.py
 vectordb_bench/frontend/utils.py
 vectordb_bench/frontend/vdb_benchmark.py
 vectordb_bench/frontend/components/check_results/charts.py
 vectordb_bench/frontend/components/check_results/data.py
+vectordb_bench/frontend/components/check_results/expanderStyle.py
 vectordb_bench/frontend/components/check_results/filters.py
+vectordb_bench/frontend/components/check_results/footer.py
 vectordb_bench/frontend/components/check_results/headerIcon.py
 vectordb_bench/frontend/components/check_results/nav.py
 vectordb_bench/frontend/components/check_results/priceTable.py
+vectordb_bench/frontend/components/check_results/stPageConfig.py
+vectordb_bench/frontend/components/get_results/saveAsImage.py
 vectordb_bench/frontend/components/run_test/autoRefresh.py
 vectordb_bench/frontend/components/run_test/caseSelector.py
 vectordb_bench/frontend/components/run_test/dbConfigSetting.py
 vectordb_bench/frontend/components/run_test/dbSelector.py
 vectordb_bench/frontend/components/run_test/generateTasks.py
 vectordb_bench/frontend/components/run_test/hideSidebar.py
 vectordb_bench/frontend/components/run_test/submitTask.py
-vectordb_bench/frontend/pages/qps_with_price.py
+vectordb_bench/frontend/const/dbCaseConfigs.py
+vectordb_bench/frontend/const/dbPrices.py
+vectordb_bench/frontend/const/styles.py
+vectordb_bench/frontend/pages/quries_per_dollar.py
 vectordb_bench/frontend/pages/run_test.py
 vectordb_bench/results/result_20230609_standard.json
```

