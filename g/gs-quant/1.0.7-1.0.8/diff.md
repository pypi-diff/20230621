# Comparing `tmp/gs_quant-1.0.7.tar.gz` & `tmp/gs_quant-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gs_quant-1.0.7.tar", last modified: Wed Jun 14 17:17:19 2023, max compression
+gzip compressed data, was "dist/gs_quant-1.0.8.tar", last modified: Wed Jun 21 17:55:13 2023, max compression
```

## Comparing `gs_quant-1.0.7.tar` & `gs_quant-1.0.8.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-14 17:16:55.000000 gs_quant-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-14 17:17:19.000000 gs_quant-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-14 17:16:55.000000 gs_quant-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/analytics/common/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/common/enumerators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/common/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/analytics/core/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/core/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/core/processor_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/core/query_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/data_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/data_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/datagrid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/analytics/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/processors/analysis_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/processors/econometrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/processors/scale_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/processors/special_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/processors/statistics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/processors/utility_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/analytics/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/workspaces/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/analytics/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/api/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/api/fred/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/fred/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/fred/fred_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/api/gs/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    38389 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/hedges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/thematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/gs/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/backtests/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/action_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/backtest_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/backtest_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/backtest_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/equity_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    41410 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/predefined_asset_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/strategy_systematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/backtests/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/config/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/content/reports_and_screens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/content/reports_and_screens/00_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/content/reports_and_screens/00_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/content/reports_and_screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/data/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/data/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/datetime/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/datetime/gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/datetime/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/datetime/relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/datetime/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/datetime/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.add.html
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
--rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.log.html
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.power.html
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.count.html
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.first.html
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.last.html
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.align.html
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.day.html
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.month.html
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.union.html
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.value.html
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.year.html
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
--rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.median.html
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.product.html
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.std.html
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.var.html
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/entities/entitlements.py
--rw-r--r--   0 runner    (1001) docker     (123)    42474 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/entities/tree_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/instrument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/instrument/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/instrument/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/json_convertors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/markets/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39137 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/historical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/indices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    21869 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/portfolio_manager_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29039 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/position_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    64256 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/markets/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/models/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29649 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/models/epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    96403 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/models/risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/models/risk_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/priceable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/quote_reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/quote_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/quote_reports/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/risk/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/result_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39946 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/scenario_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/risk/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/target/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/assets_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)   241626 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    36466 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/positions_v2_pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/secmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/workflow_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/target/workspaces_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/analytics/test_datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/analytics/test_sorting_and_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/analytics/test_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_content.py
--rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_fred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_thread_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/backtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/backtest/test_backtest_flow_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/backtest/test_backtest_predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/backtest/test_generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/backtest/test_triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/data/test_data_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/data/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/datetime_/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/datetime_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/datetime_/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/datetime_/test_gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/datetime_/test_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/datetime_/test_relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/datetime_/test_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/fixtures/content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_hedger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_pricing_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/markets/test_securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/models/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/models/test_epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/models/test_risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/timeseries/multi_measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/multi_measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/multi_measure/test_commod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    22374 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   238697 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    37505 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_rolling.py
--rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_technicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/timeseries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/utils/datagrid_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/utils/mock_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/test/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)   227438 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)    54899 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/timeseries/technicals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-14 17:16:56.000000 gs_quant-1.0.7/gs_quant/tracing/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14814 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 17:17:19.000000 gs_quant-1.0.7/gs_quant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-14 17:17:19.000000 gs_quant-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-14 17:16:56.000000 gs_quant-1.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83669 2023-06-14 17:16:56.000000 gs_quant-1.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-21 17:54:57.000000 gs_quant-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-21 17:55:13.000000 gs_quant-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 17:54:57.000000 gs_quant-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/analytics/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/common/enumerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/common/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/analytics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/core/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/core/processor_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/core/query_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/data_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/data_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/datagrid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/analytics/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/processors/analysis_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/processors/econometrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/processors/scale_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/processors/special_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/processors/statistics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/processors/utility_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/analytics/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/workspaces/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/analytics/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/api/fred/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/fred/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/fred/fred_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/api/gs/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38389 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/hedges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/thematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/gs/workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/backtests/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/action_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/backtest_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/backtest_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/backtest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/equity_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41680 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/predefined_asset_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/strategy_systematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18799 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/backtests/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/content/reports_and_screens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/content/reports_and_screens/00_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/content/reports_and_screens/00_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/content/reports_and_screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/data/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/datetime/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/datetime/gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/datetime/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/datetime/relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/datetime/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/datetime/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.add.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.log.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.power.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.count.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.first.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.last.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.align.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.day.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.month.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.union.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.value.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.year.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.median.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.product.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.var.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/entities/entitlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42474 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/entities/tree_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/instrument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/instrument/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/instrument/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/json_convertors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39137 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/indices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/portfolio_manager_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/position_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69442 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/markets/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29649 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/models/epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96403 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/models/risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/models/risk_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/priceable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/quote_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/quote_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/quote_reports/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/result_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39946 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/scenario_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/risk/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/target/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/assets_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241626 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36466 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/positions_v2_pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/secmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/workflow_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/target/workspaces_markets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/analytics/test_datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/analytics/test_sorting_and_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/analytics/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_fred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_thread_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/backtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/backtest/test_backtest_flow_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/backtest/test_backtest_predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/backtest/test_generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/backtest/test_triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/data/test_data_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/data/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/datetime_/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/datetime_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/datetime_/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/datetime_/test_gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/datetime_/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/datetime_/test_relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/datetime_/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/fixtures/content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_hedger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_pricing_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/markets/test_securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/models/test_epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/models/test_risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/timeseries/multi_measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/multi_measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/multi_measure/test_commod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22374 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238697 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37614 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_rolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_technicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/timeseries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/utils/datagrid_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/utils/mock_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/test/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)   227438 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17635 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54899 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/timeseries/technicals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-21 17:54:58.000000 gs_quant-1.0.8/gs_quant/tracing/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14814 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 17:55:13.000000 gs_quant-1.0.8/gs_quant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-21 17:55:13.000000 gs_quant-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-21 17:54:58.000000 gs_quant-1.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83669 2023-06-21 17:54:58.000000 gs_quant-1.0.8/versioneer.py
```

### Comparing `gs_quant-1.0.7/PKG-INFO` & `gs_quant-1.0.8/gs_quant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gs_quant
-Version: 1.0.7
+Name: gs-quant
+Version: 1.0.8
 Summary: Goldman Sachs Quant
 Home-page: https://marquee.gs.com
 Author: Goldman Sachs
 Author-email: developer@gs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # GS Quant
```

### Comparing `gs_quant-1.0.7/README.md` & `gs_quant-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/__init__.py` & `gs_quant-1.0.8/gs_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/common/__init__.py` & `gs_quant-1.0.8/gs_quant/analytics/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/common/constants.py` & `gs_quant-1.0.8/gs_quant/analytics/common/constants.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/common/enumerators.py` & `gs_quant-1.0.8/gs_quant/analytics/common/enumerators.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/common/helpers.py` & `gs_quant-1.0.8/gs_quant/analytics/common/helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/core/__init__.py` & `gs_quant-1.0.8/gs_quant/analytics/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/core/processor.py` & `gs_quant-1.0.8/gs_quant/analytics/core/processor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/core/processor_result.py` & `gs_quant-1.0.8/gs_quant/analytics/core/processor_result.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/core/query_helpers.py` & `gs_quant-1.0.8/gs_quant/analytics/core/query_helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/datagrid/__init__.py` & `gs_quant-1.0.8/gs_quant/analytics/datagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/datagrid/data_cell.py` & `gs_quant-1.0.8/gs_quant/analytics/datagrid/data_cell.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/datagrid/data_column.py` & `gs_quant-1.0.8/gs_quant/analytics/datagrid/data_column.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/datagrid/data_row.py` & `gs_quant-1.0.8/gs_quant/analytics/datagrid/data_row.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/datagrid/datagrid.py` & `gs_quant-1.0.8/gs_quant/analytics/datagrid/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/datagrid/serializers.py` & `gs_quant-1.0.8/gs_quant/analytics/datagrid/serializers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/datagrid/utils.py` & `gs_quant-1.0.8/gs_quant/analytics/datagrid/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/processors/__init__.py` & `gs_quant-1.0.8/gs_quant/analytics/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/processors/analysis_processors.py` & `gs_quant-1.0.8/gs_quant/analytics/processors/analysis_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/processors/econometrics_processors.py` & `gs_quant-1.0.8/gs_quant/analytics/processors/econometrics_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/processors/scale_processors.py` & `gs_quant-1.0.8/gs_quant/analytics/processors/scale_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/processors/special_processors.py` & `gs_quant-1.0.8/gs_quant/analytics/processors/special_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/processors/statistics_processors.py` & `gs_quant-1.0.8/gs_quant/analytics/processors/statistics_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/processors/utility_processors.py` & `gs_quant-1.0.8/gs_quant/analytics/processors/utility_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/workspaces/__init__.py` & `gs_quant-1.0.8/gs_quant/analytics/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/workspaces/components.py` & `gs_quant-1.0.8/gs_quant/analytics/workspaces/components.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/analytics/workspaces/workspace.py` & `gs_quant-1.0.8/gs_quant/analytics/workspaces/workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/__init__.py` & `gs_quant-1.0.8/gs_quant/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/data.py` & `gs_quant-1.0.8/gs_quant/api/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/fred/__init__.py` & `gs_quant-1.0.8/gs_quant/api/fred/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/fred/data.py` & `gs_quant-1.0.8/gs_quant/api/fred/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/fred/fred_query.py` & `gs_quant-1.0.8/gs_quant/api/fred/fred_query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/__init__.py` & `gs_quant-1.0.8/gs_quant/api/gs/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/assets.py` & `gs_quant-1.0.8/gs_quant/api/gs/assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/backtests.py` & `gs_quant-1.0.8/gs_quant/api/gs/backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/base_screener.py` & `gs_quant-1.0.8/gs_quant/api/gs/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/carbon.py` & `gs_quant-1.0.8/gs_quant/api/gs/carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/content.py` & `gs_quant-1.0.8/gs_quant/api/gs/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/countries.py` & `gs_quant-1.0.8/gs_quant/api/gs/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/data.py` & `gs_quant-1.0.8/gs_quant/api/gs/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/data_screen.py` & `gs_quant-1.0.8/gs_quant/api/gs/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/datagrid.py` & `gs_quant-1.0.8/gs_quant/api/gs/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/esg.py` & `gs_quant-1.0.8/gs_quant/api/gs/esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/groups.py` & `gs_quant-1.0.8/gs_quant/api/gs/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/hedges.py` & `gs_quant-1.0.8/gs_quant/api/gs/hedges.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/indices.py` & `gs_quant-1.0.8/gs_quant/api/gs/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/monitors.py` & `gs_quant-1.0.8/gs_quant/api/gs/monitors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/parser.py` & `gs_quant-1.0.8/gs_quant/api/gs/parser.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/plots.py` & `gs_quant-1.0.8/gs_quant/api/gs/plots.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/portfolios.py` & `gs_quant-1.0.8/gs_quant/api/gs/portfolios.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 """
 import datetime as dt
 import logging
+import deprecation
 from time import sleep
 from typing import Tuple, Union, List, Dict
 
 from gs_quant.common import PositionType
 from gs_quant.common import RiskRequest, Currency
 from gs_quant.instrument import Instrument
 from gs_quant.session import GsSession
@@ -305,26 +306,32 @@
                            portfolio_id: str,
                            backcast: bool = False) -> List[dt.date]:
         results = GsSession.current._get(f'/portfolios/{portfolio_id}/schedule/dates?backcast={str(backcast).lower()}')
         return [dt.datetime.strptime(results['startDate'], '%Y-%m-%d').date(),
                 dt.datetime.strptime(results['endDate'], '%Y-%m-%d').date()]
 
     @classmethod
+    @deprecation.deprecated(deprecated_in='1.0.10',
+                            details='GsPortfolioApi.get_custom_aum is now deprecated, please use '
+                                    'GsReportApi.get_custom_aum instead.')
     def get_custom_aum(cls,
                        portfolio_id: str,
                        start_date: dt.date = None,
                        end_date: dt.date = None) -> dict:
         url = f'/portfolios/{portfolio_id}/aum?'
         if start_date:
             url += f"&startDate={start_date.strftime('%Y-%m-%d')}"
         if end_date:
             url += f"&endDate={end_date.strftime('%Y-%m-%d')}"
         return GsSession.current._get(url)['data']
 
     @classmethod
+    @deprecation.deprecated(deprecated_in='1.0.10',
+                            details='GsPortfolioApi.upload_custom_aum is now deprecated, please use '
+                                    'GsReportApi.upload_custom_aum instead.')
     def upload_custom_aum(cls,
                           portfolio_id: str,
                           aum_data: List[Dict],
                           clear_existing_data: bool = None) -> dict:
         url = f'/portfolios/{portfolio_id}/aum'
         payload = {'data': aum_data}
         if clear_existing_data:
```

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/price.py` & `gs_quant-1.0.8/gs_quant/api/gs/price.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/reports.py` & `gs_quant-1.0.8/gs_quant/api/gs/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,37 @@
         status_body = {
             "status": '{status}'.format(status=status)
         }
         return GsSession.current._post('/reports/jobs/{report_job_id}/update'.format(report_job_id=report_job_id),
                                        status_body)
 
     @classmethod
+    def get_custom_aum(cls,
+                       report_id: str,
+                       start_date: dt.date = None,
+                       end_date: dt.date = None) -> dict:
+        url = f'/reports/{report_id}/aum?'
+        if start_date:
+            url += f"&startDate={start_date.strftime('%Y-%m-%d')}"
+        if end_date:
+            url += f"&endDate={end_date.strftime('%Y-%m-%d')}"
+        return GsSession.current._get(url)['data']
+
+    @classmethod
+    def upload_custom_aum(cls,
+                          report_id: str,
+                          aum_data: List[dict],
+                          clear_existing_data: bool = None) -> dict:
+        url = f'/reports/{report_id}/aum'
+        payload = {'data': aum_data}
+        if clear_existing_data:
+            url += '?clearExistingData=true'
+        return GsSession.current._post(url, payload)
+
+    @classmethod
     def get_factor_risk_report_results(cls,
                                        risk_report_id: str,
                                        view: str = None,
                                        factors: List[str] = None,
                                        factor_categories: List[str] = None,
                                        currency: Currency = None,
                                        start_date: dt.date = None,
```

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/risk.py` & `gs_quant-1.0.8/gs_quant/api/gs/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/risk_models.py` & `gs_quant-1.0.8/gs_quant/api/gs/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/screens.py` & `gs_quant-1.0.8/gs_quant/api/gs/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/thematics.py` & `gs_quant-1.0.8/gs_quant/api/gs/thematics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/users.py` & `gs_quant-1.0.8/gs_quant/api/gs/users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/gs/workspaces.py` & `gs_quant-1.0.8/gs_quant/api/gs/workspaces.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/risk.py` & `gs_quant-1.0.8/gs_quant/api/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/api/utils.py` & `gs_quant-1.0.8/gs_quant/api/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/__init__.py` & `gs_quant-1.0.8/gs_quant/backtests/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/action_handler.py` & `gs_quant-1.0.8/gs_quant/backtests/action_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/actions.py` & `gs_quant-1.0.8/gs_quant/backtests/actions.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/backtest_engine.py` & `gs_quant-1.0.8/gs_quant/backtests/backtest_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/backtest_objects.py` & `gs_quant-1.0.8/gs_quant/backtests/backtest_objects.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/backtest_utils.py` & `gs_quant-1.0.8/gs_quant/backtests/backtest_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/core.py` & `gs_quant-1.0.8/gs_quant/backtests/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/data_handler.py` & `gs_quant-1.0.8/gs_quant/backtests/data_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/data_sources.py` & `gs_quant-1.0.8/gs_quant/backtests/data_sources.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/decorator.py` & `gs_quant-1.0.8/gs_quant/backtests/decorator.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/equity_vol_engine.py` & `gs_quant-1.0.8/gs_quant/backtests/equity_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/event.py` & `gs_quant-1.0.8/gs_quant/backtests/event.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/execution_engine.py` & `gs_quant-1.0.8/gs_quant/backtests/execution_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/generic_engine.py` & `gs_quant-1.0.8/gs_quant/backtests/generic_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,29 +327,30 @@
                     # List of trade names not provided -> TradeDate <= exit trigger date
                     port_indexes_to_remove = [i for i, x in enumerate(pos_fut) if
                                               dt.datetime.strptime(x.name.split('_')[-1], '%Y-%m-%d').date() <= s]
                     result_indexes_to_remove = [i for i, x in enumerate(res_fut) if
                                                 dt.datetime.strptime(x.name.split('_')[-1], '%Y-%m-%d').date() <= s]
 
                 for index in sorted(port_indexes_to_remove, reverse=True):
-                    # Get list of trades' names that have been removed to check for their future cash flow date
+                    # Get list of trades that have been removed to check for their future cash flow date
                     if pos_fut[index].name not in trades_to_remove:
-                        trades_to_remove.append(pos_fut[index].name)
+                        trades_to_remove.append(pos_fut[index])
                     del pos_fut[index]
                 for index in sorted(result_indexes_to_remove, reverse=True):
                     del res_futures[index]
                 backtest.portfolio_dict[port_date] = Portfolio(tuple(pos_fut))
                 if result_indexes_to_remove:
                     backtest.results[port_date] = PortfolioRiskResult(backtest.portfolio_dict[port_date],
                                                                       backtest.results[port_date].risk_measures,
                                                                       res_futures)
 
             for cp_date, cp_list in list(backtest.cash_payments.items()):
                 if cp_date > s:
-                    indexes_to_remove = [i for i, cp in enumerate(cp_list) if cp.trade.name in trades_to_remove]
+                    indexes_to_remove = [i for i, cp in enumerate(cp_list)
+                                         if cp.trade.name in [x.name for x in trades_to_remove]]
                     for index in sorted(indexes_to_remove, reverse=True):
                         cp = cp_list[index]
                         prev_pos = [i for i, x in enumerate(backtest.cash_payments[s]) if cp.trade.name == x.trade.name]
                         # If trade already exists in exit trigger date cash payments, net out the position
                         if prev_pos:
                             backtest.cash_payments[s][prev_pos[0]].direction += cp.direction
                         else:
@@ -360,14 +361,18 @@
                         del backtest.cash_payments[cp_date][index]
                         backtest.transaction_costs[cp_date] += self.action.transaction_cost.get_cost(state, backtest,
                                                                                                      trigger_info)
 
                     if not backtest.cash_payments[cp_date]:
                         del backtest.cash_payments[cp_date]
 
+            for trade in trades_to_remove:
+                if trade.name not in [x.trade.name for x in backtest.cash_payments[s]]:
+                    backtest.cash_payments[s].append(CashPayment(trade, effective_date=s))
+
         return backtest
 
 
 class RebalanceActionImpl(ActionHandler):
     def __init__(self, action: RebalanceAction):
         super().__init__(action)
```

### Comparing `gs_quant-1.0.7/gs_quant/backtests/order.py` & `gs_quant-1.0.8/gs_quant/backtests/order.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/predefined_asset_engine.py` & `gs_quant-1.0.8/gs_quant/backtests/predefined_asset_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 self.get_action_handler(x)
         except RuntimeError:
             return False
         return True
 
     def __init__(self,
                  data_mgr: DataManager = DataManager(),
-                 calendars: Union[str, Tuple[str, ...]] = 'Weekend',
+                 calendars: Union[str, Tuple[str, ...]] = None,
                  tz: timezone = timezone('UTC'),
                  valuation_method: ValuationMethod = ValuationMethod(ValuationFixingType.PRICE),
                  action_impl_map=None):
         if action_impl_map is None:
             action_impl_map = {Action: SubmitOrderActionImpl}
         self.action_impl_map = action_impl_map
         self.calendars = calendars
@@ -139,21 +139,21 @@
                     else:
                         times.append(t)
         times.append(self._eod_valuation_time())
         times = list(dict.fromkeys(times))
 
         for d in dates:
             if isinstance(d, dt.datetime):
-                if self.calendars == 'Weekend' or is_business_day(d.date(), self.calendars):
+                if self.calendars is None or is_business_day(d.date(), self.calendars):
                     all_times.append(d)
                     for t in times:
                         if d.tzinfo is not None and d.tzinfo.utcoffset(d) is not None:
                             all_times.append(d.tzinfo.localize(dt.datetime.combine(d.date(), t)))
             else:
-                if self.calendars == 'Weekend' or is_business_day(d, self.calendars):
+                if self.calendars is None or is_business_day(d, self.calendars):
                     for t in times:
                         all_times.append(dt.datetime.combine(d, t))
         all_times = list(set(all_times))
         all_times.sort()
         return all_times
 
     def _adjust_date(self, date):
```

### Comparing `gs_quant-1.0.7/gs_quant/backtests/strategy.py` & `gs_quant-1.0.8/gs_quant/backtests/strategy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/strategy_systematic.py` & `gs_quant-1.0.8/gs_quant/backtests/strategy_systematic.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/backtests/triggers.py` & `gs_quant-1.0.8/gs_quant/backtests/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,14 +407,15 @@
                 return TriggerInfo(True, {AddTradeAction: AddTradeActionInfo(scaling=-1)})
         elif self._current_position == -1:
             if current_price > rolling_mean:
                 self._current_position = 0
                 return TriggerInfo(True, {AddTradeAction: AddTradeActionInfo(scaling=1)})
         else:
             raise RuntimeWarning(f'unexpected current position: {self._current_position}')
+        return TriggerInfo(False)
 
 
 class OrdersGeneratorTrigger(Trigger):
     """Base class for triggers used with the PredefinedAssetEngine."""
     def __init__(self):
         super().__init__(None, Action())
```

### Comparing `gs_quant-1.0.7/gs_quant/base.py` & `gs_quant-1.0.8/gs_quant/base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/common.py` & `gs_quant-1.0.8/gs_quant/common.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/config/__init__.py` & `gs_quant-1.0.8/gs_quant/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/config/options.py` & `gs_quant-1.0.8/gs_quant/config/options.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/config.ini` & `gs_quant-1.0.8/gs_quant/config.ini`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py` & `gs_quant-1.0.8/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/context_base.py` & `gs_quant-1.0.8/gs_quant/context_base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/__init__.py` & `gs_quant-1.0.8/gs_quant/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/coordinate.py` & `gs_quant-1.0.8/gs_quant/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/core.py` & `gs_quant-1.0.8/gs_quant/data/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/dataset.py` & `gs_quant-1.0.8/gs_quant/data/dataset.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/fields.py` & `gs_quant-1.0.8/gs_quant/data/fields.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/log.py` & `gs_quant-1.0.8/gs_quant/data/log.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/query.py` & `gs_quant-1.0.8/gs_quant/data/query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/data/stream.py` & `gs_quant-1.0.8/gs_quant/data/stream.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/datetime/__init__.py` & `gs_quant-1.0.8/gs_quant/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/datetime/date.py` & `gs_quant-1.0.8/gs_quant/datetime/date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/datetime/gscalendar.py` & `gs_quant-1.0.8/gs_quant/datetime/gscalendar.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/datetime/point.py` & `gs_quant-1.0.8/gs_quant/datetime/point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/datetime/relative_date.py` & `gs_quant-1.0.8/gs_quant/datetime/relative_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/datetime/rules.py` & `gs_quant-1.0.8/gs_quant/datetime/rules.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/datetime/time.py` & `gs_quant-1.0.8/gs_quant/datetime/time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.business_day_count.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.business_day_count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.date_range.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.is_business_day.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.is_business_day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.add.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.add.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.and_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.and_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.divide.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.divide.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.exp.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.exp.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.floor.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.floor.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.if_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.if_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.log.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.log.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.not_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.not_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.or_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.or_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.power.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.power.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.count.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.diff.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.diff.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.first.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.first.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.lag.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.lag.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.last.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.last.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.align.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.align.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.day.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.month.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.month.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.union.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.union.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.value.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.datetime.year.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.datetime.year.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.change.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.change.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.index.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.cov.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.cov.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.max_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.max_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.mean.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.mean.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.median.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.median.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.min_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.min_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.mode.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.mode.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.product.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.product.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.range_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.range_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.std.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.var.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.var.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html` & `gs_quant-1.0.8/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/entities/entitlements.py` & `gs_quant-1.0.8/gs_quant/entities/entitlements.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/entities/entity.py` & `gs_quant-1.0.8/gs_quant/entities/entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/entities/tree_entity.py` & `gs_quant-1.0.8/gs_quant/entities/tree_entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/errors.py` & `gs_quant-1.0.8/gs_quant/errors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/instrument/__init__.py` & `gs_quant-1.0.8/gs_quant/instrument/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/instrument/core.py` & `gs_quant-1.0.8/gs_quant/instrument/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/instrument/overrides.py` & `gs_quant-1.0.8/gs_quant/instrument/overrides.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/json_convertors.py` & `gs_quant-1.0.8/gs_quant/json_convertors.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,19 @@
 optional_date_config = config(encoder=encode_date_or_str, decoder=decode_optional_date)
 
 
 def decode_dict_date_key(value):
     return {dt.date.fromisoformat(d): v for d, v in value.items()} if value is not None else None
 
 
+def decode_dict_dict_date_key(value):
+    return {k: {dt.date.fromisoformat(d): v for d, v in val.items()} if val is not None else None
+            for k, val in value.items()} if value is not None else None
+
+
 def decode_dict_date_value(value):
     return {k: dt.date.fromisoformat(d) for k, d in value.items()} if value is not None else None
 
 
 def decode_datetime_tuple(blob: Tuple[str]):
     return tuple(optional_from_isodatetime(s) for s in blob) if isinstance(blob, (tuple, list)) else None
```

### Comparing `gs_quant-1.0.7/gs_quant/json_encoder.py` & `gs_quant-1.0.8/gs_quant/json_encoder.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/__init__.py` & `gs_quant-1.0.8/gs_quant/markets/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/baskets.py` & `gs_quant-1.0.8/gs_quant/markets/baskets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/core.py` & `gs_quant-1.0.8/gs_quant/markets/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/factor.py` & `gs_quant-1.0.8/gs_quant/markets/factor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/hedge.py` & `gs_quant-1.0.8/gs_quant/markets/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/historical.py` & `gs_quant-1.0.8/gs_quant/markets/historical.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/index.py` & `gs_quant-1.0.8/gs_quant/markets/index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/indices_utils.py` & `gs_quant-1.0.8/gs_quant/markets/indices_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/markets.py` & `gs_quant-1.0.8/gs_quant/markets/markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/optimizer.py` & `gs_quant-1.0.8/gs_quant/markets/optimizer.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/portfolio.py` & `gs_quant-1.0.8/gs_quant/markets/portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/portfolio_manager.py` & `gs_quant-1.0.8/gs_quant/markets/portfolio_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 from gs_quant.entities.entitlements import Entitlements
 from gs_quant.entities.entity import PositionedEntity, EntityType
 from gs_quant.errors import MqError
 from gs_quant.errors import MqValueError
 from gs_quant.markets.factor import Factor
 from gs_quant.markets.portfolio_manager_utils import build_exposure_df, build_portfolio_constituents_df, \
     build_sensitivity_df
-from gs_quant.markets.report import PerformanceReport
-from gs_quant.markets.report import ReportJobFuture
+from gs_quant.markets.report import PerformanceReport, ReportJobFuture
 from gs_quant.models.risk_model import MacroRiskModel, ReturnFormat, FactorType
 from gs_quant.target.common import Currency
 from gs_quant.target.portfolios import RiskAumSource
 
 _logger = logging.getLogger(__name__)
 
 
+@deprecation.deprecated(deprecated_in='1.0.10',
+                        details='portfolio_manager.CustomAUMDataPoint is now deprecated, please use '
+                                'report.CustomAUMDataPoint instead.')
 class CustomAUMDataPoint:
     """
 
     Custom AUM Data Point represents a portfolio's AUM value for a specific date
 
     """
 
@@ -324,49 +326,61 @@
         Get recommended start and end dates for a portfolio report scheduling job
 
         :param backcast: true if reports should be backcasted
         :return: a list of two dates, the first is the suggested start date and the second is the suggested end date
         """
         return GsPortfolioApi.get_schedule_dates(self.id, backcast)
 
+    @deprecation.deprecated(deprecated_in='1.0.10',
+                            details='PortfolioManager.get_aum_source is now deprecated, please use '
+                                    'PerformanceReport.get_aum_source instead.')
     def get_aum_source(self) -> RiskAumSource:
         """
         Get portfolio AUM Source
 
         :return: aum source
         """
         portfolio = GsPortfolioApi.get_portfolio(self.portfolio_id)
         return portfolio.aum_source if portfolio.aum_source is not None else RiskAumSource.Long
 
+    @deprecation.deprecated(deprecated_in='1.0.10',
+                            details='PortfolioManager.set_aum_source is now deprecated, please use '
+                                    'PerformanceReport.set_aum_source instead.')
     def set_aum_source(self,
                        aum_source: RiskAumSource):
         """
         Set portfolio AUM Source
 
         :param aum_source: aum source for portfolio
         :return: aum source
         """
         portfolio = GsPortfolioApi.get_portfolio(self.portfolio_id)
         portfolio.aum_source = aum_source
         GsPortfolioApi.update_portfolio(portfolio)
 
+    @deprecation.deprecated(deprecated_in='1.0.10',
+                            details='PortfolioManager.get_custom_aum is now deprecated, please use '
+                                    'PerformanceReport.get_custom_aum instead.')
     def get_custom_aum(self,
                        start_date: dt.date = None,
                        end_date: dt.date = None) -> List[CustomAUMDataPoint]:
         """
         Get AUM data for portfolio
 
         :param start_date: start date
         :param end_date: end date
         :return: list of AUM data between the specified range
         """
         aum_data = GsPortfolioApi.get_custom_aum(self.portfolio_id, start_date, end_date)
         return [CustomAUMDataPoint(date=dt.datetime.strptime(data['date'], '%Y-%m-%d'),
                                    aum=data['aum']) for data in aum_data]
 
+    @deprecation.deprecated(deprecated_in='1.0.10',
+                            details='PortfolioManager.get_aum is now deprecated, please use '
+                                    'PerformanceReport.get_aum instead.')
     def get_aum(self,
                 start_date: dt.date,
                 end_date: dt.date):
         """
         Get AUM data for portfolio
 
         :param start_date: start date
@@ -386,14 +400,17 @@
         if aum_source == RiskAumSource.Gross:
             aum = self.get_performance_report().get_gross_exposure(start_date=start_date, end_date=end_date)
             return {row['date']: row['grossExposure'] for index, row in aum.iterrows()}
         if aum_source == RiskAumSource.Net:
             aum = self.get_performance_report().get_net_exposure(start_date=start_date, end_date=end_date)
             return {row['date']: row['netExposure'] for index, row in aum.iterrows()}
 
+    @deprecation.deprecated(deprecated_in='1.0.10',
+                            details='PortfolioManager.upload_custom_aum is now deprecated, please use '
+                                    'PerformanceReport.upload_custom_aum instead.')
     def upload_custom_aum(self,
                           aum_data: List[CustomAUMDataPoint],
                           clear_existing_data: bool = None):
         """
         Add AUM data for portfolio
 
         :param aum_data: list of AUM data to upload
```

### Comparing `gs_quant-1.0.7/gs_quant/markets/portfolio_manager_utils.py` & `gs_quant-1.0.8/gs_quant/markets/portfolio_manager_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/position_set.py` & `gs_quant-1.0.8/gs_quant/markets/position_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,15 +550,15 @@
         """ Create PostionSet instance from PostionSet type defined in target file """
         positions = position_set.positions
         mqids = [position.asset_id for position in positions]
         position_data = cls.__get_positions_data(mqids)
         converted_positions = []
         for p in positions:
             asset = get(position_data, p.asset_id)
-            tags = {t.name: t.value for t in p.tags} if p.tags else None
+            tags = p.tags if p.tags else None
             position = Position(identifier=get(asset, 'bbid'), name=get(asset, 'name'),
                                 asset_id=p.asset_id, quantity=p.quantity, tags=tags)
             converted_positions.append(position)
         return cls(converted_positions, position_set.position_date, position_set.divisor)
 
     @classmethod
     def from_list(cls, positions: List[str], date: datetime.date = datetime.date.today()):
```

### Comparing `gs_quant-1.0.7/gs_quant/markets/report.py` & `gs_quant-1.0.8/gs_quant/markets/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 specific language governing permissions and limitations
 under the License.
 """
 import datetime as dt
 from enum import Enum, auto
 from time import sleep
 from typing import Tuple, Union, List, Dict
+import scipy.stats as st
 
 import pandas as pd
 from dateutil.relativedelta import relativedelta
 from inflection import titleize
 
 from gs_quant.api.gs.data import GsDataApi
 from gs_quant.api.gs.portfolios import GsPortfolioApi
@@ -29,14 +30,15 @@
 from gs_quant.datetime import business_day_offset
 from gs_quant.errors import MqValueError
 from gs_quant.markets.report_utils import _get_ppaa_batches
 from gs_quant.target.common import ReportParameters, Currency
 from gs_quant.target.coordinates import MDAPIDataBatchResponse
 from gs_quant.target.data import DataQuery, DataQueryResponse
 from gs_quant.target.reports import Report as TargetReport, ReportType, PositionSourceType, ReportStatus
+from gs_quant.target.portfolios import RiskAumSource
 
 
 class ReturnFormat(Enum):
     """Alternative format for data to be returned from get_data functions"""
     JSON = auto()
     DATA_FRAME = auto()
 
@@ -71,14 +73,44 @@
 
 
 class AttributionAggregationType(Enum):
     Arithmetic = 'arithmetic'
     Geometric = 'geometric'
 
 
+class CustomAUMDataPoint:
+    """
+
+    Custom AUM Data Point represents a portfolio's AUM value for a specific date
+
+    """
+
+    def __init__(self,
+                 date: dt.date,
+                 aum: float):
+        self.__date = date
+        self.__aum = aum
+
+    @property
+    def date(self) -> dt.date:
+        return self.__date
+
+    @date.setter
+    def date(self, value: dt.date):
+        self.__date = value
+
+    @property
+    def aum(self) -> float:
+        return self.__aum
+
+    @aum.setter
+    def aum(self, value: float):
+        self.__aum = value
+
+
 class ReportJobFuture:
     """Report job future that monitors report status and results"""
     def __init__(self,
                  report_id: str,
                  job_id: str,
                  report_type: ReportType,
                  start_date: dt.date,
@@ -623,14 +655,88 @@
             measures = []
         fields = tuple(measure for measure in measures)
         where = {'reportId': self.id}
         query = DataQuery(where=where, fields=fields, start_date=start_date, end_date=end_date)
         results = GsDataApi.query_data(query=query, dataset_id=ReportDataset.PPA_DATASET.value)
         return pd.DataFrame(results) if return_format == ReturnFormat.DATA_FRAME else results
 
+    def get_aum_source(self) -> RiskAumSource:
+        """
+        Get AUM Source for the portfolio associated with the performance report
+
+        :return: aum source
+        """
+        portfolio = GsPortfolioApi.get_portfolio(self.position_source_id)
+        return portfolio.aum_source if portfolio.aum_source is not None else RiskAumSource.Long
+
+    def set_aum_source(self,
+                       aum_source: RiskAumSource):
+        """
+        Set AUM Source for the portfolio associated with the performance report
+
+        :param aum_source: aum source for portfolio
+        :return: aum source
+        """
+        portfolio = GsPortfolioApi.get_portfolio(self.position_source_id)
+        portfolio.aum_source = aum_source
+        GsPortfolioApi.update_portfolio(portfolio)
+
+    def get_custom_aum(self,
+                       start_date: dt.date = None,
+                       end_date: dt.date = None) -> List[CustomAUMDataPoint]:
+        """
+        Get AUM data for performance report
+
+        :param start_date: start date
+        :param end_date: end date
+        :return: list of AUM data between the specified range
+        """
+        aum_data = GsReportApi.get_custom_aum(self.id, start_date, end_date)
+        return [CustomAUMDataPoint(date=dt.datetime.strptime(data['date'], '%Y-%m-%d'),
+                                   aum=data['aum']) for data in aum_data]
+
+    def get_aum(self,
+                start_date: dt.date,
+                end_date: dt.date):
+        """
+        Get AUM data for performance report
+
+        :param start_date: start date
+        :param end_date: end date
+        :return: dictionary of dates with corresponding AUM values
+        """
+        aum_source = self.get_aum_source()
+        if aum_source == RiskAumSource.Custom_AUM:
+            aum = self.get_custom_aum(start_date=start_date, end_date=end_date)
+            return {aum_point.date.strftime('%Y-%m-%d'): aum_point.aum for aum_point in aum}
+        if aum_source == RiskAumSource.Long:
+            aum = self.get_long_exposure(start_date=start_date, end_date=end_date)
+            return {row['date']: row['longExposure'] for index, row in aum.iterrows()}
+        if aum_source == RiskAumSource.Short:
+            aum = self.get_short_exposure(start_date=start_date, end_date=end_date)
+            return {row['date']: row['shortExposure'] for index, row in aum.iterrows()}
+        if aum_source == RiskAumSource.Gross:
+            aum = self.get_gross_exposure(start_date=start_date, end_date=end_date)
+            return {row['date']: row['grossExposure'] for index, row in aum.iterrows()}
+        if aum_source == RiskAumSource.Net:
+            aum = self.get_net_exposure(start_date=start_date, end_date=end_date)
+            return {row['date']: row['netExposure'] for index, row in aum.iterrows()}
+
+    def upload_custom_aum(self,
+                          aum_data: List[CustomAUMDataPoint],
+                          clear_existing_data: bool = None):
+        """
+        Add AUM data for portfolio corresponding to the performance report
+
+        :param aum_data: list of AUM data to upload
+        :param clear_existing_data: delete all previously uploaded AUM data for the portfolio (defaults to false)
+        """
+        formatted_aum_data = [{'date': data.date.strftime('%Y-%m-%d'), 'aum': data.aum} for data in aum_data]
+        GsReportApi.upload_custom_aum(self.id, formatted_aum_data, clear_existing_data)
+
     def get_positions_data(self,
                            start: dt.date = None,
                            end: dt.date = dt.date.today(),
                            fields: [str] = None,
                            include_all_business_days: bool = False) -> List[Dict]:
         return GsPortfolioApi.get_positions_data(self.position_source_id,
                                                  start,
@@ -1070,15 +1176,15 @@
                         factor_names: List[str] = None,
                         start_date: dt.date = None,
                         end_date: dt.date = None,
                         currency: Currency = None) -> pd.DataFrame:
         """
         Get historical annual risk
 
-        :param factor_names: optional list of factor names; must be from the following: "Factor", "Specific", "Total
+        :param factor_names: optional list of factor names; must be from the following: "Factor", "Specific", "Total"
         :param start_date: start date
         :param end_date: end date
         :param currency: currency
         :return: a Pandas DataFrame with the results
         """
         factor_data = self.get_results(factors=factor_names,
                                        start_date=start_date,
@@ -1091,27 +1197,51 @@
                        factor_names: List[str] = None,
                        start_date: dt.date = None,
                        end_date: dt.date = None,
                        currency: Currency = None) -> pd.DataFrame:
         """
         Get historical daily risk
 
-        :param factor_names: optional list of factor names; must be from the following: "Factor", "Specific", "Total
+        :param factor_names: optional list of factor names; must be from the following: "Factor", "Specific", "Total"
         :param start_date: start date
         :param end_date: end date
         :param currency: currency
         :return: a Pandas DataFrame with the results
         """
         factor_data = self.get_results(factors=factor_names,
                                        start_date=start_date,
                                        end_date=end_date,
                                        currency=currency,
                                        return_format=ReturnFormat.JSON)
         return _format_multiple_factor_table(factor_data, 'dailyRisk')
 
+    def get_ex_ante_var(self,
+                        confidence_interval: float = 95.0,
+                        start_date: dt.date = None,
+                        end_date: dt.date = None,
+                        currency: Currency = None) -> pd.DataFrame:
+        """
+        Get ex-ante Value at Risk as defined by the risk model
+
+        :param confidence_interval: the VaR confidence interval as a percent
+        :param start_date: start date
+        :param end_date: end date
+        :param currency: currency
+        :return: a Pandas DataFrame with the results
+        """
+        factor_data = self.get_results(factors=['Total'],
+                                       start_date=start_date,
+                                       end_date=end_date,
+                                       currency=currency,
+                                       return_format=ReturnFormat.JSON)
+        z_score = st.norm.ppf(confidence_interval / 100)
+        for data in factor_data:
+            data['var'] = data['dailyRisk'] * z_score
+        return _format_multiple_factor_table(factor_data, 'var')
+
 
 def _format_multiple_factor_table(factor_data: List[Dict],
                                   key: str) -> pd.DataFrame:
     formatted_data = {}
     for data in factor_data:
         date = data['date']
         if date in formatted_data:
```

### Comparing `gs_quant-1.0.7/gs_quant/markets/report_utils.py` & `gs_quant-1.0.8/gs_quant/markets/report_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/screens.py` & `gs_quant-1.0.8/gs_quant/markets/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/markets/securities.py` & `gs_quant-1.0.8/gs_quant/markets/securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/models/__init__.py` & `gs_quant-1.0.8/gs_quant/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/models/epidemiology.py` & `gs_quant-1.0.8/gs_quant/models/epidemiology.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/models/risk_model.py` & `gs_quant-1.0.8/gs_quant/models/risk_model.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/models/risk_model_utils.py` & `gs_quant-1.0.8/gs_quant/models/risk_model_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/priceable.py` & `gs_quant-1.0.8/gs_quant/priceable.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/quote_reports/core.py` & `gs_quant-1.0.8/gs_quant/quote_reports/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/risk/__init__.py` & `gs_quant-1.0.8/gs_quant/risk/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/risk/core.py` & `gs_quant-1.0.8/gs_quant/risk/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,27 +362,27 @@
 
 
 @dataclass_json
 @dataclass
 class MQVSValidationTarget:
     env: Optional[str] = None
     operator: Optional[str] = None
-    mqGroups: Optional[Tuple[str]] = None
+    mqGroups: Optional[Tuple[str, ...]] = None
     users: Optional[Tuple[str]] = None
-    assetClasses: Optional[Tuple[str]] = None
-    assets: Optional[Tuple[str]] = None
-    legTypes: Optional[Tuple[str]] = None
+    assetClasses: Optional[Tuple[str, ...]] = None
+    assets: Optional[Tuple[str, ...]] = None
+    legTypes: Optional[Tuple[str, ...]] = None
     legFields: Optional[Dict[str, str]] = None
 
 
 @dataclass_json
 @dataclass
 class MQVSValidatorDefn:
     validatorType: str
-    targets: Tuple[MQVSValidationTarget]
+    targets: Tuple[MQVSValidationTarget, ...]
     args: Dict[str, str]
     groupId: Optional[str] = None
     groupIndex: Optional[int] = None
     groupMethod: Optional[str] = None
 
 class MQVSValidatorDefnsWithInfo(ResultInfo):
     validators: Tuple[MQVSValidatorDefn]
```

### Comparing `gs_quant-1.0.7/gs_quant/risk/measures.py` & `gs_quant-1.0.8/gs_quant/risk/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/risk/result_handlers.py` & `gs_quant-1.0.8/gs_quant/risk/result_handlers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/risk/results.py` & `gs_quant-1.0.8/gs_quant/risk/results.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/risk/scenario_utils.py` & `gs_quant-1.0.8/gs_quant/risk/scenario_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/risk/scenarios.py` & `gs_quant-1.0.8/gs_quant/risk/scenarios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/risk/transform.py` & `gs_quant-1.0.8/gs_quant/risk/transform.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/session.py` & `gs_quant-1.0.8/gs_quant/session.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/__init__.py` & `gs_quant-1.0.8/gs_quant/target/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/assets.py` & `gs_quant-1.0.8/gs_quant/target/assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/assets_screener.py` & `gs_quant-1.0.8/gs_quant/target/assets_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/backtests.py` & `gs_quant-1.0.8/gs_quant/target/backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/base_screener.py` & `gs_quant-1.0.8/gs_quant/target/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/charts.py` & `gs_quant-1.0.8/gs_quant/target/charts.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/common.py` & `gs_quant-1.0.8/gs_quant/target/common.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/content.py` & `gs_quant-1.0.8/gs_quant/target/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/coordinates.py` & `gs_quant-1.0.8/gs_quant/target/coordinates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/countries.py` & `gs_quant-1.0.8/gs_quant/target/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/data.py` & `gs_quant-1.0.8/gs_quant/target/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/data_screen.py` & `gs_quant-1.0.8/gs_quant/target/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/groups.py` & `gs_quant-1.0.8/gs_quant/target/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/hedge.py` & `gs_quant-1.0.8/gs_quant/target/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/indices.py` & `gs_quant-1.0.8/gs_quant/target/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/instrument.py` & `gs_quant-1.0.8/gs_quant/target/instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/measures.py` & `gs_quant-1.0.8/gs_quant/target/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/monitor.py` & `gs_quant-1.0.8/gs_quant/target/monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/portfolios.py` & `gs_quant-1.0.8/gs_quant/target/portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/positions_v2_pricing.py` & `gs_quant-1.0.8/gs_quant/target/positions_v2_pricing.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/price.py` & `gs_quant-1.0.8/gs_quant/target/price.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/reports.py` & `gs_quant-1.0.8/gs_quant/target/reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     Basket_Rebalance_Auto_Approval = 'Basket Rebalance Auto Approval'
     Scenario = 'Scenario'
     Iselect_Backtest = 'Iselect Backtest'
     Backtest_Run = 'Backtest Run'
     Analytics = 'Analytics'
     Risk_Calculation = 'Risk Calculation'
     Factor_Overview_Email = 'Factor Overview Email'
-    PCO = 'PCO'    
+    PCO = 'PCO'
 
 
 @handle_camel_case_args
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(unsafe_hash=True, repr=False)
 class ParametersOverrides(Base):
     csa_term: Optional[str] = field(default=None, metadata=field_metadata)
```

### Comparing `gs_quant-1.0.7/gs_quant/target/risk.py` & `gs_quant-1.0.8/gs_quant/target/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/risk_models.py` & `gs_quant-1.0.8/gs_quant/target/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/screens.py` & `gs_quant-1.0.8/gs_quant/target/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/secmaster.py` & `gs_quant-1.0.8/gs_quant/target/secmaster.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/trades.py` & `gs_quant-1.0.8/gs_quant/target/trades.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/workflow_quote.py` & `gs_quant-1.0.8/gs_quant/target/workflow_quote.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/target/workspaces_markets.py` & `gs_quant-1.0.8/gs_quant/target/workspaces_markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/analytics/test_datagrid.py` & `gs_quant-1.0.8/gs_quant/test/analytics/test_datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/analytics/test_sorting_and_filtering.py` & `gs_quant-1.0.8/gs_quant/test/analytics/test_sorting_and_filtering.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/analytics/test_workspace.py` & `gs_quant-1.0.8/gs_quant/test/analytics/test_workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_assets.py` & `gs_quant-1.0.8/gs_quant/test/api/test_assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_backtests.py` & `gs_quant-1.0.8/gs_quant/test/api/test_backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_base_screener.py` & `gs_quant-1.0.8/gs_quant/test/api/test_base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_cache.py` & `gs_quant-1.0.8/gs_quant/test/api/test_cache.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_carbon.py` & `gs_quant-1.0.8/gs_quant/test/api/test_carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_content.py` & `gs_quant-1.0.8/gs_quant/test/api/test_content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_data.py` & `gs_quant-1.0.8/gs_quant/test/api/test_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_data_screen.py` & `gs_quant-1.0.8/gs_quant/test/api/test_data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_esg.py` & `gs_quant-1.0.8/gs_quant/test/api/test_esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_fred.py` & `gs_quant-1.0.8/gs_quant/test/api/test_fred.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_groups.py` & `gs_quant-1.0.8/gs_quant/test/api/test_groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_index.py` & `gs_quant-1.0.8/gs_quant/test/api/test_index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_instruments.py` & `gs_quant-1.0.8/gs_quant/test/api/test_instruments.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_json.py` & `gs_quant-1.0.8/gs_quant/test/api/test_json.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_monitor.py` & `gs_quant-1.0.8/gs_quant/test/api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_portfolios.py` & `gs_quant-1.0.8/gs_quant/test/api/test_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_reports.py` & `gs_quant-1.0.8/gs_quant/test/api/test_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_risk.py` & `gs_quant-1.0.8/gs_quant/test/api/test_risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_risk_models.py` & `gs_quant-1.0.8/gs_quant/test/api/test_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_target.py` & `gs_quant-1.0.8/gs_quant/test/api/test_target.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_thread_manager.py` & `gs_quant-1.0.8/gs_quant/test/api/test_thread_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/api/test_users.py` & `gs_quant-1.0.8/gs_quant/test/api/test_users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/backtest/test_backtest_eq_vol_engine.py` & `gs_quant-1.0.8/gs_quant/test/backtest/test_backtest_eq_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/backtest/test_backtest_flow_vol.py` & `gs_quant-1.0.8/gs_quant/test/backtest/test_backtest_flow_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/backtest/test_backtest_predefined.py` & `gs_quant-1.0.8/gs_quant/test/backtest/test_backtest_predefined.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                                  ValuationFixingType.PRICE)
     data_manager.add_data_source(s_eod, DataFrequency.DAILY, generic_bond_future,
                                  ValuationFixingType.PRICE)
 
     # instantiate a new strategy
     strategy = Strategy(None, triggers=simple_date_trigger)
 
-    engine = PredefinedAssetEngine(data_mgr=data_manager, tz=timezone(tz), calendars='Weekend')
+    engine = PredefinedAssetEngine(data_mgr=data_manager, tz=timezone(tz))
     backtest = engine.run_backtest(strategy=strategy, start=states[0], end=states[-1], states=states)
     assert len(backtest.trade_ledger()) == 364
 
 
 def test_backtest_predefined():
     # Test simple MOC order
     trigger = ExampleTestTrigger()
```

### Comparing `gs_quant-1.0.7/gs_quant/test/backtest/test_generic_engine.py` & `gs_quant-1.0.8/gs_quant/test/backtest/test_generic_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/backtest/test_triggers.py` & `gs_quant-1.0.8/gs_quant/test/backtest/test_triggers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/data/test_data_coordinate.py` & `gs_quant-1.0.8/gs_quant/test/data/test_data_coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/data/test_dataset.py` & `gs_quant-1.0.8/gs_quant/test/data/test_dataset.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/datetime_/test_date.py` & `gs_quant-1.0.8/gs_quant/test/datetime_/test_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/datetime_/test_gscalendar.py` & `gs_quant-1.0.8/gs_quant/test/datetime_/test_gscalendar.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/datetime_/test_point.py` & `gs_quant-1.0.8/gs_quant/test/datetime_/test_point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/datetime_/test_relative_date.py` & `gs_quant-1.0.8/gs_quant/test/datetime_/test_relative_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/datetime_/test_time.py` & `gs_quant-1.0.8/gs_quant/test/datetime_/test_time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/fixtures/content.py` & `gs_quant-1.0.8/gs_quant/test/fixtures/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_baskets.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_baskets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_hedger.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_hedger.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_instrument.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_portfolio.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_portfolio_manager.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_pricing_context.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_pricing_context.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_report.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 
 import datetime as dt
 
 import pytest
 
 from gs_quant.api.gs.data import GsDataApi
 from gs_quant.api.gs.thematics import GsThematicApi
+from gs_quant.api.gs.portfolios import Portfolio
 from gs_quant.markets.report import FactorRiskReport, PerformanceReport, ThematicReport, flatten_results_into_df
 from gs_quant.session import *
-from gs_quant.target.reports import ReportStatus, PositionSourceType, ReportType, ReportParameters, Report
+from gs_quant.target.reports import *
+from gs_quant.target.portfolios import RiskAumSource
 
 fake_pfr = FactorRiskReport(risk_model_id='AXUS4M',
                             fx_hedged=True,
                             report_id='PFRID',
                             position_source_type=PositionSourceType.Portfolio,
                             position_source_id='PORTFOLIOID',
                             report_type=ReportType.Portfolio_Factor_Risk,
@@ -113,14 +115,63 @@
         "region": "Asia",
         "grossExposure": 3.274071805135091E8,
         "thematicExposure": 9.706991264825605E7,
         "updateTime": "2021-07-20T23:43:38Z"
     }
 ]
 
+custom_aum = {
+    'data': [
+        {
+            'date': '2023-06-01',
+            'aum': 100
+        },
+        {
+            'date': '2023-06-02',
+            'aum': 100
+        },
+        {
+            'date': '2023-06-05',
+            'aum': 100
+        },
+        {
+            'date': '2023-06-06',
+            'aum': 100
+        }
+    ]
+}
+
+ppa_data = [
+    {
+        'date': "2023-06-01",
+        'reportId': "PPAID",
+        'netExposure': 2414214.74
+    },
+    {
+        'date': "2023-06-02",
+        'reportId': "PPAID",
+        'netExposure': 2414214.74
+    },
+    {
+        'date': "2023-06-05",
+        'reportId': "PPAID",
+        'netExposure': 2414214.74
+    },
+    {
+        'date': "2023-06-06",
+        'reportId': "PPAID",
+        'netExposure': 2414214.74
+    },
+    {
+        'date': "2023-06-07",
+        'reportId': "PPAID",
+        'netExposure': 2414214.74
+    }
+]
+
 
 def test_get_performance_report(mocker):
     # mock GsSession
     mocker.patch.object(
         GsSession.__class__,
         'default_value',
         return_value=GsSession.get(
@@ -135,14 +186,65 @@
                                             type=ReportType.Portfolio_Performance_Analytics,
                                             status=ReportStatus.done))
     # run test
     response = PerformanceReport.get('PPAID')
     assert response.type == ReportType.Portfolio_Performance_Analytics
 
 
+def test_get_aum_source(mocker):
+    portfolio = Portfolio(id='MP123', currency='USD', name='Example Port', aum_source=RiskAumSource.Gross)
+    # mock GsSession
+    mocker.patch.object(
+        GsSession.__class__,
+        'default_value',
+        return_value=GsSession.get(
+            Environment.QA,
+            'client_id',
+            'secret'))
+    mocker.patch.object(GsSession.current, '_get', return_value=portfolio)
+
+    # run test
+    response = fake_ppa.get_aum_source()
+    assert response == RiskAumSource.Gross
+
+
+def test_get_custom_aum(mocker):
+    # mock GsSession
+    mocker.patch.object(
+        GsSession.__class__,
+        'default_value',
+        return_value=GsSession.get(
+            Environment.QA,
+            'client_id',
+            'secret'))
+    mocker.patch.object(GsSession.current, '_get', return_value=custom_aum)
+
+    # run test
+    response = fake_ppa.get_custom_aum()
+    assert len(response) == 4
+
+
+def test_get_aum(mocker):
+    portfolio = Portfolio(id='MP123', currency='USD', name='Example Port', aum_source=RiskAumSource.Net)
+    # mock GsSession
+    mocker.patch.object(
+        GsSession.__class__,
+        'default_value',
+        return_value=GsSession.get(
+            Environment.QA,
+            'client_id',
+            'secret'))
+    mocker.patch.object(GsSession.current, '_get', return_value=portfolio)
+    mocker.patch.object(GsDataApi, 'query_data', return_value=ppa_data)
+
+    # run test
+    response = fake_ppa.get_aum(start_date=dt.date(2023, 6, 1), end_date=dt.date(2023, 6, 7))
+    assert len(response) == 5
+
+
 def test_get_risk_model_id():
     assert fake_pfr.get_risk_model_id() == 'AXUS4M'
 
 
 def test_set_position_target():
     factor_report = FactorRiskReport(report_id='PFRID',
                                      position_source_type=PositionSourceType.Portfolio,
```

### Comparing `gs_quant-1.0.7/gs_quant/test/markets/test_securities.py` & `gs_quant-1.0.8/gs_quant/test/markets/test_securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/models/__init__.py` & `gs_quant-1.0.8/gs_quant/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/models/test_epidemiology.py` & `gs_quant-1.0.8/gs_quant/test/models/test_epidemiology.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/models/test_risk_model.py` & `gs_quant-1.0.8/gs_quant/test/models/test_risk_model.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/test_base.py` & `gs_quant-1.0.8/gs_quant/test/test_base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/test_session.py` & `gs_quant-1.0.8/gs_quant/test/test_session.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/multi_measure/test_commod.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/multi_measure/test_commod.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/multi_measure/test_measure_registry.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/multi_measure/test_measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_algebra.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_analysis.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_analysis.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_backtesting.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_backtesting.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_datetime.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_datetime.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_econometrics.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_econometrics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_helper.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_countries.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_fx_vol.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_fx_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_inflation.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_portfolios.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_rates.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_rates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_reports.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 from testfixtures.mock import Mock
 
 import gs_quant.timeseries.measures_reports as mr
 from gs_quant.api.gs.assets import GsTemporalXRef
 from gs_quant.api.gs.data import MarketDataResponseFrame
 from gs_quant.data.core import DataContext
 from gs_quant.errors import MqValueError
-from gs_quant.markets.portfolio_manager import CustomAUMDataPoint
-from gs_quant.markets.report import PerformanceReport, ThematicReport
+from gs_quant.markets.report import PerformanceReport, ThematicReport, CustomAUMDataPoint
 from gs_quant.markets.securities import Stock
 from gs_quant.models.risk_model import FactorRiskModel as Factor_Risk_Model
 from gs_quant.target.common import ReportParameters, XRef
 from gs_quant.target.portfolios import RiskAumSource
 from gs_quant.target.reports import Report, PositionSourceType, ReportType
 from gs_quant.target.risk_models import RiskModel, RiskModelCoverage, RiskModelTerm, RiskModelUniverseIdentifier
 
@@ -49,20 +48,20 @@
 asset_factor_risk_report = Report(position_source_id='position source id',
                                   position_source_type=PositionSourceType.Asset,
                                   type_=ReportType.Portfolio_Factor_Risk,
                                   id_='report_id',
                                   parameters=ReportParameters(risk_model='risk_model_id'),
                                   status='new')
 
-ppa_report = Report(position_source_id='position source id',
-                    position_source_type=PositionSourceType.Portfolio,
-                    type_=ReportType.Portfolio_Performance_Analytics,
-                    id_='report_id',
-                    parameters=ReportParameters(risk_model='risk_model_id'),
-                    status='new')
+ppa_report = PerformanceReport(position_source_id='position source id',
+                               position_source_type=PositionSourceType.Portfolio,
+                               type_=ReportType.Portfolio_Performance_Analytics,
+                               id_='report_id',
+                               parameters=ReportParameters(risk_model='risk_model_id'),
+                               status='new')
 
 factor_data = [
     {
         'date': '2020-11-23',
         'reportId': 'report_id',
         'factor': 'factor_id',
         'factorCategory': 'CNT',
@@ -409,30 +408,34 @@
     mock.return_value = [{
         'identifier': 'factor_id',
         'type': 'Factor',
         'name': 'Factor Name',
         'factorCategory': 'Factor Name'
     }]
 
+    # mock getting performance report
+    mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_performance_report', Mock())
+    mock.return_value = ppa_report
+
     # mock getting aum source
-    mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_aum_source', Mock())
+    mock = replace('gs_quant.markets.report.PerformanceReport.get_aum_source', Mock())
     mock.return_value = RiskAumSource.Custom_AUM
 
     with DataContext(datetime.date(2020, 11, 23), datetime.date(2020, 11, 25)):
         # mock getting aum
-        mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_custom_aum', Mock())
+        mock = replace('gs_quant.markets.report.PerformanceReport.get_custom_aum', Mock())
         mock.return_value = [CustomAUMDataPoint(date=datetime.date(2020, 11, 23), aum=2),
                              CustomAUMDataPoint(date=datetime.date(2020, 11, 24), aum=2),
                              CustomAUMDataPoint(date=datetime.date(2020, 11, 25), aum=2)]
         actual = mr.factor_exposure('report_id', 'Factor Name', 'Percent')
         assert all(actual.values == [-11.23 * 50, -11.24 * 50, -11.25 * 50])
 
     with pytest.raises(MqValueError):
         # mock getting aum with missing data
-        mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_custom_aum', Mock())
+        mock = replace('gs_quant.markets.report.PerformanceReport.get_custom_aum', Mock())
         mock.return_value = [CustomAUMDataPoint(date=datetime.date(2020, 11, 23), aum=2),
                              CustomAUMDataPoint(date=datetime.date(2020, 11, 25), aum=2)]
         mr.factor_exposure('report_id', 'Factor Name', 'Percent')
 
     replace.restore()
 
 
@@ -517,75 +520,75 @@
         'type': 'Factor',
         'name': 'Factor Name',
         'factorCategory': 'Factor Name'
     }]
 
     with DataContext(datetime.date(2020, 11, 23), datetime.date(2020, 11, 25)):
         # mock getting aum source
-        mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_aum_source', Mock())
+        mock = replace('gs_quant.markets.report.PerformanceReport.get_aum_source', Mock())
         mock.return_value = RiskAumSource.Long
 
         # mock getting performance report
         mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_performance_report', Mock())
         mock.return_value = PerformanceReport(id='ID')
 
         # mock getting aum
         mock = replace('gs_quant.markets.report.PerformanceReport.get_long_exposure', Mock())
         mock.return_value = pandas.DataFrame.from_dict({'date': ['2020-11-25'], 'longExposure': [100]})
         actual = mr.factor_pnl('report_id', 'Factor Name', 'Percent')
         assert all(actual.values == [11.23, 11.24, 11.25])
 
     with DataContext(datetime.date(2020, 11, 23), datetime.date(2020, 11, 25)):
         # mock getting aum source
-        mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_aum_source', Mock())
+        mock = replace('gs_quant.markets.report.PerformanceReport.get_aum_source', Mock())
         mock.return_value = RiskAumSource.Short
 
         # mock getting performance report
         mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_performance_report', Mock())
         mock.return_value = PerformanceReport(id='ID')
 
         # mock getting aum
         mock = replace('gs_quant.markets.report.PerformanceReport.get_short_exposure', Mock())
         mock.return_value = pandas.DataFrame.from_dict({'date': ['2020-11-25'], 'shortExposure': [100]})
         actual = mr.factor_pnl('report_id', 'Factor Name', 'Percent')
         assert all(actual.values == [11.23, 11.24, 11.25])
 
     with DataContext(datetime.date(2020, 11, 23), datetime.date(2020, 11, 25)):
         # mock getting aum source
-        mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_aum_source', Mock())
+        mock = replace('gs_quant.markets.report.PerformanceReport.get_aum_source', Mock())
         mock.return_value = RiskAumSource.Gross
 
         # mock getting performance report
         mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_performance_report', Mock())
         mock.return_value = PerformanceReport(id='ID')
 
         # mock getting aum
         mock = replace('gs_quant.markets.report.PerformanceReport.get_gross_exposure', Mock())
         mock.return_value = pandas.DataFrame.from_dict({'date': ['2020-11-25'], 'grossExposure': [400]})
         actual = mr.factor_pnl('report_id', 'Factor Name', 'Percent')
         assert all(actual.values == [11.23 / 4, 11.24 / 4, 11.25 / 4])
 
     with DataContext(datetime.date(2020, 11, 23), datetime.date(2020, 11, 25)):
         # mock getting aum source
-        mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_aum_source', Mock())
+        mock = replace('gs_quant.markets.report.PerformanceReport.get_aum_source', Mock())
         mock.return_value = RiskAumSource.Net
 
         # mock getting performance report
         mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_performance_report', Mock())
         mock.return_value = PerformanceReport(id='ID')
 
         # mock getting aum
         mock = replace('gs_quant.markets.report.PerformanceReport.get_net_exposure', Mock())
         mock.return_value = pandas.DataFrame.from_dict({'date': ['2020-11-25'], 'netExposure': [200]})
         actual = mr.factor_pnl('report_id', 'Factor Name', 'Percent')
         assert all(actual.values == [11.23 / 2, 11.24 / 2, 11.25 / 2])
 
     with pytest.raises(MqValueError):
         # mock getting aum source
-        mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_aum_source', Mock())
+        mock = replace('gs_quant.markets.report.PerformanceReport.get_aum_source', Mock())
         mock.return_value = RiskAumSource.Net
 
         # mock getting performance report
         mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_performance_report', Mock())
         mock.return_value = PerformanceReport(id='ID')
 
         # mock getting aum
@@ -993,15 +996,15 @@
     mock.return_value = PerformanceReport(report_id='RP1',
                                           position_source_type='Portfolio',
                                           position_source_id='MP1',
                                           report_type='Portfolio Performance Analytics',
                                           parameters=ReportParameters(transaction_cost_model='FIXED'))
 
     # mock PerformanceReport.get()
-    mock = replace('gs_quant.markets.portfolio_manager.PortfolioManager.get_aum', Mock())
+    mock = replace('gs_quant.markets.report.PerformanceReport.get_aum', Mock())
     mock.return_value = {
         '2022-07-01': 100,
         '2022-07-02': 200
     }
 
     with DataContext(datetime.date(2022, 7, 1), datetime.date(2022, 7, 3)):
         actual = mr.aum('RP1')
```

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_risk_models.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_measures_xccy.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_rolling.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_rolling.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_statistics.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_statistics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_tca.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_technicals.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_technicals.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/test_timeseries.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/timeseries/utils.py` & `gs_quant-1.0.8/gs_quant/test/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/utils/datagrid_test_utils.py` & `gs_quant-1.0.8/gs_quant/test/utils/datagrid_test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/utils/mock_calc.py` & `gs_quant-1.0.8/gs_quant/test/utils/mock_calc.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/utils/mock_data.py` & `gs_quant-1.0.8/gs_quant/test/utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/utils/mock_request.py` & `gs_quant-1.0.8/gs_quant/test/utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/test/utils/test_utils.py` & `gs_quant-1.0.8/gs_quant/test/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/__init__.py` & `gs_quant-1.0.8/gs_quant/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/algebra.py` & `gs_quant-1.0.8/gs_quant/timeseries/algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/analysis.py` & `gs_quant-1.0.8/gs_quant/timeseries/analysis.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/backtesting.py` & `gs_quant-1.0.8/gs_quant/timeseries/backtesting.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/datetime.py` & `gs_quant-1.0.8/gs_quant/timeseries/datetime.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/econometrics.py` & `gs_quant-1.0.8/gs_quant/timeseries/econometrics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/helper.py` & `gs_quant-1.0.8/gs_quant/timeseries/helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measure_registry.py` & `gs_quant-1.0.8/gs_quant/timeseries/measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_countries.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_fx_vol.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_fx_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_helper.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_inflation.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_portfolios.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_rates.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_rates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_reports.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,16 +292,15 @@
     :param real_time: whether to retrieve intraday data instead of EOD
     :param request_id: server request id
     :return: portfolio long pnl
     """
     start_date = DataContext.current.start_time.date()
     end_date = DataContext.current.end_time.date()
     performance_report = PerformanceReport.get(report_id)
-    portfolio_id = performance_report.position_source_id
-    aum_curve = PortfolioManager(portfolio_id).get_aum(start_date=start_date, end_date=end_date)
+    aum_curve = performance_report.get_aum(start_date=start_date, end_date=end_date)
     aum_dict = [{'date': key, 'aum': aum_curve[key]} for key in aum_curve]
 
     # Create and return timeseries
     df = pd.DataFrame(aum_dict)
     if not df.empty:
         df.set_index('date', inplace=True)
         df.index = pd.to_datetime(df.index)
@@ -330,25 +329,26 @@
         return_format=ReturnFormat.JSON
     )
     factor_data = [d for d in factor_data if d.get(data_type)]
     if unit == Unit.PERCENT:
         if report.position_source_type != PositionSourceType.Portfolio:
             raise MqValueError('Unit can only be set to percent for portfolio reports')
         pm = PortfolioManager(report.position_source_id)
+        performance_report = pm.get_performance_report()
         if query_type == QueryType.FACTOR_PNL:
             last_date = dt.datetime.strptime(max([d['date'] for d in factor_data]), '%Y-%m-%d').date()
-            aum = pm.get_aum(start_date=last_date, end_date=last_date)
+            aum = performance_report.get_aum(start_date=last_date, end_date=last_date)
             last_aum = aum.get(last_date.strftime('%Y-%m-%d'))
             if last_aum is None:
                 raise MqValueError('Cannot convert to percent: Missing AUM on the last date in the date range')
             factor_exposures = [{'date': d['date'], col_name: d[data_type] / last_aum * 100} for d in factor_data]
         else:
             start_date = dt.datetime.strptime(min([d['date'] for d in factor_data]), '%Y-%m-%d').date()
             end_date = dt.datetime.strptime(max([d['date'] for d in factor_data]), '%Y-%m-%d').date()
-            aum = pm.get_aum(start_date=start_date, end_date=end_date)
+            aum = performance_report.get_aum(start_date=start_date, end_date=end_date)
             for data in factor_data:
                 if aum.get(data['date']) is None:
                     raise MqValueError('Cannot convert to percent: Missing AUM on some dates in the date range')
             factor_exposures = [{
                 'date': d['date'],
                 col_name: d[data_type] / aum.get(d['date']) * 100
             } for d in factor_data]
```

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_risk_models.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/measures_xccy.py` & `gs_quant-1.0.8/gs_quant/timeseries/measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/statistics.py` & `gs_quant-1.0.8/gs_quant/timeseries/statistics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/tca.py` & `gs_quant-1.0.8/gs_quant/timeseries/tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/timeseries/technicals.py` & `gs_quant-1.0.8/gs_quant/timeseries/technicals.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/tracing/__init__.py` & `gs_quant-1.0.8/gs_quant/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant/tracing/tracing.py` & `gs_quant-1.0.8/gs_quant/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant.egg-info/PKG-INFO` & `gs_quant-1.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gs-quant
-Version: 1.0.7
+Name: gs_quant
+Version: 1.0.8
 Summary: Goldman Sachs Quant
 Home-page: https://marquee.gs.com
 Author: Goldman Sachs
 Author-email: developer@gs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # GS Quant
```

### Comparing `gs_quant-1.0.7/gs_quant.egg-info/SOURCES.txt` & `gs_quant-1.0.8/gs_quant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/gs_quant.egg-info/requires.txt` & `gs_quant-1.0.8/gs_quant.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/setup.py` & `gs_quant-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.7/versioneer.py` & `gs_quant-1.0.8/versioneer.py`

 * *Files identical despite different names*

