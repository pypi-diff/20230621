# Comparing `tmp/splink-3.9.1.tar.gz` & `tmp/splink-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.9.1.tar", max compression
+gzip compressed data, was "splink-3.9.2.tar", max compression
```

## Comparing `splink-3.9.1.tar` & `splink-3.9.2.tar`

### file list

```diff
@@ -1,140 +1,144 @@
--rw-r--r--   0        0        0     1076 2023-06-07 15:39:58.384966 splink-3.9.1/LICENSE
--rw-r--r--   0        0        0     8787 2023-06-07 15:39:58.384966 splink-3.9.1/README.md
--rw-r--r--   0        0        0     1799 2023-06-07 15:39:58.420966 splink-3.9.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-07 15:39:58.420966 splink-3.9.1/splink/__init__.py
--rw-r--r--   0        0        0    10852 2023-06-07 15:39:58.420966 splink-3.9.1/splink/accuracy.py
--rw-r--r--   0        0        0     4759 2023-06-07 15:39:58.420966 splink-3.9.1/splink/analyse_blocking.py
--rw-r--r--   0        0        0      387 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0      396 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_comparison_template_library.py
--rw-r--r--   0        0        0      661 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_base.py
--rw-r--r--   0        0        0     3120 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_comparison_imports.py
--rw-r--r--   0        0        0      350 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_transforms.py
--rw-r--r--   0        0        0     2903 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_helpers/athena_utils.py
--rw-r--r--   0        0        0      361 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/athena_linker.py
--rw-r--r--   0        0        0      366 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/comparison_level_library.py
--rw-r--r--   0        0        0      221 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/comparison_library.py
--rw-r--r--   0        0        0      252 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/comparison_template_library.py
--rw-r--r--   0        0        0    20873 2023-06-07 15:39:58.420966 splink-3.9.1/splink/athena/linker.py
--rw-r--r--   0        0        0     2867 2023-06-07 15:39:58.420966 splink-3.9.1/splink/block_from_labels.py
--rw-r--r--   0        0        0     6239 2023-06-07 15:39:58.420966 splink-3.9.1/splink/blocking.py
--rw-r--r--   0        0        0    11739 2023-06-07 15:39:58.420966 splink-3.9.1/splink/charts.py
--rw-r--r--   0        0        0     9088 2023-06-07 15:39:58.420966 splink-3.9.1/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison.py
--rw-r--r--   0        0        0     8766 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_helpers.py
--rw-r--r--   0        0        0      554 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_helpers_utils.py
--rw-r--r--   0        0        0    25479 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level.py
--rw-r--r--   0        0        0    16492 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    48250 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    56259 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_library.py
--rw-r--r--   0        0        0     4810 2023-06-07 15:39:58.420966 splink-3.9.1/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    62023 2023-06-07 15:39:58.424966 splink-3.9.1/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2023-06-07 15:39:58.424966 splink-3.9.1/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-06-07 15:39:58.424966 splink-3.9.1/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16886 2023-06-07 15:39:58.424966 splink-3.9.1/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-06-07 15:39:58.424966 splink-3.9.1/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-06-07 15:39:58.424966 splink-3.9.1/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-06-07 15:39:58.424966 splink-3.9.1/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0      609 2023-06-07 15:39:58.424966 splink-3.9.1/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1608 2023-06-07 15:39:58.424966 splink-3.9.1/splink/dialect_base.py
--rw-r--r--   0        0        0      476 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/comparison_level_library.py
--rw-r--r--   0        0        0      371 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/comparison_library.py
--rw-r--r--   0        0        0      172 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/comparison_template_library.py
--rw-r--r--   0        0        0      387 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      396 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1532 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_base.py
--rw-r--r--   0        0        0     5597 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
--rw-r--r--   0        0        0     1750 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_helpers.py
--rw-r--r--   0        0        0      367 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    11612 2023-06-07 15:39:58.424966 splink-3.9.1/splink/duckdb/linker.py
--rw-r--r--   0        0        0    17471 2023-06-07 15:39:58.424966 splink-3.9.1/splink/em_training_session.py
--rw-r--r--   0        0        0     5244 2023-06-07 15:39:58.424966 splink-3.9.1/splink/estimate_u.py
--rw-r--r--   0        0        0      268 2023-06-07 15:39:58.424966 splink-3.9.1/splink/exceptions.py
--rw-r--r--   0        0        0     7333 2023-06-07 15:39:58.424966 splink-3.9.1/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1558 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     5212 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/comparator_score_chart.json
--rw-r--r--   0        0        0     1907 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/comparator_score_threshold_chart.json
--rw-r--r--   0        0        0     2779 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     6737 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
--rw-r--r--   0        0        0     7747 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
--rw-r--r--   0        0        0     6298 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/compare_estimates.json
--rw-r--r--   0        0        0     2155 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json
--rw-r--r--   0        0        0      743 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/gamma_histogram.json
--rw-r--r--   0        0        0     1309 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/del/score_histogram.json
--rw-r--r--   0        0        0     5831 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0      977 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5766 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9159 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1734 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     2708 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1962 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/phonetic_match_chart.json
--rw-r--r--   0        0        0     1465 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1123 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1745 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     9924 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/tf_adjustment_chart.json
--rw-r--r--   0        0        0     2645 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-06-07 15:39:58.424966 splink-3.9.1/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-06-07 15:39:58.428966 splink-3.9.1/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0    12871 2023-06-07 15:39:58.428966 splink-3.9.1/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-06-07 15:39:58.436967 splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     5486 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-06-07 15:39:58.440966 splink-3.9.1/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-06-07 15:39:58.444967 splink-3.9.1/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-06-07 15:39:58.444967 splink-3.9.1/splink/files/templates/single_chart_template.txt
--rw-r--r--   0        0        0      195 2023-06-07 15:39:58.444967 splink-3.9.1/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-06-07 15:39:58.444967 splink-3.9.1/splink/input_column.py
--rw-r--r--   0        0        0   131359 2023-06-07 15:39:58.444967 splink-3.9.1/splink/linker.py
--rw-r--r--   0        0        0      300 2023-06-07 15:39:58.444967 splink-3.9.1/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-06-07 15:39:58.444967 splink-3.9.1/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-06-07 15:39:58.444967 splink-3.9.1/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-06-07 15:39:58.444967 splink-3.9.1/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-06-07 15:39:58.444967 splink-3.9.1/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-06-07 15:39:58.444967 splink-3.9.1/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-06-07 15:39:58.444967 splink-3.9.1/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     4548 2023-06-07 15:39:58.444967 splink-3.9.1/splink/misc.py
--rw-r--r--   0        0        0     2791 2023-06-07 15:39:58.444967 splink-3.9.1/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-06-07 15:39:58.444967 splink-3.9.1/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-06-07 15:39:58.444967 splink-3.9.1/splink/pipeline.py
--rw-r--r--   0        0        0     3205 2023-06-07 15:39:58.444967 splink-3.9.1/splink/predict.py
--rw-r--r--   0        0        0     8245 2023-06-07 15:39:58.444967 splink-3.9.1/splink/profile_data.py
--rw-r--r--   0        0        0    18694 2023-06-07 15:39:58.444967 splink-3.9.1/splink/settings.py
--rw-r--r--   0        0        0      474 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/comparison_library.py
--rw-r--r--   0        0        0      170 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/comparison_template_library.py
--rw-r--r--   0        0        0      473 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/jar_location.py
--rw-r--r--   0        0        0    23101 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/linker.py
--rw-r--r--   0        0        0      384 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0      366 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      393 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0     1083 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_helpers/custom_spark_dialect.py
--rw-r--r--   0        0        0     1875 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_helpers/spark_base.py
--rw-r--r--   0        0        0     5565 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_helpers/spark_comparison_imports.py
--rw-r--r--   0        0        0      356 2023-06-07 15:39:58.444967 splink-3.9.1/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4507 2023-06-07 15:39:58.444967 splink-3.9.1/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     3836 2023-06-07 15:39:58.444967 splink-3.9.1/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1181 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sql_transform.py
--rw-r--r--   0        0        0      313 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/comparison_level_library.py
--rw-r--r--   0        0        0      157 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/comparison_library.py
--rw-r--r--   0        0        0      390 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/comparison_template_library.py
--rw-r--r--   0        0        0     6173 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/linker.py
--rw-r--r--   0        0        0      387 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0      396 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_comparison_template_library.py
--rw-r--r--   0        0        0      148 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_helpers/sqlite_base.py
--rw-r--r--   0        0        0     2061 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
--rw-r--r--   0        0        0      361 2023-06-07 15:39:58.444967 splink-3.9.1/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0    10205 2023-06-07 15:39:58.444967 splink-3.9.1/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-06-07 15:39:58.444967 splink-3.9.1/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1424 2023-06-07 15:39:58.444967 splink-3.9.1/splink/unlinkables.py
--rw-r--r--   0        0        0     2431 2023-06-07 15:39:58.444967 splink-3.9.1/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2326 2023-06-07 15:39:58.444967 splink-3.9.1/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-06-07 15:39:58.444967 splink-3.9.1/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9755 1970-01-01 00:00:00.000000 splink-3.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-21 11:04:52.562420 splink-3.9.2/LICENSE
+-rw-r--r--   0        0        0     8755 2023-06-21 11:04:52.562420 splink-3.9.2/README.md
+-rw-r--r--   0        0        0     2081 2023-06-21 11:04:52.598421 splink-3.9.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-21 11:04:52.598421 splink-3.9.2/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-06-21 11:04:52.598421 splink-3.9.2/splink/accuracy.py
+-rw-r--r--   0        0        0     4759 2023-06-21 11:04:52.598421 splink-3.9.2/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      387 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_comparison_template_library.py
+-rw-r--r--   0        0        0      661 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_base.py
+-rw-r--r--   0        0        0     3120 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_comparison_imports.py
+-rw-r--r--   0        0        0      350 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     2903 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0      361 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0      366 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/comparison_level_library.py
+-rw-r--r--   0        0        0      221 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/comparison_library.py
+-rw-r--r--   0        0        0      252 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/comparison_template_library.py
+-rw-r--r--   0        0        0    20901 2023-06-21 11:04:52.598421 splink-3.9.2/splink/athena/linker.py
+-rw-r--r--   0        0        0     2867 2023-06-21 11:04:52.598421 splink-3.9.2/splink/block_from_labels.py
+-rw-r--r--   0        0        0     6239 2023-06-21 11:04:52.598421 splink-3.9.2/splink/blocking.py
+-rw-r--r--   0        0        0    11221 2023-06-21 11:04:52.598421 splink-3.9.2/splink/charts.py
+-rw-r--r--   0        0        0     9244 2023-06-21 11:04:52.598421 splink-3.9.2/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison.py
+-rw-r--r--   0        0        0     8766 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_helpers.py
+-rw-r--r--   0        0        0      554 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_helpers_utils.py
+-rw-r--r--   0        0        0    25479 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level.py
+-rw-r--r--   0        0        0    16344 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    55194 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    61094 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_library.py
+-rw-r--r--   0        0        0     4932 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    81134 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-06-21 11:04:52.598421 splink-3.9.2/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16917 2023-06-21 11:04:52.598421 splink-3.9.2/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-06-21 11:04:52.598421 splink-3.9.2/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-06-21 11:04:52.598421 splink-3.9.2/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-06-21 11:04:52.598421 splink-3.9.2/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0      609 2023-06-21 11:04:52.598421 splink-3.9.2/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1608 2023-06-21 11:04:52.598421 splink-3.9.2/splink/dialect_base.py
+-rw-r--r--   0        0        0      476 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/comparison_level_library.py
+-rw-r--r--   0        0        0      371 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/comparison_library.py
+-rw-r--r--   0        0        0      194 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/comparison_template_library.py
+-rw-r--r--   0        0        0      387 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1532 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_base.py
+-rw-r--r--   0        0        0     5821 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
+-rw-r--r--   0        0        0     1750 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0      367 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    11654 2023-06-21 11:04:52.598421 splink-3.9.2/splink/duckdb/linker.py
+-rw-r--r--   0        0        0    17471 2023-06-21 11:04:52.598421 splink-3.9.2/splink/em_training_session.py
+-rw-r--r--   0        0        0     5655 2023-06-21 11:04:52.602421 splink-3.9.2/splink/estimate_u.py
+-rw-r--r--   0        0        0      269 2023-06-21 11:04:52.602421 splink-3.9.2/splink/exceptions.py
+-rw-r--r--   0        0        0     7333 2023-06-21 11:04:52.602421 splink-3.9.2/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1562 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     5153 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     1836 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2775 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     5795 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0     1111 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5691 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9113 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1714 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     2753 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1891 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1654 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1125 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1805 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9910 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0     2910 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-06-21 11:04:52.602421 splink-3.9.2/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-06-21 11:04:52.606421 splink-3.9.2/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0    13833 2023-06-21 11:04:52.606421 splink-3.9.2/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-06-21 11:04:52.614421 splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-06-21 11:04:52.618421 splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-06-21 11:04:52.626421 splink-3.9.2/splink/files/templates/single_chart_template.txt
+-rw-r--r--   0        0        0      195 2023-06-21 11:04:52.626421 splink-3.9.2/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-06-21 11:04:52.626421 splink-3.9.2/splink/input_column.py
+-rw-r--r--   0        0        0   129980 2023-06-21 11:04:52.626421 splink-3.9.2/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-06-21 11:04:52.626421 splink-3.9.2/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-06-21 11:04:52.626421 splink-3.9.2/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-06-21 11:04:52.626421 splink-3.9.2/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-06-21 11:04:52.626421 splink-3.9.2/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-06-21 11:04:52.626421 splink-3.9.2/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-06-21 11:04:52.626421 splink-3.9.2/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-06-21 11:04:52.626421 splink-3.9.2/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     4548 2023-06-21 11:04:52.626421 splink-3.9.2/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-06-21 11:04:52.626421 splink-3.9.2/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-06-21 11:04:52.626421 splink-3.9.2/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-06-21 11:04:52.626421 splink-3.9.2/splink/pipeline.py
+-rw-r--r--   0        0        0      390 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/comparison_level_library.py
+-rw-r--r--   0        0        0      253 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/comparison_library.py
+-rw-r--r--   0        0        0      394 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/comparison_template_library.py
+-rw-r--r--   0        0        0    10365 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/linker.py
+-rw-r--r--   0        0        0      393 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_comparison_level_library.py
+-rw-r--r--   0        0        0      375 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_comparison_library.py
+-rw-r--r--   0        0        0      402 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_comparison_template_library.py
+-rw-r--r--   0        0        0     1530 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_helpers/postgres_base.py
+-rw-r--r--   0        0        0     3241 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_helpers/postgres_comparison_imports.py
+-rw-r--r--   0        0        0      371 2023-06-21 11:04:52.626421 splink-3.9.2/splink/postgres/postgres_linker.py
+-rw-r--r--   0        0        0     3205 2023-06-21 11:04:52.626421 splink-3.9.2/splink/predict.py
+-rw-r--r--   0        0        0     8241 2023-06-21 11:04:52.626421 splink-3.9.2/splink/profile_data.py
+-rw-r--r--   0        0        0    18694 2023-06-21 11:04:52.626421 splink-3.9.2/splink/settings.py
+-rw-r--r--   0        0        0      474 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/comparison_library.py
+-rw-r--r--   0        0        0      192 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/comparison_template_library.py
+-rw-r--r--   0        0        0      473 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/jar_location.py
+-rw-r--r--   0        0        0    23143 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/linker.py
+-rw-r--r--   0        0        0      384 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0      366 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      393 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0     1083 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     1875 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_helpers/spark_base.py
+-rw-r--r--   0        0        0     5788 2023-06-21 11:04:52.626421 splink-3.9.2/splink/spark/spark_helpers/spark_comparison_imports.py
+-rw-r--r--   0        0        0      356 2023-06-21 11:04:52.630421 splink-3.9.2/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4507 2023-06-21 11:04:52.630421 splink-3.9.2/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     3750 2023-06-21 11:04:52.630421 splink-3.9.2/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1181 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sql_transform.py
+-rw-r--r--   0        0        0      384 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/comparison_level_library.py
+-rw-r--r--   0        0        0      252 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/comparison_library.py
+-rw-r--r--   0        0        0      126 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/comparison_template_library.py
+-rw-r--r--   0        0        0     8472 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/linker.py
+-rw-r--r--   0        0        0      387 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_comparison_template_library.py
+-rw-r--r--   0        0        0      270 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_helpers/sqlite_base.py
+-rw-r--r--   0        0        0     3861 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
+-rw-r--r--   0        0        0      361 2023-06-21 11:04:52.630421 splink-3.9.2/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0     9825 2023-06-21 11:04:52.630421 splink-3.9.2/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-06-21 11:04:52.630421 splink-3.9.2/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1424 2023-06-21 11:04:52.630421 splink-3.9.2/splink/unlinkables.py
+-rw-r--r--   0        0        0     2431 2023-06-21 11:04:52.630421 splink-3.9.2/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-06-21 11:04:52.630421 splink-3.9.2/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-06-21 11:04:52.630421 splink-3.9.2/splink/waterfall_chart.py
+-rw-r--r--   0        0        0     9738 1970-01-01 00:00:00.000000 splink-3.9.2/PKG-INFO
```

### Comparing `splink-3.9.1/LICENSE` & `splink-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/README.md` & `splink-3.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 ## Quickstart
 
 The following code demonstrates how to estimate the parameters of a deduplication model, use it to identify duplicate records, and then use clustering to generate an estimated unique person ID.
 
 For more detailed tutorials, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
-from splink.duckdb.duckdb_linker import DuckDBLinker
-import splink.duckdb.duckdb_comparison_library as cl
-import splink.duckdb.duckdb_comparison_template_library as ctl
+from splink.duckdb.linker import DuckDBLinker
+import splink.duckdb.comparison_library as cl
+import splink.duckdb.comparison_template_library as ctl
 
 import pandas as pd
 
 df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
 
 settings = {
     "link_type": "dedupe_only",
@@ -93,15 +93,15 @@
         "l.surname = r.surname",
     ],
     "comparisons": [
         ctl.name_comparison("first_name"),
         ctl.name_comparison("surname"),
         ctl.date_comparison("dob", cast_strings_to_date=True),
         cl.exact_match("city", term_frequency_adjustments=True),
-        cl.levenshtein_at_thresholds("email", 2),
+        ctl.email_comparison("email"),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
 blocking_rule_for_training = "l.first_name = r.first_name and l.surname = r.surname"
```

### Comparing `splink-3.9.1/pyproject.toml` & `splink-3.9.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 [tool.poetry]
 name = "splink"
-version = "3.9.1"
+version = "3.9.2"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 jsonschema = ">=3.2,<5.0"
 pandas = ">=1.0.0"
 duckdb = ">=0.6.0"
-sqlglot = ">=5.1.0"
-altair = ">=4.2.0"
+# normalize issue in sqlglot - temporarily exclude updates
+sqlglot = ">=5.1.0,<11.4.2"
+altair = "^5.0.1"
 Jinja2 = ">=3.0.3"
 phonetics = "^1.0.5"
 
 [tool.poetry.group.dev]
 [tool.poetry.group.dev.dependencies]
 tabulate = "0.8.9"
 pyspark = "^3.2.1"
+# sqlalchemy >= 2.0.0 not working well with older pandas
+sqlalchemy = ">=1.4.0,<2.0.0"
+# temporarily use binary version, to avoid issues with pg_config path
+psycopg2-binary = ">=2.8.0"
 
 [tool.poetry.group.linting]
 [tool.poetry.group.linting.dependencies]
 black = "22.6.0"
 ruff = "0.0.257"
 
 [tool.poetry.group.testing]
@@ -41,14 +46,16 @@
 pytest-benchmark = "^4"
 lzstring = "1.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.isort]
+profile = "black"
 
 [tool.ruff]
 line-length = 88
 select = [
     # Pyflakes
     "F",
     # Pycodestyle
```

### Comparing `splink-3.9.1/splink/accuracy.py` & `splink-3.9.2/splink/accuracy.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/analyse_blocking.py` & `splink-3.9.2/splink/analyse_blocking.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/athena/athena_helpers/athena_base.py` & `splink-3.9.2/splink/athena/athena_helpers/athena_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/athena/athena_helpers/athena_comparison_imports.py` & `splink-3.9.2/splink/athena/athena_helpers/athena_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/athena/athena_helpers/athena_utils.py` & `splink-3.9.2/splink/athena/athena_helpers/athena_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/athena/linker.py` & `splink-3.9.2/splink/athena/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                 Defaults to "splink_warehouse/{unique_id}".
         Examples:
             ```py
             # Creating a database in athena and writing to it
             import awswrangler as wr
             wr.catalog.create_database("splink_awswrangler_test", exist_ok=True)
             >>>
-            from splink.athena.athena_linker import AthenaLinker
+            from splink.athena.linker import AthenaLinker
             import boto3
             # Create a session - please see the boto3 documentation for more info
             my_session = boto3.Session(region_name="eu-west-1")
             >>>
             linker = AthenaLinker(
                 settings_dict=settings_dict,
                 input_table_or_tables="synthetic_data_all",
@@ -170,15 +170,15 @@
             )
             ```
             ```py
             # Creating a secondary database and use data on and existing db
             import awswrangler as wr
             wr.catalog.create_database("splink_awswrangler_test2", exist_ok=True)
             >>>
-            from splink.athena.athena_linker import AthenaLinker
+            from splink.athena.linker import AthenaLinker
             import boto3
             my_session = boto3.Session(region_name="eu-west-1")
             >>>
             # To read and write from separate databases, specify your secondary
             # database as the output and enter your primary database as a schema
             # for your input table(s)
             linker = AthenaLinker(
@@ -336,15 +336,17 @@
             input = pd.DataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         # Errors if an invalid data type is passed
         self.register_data_on_s3(input, table_name)
 
-    def _random_sample_sql(self, proportion, sample_size, seed=None):
+    def _random_sample_sql(
+        self, proportion, sample_size, seed=None, table=None, unique_id=None
+    ):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         return f" TABLESAMPLE BERNOULLI ({percent})"
 
     @property
     def _infinity_expression(self):
```

### Comparing `splink-3.9.1/splink/block_from_labels.py` & `splink-3.9.2/splink/block_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/blocking.py` & `splink-3.9.2/splink/blocking.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/charts.py` & `splink-3.9.2/splink/charts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 import json
 import os
 import pkgutil
 
 from .waterfall_chart import records_to_waterfall_data
 
 altair_installed = True
-try:
-    from altair.vegalite.v4.display import VegaLite
-
-    # Slightly re-write logic to avoid validation
-    # Some splink3 charts do not validate but display fine
-    # When Altair supports Vega Lite v5, this should no longer be a problem
-    # and this logic should be able to be removed
-    class VegaliteNoValidate(VegaLite):
-        def _validate(self):
-            pass
-
-    def vegalite_no_validate(spec):
-        return VegaliteNoValidate(spec)
 
+try:
+    import altair as alt
 except ImportError:
     altair_installed = False
 
 
 def load_chart_definition(filename):
     path = f"files/chart_defs/{filename}"
     data = pkgutil.get_data(__name__, path)
@@ -41,20 +30,19 @@
     for k, v in to_load.items():
         script = pkgutil.get_data(__name__, v).decode("utf-8")
         loaded[k] = script
 
     return loaded
 
 
-def vegalite_or_json(chart_dict, as_dict=False):
+def altair_or_json(chart_dict, as_dict=False):
     if altair_installed:
         if not as_dict:
             try:
-                # Display chart then return its spec
-                return vegalite_no_validate(chart_dict)
+                return alt.Chart.from_dict(chart_dict)
 
             except ModuleNotFoundError:
                 return chart_dict
 
     return chart_dict
 
 
@@ -111,30 +99,30 @@
 
     # Remove iteration history since this is a static chart
     del chart["params"]
     del chart["transform"]
 
     records = [r for r in records if r["comparison_vector_value"] != -1]
     chart["data"]["values"] = records
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def comparison_match_weights_chart(records, as_dict=False):
     chart_path = "match_weights_interactive_history.json"
     chart = load_chart_definition(chart_path)
 
     # Remove iteration history since this is a static chart
     del chart["vconcat"][0]
     del chart["params"]
     del chart["transform"]
 
     chart["title"]["text"] = "Comparison summary"
     records = [r for r in records if r["comparison_vector_value"] != -1]
     chart["data"]["values"] = records
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def m_u_parameters_chart(records, as_dict=False):
     chart_path = "m_u_parameters_interactive_history.json"
     chart = load_chart_definition(chart_path)
 
     # Remove iteration history since this is a static chart
@@ -144,23 +132,23 @@
     records = [
         r
         for r in records
         if r["comparison_vector_value"] != -1
         and r["comparison_name"] != "probability_two_random_records_match"
     ]
     chart["data"]["values"] = records
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def probability_two_random_records_match_iteration_chart(records, as_dict=False):
     chart_path = "probability_two_random_records_match_iteration.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def match_weights_interactive_history_chart(records, as_dict=False, blocking_rule=None):
     chart_path = "match_weights_interactive_history.json"
     chart = load_chart_definition(chart_path)
 
     chart["title"]["subtitle"] = f"Training session blocked on {blocking_rule}"
@@ -170,15 +158,15 @@
 
     max_iteration = 0
     for r in records:
         max_iteration = max(r["iteration"], max_iteration)
 
     chart["params"][0]["bind"]["max"] = max_iteration
     chart["params"][0]["value"] = max_iteration
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def m_u_parameters_interactive_history_chart(records, as_dict=False):
     chart_path = "m_u_parameters_interactive_history.json"
     chart = load_chart_definition(chart_path)
     records = [
         r
@@ -190,15 +178,15 @@
 
     max_iteration = 0
     for r in records:
         max_iteration = max(r["iteration"], max_iteration)
 
     chart["params"][0]["bind"]["max"] = max_iteration
     chart["params"][0]["value"] = max_iteration
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def waterfall_chart(
     records,
     settings_obj,
     filter_nulls=True,
     as_dict=False,
@@ -207,15 +195,15 @@
     chart_path = "match_weights_waterfall.json"
     chart = load_chart_definition(chart_path)
     chart["data"]["values"] = data
     chart["params"][0]["bind"]["max"] = len(records) - 1
     if filter_nulls:
         chart["transform"].insert(1, {"filter": "(datum.bayes_factor !== 1.0)"})
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def roc_chart(records, width=400, height=400, as_dict=False):
     chart_path = "roc.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
@@ -225,15 +213,15 @@
     r = records[0]
     if "curve_label" not in r.keys():
         del chart["encoding"]["color"]
 
     chart["height"] = height
     chart["width"] = width
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def precision_recall_chart(records, width=400, height=400, as_dict=False):
     chart_path = "precision_recall.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
@@ -243,50 +231,50 @@
     r = records[0]
     if "curve_label" not in r.keys():
         del chart["encoding"]["color"]
 
     chart["height"] = height
     chart["width"] = width
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def match_weights_histogram(records, width=500, height=250, as_dict=False):
     chart_path = "match_weight_histogram.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
 
     chart["height"] = height
     chart["width"] = width
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def parameter_estimate_comparisons(records, as_dict=False):
     chart_path = "parameter_estimate_comparisons.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def missingness_chart(records, as_dict=False):
     chart_path = "missingness.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
 
     record_count = records[0]["total_record_count"]
 
     for c in chart["layer"]:
         c["title"] = f"Missingness per column out of {record_count:,.0f} records"
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def unlinkables_chart(
     records,
     x_col="match_weight",
     source_dataset=None,
     as_dict=False,
@@ -327,43 +315,43 @@
         unlinkables_chart_def["layer"][3]["encoding"]["x"][
             "field"
         ] = "match_probability"
 
     if source_dataset:
         unlinkables_chart_def["title"]["text"] += f" - {source_dataset}"
 
-    return vegalite_or_json(unlinkables_chart_def, as_dict=as_dict)
+    return altair_or_json(unlinkables_chart_def, as_dict=as_dict)
 
 
 def completeness_chart(records, as_dict=False):
     chart_path = "completeness.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def cumulative_blocking_rule_comparisons_generated(records, as_dict=False):
     chart_path = "blocking_rule_generated_comparisons.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def _comparator_score_chart(similarity_records, distance_records, as_dict=False):
     chart_path = "comparator_score_chart.json"
     chart = load_chart_definition(chart_path)
 
     chart["datasets"]["data-similarity"] = similarity_records
     chart["datasets"]["data-distance"] = distance_records
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def _comparator_score_threshold_chart(
     records, similarity_threshold, distance_threshold, as_dict=False
 ):
     chart_path = "comparator_score_threshold_chart.json"
     chart = load_chart_definition(chart_path)
@@ -371,17 +359,17 @@
     chart["layer"][0]["title"] = (
         f"Heatmap of Matches for "
         f"distance_threshold = {distance_threshold}, "
         f"similarity_threshold = {similarity_threshold}"
     )
     chart["datasets"]["data-with-thresholds"] = records
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
 
 
 def _phonetic_match_chart(records, as_dict=False):
     chart_path = "phonetic_match_chart.json"
     chart = load_chart_definition(chart_path)
 
     chart["datasets"]["data-phonetic"] = records
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
```

### Comparing `splink-3.9.1/splink/cluster_studio.py` & `splink-3.9.2/splink/cluster_studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,21 +127,29 @@
         sql, "__splink__cluster_count"
     )
     cluster_count = df_cluster_count.as_record_dict()[0]["count"]
     df_cluster_count.drop_table_from_database()
 
     proportion = sample_size / cluster_count
 
+    random_sample_sql = linker._random_sample_sql(
+        proportion,
+        sample_size,
+        seed,
+        table=connected_components.physical_name,
+        unique_id="cluster_id",
+    )
+
     sql = f"""
     with distinct_clusters as (
     select distinct(cluster_id)
     from {connected_components.physical_name}
     )
     select cluster_id from distinct_clusters
-    {linker._random_sample_sql(proportion, sample_size, seed)}
+    {random_sample_sql}
     """
 
     df_sample = linker._sql_to_splink_dataframe_checking_cache(
         sql,
         "__splink__df_concat_with_tf_sample",
     )
     return [r["cluster_id"] for r in df_sample.as_record_dict()]
```

### Comparing `splink-3.9.1/splink/comparison.py` & `splink-3.9.2/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/comparison_helpers.py` & `splink-3.9.2/splink/comparison_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/comparison_helpers_utils.py` & `splink-3.9.2/splink/comparison_helpers_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/comparison_level.py` & `splink-3.9.2/splink/comparison_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,34 +538,34 @@
     def _bayes_factor_sql(self):
         bayes_factor = (
             self._bayes_factor if self._bayes_factor != math.inf else "'Infinity'"
         )
         sql = f"""
         WHEN
         {self.comparison._gamma_column_name} = {self._comparison_vector_value}
-        THEN cast({bayes_factor} as double)
+        THEN cast({bayes_factor} as float8)
         """
         return dedent(sql)
 
     @property
     def _tf_adjustment_sql(self):
         gamma_column_name = self.comparison._gamma_column_name
         gamma_colname_value_is_this_level = (
             f"{gamma_column_name} = {self._comparison_vector_value}"
         )
 
         # A tf adjustment of 1D is a multiplier of 1.0, i.e. no adjustment
         if self._comparison_vector_value == -1:
-            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as double)"
+            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
         elif not self._has_tf_adjustments:
-            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as double)"
+            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
         elif self._tf_adjustment_weight == 0:
-            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as double)"
+            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
         elif self._is_else_level:
-            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as double)"
+            sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
         else:
             tf_adj_col = self._tf_adjustment_input_column
 
             coalesce_l_r = (
                 f"coalesce({tf_adj_col.tf_name_l()}, {tf_adj_col.tf_name_r()})"
             )
             coalesce_r_l = (
@@ -592,31 +592,31 @@
                 """
             else:
                 # This sql works correctly even when the tf_minimum_u_value is 0.0
                 # but is less efficient to execute, hence the above if statement
                 divisor_sql = f"""
                 (CASE
                     WHEN {coalesce_l_r} >= {coalesce_r_l}
-                    AND {coalesce_l_r} > cast({self._tf_minimum_u_value} as double)
+                    AND {coalesce_l_r} > cast({self._tf_minimum_u_value} as float8)
                         THEN {coalesce_l_r}
-                    WHEN {coalesce_r_l}  > cast({self._tf_minimum_u_value} as double)
+                    WHEN {coalesce_r_l}  > cast({self._tf_minimum_u_value} as float8)
                         THEN {coalesce_r_l}
-                    ELSE cast({self._tf_minimum_u_value} as double)
+                    ELSE cast({self._tf_minimum_u_value} as float8)
                 END)
                 """
 
             sql = f"""
             WHEN  {gamma_colname_value_is_this_level} then
                 (CASE WHEN {tf_adjustment_exists}
                 THEN
                 POW(
-                    cast({u_prob_exact_match} as double) /{divisor_sql},
-                    cast({self._tf_adjustment_weight} as double)
+                    cast({u_prob_exact_match} as float8) /{divisor_sql},
+                    cast({self._tf_adjustment_weight} as float8)
                 )
-                ELSE cast(1 as double)
+                ELSE cast(1 as float8)
                 END)
             """
         return dedent(sql).strip()
 
     def as_dict(self):
         "The minimal representation of this level to use as an input to Splink"
         output = {}
```

### Comparing `splink-3.9.1/splink/comparison_level_composition.py` & `splink-3.9.2/splink/comparison_level_composition.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,20 @@
             estimated and instead the match weight will be zero for this column.
             Defaults to None.
 
     Examples:
         === "DuckDB"
             Simple null level composition with an `AND` clause
             ``` python
-            import splink.duckdb.duckdb_comparison_level_library as cll
+            import splink.duckdb.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
-            import splink.duckdb.duckdb_comparison_level_library as cll
+            import splink.duckdb.comparison_level_library as cll
             misspelling = cll.levenshtein_level("name", 1)
             contains = {
                 "sql_condition": "(contains(name_l, name_r) OR " \
                 "contains(name_r, name_l))"
             }
             merged = cll.and_(misspelling, contains, label_for_charts="Spelling error")
             ```
@@ -56,20 +56,20 @@
             > 'sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'AND ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
         === "Spark"
             Simple null level composition with an `AND` clause
             ``` python
-            import splink.spark.spark_comparison_level_library as cll
+            import splink.spark.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
-            import splink.spark.spark_comparison_level_library as cll
+            import splink.spark.comparison_level_library as cll
             misspelling = cll.levenshtein_level("name", 1)
             contains = {
                 "sql_condition": "(contains(name_l, name_r) OR " \
                 "contains(name_r, name_l))"
             }
             merged = cll.and_(misspelling, contains, label_for_charts="Spelling error")
             ```
@@ -80,20 +80,20 @@
             > 'sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'AND ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
         === "Athena"
             Simple null level composition with an `AND` clause
             ``` python
-            import splink.athena.athena_comparison_level_library as cll
+            import splink.athena.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
-            import splink.athena.athena_comparison_level_library as cll
+            import splink.athena.comparison_level_library as cll
             misspelling = cll.levenshtein_level("name", 1)
             contains = {
                 "sql_condition": "(contains(name_l, name_r) OR " \
                 "contains(name_r, name_l))"
             }
             merged = cll.and_(misspelling, contains, label_for_charts="Spelling error")
             ```
@@ -104,15 +104,15 @@
             > 'sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'AND ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
         === "SQLite"
             Simple null level composition with an `AND` clause
             ``` python
-            import splink.sqlite.sqlite_comparison_level_library as cll
+            import splink.sqlite.comparison_level_library as cll
             cll.and_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
 
     Returns:
         ComparisonLevel: A new ComparisonLevel with the merged
             SQL condition
     """
@@ -152,20 +152,20 @@
             estimated and instead the match weight will be zero for this column.
             Defaults to None.
 
     Examples:
         === "DuckDB"
             Simple null level composition with an `OR` clause
             ``` python
-            import splink.duckdb.duckdb_comparison_level_library as cll
+            import splink.duckdb.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
-            import splink.duckdb.duckdb_comparison_level_library as cll
+            import splink.duckdb.comparison_level_library as cll
             misspelling = cll.levenshtein_level("name", 1)
             contains = {
                 "sql_condition": "(contains(name_l, name_r) OR " \
                 "contains(name_r, name_l))"
             }
             merged = cll.or_(misspelling, contains, label_for_charts="Spelling error")
             ```
@@ -176,20 +176,20 @@
             > sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'OR ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
         === "Spark"
             Simple null level composition with an `OR` clause
             ``` python
-            import splink.spark.spark_comparison_level_library as cll
+            import splink.spark.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
-            import splink.spark.spark_comparison_level_library as cll
+            import splink.spark.comparison_level_library as cll
             misspelling = cll.levenshtein_level("name", 1)
             contains = {
                 "sql_condition": "(contains(name_l, name_r) OR " \
                 "contains(name_r, name_l))"
             }
             merged = cll.or_(misspelling, contains, label_for_charts="Spelling error")
             ```
@@ -200,20 +200,20 @@
             > sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'OR ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
         === "Athena"
             Simple null level composition with an `OR` clause
             ``` python
-            import splink.athena.athena_comparison_level_library as cll
+            import splink.athena.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
             Composing a levenshtein level with a custom `contains` level
             ``` python
-            import splink.athena.athena_comparison_level_library as cll
+            import splink.athena.comparison_level_library as cll
             misspelling = cll.levenshtein_level("name", 1)
             contains = {
                 "sql_condition": "(contains(name_l, name_r) OR " \
                 "contains(name_r, name_l))"
             }
             merged = cll.or_(misspelling, contains, label_for_charts="Spelling error")
             ```
@@ -224,15 +224,15 @@
             > sql_condition': '(levenshtein("name_l", "name_r") <= 1) ' \
             >  'OR ((contains(name_l, name_r) OR contains(name_r, name_l)))',
             >  'label_for_charts': 'Spelling error'
             >}
         === "SQLite"
             Simple null level composition with an `OR` clause
             ``` python
-            import splink.sqlite.sqlite_comparison_level_library as cll
+            import splink.sqlite.comparison_level_library as cll
             cll.or_(cll.null_level("first_name"), cll.null_level("surname"))
             ```
 
     Returns:
         ComparisonLevel: A new ComparisonLevel with the merged
             SQL condition
     """
@@ -268,77 +268,77 @@
         m_probability (float, optional): Starting value for m probability.
             Defaults to None.
 
     Examples:
         === "DuckDB"
             *Not* an exact match on first name
             ``` python
-            import splink.duckdb.duckdb_comparison_level_library as cll
+            import splink.duckdb.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
-            import splink.duckdb.duckdb_comparison_level_library as cll
+            import splink.duckdb.comparison_level_library as cll
             dob_first_jan =  {
                "sql_condition": "SUBSTR(dob_std_l, -5) = '01-01'",
                "label_for_charts": "Date is 1st Jan",
             }
             exact_match_not_first_jan = cll.and_(
                 cll.exact_match_level("dob"),
                 cll.not_(dob_first_jan),
                 label_for_charts = "Exact match and not the 1st Jan"
             )
             ```
         === "Spark"
             *Not* an exact match on first name
             ``` python
-            import splink.spark.spark_comparison_level_library as cll
+            import splink.spark.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
-            import splink.spark.spark_comparison_level_library as cll
+            import splink.spark.comparison_level_library as cll
             dob_first_jan =  {
                "sql_condition": "SUBSTR(dob_std_l, -5) = '01-01'",
                "label_for_charts": "Date is 1st Jan",
             }
             exact_match_not_first_jan = cll.and_(
                 cll.exact_match_level("dob"),
                 cll.not_(dob_first_jan),
                 label_for_charts = "Exact match and not the 1st Jan"
             )
             ```
         === "Athena"
             *Not* an exact match on first name
             ``` python
-            import splink.athena.athena_comparison_level_library as cll
+            import splink.athena.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
-            import splink.athena.athena_comparison_level_library as cll
+            import splink.athena.comparison_level_library as cll
             dob_first_jan =  {
                "sql_condition": "SUBSTR(dob_std_l, -5) = '01-01'",
                "label_for_charts": "Date is 1st Jan",
             }
             exact_match_not_first_jan = cll.and_(
                 cll.exact_match_level("dob"),
                 cll.not_(dob_first_jan),
                 label_for_charts = "Exact match and not the 1st Jan"
             )
             ```
         === "SQLite"
             *Not* an exact match on first name
             ``` python
-            import splink.sqlite.sqlite_comparison_level_library as cll
+            import splink.sqlite.comparison_level_library as cll
             cll.not_(cll.exact_match("first_name"))
             ```
             Find all exact matches *not* on the first of January
             ``` python
-            import splink.sqlite.sqlite_comparison_level_library as cll
+            import splink.sqlite.comparison_level_library as cll
             dob_first_jan =  {
                "sql_condition": "SUBSTR(dob_std_l, -5) = '01-01'",
                "label_for_charts": "Date is 1st Jan",
             }
             exact_match_not_first_jan = cll.and_(
                 cll.exact_match_level("dob"),
                 cll.not_(dob_first_jan),
```

### Comparing `splink-3.9.1/splink/comparison_level_library.py` & `splink-3.9.2/splink/comparison_level_library.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,51 +16,57 @@
             valid_string_regex (str): regular expression pattern that if not
                 matched will result in column being treated as a null.
 
         Examples:
             === "DuckDB"
                 Simple null comparison level
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.null_level("name")
                 ```
                 Null comparison level including strings that do not match
                 a given regex pattern
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.null_level("name", valid_string_regex="^[A-Z]{1,7}$")
                 ```
             === "Spark"
                 Simple null level
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.null_level("name")
                 ```
                 Null comparison level including strings that do not match
                 a given regex pattern
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.null_level("name", valid_string_regex="^[A-Z]{1,7}$")
                 ```
             === "Athena"
                 Simple null level
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.null_level("name")
                 ```
                 Null comparison level including strings that do not match
                 a given regex pattern
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.null_level("name", valid_string_regex="^[A-Z]{1,7}$")
                 ```
             === "SQLite"
                 Simple null level
                 ``` python
-                import splink.sqlite.sqlite_comparison_level_library as cll
+                import splink.sqlite.comparison_level_library as cll
+                cll.null_level("name")
+                ```
+            === "PostgreSQL"
+                Simple null level
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.null_level("name")
                 ```
         Returns:
             ComparisonLevel: Comparison level for null entries
         """
 
         col = InputColumn(col_name, sql_dialect=self._sql_dialect)
@@ -86,101 +92,112 @@
         self,
         col_name,
         regex_extract: str = None,
         set_to_lowercase: bool = False,
         m_probability=None,
         term_frequency_adjustments=False,
         include_colname_in_charts_label=False,
-        manual_chart_label=None,
+        manual_col_name_for_charts_label=None,
     ) -> ComparisonLevel:
         """Represents a comparison level where there is an exact match,
 
         Args:
             col_name (str): Input column name
             regex_extract (str): Regular expression pattern to evaluate a match on.
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             m_probability (float, optional): Starting value for m probability
                 Defaults to None.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             include_colname_in_charts_label (bool, optional): If True, include col_name
                 in chart labels (e.g. linker.match_weights_chart())
-            chart_label (str, optional): string to include in chart label. Setting to
-                col_name would recreate behaviour of
+            manual_col_name_for_charts_label (str, optional): string to include as
+                 column name in chart label. Acts as a manual overwrite of the
+                 colname when include_colname_in_charts_label is True.
                 include_colname_in_charts_label=True
         Examples:
             === "DuckDB"
                 Simple Exact match level
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.exact_match_level("name", term_frequency_adjustments=True)
                 ```
                 Exact match level on a substring of col_name as
                  determined by a regular expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.exact_match_level("name", regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Simple Exact match level
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.exact_match_level("name", term_frequency_adjustments=True)
                 ```
                 Exact match level on a substring of col_name as
                  determined by a regular expression
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.exact_match_level("name", regex_extract="^[A-Z]{1,4}")
                 ```
             === "Athena"
                 Simple Exact match level
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.exact_match_level("name", term_frequency_adjustments=True)
                 ```
                 Exact match level on a substring of col_name as
                  determined by a regular expression
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.exact_match_level("name", regex_extract="^[A-Z]{1,4}")
                 ```
             === "SQLite"
                 Simple Exact match level
                 ``` python
-                import splink.sqlite.sqlite_comparison_level_library as cll
+                import splink.sqlite.comparison_level_library as cll
+                cll.exact_match_level("name")
+                ```
+                Exact match level with term-frequency adjustments
+                ``` python
+                import splink.sqlite.comparison_level_library as cll
+                cll.exact_match_level("name", term_frequency_adjustments=True)
+            === "PostgreSQL"
+                Simple Exact match level
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.exact_match_level("name")
                 ```
                 Exact match level with term-frequency adjustments
                 ``` python
-                import splink.sqlite.sqlite_comparison_level_library as cll
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.exact_match_level("name", term_frequency_adjustments=True)
                 ```
         """
         col = InputColumn(col_name, sql_dialect=self._sql_dialect)
 
         if include_colname_in_charts_label:
             label_suffix = f" {col_name}"
-        elif manual_chart_label:
-            label_suffix = f" {manual_chart_label}"
+        elif manual_col_name_for_charts_label:
+            label_suffix = f" {manual_col_name_for_charts_label}"
         else:
             label_suffix = ""
 
         col_name_l, col_name_r = col.name_l(), col.name_r()
 
         if set_to_lowercase:
             col_name_l = f"lower({col_name_l})"
@@ -210,30 +227,34 @@
     ) -> ComparisonLevel:
         """Represents a comparison level for all cases which have not been
         considered by preceding comparison levels,
 
         Examples:
             === "DuckDB"
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.else_level("name")
                 ```
             === "Spark"
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.else_level("name")
                 ```
             === "Athena"
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.else_level("name")
                 ```
             === "SQLite"
                 ``` python
-                import splink.sqlite.sqlite_comparison_level_library as cll
+                import splink.sqlite.comparison_level_library as cll
+                cll.else_level("name")
+            === "PostgreSQL"
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.else_level("name")
                 ```
         """
         if isinstance(m_probability, str):
             raise ValueError(
                 "You provided a string for the value of m probability when it should "
                 "be numeric.  Perhaps you passed a column name.  Note that you do "
@@ -254,14 +275,15 @@
         col_name: str,
         distance_function_name: str,
         distance_threshold: int | float,
         regex_extract: str = None,
         set_to_lowercase=False,
         higher_is_more_similar: bool = True,
         include_colname_in_charts_label=False,
+        manual_col_name_for_charts_label=None,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a user-provided distance function,
         where the similarity
 
         Args:
             col_name (str): Input column name
@@ -271,46 +293,65 @@
             regex_extract (str): Regular expression pattern to evaluate a match on.
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             higher_is_more_similar (bool): If True, a higher value of the
                 distance function indicates a higher similarity (e.g. jaro_winkler).
                 If false, a higher value indicates a lower similarity
                 (e.g. levenshtein).
             include_colname_in_charts_label (bool, optional): If True, includes
-                col_name in charts label
+                col_name in charts label.
+            manual_col_name_for_charts_label (str, optional): string to include as
+                 column name in chart label. Acts as a manual overwrite of the
+                 colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability
                 Defaults to None.
 
         Examples:
 
             === "DuckDB"
                 Apply the `levenshtein` function to a comparison level
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein",
                                             2,
                                             False)
                 ```
             === "Spark"
                 Apply the `levenshtein` function to a comparison level
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein",
                                             2,
                                             False)
                 ```
             === "Athena"
                 Apply the `levenshtein_distance` function to a comparison level
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.distance_function_level("name",
                                             "levenshtein_distance",
                                             2,
                                             False)
+            === "SQLite
+                Apply the `levenshtein` function to a comparison level
+                ``` python
+                import splink.sqlite.comparison_level_library as cll
+                cll.distance_function_level("name",
+                                            "levenshtein",
+                                            2,
+                                            False)
+            === "PostgreSQL"
+                Apply the `levenshtein` function to a comparison level
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
+                cll.distance_function_level("name",
+                                            "levenshtein",
+                                            2,
+                                            False)
                 ```
 
         Returns:
             ComparisonLevel: A comparison level for a given distance function
         """
         col = InputColumn(col_name, sql_dialect=self._sql_dialect)
 
@@ -330,15 +371,21 @@
             col_name_r = self._regex_extract_function(col_name_r, regex_extract)
 
         sql_cond = (
             f"{distance_function_name}({col_name_l}, {col_name_r}) "
             f"{operator} {distance_threshold}"
         )
 
-        label_suffix = f" {col_name}" if include_colname_in_charts_label else ""
+        if include_colname_in_charts_label:
+            if manual_col_name_for_charts_label:
+                col_name = manual_col_name_for_charts_label
+
+            label_suffix = f" {col_name}"
+        else:
+            label_suffix = ""
 
         chart_label = (
             f"{distance_function_name.capitalize()}{label_suffix} {operator} "
             f"{distance_threshold}"
         )
 
         level_dict = {
@@ -359,74 +406,91 @@
     def __init__(
         self,
         col_name: str,
         distance_threshold: int,
         regex_extract: str = None,
         set_to_lowercase=False,
         include_colname_in_charts_label=False,
+        manual_col_name_for_charts_label=None,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a levenshtein distance function,
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
+            manual_col_name_for_charts_label (str, optional): string to include as
+                 column name in chart label. Acts as a manual overwrite of the
+                 colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
                 ```
 
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
                 ```
 
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
                 ```
             === "Athena"
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.levenshtein_level("name", 1)
                 ```
 
                 Comparison level with levenshtein distance score less than (or equal
                  to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
+            === "SQLite"
+                Comparison level with levenshtein distance score less than (or equal
+                 to) 1
+                ``` python
+                import splink.sqlite.comparison_level_library as cll
+                cll.levenshtein_level("name", 1)
+            === "PostgreSQL"
+                Comparison level with levenshtein distance score less than (or equal
+                 to) 1
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
+                cll.levenshtein_level("name", 1)
+                ```
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the
                 levenshtein similarity
         """
         super().__init__(
@@ -445,60 +509,70 @@
     def __init__(
         self,
         col_name: str,
         distance_threshold: int,
         regex_extract: str = None,
         set_to_lowercase=False,
         include_colname_in_charts_label=False,
+        manual_col_name_for_charts_label=None,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a damerau-levenshtein distance
         function,
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
+            manual_col_name_for_charts_label (str, optional): string to include as
+                 column name in chart label. Acts as a manual overwrite of the
+                 colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1)
                 ```
 
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1)
                 ```
 
                 Comparison level with damerau-levenshtein distance score less than
                 (or equal to) 1 on a subtring of name column as determined by a regular
                 expression.
                 ```python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.damerau_levenshtein_level("name", 1, regex_extract="^[A-Z]{1,4}")
+            === "SQLite"
+                Comparison level with damerau-levenshtein distance score less than
+                (or equal to) 1
+                ``` python
+                import splink.sqlite.comparison_level_library as cll
+                cll.damerau_levenshtein_level("name", 1)
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the
                 Damerau-Levenshtein similarity
         """
         super().__init__(
@@ -517,56 +591,66 @@
     def __init__(
         self,
         col_name: str,
         distance_threshold: float,
         regex_extract: str = None,
         set_to_lowercase=False,
         include_colname_in_charts_label=False,
+        manual_col_name_for_charts_label=None,
         m_probability=None,
     ):
         """Represents a comparison using the jaro distance function
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
+            manual_col_name_for_charts_label (str, optional): string to include as
+                 column name in chart label. Acts as a manual overwrite of the
+                 colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
                 Comparison level with jaro score greater than 0.9
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.jaro_level("name", 0.9)
                 ```
                 Comparison level with a jaro score greater than 0.9 on a substring
                 of name column as determined by a regular expression.
 
                 ```python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.jaro_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Comparison level with jaro score greater than 0.9
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.jaro_level("name", 0.9)
                 ```
                 Comparison level with a jaro score greater than 0.9 on a substring
                 of name column as determined by a regular expression.
 
                 ```python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.jaro_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
+            === "SQLite"
+                Comparison level with jaro score greater than 0.9
+                ``` python
+                import splink.sqlite.comparison_level_library as cll
+                cll.jaro_level("name", 0.9)
+                ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the
                 jaro similarity
         """
 
         super().__init__(
@@ -585,54 +669,64 @@
     def __init__(
         self,
         col_name: str,
         distance_threshold: float,
         regex_extract: str = None,
         set_to_lowercase=False,
         include_colname_in_charts_label=False,
+        manual_col_name_for_charts_label=None,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using the jaro winkler distance function
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
+            manual_col_name_for_charts_label (str, optional): string to include as
+                 column name in chart label. Acts as a manual overwrite of the
+                 colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
                 Comparison level with jaro-winkler score greater than 0.9
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9)
                 ```
                 Comparison level with jaro-winkler score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Comparison level with jaro-winkler score greater than 0.9
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9)
                 ```
                 Comparison level with jaro-winkler score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.jaro_winkler_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
+            === "SQLite"
+                Comparison level with jaro-winkler score greater than 0.9
+                ``` python
+                import splink.sqlite.comparison_level_library as cll
+                cll.jaro_winkler_level("name", 0.9)
+                ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the
                 jaro winkler similarity
         """
 
         super().__init__(
@@ -657,51 +751,55 @@
     def __init__(
         self,
         col_name: str,
         distance_threshold: int | float,
         regex_extract: str = None,
         set_to_lowercase=False,
         include_colname_in_charts_label=False,
+        manual_col_name_for_charts_label=None,
         m_probability=None,
     ) -> ComparisonLevel:
         """Represents a comparison level using a jaccard distance function
 
         Args:
             col_name (str): Input column name
             distance_threshold (Union[int, float]): The threshold to use to assess
                 similarity
             regex_extract (str): Regular expression pattern to evaluate a match on.
             set_to_lowercase (bool): If True, sets all entries to lowercase.
             include_colname_in_charts_label (bool, optional): If True, includes
                 col_name in charts label
+            manual_col_name_for_charts_label (str, optional): string to include as
+                 column name in chart label. Acts as a manual overwrite of the
+                 colname when include_colname_in_charts_label is True.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
         Examples:
             === "DuckDB"
                 Comparison level with jaccard score greater than 0.9
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.jaccard_level("name", 0.9)
                 ```
                 Comparison level with jaccard score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.jaccard_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Comparison level with jaccard score greater than 0.9
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.jaccard_level("name", 0.9)
                 ```
                 Comparison level with jaccard score greater than 0.9 on a
                 substring of name column as determined by a regular expression.
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.jaccard_level("name", 0.9, regex_extract="^[A-Z]{1,4}")
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the jaccard similarity
         """
         super().__init__(
@@ -739,57 +837,61 @@
             tf_adjustment_column (str, optional): Column to use for term frequency
                 adjustments if an exact match is observed. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Comparison level on first_name and surname columns reversed
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Comparison level on first_name and surname columns reversed
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
             === "Athena"
                 Comparison level on first_name and surname columns reversed
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
                 Comparison level on first_name and surname column reversed
                 on a substring of each column as determined by a regular expression.
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.columns_reversed_level("first_name",
                                            "surname",
                                            regex_extract="^[A-Z]{1,4}")
                 ```
             === "SQLite"
                 Comparison level on first_name and surname columns reversed
                 ``` python
-                import splink.sqlite.sqlite_comparison_level_library as cll
+                import splink.sqlite.comparison_level_library as cll
+                cll.columns_reversed_level("first_name", "surname")
+            === "PostgreSQL"
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.columns_reversed_level("first_name", "surname")
                 ```
 
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the exact match of two
                 columns.
@@ -852,29 +954,35 @@
                 capturing nulls elsewhere in your comparison level.
             m_probability (float, optional): Starting value for m probability.
                 Defaults to None.
 
         Examples:
             === "DuckDB"
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.distance_in_km_level("lat_col",
                                         "long_col",
                                         km_threshold=5)
                 ```
             === "Spark"
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.distance_in_km_level("lat_col",
                                         "long_col",
                                         km_threshold=5)
                 ```
             === "Athena"
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
+                cll.distance_in_km_level("lat_col",
+                                        "long_col",
+                                        km_threshold=5)
+            === "PostgreSQL"
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.distance_in_km_level("lat_col",
                                         "long_col",
                                         km_threshold=5)
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the distance between
@@ -926,30 +1034,34 @@
                 the comparison level
             m_probability (float, optional): Starting value for m probability. Defaults
                 to None.
 
         Examples:
             === "DuckDB"
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
             === "Spark"
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
             === "Athena"
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
             === "SQLite"
                 ``` python
-                import splink.sqlite.sqlite_comparison_level_library as cll
+                import splink.sqlite.comparison_level_library as cll
+                cll.percentage_difference_level("value", 0.5)
+            === "PostgreSQL"
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.percentage_difference_level("value", 0.5)
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the percentage difference
                 between two values
 
@@ -996,25 +1108,29 @@
                 intersection of arrays for this comparison level. Defaults to 1
             include_colname_in_charts_label (bool, optional): Should the charts label
                 contain the column name? Defaults to False
 
         Examples:
             === "DuckDB"
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.array_intersect_level("name")
                 ```
             === "Spark"
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.array_intersect_level("name")
                 ```
             === "Athena"
                 ``` python
-                import splink.athena.athena_comparison_level_library as cll
+                import splink.athena.comparison_level_library as cll
+                cll.array_intersect_level("name")
+            === "PostgreSQL"
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
                 cll.array_intersect_level("name")
                 ```
 
         Returns:
             ComparisonLevel: A comparison level that evaluates the size of intersection
                 of arrays
         """
@@ -1079,68 +1195,96 @@
                 (the default), downstream functions for each backend assign
                 date_format to ISO 8601 format (yyyy-mm-dd).
 
         Examples:
             === "DuckDB"
                 Date Difference comparison level at threshold 1 year
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.datediff_level("date",
                                     date_threshold=1,
                                     date_metric="year"
                                     )
                 ```
                 Date Difference comparison with date-casting and unspecified
                 date_format (default = %Y-%m-%d)
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True
                                     )
                 ```
                 Date Difference comparison with date-casting and specified date_format
                 ``` python
-                import splink.duckdb.duckdb_comparison_level_library as cll
+                import splink.duckdb.comparison_level_library as cll
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True,
                                     date_format='%d/%m/%Y'
                                     )
                 ```
             === "Spark"
                 Date Difference comparison level at threshold 1 year
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.datediff_level("date",
                                     date_threshold=1,
                                     date_metric="year"
                                     )
                 ```
                 Date Difference comparison with date-casting and unspecified
                 date_format (default = %Y-%m-%d)
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True
                                     )
                 ```
                 Date Difference comparison with date-casting and specified date_format
                 ``` python
-                import splink.spark.spark_comparison_level_library as cll
+                import splink.spark.comparison_level_library as cll
                 cll.datediff_level("dob",
                                     date_threshold=3,
                                     date_metric='month',
                                     cast_strings_to_date=True,
                                     date_format='%d/%m/%Y'
                                     )
+            === "PostgreSQL"
+                Date Difference comparison level at threshold 1 year
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
+                cll.datediff_level("date",
+                                    date_threshold=1,
+                                    date_metric="year"
+                                    )
+                ```
+                Date Difference comparison with date-casting and unspecified
+                date_format (default = yyyy-MM-dd)
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
+                cll.datediff_level("dob",
+                                    date_threshold=3,
+                                    date_metric='month',
+                                    cast_strings_to_date=True
+                                    )
+                ```
+                Date Difference comparison with date-casting and specified date_format
+                ``` python
+                import splink.postgres.postgres_comparison_level_library as cll
+                cll.datediff_level("dob",
+                                    date_threshold=3,
+                                    date_metric='month',
+                                    cast_strings_to_date=True,
+                                    date_format='dd/MM/yyyy'
+                                    )
                 ```
         Returns:
             ComparisonLevel: A comparison level that evaluates whether two dates fall
                 within a given interval.
         """
 
         date = InputColumn(date_col, sql_dialect=self._sql_dialect)
```

### Comparing `splink-3.9.1/splink/comparison_level_sql.py` & `splink-3.9.2/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/comparison_library.py` & `splink-3.9.2/splink/comparison_library.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,51 +41,56 @@
             include_colname_in_charts_label: If true, append col name to label for
                 charts.  Defaults to False.
 
         Examples:
             === "DuckDB"
                 Create comparison with exact match level
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
                 ```
             === "Spark"
                 Create comparison with exact match level
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
                 ```
             === "Athena"
                 Create comparison with exact match level
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
                 cl.exact_match("first_name")
                 ```
                 Create comparison with exact match level based on a
                 substring of first_name as determined by a regular expression
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
                 cl.exact_match("first_name", regex_extract="^[A-Z]{1,4}")
                 ```
             === "SQLite"
                 Create comparison with exact match level
                 ``` python
-                import splink.sqlite.sqlite_comparison_library as cl
+                import splink.sqlite.comparison_library as cl
+                cl.exact_match("first_name")
+            === "PostgreSQL"
+                Create comparison with exact match level
+                ``` python
+                import splink.postgres.postgres_comparison_library as cl
                 cl.exact_match("first_name")
                 ```
 
         Returns:
             Comparison: A comparison for exact match that can be included in the Splink
                 settings dictionary
         """
@@ -167,69 +172,91 @@
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Apply the `jaccard` function in a comparison with levels 0.9 and 0.7
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7]
                                    )
                 ```
                 Apply the `jaccard` function in a comparison with levels 0.9 and 0.7 on
                 a substring of name column as determined by a regular expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7],
                                    regex_extract="^[A-Z]{1,4}
                                    )
                 ```
             === "Spark"
                 Apply the `jaccard` function in a comparison with levels 0.9 and 0.7
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7]
                                    )
                 ```
                 Apply the `jaccard` function in a comparison with levels 0.9 and 0.7 on
                 a substring of name column as determined by a regular expression
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7],
                                    regex_extract="^[A-Z]{1,4}
                                    )
                 ```
             === "Athena"
                 Apply the `levenshtein_distance` function in a comparison with
                 levels 1 and 2
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'levenshtein_distance',
                                    distance_threshold_or_thresholds = [1, 2],
                                    higher_is_more_similar = False
                                    )
                 ```
                 Apply the `jaccard` function in a comparison with levels 0.9 and 0.7 on
                 a substring of name column as determined by a regular expression
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
                 cl.distance_function_at_thresholds("name",
                                    distance_function_name = 'jaccard',
                                    distance_threshold_or_thresholds = [0.9, 0.7],
                                    regex_extract="^[A-Z]{1,4}
                                    )
+            === "SQLite"
+                Apply the `levenshtein` function in a comparison with
+                levels 1 and 2
+                ``` python
+                import splink.sqlite.comparison_library as cl
+                cl.distance_function_at_thresholds("name",
+                                   distance_function_name = 'levenshtein',
+                                   distance_threshold_or_thresholds = [1, 2],
+                                   higher_is_more_similar = False
+                                   )
+                ```
+            === "PostgreSQL"
+                Apply the `levenshtein` function in a comparison with
+                levels 1 and 2
+                ``` python
+                import splink.postgres.postgres_comparison_library as cl
+                cl.distance_function_at_thresholds("name",
+                                   distance_function_name = 'levenshtein',
+                                   distance_threshold_or_thresholds = [1, 2],
+                                   higher_is_more_similar = False
+                                   )
+                ```
                 ```
 
         Returns:
             Comparison: A comparison for a chosen distance function similarity that
                 can be included in the Splink settings dictionary.
         """
         # Validate user inputs
@@ -338,51 +365,65 @@
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 on a substring of name column as determined by a regular expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2], regex_extract="^A|B")
                 ```
             === "Spark"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 on a substring of name column as determined by a regular expression
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2], regex_extract="^A|B")
                 ```
             === "Athena"
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with levenshtein match levels with distance <=1
                 and <=2
                 on a substring of name column as determined by a regular expression
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
                 cl.levenshtein_at_thresholds("first_name", [1,2], regex_extract="^A|B")
+            === "SQLite"
+                Create comparison with levenshtein match levels with distance <=1
+                and <=2
+                ``` python
+                import splink.athena.comparison_library as cl
+                cl.levenshtein_at_thresholds("first_name", [1,2])
+                ```
+            === "PostgreSQL"
+                Create comparison with levenshtein match levels with distance <=1
+                and <=2
+                ``` python
+                import splink.postgres.postgres_comparison_library as cl
+                cl.levenshtein_at_thresholds("first_name", [1,2])
+                ```
                 ```
 
         Returns:
             Comparison: A comparison for Levenshtein similarity that can be included
                 in the Splink settings dictionary.
         """
 
@@ -450,44 +491,51 @@
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
         Examples:
             === "DuckDB"
                 Create comparison with damerau-levenshtein match levels with
-                distance <= 1
+                distance <= 1, 2
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with damerau-levenshtein match levels with
                 distance <= 1
                 on a substring of name column as determined by a regular expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name",
                                                      [1,2],
                                                      regex_extract="^A|B")
                 ```
             === "Spark"
                 Create comparison with damerau-levenshtein match levels with
-                distance <= 1
+                distance <= 1, 2
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with damerau-evenshtein match levels with
-                distance <= 1
+                distance <= 1, 2
                 on a substring of name column as determined by a regular expression
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.damerau_levenshtein_at_thresholds("first_name",
                                                      [1,2],
                                                      regex_extract="^A|B")
                 ```
+            === "SQLite"
+                Create comparison with damerau-levenshtein match levels with
+                distance <= 1, 2
+                ``` python
+                import splink.sqlite.comparison_library as cl
+                cl.damerau_levenshtein_at_thresholds("first_name", [1,2])
+                ```
 
         Returns:
             Comparison: A comparison for Damerau-Levenshtein similarity that can be
             included in the Splink settings dictionary.
         """
 
         super().__init__(
@@ -556,36 +604,36 @@
                 default m probability for the 'anything else' level. Defaults to None.
 
                 Examples:
             === "DuckDB"
                 Create comparison with jaccard match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.jaccard_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with jaccard match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.jaccard_at_thresholds("first_name", [1,2], regex_extract="^A|B")
                 ```
             === "Spark"
                 Create comparison with jaccard match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.jaccard_at_thresholds("first_name", [1,2])
                 ```
                 Create comparison with jaccard match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.jaccard_at_thresholds("first_name", [1,2], regex_extract="^A|B")
                 ```
 
         Returns:
             Comparison: A comparison for Jaccard similarity that can be included
                 in the Splink settings dictionary.
         """
@@ -656,38 +704,45 @@
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7], regex_extract="^[A-Z]")
                 ```
             === "Spark"
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro match levels with similarity score >=0.9
                 and >=0.7 on a substring of name column as determined by a regular
                 expression
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.jaro_at_thresholds("first_name", [0.9, 0.7], regex_extract="^[A-Z]")
                 ```
+            === "SQLite"
+                Create comparison with jaro match levels with similarity score >=0.9
+                and >=0.7
+                ``` python
+                import splink.sqlite.comparison_library as cl
+                cl.jaro_at_thresholds("first_name", [0.9, 0.7])
+                ```
 
         Returns:
             Comparison:
         """
 
         super().__init__(
             col_name,
@@ -756,44 +811,51 @@
 
 
         Examples:
             === "DuckDB"
                 Create comparison with jaro_winkler match levels with similarity
                 score >= 0.9 and >=0.7
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro_winkler match levels with similarity
                 score =>0.9 and >=0.7 on a substring of name column as determined by
                 a regular expression
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name",
                                               [0.9, 0.7],
                                               regex_extract="^[A-Z]"
                                               )
                 ```
             === "Spark"
                 Create comparison with jaro_winkler match levels with similarity
                 score >=0.9 and >=0.7
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
                 ```
                 Create comparison with jaro_winkler match levels with similarity
                 score >=0.9 and >=0.7 on a substring of name column as determined
                 by a regular expression
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.jaro_winkler_at_thresholds("first_name",
                                               [0.9, 0.7],
                                               regex_extract="^[A-Z]"
                                               )
                 ```
+            === "SQLite"
+                Create comparison with jaro_winkler match levels with similarity
+                score >=0.9 and >=0.7
+                ``` python
+                import splink.sqlite.comparison_library as cl
+                cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
+                ```
 
         Returns:
             Comparison: A comparison for Jaro Winkler similarity that can be included
                 in the Splink settings dictionary.
         """
 
         super().__init__(
@@ -844,25 +906,29 @@
                 for the sizes specified. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.array_intersect_at_sizes("first_name", [3, 1])
                 ```
             === "Spark"
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.array_intersect_at_sizes("first_name", [3, 1])
                 ```
             === "Athena"
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
+                cl.array_intersect_at_sizes("first_name", [3, 1])
+            === "PostgreSQL"
+                ``` python
+                import splink.postgres.postgres_comparison_library as cl
                 cl.array_intersect_at_sizes("first_name", [3, 1])
                 ```
 
         Returns:
             Comparison: A comparison for the intersection of arrays that can be included
                 in the Splink settings dictionary.
         """
@@ -979,73 +1045,104 @@
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Date Difference comparison at thresholds 10 days, 12 months and 15 years
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds = [10, 12, 15],
                                             date_metrics = ['day', 'month', 'year']
                                             )
                 ```
 
                 Datediff comparison with date-casting and unspecified date_format
                 (default = %Y-%m-%d)
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds=[1,5],
                                             date_metrics = ["day", "year"],
                                             cast_strings_to_date=True
                                             )
                 ```
                 Datediff comparison with date-casting and specified (non-default)
                 date_format
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds=[1,5],
                                             date_metrics = ["day", "year"],
                                             cast_strings_to_date=True,
                                             date_format='%d/%m/%Y'
                                             )
                 ```
             === "Spark"
                 Date Difference comparison at thresholds 10 days, 12 months and 15 years
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds = [10, 12, 15],
                                             date_metrics = ['day', 'month', 'year']
                                             )
                 ```
 
                 Datediff comparison with date-casting and unspecified date_format
                 (default = %Y-%m-%d)
                 ``` python
-                    import splink.spark.spark_comparison_library as cl
+                    import splink.spark.comparison_library as cl
                     cl.datediff_at_thresholds("date",
                                                 date_thresholds=[1,5],
                                                 date_metrics = ["day", "year"],
                                                 cast_strings_to_date=True
                                                 )
                 ```
 
                 Datediff comparison with date-casting and specified (non-default)
                 date_format
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.datediff_at_thresholds("date",
                                             date_thresholds=[1,5],
                                             date_metrics = ["day", "year"],
                                             cast_strings_to_date=True,
                                             date_format='%d/%m/%Y'
                                             )
+            === "PostgreSQL"
+                Date Difference comparison at thresholds 10 days, 12 months and 15 years
+                ``` python
+                import splink.postgres.postgres_comparison_library as cl
+                cl.datediff_at_thresholds("date",
+                                            date_thresholds = [10, 12, 15],
+                                            date_metrics = ['day', 'month', 'year']
+                                            )
+                ```
+
+                Datediff comparison with date-casting and unspecified date_format
+                (default = yyyy-MM-dd)
+                ``` python
+                    import splink.postgres.postgres_comparison_library as cl
+                    cl.datediff_at_thresholds("date",
+                                                date_thresholds=[1,5],
+                                                date_metrics = ["day", "year"],
+                                                cast_strings_to_date=True
+                                                )
+                ```
+
+                Datediff comparison with date-casting and specified (non-default)
+                date_format
+                ``` python
+                import splink.postgres.postgres_comparison_library as cl
+                cl.datediff_at_thresholds("date",
+                                            date_thresholds=[1,5],
+                                            date_metrics = ["day", "year"],
+                                            cast_strings_to_date=True,
+                                            date_format='dd/MM/yyyy'
+                                            )
                 ```
 
         Returns:
             Comparison: A comparison for Datediff that can be included in the Splink
                 settings dictionary.
         """
 
@@ -1152,31 +1249,38 @@
                 for the sizes specified. Defaults to None.
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 ``` python
-                import splink.duckdb.duckdb_comparison_library as cl
+                import splink.duckdb.comparison_library as cl
                 cl.distance_in_km_at_thresholds("lat_col",
                                            "long_col",
                                            km_thresholds = [0.1, 1, 10]
                                         )
                 ```
             === "Spark"
                 ``` python
-                import splink.spark.spark_comparison_library as cl
+                import splink.spark.comparison_library as cl
                 cl.distance_in_km_at_thresholds("lat_col",
                                            "long_col",
                                            km_thresholds = [0.1, 1, 10]
                                         )
                 ```
             === "Athena"
                 ``` python
-                import splink.athena.athena_comparison_library as cl
+                import splink.athena.comparison_library as cl
+                cl.distance_in_km_at_thresholds("lat_col",
+                                           "long_col",
+                                           km_thresholds = [0.1, 1, 10]
+                                        )
+            === "PostgreSQL"
+                ``` python
+                import splink.postgres.postgres_comparison_library as cl
                 cl.distance_in_km_at_thresholds("lat_col",
                                            "long_col",
                                            km_thresholds = [0.1, 1, 10]
                                         )
                 ```
 
         Returns:
```

### Comparing `splink-3.9.1/splink/comparison_library_utils.py` & `splink-3.9.2/splink/comparison_library_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     col_name: str,
     distance_function_name: str,
     distance_threshold_or_thresholds,
     regex_extract: str = None,
     set_to_lowercase: bool = False,
     higher_is_more_similar: bool = True,
     include_colname_in_charts_label=False,
+    manual_col_name_for_charts_label=None,
     m_probability_or_probabilities_thres: list = None,
 ):
     thresholds = ensure_is_iterable(distance_threshold_or_thresholds)
     threshold_comparison_levels = []
 
     if m_probability_or_probabilities_thres is None:
         m_probability_or_probabilities_thres = [None] * len(thresholds)
@@ -100,14 +101,15 @@
             higher_is_more_similar = True
 
         # these function arguments hold for all cases.
         kwargs = dict(
             col_name=col_name,
             distance_threshold=thres,
             include_colname_in_charts_label=include_colname_in_charts_label,
+            manual_col_name_for_charts_label=manual_col_name_for_charts_label,
             regex_extract=regex_extract,
             set_to_lowercase=set_to_lowercase,
             m_probability=m_prob,
         )
         # separate out the two that are only used
         # when we have a user-supplied function, rather than a predefined subclass
         # feels a bit hacky, but will do at least for time being
```

### Comparing `splink-3.9.1/splink/comparison_template_library.py` & `splink-3.9.2/splink/comparison_template_library.py`

 * *Files 12% similar despite different names*

```diff
@@ -104,54 +104,54 @@
             m_probability_else (float, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Basic Date Comparison
                 ``` python
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth")
                 ```
                 Bespoke Date Comparison
                 ``` python
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth",
                                     damerau_levenshtein_thresholds=[],
                                     levenshtein_thresholds=[2],
                                     datediff_thresholds=[1, 1],
                                     datediff_metrics=["month", "year"])
                 ```
                 Date Comparison casting columns date and assigning values that do not
                 match the date_format to the null level
                 ``` python
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth",
                                     cast_strings_to_date=True,
                                     date_format='%d/%m/%Y',
                                     invalid_dates_as_null=True)
                 ```
             === "Spark"
                 Basic Date Comparison
                 ``` python
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth")
                 ```
                 Bespoke Date Comparison
                 ``` python
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth",
                                     damerau_levenshtein_thresholds=[],
                                     levenshtein_thresholds=[2],
                                     datediff_thresholds=[1, 1],
                                     datediff_metrics=["month", "year"])
                 ```
                 Date Comparison casting columns date and assigning values that do not
                 match the date_format to the null level
                 ``` python
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.date_comparison("date_of_birth",
                                     cast_strings_to_date=True,
                                     date_format='dd/mm/yyyy',
                                     invalid_dates_as_null=True)
                 ```
         Returns:
             Comparison: A comparison that can be inclued in the Splink settings
@@ -388,46 +388,62 @@
                 the 'everything else' level. Defaults to None.
 
         Examples:
 
             === "DuckDB"
                 Basic Name Comparison
                 ``` python
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.name_comparison("name")
                 ```
                 Bespoke Name Comparison
                 ``` python
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.name_comparison("name",
                                     phonetic_col_name = "name_dm",
                                     term_frequency_adjustments = True,
                                     levenshtein_thresholds=[2],
                                     damerau_levenshtein_thresholds=[],
                                     jaro_winkler_thresholds=[],
                                     jaccard_thresholds=[1]
                                     )
                 ```
             === "Spark"
                 Basic Name Comparison
                 ``` python
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.name_comparison("name")
                 ```
                 Bespoke Name Comparison
                 ``` python
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.name_comparison("name",
                                     phonetic_col_name = "name_dm",
                                     term_frequency_adjustments = True,
                                     levenshtein_thresholds=[2],
                                     damerau_levenshtein_thresholds=[],
                                     jaro_winkler_thresholds=[],
                                     jaccard_thresholds=[1]
                                     )
+            === "SQLite"
+                Basic Name Comparison
+                ``` python
+                import splink.sqlite.comparison_template_library as ctl
+                ctl.name_comparison("name")
+                ```
+                Bespoke Name Comparison
+                ``` python
+                import splink.sqlite.comparison_template_library as ctl
+                ctl.name_comparison("name",
+                                    phonetic_col_name = "name_dm",
+                                    term_frequency_adjustments = True,
+                                    levenshtein_thresholds=[2],
+                                    damerau_levenshtein_thresholds=[],
+                                    jaro_winkler_thresholds=[0.8],
+                                    )
                 ```
 
         Returns:
             Comparison: A comparison that can be included in the Splink settings
                 dictionary.
         """
 
@@ -517,15 +533,15 @@
             threshold_comparison_levels = distance_threshold_comparison_levels(
                 self,
                 col_name,
                 distance_function_name="jaccard",
                 distance_threshold_or_thresholds=jaccard_thresholds,
                 regex_extract=regex_extract,
                 set_to_lowercase=set_to_lowercase,
-                m_probability_or_probabilities_thres=m_probability_or_probabilities_jar,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_jac,
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         comparison_levels.append(
             self._else_level(m_probability=m_probability_else),
         )
 
@@ -596,23 +612,23 @@
         jaro_thresholds: float | list = [],
         jaccard_thresholds: float | list = [],
         m_probability_exact_match_forename_surname: float = None,
         m_probability_exact_match_phonetic_forename_surname: float = None,
         m_probability_columns_reversed_forename_surname: float = None,
         m_probability_exact_match_surname: float = None,
         m_probability_exact_match_forename: float = None,
-        m_probability_exact_match_phonetic_surname: float = None,
-        m_probability_exact_match_phonetic_forename: float = None,
         m_probability_or_probabilities_surname_lev: float | list = None,
         m_probability_or_probabilities_surname_dl: float | list = None,
         m_probability_or_probabilities_surname_jw: float | list = None,
+        m_probability_or_probabilities_surname_jar: float | list = None,
         m_probability_or_probabilities_surname_jac: float | list = None,
         m_probability_or_probabilities_forename_lev: float | list = None,
         m_probability_or_probabilities_forename_dl: float | list = None,
         m_probability_or_probabilities_forename_jw: float | list = None,
+        m_probability_or_probabilities_forename_jar: float | list = None,
         m_probability_or_probabilities_forename_jac: float | list = None,
         m_probability_else: float = None,
     ) -> Comparison:
         """A wrapper to generate a comparison for a name column the data in
         `col_name` with preselected defaults.
 
         The default arguments will give a comparison with comparison levels:\n
@@ -720,43 +736,49 @@
                 for the thresholds specified. Defaults to None.
             m_probability_or_probabilities_surname_dl (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_or_probabilities_surname_jw (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_surname_jar (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
             m_probability_or_probabilities_surname_jac (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_or_probabilities_forename_lev (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_or_probabilities_forename_dl (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_or_probabilities_forename_jw (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_forename_jar (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
             m_probability_or_probabilities_forename_jac (Union[float, list], optional):
                 _description_. If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Basic Forename Surname Comparison
                 ```py
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.forename_surname_comparison("first_name", "surname)
                 ```
 
                 Bespoke Forename Surname Comparison
                 ```py
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.forename_surname_comparison(
                         "forename",
                         "surname",
                         term_frequency_adjustments=True,
                         tf_adjustment_col_forename_and_surname="full_name",
                         phonetic_forename_col_name="forename_dm",
                         phonetic_surname_col_name="surname_dm",
@@ -764,33 +786,54 @@
                         jaro_winkler_thresholds=[],
                         jaccard_thresholds=[1],
                     )
                 ```
             === "Spark"
                 Basic Forename Surname Comparison
                 ```py
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.forename_surname_comparison("first_name", "surname)
                 ```
 
                 Bespoke Forename Surname Comparison
                 ```py
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.forename_surname_comparison(
                         "forename",
                         "surname",
                         term_frequency_adjustments=True,
                         tf_adjustment_col_forename_and_surname="full_name",
                         phonetic_forename_col_name="forename_dm",
                         phonetic_surname_col_name="surname_dm",
                         levenshtein_thresholds=[2],
                         jaro_winkler_thresholds=[],
                         jaccard_thresholds=[1],
                     )
                 ```
+            === "SQLite"
+                Basic Forename Surname Comparison
+                ```py
+                import splink.sqlite.comparison_template_library as ctl
+                ctl.forename_surname_comparison("first_name", "surname)
+                ```
+
+                Bespoke Forename Surname Comparison
+                ```py
+                import splink.sqlite.comparison_template_library as ctl
+                ctl.forename_surname_comparison(
+                        "forename",
+                        "surname",
+                        term_frequency_adjustments=True,
+                        tf_adjustment_col_forename_and_surname="full_name",
+                        phonetic_forename_col_name="forename_dm",
+                        phonetic_surname_col_name="surname_dm",
+                        levenshtein_thresholds=[2],
+                        jaro_winkler_thresholds=[0.8],
+                    )
+                ```
 
 
         Returns:
             Comparison: A comparison that can be included in the Splink settings
                 dictionary.
         """
 
@@ -858,15 +901,15 @@
 
         ### Surname Exact match
 
         comparison_level = self._exact_match_level(
             surname_col_name,
             set_to_lowercase=set_to_lowercase,
             term_frequency_adjustments=term_frequency_adjustments,
-            m_probability=m_probability_exact_match_forename,
+            m_probability=m_probability_exact_match_surname,
             include_colname_in_charts_label=True,
         )
         comparison_levels.append(comparison_level)
 
         ### Forename Exact match
 
         comparison_level = self._exact_match_level(
@@ -912,18 +955,18 @@
             )
             comparison_levels = comparison_levels + threshold_comparison_levels
 
         if len(jaro_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 surname_col_name,
-                distance_function_name="jaro-winkler",
-                distance_threshold_or_thresholds=jaro_winkler_thresholds,
+                distance_function_name="jaro-",
+                distance_threshold_or_thresholds=jaro_thresholds,
                 set_to_lowercase=set_to_lowercase,
-                m_probability_or_probabilities_thres=m_probability_or_probabilities_surname_jw,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_surname_jar,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
         if len(jaro_winkler_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
@@ -982,14 +1025,26 @@
                 distance_threshold_or_thresholds=jaro_winkler_thresholds,
                 set_to_lowercase=set_to_lowercase,
                 m_probability_or_probabilities_thres=m_probability_or_probabilities_forename_jw,
                 include_colname_in_charts_label=True,
             )
             comparison_levels = comparison_levels + threshold_levels
 
+        if len(jaro_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                forename_col_name,
+                distance_function_name="jaro",
+                distance_threshold_or_thresholds=jaro_thresholds,
+                set_to_lowercase=set_to_lowercase,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_forename_jar,
+                include_colname_in_charts_label=True,
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
         if len(jaccard_thresholds) > 0:
             threshold_levels = distance_threshold_comparison_levels(
                 self,
                 forename_col_name,
                 distance_function_name="jaccard",
                 distance_threshold_or_thresholds=jaccard_thresholds,
                 set_to_lowercase=set_to_lowercase,
@@ -1160,54 +1215,54 @@
             m_probability_else (float, optional): Starting m probability for
                 the 'everything else' level. Defaults to None.
 
         Examples:
             === "DuckDB"
                 Basic Postcode Comparison
                 ``` python
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode")
                 ```
                 Bespoke Postcode Comparison
                 ``` python
-                import splink.duckdb.duckdb_comparison_template_library as ctl
+                import splink.duckdb.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode",
                                     invalid_postcodes_as_null=True,
                                     include_distance_in_km_level=True,
                                     lat_col="lat",
                                     long_col="long",
                                     km_thresholds=[10, 100]
                                     )
                 ```
             === "Spark"
                 Basic Postcode Comparison
                 ``` python
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode")
                 ```
                 Bespoke Postcode Comparison
                 ``` python
-                import splink.spark.spark_comparison_template_library as ctl
+                import splink.spark.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode",
                                     invalid_postcodes_as_null=True,
                                     include_distance_in_km_level=True,
                                     lat_col="lat",
                                     long_col="long",
                                     km_thresholds=[10, 100]
                                     )
                 ```
             === "Athena"
                 Basic Postcode Comparison
                 ``` python
-                import splink.athean.athena_comparison_template_library as ctl
+                import splink.athena.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode")
                 ```
                 Bespoke Postcode Comparison
                 ``` python
-                import splink.athena.athena_comparison_template_library as ctl
+                import splink.athena.comparison_template_library as ctl
                 ctl.postcode_comparison("postcode",
                                     invalid_postcodes_as_null=True,
                                     include_distance_in_km_level=True,
                                     lat_col="lat",
                                     long_col="long",
                                     km_thresholds=[10, 100]
                                     )
@@ -1238,35 +1293,35 @@
 
         if include_sector_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
                 regex_extract="^[A-Za-z]{1,2}[0-9][A-Za-z0-9]? [0-9]",
                 set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_sector_match,
-                manual_chart_label="Postcode Sector",
+                manual_col_name_for_charts_label="Postcode Sector",
             )
             comparison_levels.append(comparison_level)
 
         if include_district_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
                 regex_extract="^[A-Za-z]{1,2}[0-9][A-Za-z0-9]?",
                 set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_district_match,
-                manual_chart_label="Postcode District",
+                manual_col_name_for_charts_label="Postcode District",
             )
             comparison_levels.append(comparison_level)
 
         if include_area_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
                 regex_extract="^[A-Za-z]{1,2}",
                 set_to_lowercase=set_to_lowercase,
                 m_probability=m_probability_area_match,
-                manual_chart_label="Postcode Area",
+                manual_col_name_for_charts_label="Postcode Area",
             )
             comparison_levels.append(comparison_level)
 
         km_thresholds = ensure_is_iterable(km_thresholds)
         if len(km_thresholds) > 0:
             if m_probability_or_probabilities_km_distance is None:
                 m_probability_or_probabilities_km_distance = [None] * len(km_thresholds)
@@ -1314,7 +1369,353 @@
 
         comparison_dict = {
             "output_column_name": col_name,
             "comparison_description": comparison_desc,
             "comparison_levels": comparison_levels,
         }
         super().__init__(comparison_dict)
+
+
+class EmailComparisonBase(Comparison):
+    def __init__(
+        self,
+        col_name: str,
+        invalid_emails_as_null: bool = False,
+        valid_email_regex: str = "^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+[.][a-zA-Z]{2,}$",
+        term_frequency_adjustments_full: bool = False,
+        include_exact_match_level: bool = True,
+        include_username_match_level: bool = True,
+        include_domain_match_level: bool = False,
+        levenshtein_thresholds: int | list = [],
+        damerau_levenshtein_thresholds: int | list = [],
+        jaro_winkler_thresholds: float | list = [0.88],
+        jaro_thresholds: float | list = [],
+        m_probability_full_match: bool = None,
+        m_probability_username_match: bool = None,
+        m_probability_or_probabilities_username_lev: float | list = None,
+        m_probability_or_probabilities_username_dl: float | list = None,
+        m_probability_or_probabilities_username_jw: float | list = None,
+        m_probability_or_probabilities_username_jar: float | list = None,
+        m_probability_or_probabilities_email_lev: float | list = None,
+        m_probability_or_probabilities_email_dl: float | list = None,
+        m_probability_or_probabilities_email_jw: float | list = None,
+        m_probability_or_probabilities_email_jar: float | list = None,
+        m_probability_domain_match: float | list = None,
+        m_probability_else: float | list = None,
+    ) -> Comparison:
+        """A wrapped to generate a comparison for an email colummn
+        'col_name' with preselected defaults.
+
+        The default arguments will give a comparison with levels:\n
+        - Exact match on email\n
+        - Exact match on username with different domain\n
+        - Fuzzy match on email user Jaro-Winkler\n
+        - Fuzzy match on username using Jaro-Winkler \n
+        - All other comparisons
+
+        Args:
+            col_name (str): The name of the column to compare.
+            invalid_email_as_null (bool): If True, emails that do not adhere
+                to valid_email_regex will be included in the null level.
+                Defaults to False
+            valid_email_regex (str): regular expression pattern that is used
+                to validate emails. If invalid_emails_as_null is True,
+                emails that do not adhere to valid_email_regex will be included
+                 in the null level.
+                 Defaults to "^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$"
+            term_frequency_adjustments_full (bool, optional): If True, apply
+                term frequency adjustments to the full email exact match level.
+                Defaults to False.
+            include_exact_match_level (bool, optional): If True, include an exact
+                match on full email level. Defaults to True.
+            include_username_match_level (bool, optional): If True, include an exact
+                match on username only level. Defaults to True.
+            include_domain_match_level (bool, optional): If True, include an exact
+                match on domain only level. Defaults to True.
+            levenshtein_thresholds (Union[int, list], optional): The thresholds
+                to use for levenshtein similarity level(s).
+                Defaults to []
+            damerau_levenshtein_thresholds (Union[int, list], optional): The thresholds
+                to use for damerau-levenshtein similarity level(s).
+                Defaults to []
+            jaro_winkler_thresholds (Union[int, list], optional): The thresholds
+                to use for jaro_winkler similarity level(s).
+                Defaults to [0.88]
+            jaro_thresholds (Union[int, list], optional): The thresholds
+                to use for jaro similarity level(s).
+                Defaults to []
+            m_probability_full_match (float, optional): Starting m
+                probability for full match level. Defaults to None.
+            m_probability_username_match (float, optional): Starting m probability
+                for username only match level. Defaults to None.
+            m_probability_or_probabilities_username_lev (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_username_dl (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_username_jw (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_username_jar (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_email_lev (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_email_dl (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_email_jw (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_email_jar (Union[float, list], optional):
+                _description_. If provided, overrides the default m probabilities
+                for the thresholds specified. Defaults to None.
+            m_probability_domain_match (float, optional): Starting m probability
+                for domain only match level. Defaults to None.
+            m_probability_else (float, optional): Starting m probability for
+                the 'everything else' level. Defaults to None.
+
+        Examples:
+            === "DuckDB"
+                Basic email Comparison
+                ``` python
+                import splink.duckdb.duckdb_comparison_template_library as ctl
+                ctl.email_comparison("email")
+                ```
+                Bespoke email Comparison
+                ``` python
+                import splink.duckdb.duckdb_comparison_template_library as ctl
+                ctl.email_comparison("email",
+                                    levenshtein_thresholds = [2],
+                                    damerau_levenshtein_thresholds = [2],
+                                    invalid_emails_as_null = True,
+                                    include_username_match_level = True,
+                                    include_domain_match_level = True,
+                                    )
+                ```
+            === "Spark"
+                Basic email Comparison
+                ``` python
+                import splink.spark.spark_comparison_template_library as ctl
+                ctl.email_comparison(col_name = "email")
+                ```
+                Bespoke email Comparison
+                ``` python
+                import splink.spark.spark_comparison_template_library as ctl
+                ctl.email_comparison("email",
+                                    levenshtein_thresholds = [2],
+                                    damerau_levenshtein_thresholds = [2],
+                                    invalid_emails_as_null = True,
+                                    include_username_match_level = True,
+                                    include_domain_match_level = True,
+                                    )
+
+                ```
+
+        Returns:
+            Comparison: A comparison that can be inclued in the Splink settings
+                dictionary.
+        """
+        # Contstruct comparrison
+
+        comparison_levels = []
+
+        # Decide whether invalid emails should be treated as null
+        if invalid_emails_as_null:
+            comparison_levels.append(self._null_level(col_name, valid_email_regex))
+        else:
+            comparison_levels.append(self._null_level(col_name))
+
+        # Exact match on full email
+
+        if include_exact_match_level:
+            comparison_level = self._exact_match_level(
+                col_name,
+                regex_extract=None,
+                term_frequency_adjustments=term_frequency_adjustments_full,
+                m_probability=m_probability_full_match,
+                include_colname_in_charts_label=True,
+            )
+            comparison_levels.append(comparison_level)
+
+        # Exact match on username with different domain
+
+        if include_username_match_level:
+            comparison_level = self._exact_match_level(
+                col_name,
+                regex_extract="^[^@]+",
+                m_probability=m_probability_username_match,
+                include_colname_in_charts_label=True,
+                manual_col_name_for_charts_label="Username",
+            )
+            comparison_levels.append(comparison_level)
+
+        # Ensure fuzzy match thresholds are iterable
+
+        damerau_levenshtein_thresholds = ensure_is_iterable(
+            damerau_levenshtein_thresholds
+        )
+        levenshtein_thresholds = ensure_is_iterable(levenshtein_thresholds)
+        jaro_winkler_thresholds = ensure_is_iterable(jaro_winkler_thresholds)
+        jaro_thresholds = ensure_is_iterable(jaro_thresholds)
+
+        # Fuzzy match on full email
+
+        if len(levenshtein_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                distance_function_name="levenshtein",
+                distance_threshold_or_thresholds=levenshtein_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_email_lev,
+                include_colname_in_charts_label=True,
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        if len(damerau_levenshtein_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                distance_function_name="damerau-levenshtein",
+                distance_threshold_or_thresholds=damerau_levenshtein_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_email_dl,
+                include_colname_in_charts_label=True,
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        if len(jaro_winkler_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                distance_function_name="jaro-winkler",
+                distance_threshold_or_thresholds=jaro_winkler_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_email_jw,
+                include_colname_in_charts_label=True,
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        if len(jaro_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                distance_function_name="jaro",
+                distance_threshold_or_thresholds=jaro_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_email_jar,
+                include_colname_in_charts_label=True,
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        # Fuzzy match on username only
+        if len(levenshtein_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                regex_extract="^[^@]+",
+                distance_function_name="levenshtein",
+                distance_threshold_or_thresholds=levenshtein_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_username_lev,
+                include_colname_in_charts_label=True,
+                manual_col_name_for_charts_label="Username",
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        if len(damerau_levenshtein_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                regex_extract="^[^@]+",
+                distance_function_name="damerau-levenshtein",
+                distance_threshold_or_thresholds=damerau_levenshtein_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_username_dl,
+                include_colname_in_charts_label=True,
+                manual_col_name_for_charts_label="Username",
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        if len(jaro_winkler_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                regex_extract="^[^@]+",
+                distance_function_name="jaro-winkler",
+                distance_threshold_or_thresholds=jaro_winkler_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_username_jw,
+                include_colname_in_charts_label=True,
+                manual_col_name_for_charts_label="Username",
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        if len(jaro_thresholds) > 0:
+            threshold_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                distance_function_name="jaro",
+                distance_threshold_or_thresholds=jaro_thresholds,
+                m_probability_or_probabilities_thres=m_probability_or_probabilities_email_jar,
+                include_colname_in_charts_label=True,
+            )
+            comparison_levels = comparison_levels + threshold_levels
+
+        # Domain-only match
+
+        if include_domain_match_level:
+            comparison_level = self._exact_match_level(
+                col_name,
+                regex_extract="@([^@]+)$",
+                m_probability=m_probability_domain_match,
+                manual_col_name_for_charts_label="Email Domain",
+            )
+            comparison_levels.append(comparison_level)
+
+        comparison_levels.append(
+            self._else_level(m_probability=m_probability_else),
+        )
+
+        # Construct Description
+
+        comparison_desc = ""
+        if include_exact_match_level:
+            comparison_desc += "Exact match vs. "
+
+        if include_username_match_level:
+            comparison_desc += "Exact username match different domain vs. "
+
+        if len(levenshtein_thresholds) > 0:
+            comparison_desc += distance_threshold_description(
+                "fuzzy email", "levenshtein", jaro_winkler_thresholds
+            )
+            comparison_desc += distance_threshold_description(
+                "fuzzy username", "levenshtein", jaro_winkler_thresholds
+            )
+
+        if len(damerau_levenshtein_thresholds) > 0:
+            comparison_desc += distance_threshold_description(
+                "fuzzy email", "damerau_levenshtein", jaro_winkler_thresholds
+            )
+            comparison_desc += distance_threshold_description(
+                "fuzzy username", "levenshtein", jaro_winkler_thresholds
+            )
+
+        if len(jaro_winkler_thresholds) > 0:
+            comparison_desc += distance_threshold_description(
+                "fuzzy email", "jaro_winkler", jaro_winkler_thresholds
+            )
+            comparison_desc += distance_threshold_description(
+                "fuzzy username", "jaro_winkler", jaro_winkler_thresholds
+            )
+
+        if include_domain_match_level:
+            comparison_desc += "Domain-only match vs."
+
+        comparison_desc += "anything else"
+
+        comparison_dict = {
+            "comparison_description": comparison_desc,
+            "comparison_levels": comparison_levels,
+        }
+        super().__init__(comparison_dict)
+
+    @property
+    def _is_distance_subclass(self):
+        return False
```

### Comparing `splink-3.9.1/splink/comparison_vector_distribution.py` & `splink-3.9.2/splink/comparison_vector_distribution.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/comparison_vector_values.py` & `splink-3.9.2/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/connected_components.py` & `splink-3.9.2/splink/connected_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,16 +211,16 @@
     and it can be used here to reduce our neighbours table to only those nodes that need
     updating.
     """
 
     sql = f"""
     select
 
-    node_id,
-    min(representative) as representative
+    source.node_id,
+    min(source.representative) as representative
 
     from
     (
 
         select
 
             neighbours.node_id,
@@ -239,16 +239,16 @@
         select
 
             node_id,
             representative
 
         from {prev_representatives}
 
-    )
-    group by node_id
+    ) AS source
+    group by source.node_id
         """
 
     return sql
 
 
 def _cc_update_representatives_loop_cond(
     prev_representatives,
```

### Comparing `splink-3.9.1/splink/convert_v2_to_v3.py` & `splink-3.9.2/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/databricks/enable_splink.py` & `splink-3.9.2/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/default_from_jsonschema.py` & `splink-3.9.2/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/dialect_base.py` & `splink-3.9.2/splink/dialect_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_base.py` & `splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py` & `splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ...comparison_level_library import (
     ArrayIntersectLevelBase,
     ColumnsReversedLevelBase,
+    DamerauLevenshteinLevelBase,
     DateDiffLevelBase,
     DistanceFunctionLevelBase,
     DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
     JaccardLevelBase,
     JaroLevelBase,
@@ -23,14 +24,15 @@
     JaccardAtThresholdsComparisonBase,
     JaroAtThresholdsComparisonBase,
     JaroWinklerAtThresholdsComparisonBase,
     LevenshteinAtThresholdsComparisonBase,
 )
 from ...comparison_template_library import (
     DateComparisonBase,
+    EmailComparisonBase,
     ForenameSurnameComparisonBase,
     NameComparisonBase,
     PostcodeComparisonBase,
 )
 from .duckdb_base import (
     DuckDBBase,
 )
@@ -114,15 +116,15 @@
     pass
 
 
 class levenshtein_level(DuckDBBase, LevenshteinLevelBase):
     pass
 
 
-class damerau_levenshtein_level(DuckDBBase, LevenshteinLevelBase):
+class damerau_levenshtein_level(DuckDBBase, DamerauLevenshteinLevelBase):
     pass
 
 
 class jaro_level(DuckDBBase, JaroLevelBase):
     pass
 
 
@@ -242,7 +244,13 @@
     @property
     def _distance_level(self):
         return distance_function_level
 
 
 class postcode_comparison(DuckDBComparisonProperties, PostcodeComparisonBase):
     pass
+
+
+class email_comparison(DuckDBComparisonProperties, EmailComparisonBase):
+    @property
+    def _distance_level(self):
+        return distance_function_level
```

### Comparing `splink-3.9.1/splink/duckdb/duckdb_helpers/duckdb_helpers.py` & `splink-3.9.2/splink/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/duckdb/linker.py` & `splink-3.9.2/splink/duckdb/linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,26 +245,28 @@
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         # Registration errors will automatically
         # occur if an invalid data type is passed as an argument
         self._con.register(table_name, input)
 
-    def _random_sample_sql(self, proportion, sample_size, seed=None):
+    def _random_sample_sql(
+        self, proportion, sample_size, seed=None, table=None, unique_id=None
+    ):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         if seed:
             return f"USING SAMPLE bernoulli({percent}%) REPEATABLE({seed})"
         else:
             return f"USING SAMPLE {percent}% (bernoulli)"
 
     @property
     def _infinity_expression(self):
-        return "cast('infinity' as double)"
+        return "cast('infinity' as float8)"
 
     def _table_exists_in_database(self, table_name):
         sql = f"PRAGMA table_info('{table_name}');"
 
         # From duckdb 0.5.0, duckdb will raise a CatalogException
         # which does not exist in 0.4.0 or before
```

### Comparing `splink-3.9.1/splink/em_training_session.py` & `splink-3.9.2/splink/em_training_session.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/estimate_u.py` & `splink-3.9.2/splink/estimate_u.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,42 +57,48 @@
         """
 
         training_linker._enqueue_sql(sql, "__splink__df_concat_count")
         dataframe = training_linker._execute_sql_pipeline([nodes_with_tf])
 
         result = dataframe.as_record_dict()
         dataframe.drop_table_from_database()
-        count_rows = result[0]["count"]
+        total_nodes = result[0]["count"]
         sample_size = _rows_needed_for_n_pairs(max_pairs)
-        proportion = sample_size / count_rows
+        proportion = sample_size / total_nodes
 
     if settings_obj._link_type == "link_only":
         sql = """
         select count(source_dataset) as count
         from __splink__df_concat_with_tf
         group by source_dataset
         """
         training_linker._enqueue_sql(sql, "__splink__df_concat_count")
         dataframe = training_linker._execute_sql_pipeline([nodes_with_tf])
         result = dataframe.as_record_dict()
         dataframe.drop_table_from_database()
         frame_counts = [res["count"] for res in result]
         # total valid links is sum of pairwise product of individual row counts
-        count_rows = (
+        # i.e. if frame_counts are [a, b, c, d, ...],
+        # total_links = a*b + a*c + a*d + ... + b*c + b*d + ... + c*d + ...
+        total_links = (
             sum(frame_counts) ** 2 - sum([count**2 for count in frame_counts])
         ) / 2
+        total_nodes = sum(frame_counts)
 
-        sample_size = (max_pairs * count_rows) ** 0.5
-        proportion = sample_size / count_rows
+        # if we scale each frame by a proportion total_links scales with the square
+        # i.e. (our target) max_pairs == proportion^2 * total_links
+        proportion = (max_pairs / total_links) ** 0.5
+        # sample size is for df_concat_with_tf, i.e. proportion of the total nodes
+        sample_size = proportion * total_nodes
 
     if proportion >= 1.0:
         proportion = 1.0
 
-    if sample_size > count_rows:
-        sample_size = count_rows
+    if sample_size > total_nodes:
+        sample_size = total_nodes
 
     sql = f"""
     select *
     from __splink__df_concat_with_tf
     {training_linker._random_sample_sql(proportion, sample_size, seed)}
     """
     training_linker._enqueue_sql(sql, "__splink__df_concat_with_tf_sample")
@@ -114,15 +120,15 @@
         sample_dataframe = [df_sample]
 
     sql = compute_comparison_vector_values_sql(settings_obj)
 
     training_linker._enqueue_sql(sql, "__splink__df_comparison_vectors")
 
     sql = """
-    select *, cast(0.0 as double) as match_probability
+    select *, cast(0.0 as float8) as match_probability
     from __splink__df_comparison_vectors
     """
 
     training_linker._enqueue_sql(sql, "__splink__df_predict")
 
     sql = compute_new_parameters_sql(settings_obj)
     linker._enqueue_sql(sql, "__splink__m_u_counts")
```

### Comparing `splink-3.9.1/splink/expectation_maximisation.py` & `splink-3.9.2/splink/expectation_maximisation.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.9.2/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "data": {
         "values": []
     },
     "encoding": {
         "color": {
             "field": "rule",
             "legend": null,
```

### Comparing `splink-3.9.1/splink/files/chart_defs/comparator_score_chart.json` & `splink-3.9.2/splink/files/chart_defs/comparator_score_chart.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.844375%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'hconcat'": "{0: {'layer': {0: {'mark': {replace: OrderedDict([('type', 'rect')])}, delete: "*

 * *              "['height', 'width']}, 1: {delete: ['height', 'width']}}, 'height': 300, 'width': "*

 * *              "300}, 1: {'layer': {0: {'mark': {replace: OrderedDict([('type', 'rect')])}, delete: "*

 * *              "['height', 'width']}, 1: {delete: ['height', 'width']}}, 'height': 300, 'width': "*

 * *              '200}}'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.17.0.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "view": {
             "continuousHeight": 300,
             "continuousWidth": 400
         }
     },
     "datasets": {
@@ -11,14 +11,15 @@
         "data-similarity": []
     },
     "hconcat": [
         {
             "data": {
                 "name": "data-similarity"
             },
+            "height": 300,
             "layer": [
                 {
                     "encoding": {
                         "color": {
                             "field": "score",
                             "scale": {
                                 "domain": [
@@ -37,18 +38,18 @@
                             "type": "ordinal"
                         },
                         "y": {
                             "field": "strings_to_compare",
                             "type": "ordinal"
                         }
                     },
-                    "height": 300,
-                    "mark": "rect",
-                    "title": "Heatmap of Similarity Scores",
-                    "width": 300
+                    "mark": {
+                        "type": "rect"
+                    },
+                    "title": "Heatmap of Similarity Scores"
                 },
                 {
                     "encoding": {
                         "color": {
                             "condition": {
                                 "test": "(datum.quantity > 3)",
                                 "value": "white"
@@ -65,28 +66,28 @@
                             "type": "ordinal"
                         },
                         "y": {
                             "field": "strings_to_compare",
                             "type": "ordinal"
                         }
                     },
-                    "height": 300,
                     "mark": {
                         "baseline": "middle",
                         "type": "text"
                     },
-                    "title": "Heatmap of Similarity Scores",
-                    "width": 300
+                    "title": "Heatmap of Similarity Scores"
                 }
-            ]
+            ],
+            "width": 300
         },
         {
             "data": {
                 "name": "data-distance"
             },
+            "height": 300,
             "layer": [
                 {
                     "encoding": {
                         "color": {
                             "field": "score",
                             "scale": {
                                 "domain": [
@@ -105,18 +106,18 @@
                             "type": "ordinal"
                         },
                         "y": {
                             "field": "strings_to_compare",
                             "type": "ordinal"
                         }
                     },
-                    "height": 300,
-                    "mark": "rect",
-                    "title": "Heatmap of Distance Scores",
-                    "width": 200
+                    "mark": {
+                        "type": "rect"
+                    },
+                    "title": "Heatmap of Distance Scores"
                 },
                 {
                     "encoding": {
                         "color": {
                             "condition": {
                                 "test": "(datum.quantity > 3)",
                                 "value": "white"
@@ -132,23 +133,22 @@
                             "type": "ordinal"
                         },
                         "y": {
                             "field": "strings_to_compare",
                             "type": "ordinal"
                         }
                     },
-                    "height": 300,
                     "mark": {
                         "baseline": "middle",
                         "type": "text"
                     },
-                    "title": "Heatmap of Distance Scores",
-                    "width": 200
+                    "title": "Heatmap of Distance Scores"
                 }
-            ]
+            ],
+            "width": 200
         }
     ],
     "resolve": {
         "scale": {
             "color": "independent"
         }
     }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/comparator_score_threshold_chart.json` & `splink-3.9.2/splink/files/chart_defs/comparator_score_threshold_chart.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{'view': {replace: OrderedDict([('discreteWidth', 500), ('discreteHeight', 300)])}}",*

 * * "'layer'": "{0: {'mark': {replace: OrderedDict([('type', 'rect')])}, delete: ['height', "*

 * *            "'width']}, 1: {delete: ['height', 'width']}}"}*

```diff
@@ -1,13 +1,13 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.17.0.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "view": {
-            "continuousHeight": 300,
-            "continuousWidth": 400
+            "discreteHeight": 300,
+            "discreteWidth": 500
         }
     },
     "data": {
         "name": "data-with-thresholds"
     },
     "datasets": {
         "data-with-thresholds": []
@@ -30,18 +30,18 @@
                     "type": "ordinal"
                 },
                 "y": {
                     "field": "strings_to_compare",
                     "type": "ordinal"
                 }
             },
-            "height": 300,
-            "mark": "rect",
-            "title": [],
-            "width": 500
+            "mark": {
+                "type": "rect"
+            },
+            "title": []
         },
         {
             "encoding": {
                 "color": {
                     "condition": {
                         "test": "(datum.quantity > 3)",
                         "value": "white"
@@ -57,16 +57,14 @@
                     "type": "ordinal"
                 },
                 "y": {
                     "field": "strings_to_compare",
                     "type": "ordinal"
                 }
             },
-            "height": 300,
             "mark": {
                 "baseline": "middle",
                 "type": "text"
-            },
-            "width": 500
+            }
         }
     ]
 }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/completeness.json` & `splink-3.9.2/splink/files/chart_defs/completeness.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.17.0.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "view": {
             "continuousHeight": 300,
             "continuousWidth": 400
         }
     },
     "data": {},
```

### Comparing `splink-3.9.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json` & `splink-3.9.2/splink/files/chart_defs/tf_adjustment_chart.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.17708333333333334%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{replace: OrderedDict([('params', [OrderedDict([('name', 'gamma_sel'), ('bind', "*

 * *             "OrderedDict([('input', 'select'), ('name', 'Gamma level:'), ('options', []), "*

 * *             "('labels', [])])), ('value', 0)])])])}",*

 * * "'datasets'": 'OrderedDict()',*

 * * "'hconcat'": "[OrderedDict([('height', 400), ('transform', [OrderedDict([('filter', 'datum.gamma "*

 * *              "== gamma_sel')])]), ('data', OrderedDict([('name', […]*

```diff
@@ -1,358 +1,284 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
-        "view": {
-            "continuousHeight": 300,
-            "continuousWidth": 400
-        }
-    },
-    "data": {
-        "values": null
+        "params": [
+            {
+                "bind": {
+                    "input": "select",
+                    "labels": [],
+                    "name": "Gamma level:",
+                    "options": []
+                },
+                "name": "gamma_sel",
+                "value": 0
+            }
+        ]
     },
-    "height": 450,
-    "layer": [
+    "datasets": {},
+    "hconcat": [
         {
+            "data": {
+                "name": "data"
+            },
+            "height": 400,
             "layer": [
                 {
                     "encoding": {
                         "color": {
-                            "value": "black"
-                        },
-                        "size": {
-                            "value": 0.5
-                        },
-                        "y": {
-                            "field": "zero",
-                            "type": "quantitative"
-                        }
-                    },
-                    "mark": "rule"
-                },
-                {
-                    "encoding": {
-                        "color": {
-                            "condition": {
-                                "test": "(datum.log2_bayes_factor < 0)",
-                                "value": "red"
-                            },
-                            "value": "green"
-                        },
-                        "opacity": {
-                            "condition": {
-                                "test": "datum.column_name == 'Prior lambda' || datum.column_name == 'Final score'",
-                                "value": 1
+                            "field": "log2_bf_tf",
+                            "scale": {
+                                "domain": [
+                                    -2.5,
+                                    2.5
+                                ],
+                                "scheme": "redyellowgreen"
                             },
-                            "value": 0.5
+                            "title": "TF adjustment weight",
+                            "type": "quantitative"
                         },
                         "tooltip": [
                             {
-                                "field": "column_name",
-                                "title": "Comparison column",
+                                "field": "value",
+                                "title": "Value",
                                 "type": "nominal"
                             },
                             {
-                                "field": "value_l",
-                                "title": "Value (L)",
-                                "type": "nominal"
-                            },
-                            {
-                                "field": "value_r",
-                                "title": "Value (R)",
-                                "type": "nominal"
-                            },
-                            {
-                                "field": "label",
-                                "title": "Level label",
-                                "type": "nominal"
-                            },
-                            {
-                                "field": "sql_expr",
-                                "title": "SQL for level",
-                                "type": "nominal"
-                            },
-                            {
-                                "field": "gamma_index",
-                                "title": "Comparison vector value",
-                                "type": "nominal"
-                            },
-                            {
-                                "field": "bayes_factor",
-                                "format": ".3r",
-                                "title": "Bayes factor",
+                                "field": "log2_bf",
+                                "format": "+.3",
+                                "title": "Match weight",
                                 "type": "quantitative"
                             },
                             {
-                                "field": "log2_bayes_factor",
-                                "format": ".3r",
-                                "title": "log2(Bayes factor)",
+                                "field": "log2_bf_tf",
+                                "format": "+.3",
+                                "title": "TF adjusted match weight",
                                 "type": "quantitative"
                             },
                             {
-                                "field": "prob",
-                                "format": ".3r",
-                                "title": "Adjusted match score",
+                                "field": "log2_bf_final",
+                                "format": "+.3",
+                                "title": "Final match weight",
                                 "type": "quantitative"
                             }
                         ],
                         "x": {
                             "axis": {
-                                "grid": true,
-                                "labelAlign": "center",
-                                "labelAngle": -20,
-                                "labelExpr": "datum.value == 'Prior lambda' || datum.value == 'Final score' ? '' : datum.value",
-                                "labelPadding": 10,
-                                "tickBand": "extent",
-                                "title": "Column"
+                                "labelAngle": -60,
+                                "labelFontSize": 16,
+                                "titleFontSize": 20
+                            },
+                            "field": "value",
+                            "sort": {
+                                "field": "log2_bf_final",
+                                "order": "ascending"
                             },
-                            "field": "column_name",
-                            "sort": null,
+                            "title": "TF column value",
                             "type": "nominal"
                         },
                         "y": {
                             "axis": {
-                                "grid": false,
-                                "orient": "left",
-                                "title": "log2(Bayes factor)"
+                                "format": "+",
+                                "labelFontSize": 16,
+                                "titleFontSize": 18,
+                                "values": [
+                                    -5,
+                                    -4,
+                                    -3,
+                                    -2,
+                                    -1,
+                                    0,
+                                    1,
+                                    2,
+                                    3,
+                                    4,
+                                    5,
+                                    6,
+                                    7,
+                                    8,
+                                    9,
+                                    10,
+                                    11,
+                                    12,
+                                    13,
+                                    14,
+                                    15,
+                                    16,
+                                    17,
+                                    18,
+                                    19,
+                                    20
+                                ]
                             },
-                            "field": "previous_sum",
+                            "field": "log2_bf_final",
+                            "title": "Match weight",
                             "type": "quantitative"
-                        },
-                        "y2": {
-                            "field": "sum"
                         }
                     },
                     "mark": {
-                        "type": "bar",
-                        "width": 60
+                        "filled": true,
+                        "size": 100,
+                        "stroke": "black",
+                        "strokeWidth": 1,
+                        "type": "point"
                     }
                 },
                 {
                     "encoding": {
-                        "color": {
-                            "value": "white"
-                        },
-                        "text": {
-                            "condition": {
-                                "field": "log2_bayes_factor",
-                                "format": ".2f",
-                                "test": "abs(datum.log2_bayes_factor) > 1",
-                                "type": "nominal"
-                            },
-                            "value": ""
-                        },
-                        "x": {
-                            "axis": {
-                                "labelAngle": 0,
-                                "title": "Column"
-                            },
-                            "field": "column_name",
-                            "sort": null,
-                            "type": "nominal"
-                        },
                         "y": {
-                            "axis": {
-                                "orient": "left"
-                            },
-                            "field": "center",
+                            "field": "log2_bf",
                             "type": "quantitative"
                         }
                     },
-                    "mark": {
-                        "fontWeight": "bold",
-                        "type": "text"
-                    }
+                    "mark": "rule",
+                    "transform": [
+                        {
+                            "filter": "datum.gamma == gamma_sel"
+                        }
+                    ]
                 },
                 {
                     "encoding": {
                         "color": {
-                            "value": "black"
-                        },
-                        "text": {
-                            "condition": {
-                                "field": "top_label",
-                                "test": "abs(datum.log2_bayes_factor) > 1",
-                                "type": "nominal"
+                            "field": "log2_bf_tf",
+                            "legend": null,
+                            "scale": {
+                                "domain": [
+                                    -2.5,
+                                    2.5
+                                ],
+                                "scheme": "redyellowgreen"
                             },
-                            "value": ""
+                            "title": "TF adjustment weight",
+                            "type": "quantitative"
                         },
                         "x": {
-                            "axis": {
-                                "labelAngle": 0,
-                                "title": "Column"
+                            "field": "value",
+                            "sort": {
+                                "field": "log2_bf_final",
+                                "order": "ascending"
                             },
-                            "field": "column_name",
-                            "sort": null,
+                            "title": "TF column value",
                             "type": "nominal"
                         },
                         "y": {
-                            "field": "sum_top",
+                            "field": "log2_bf_final",
                             "type": "quantitative"
-                        }
-                    },
-                    "mark": {
-                        "baseline": "bottom",
-                        "dy": -5,
-                        "fontWeight": "bold",
-                        "type": "text"
-                    }
-                },
-                {
-                    "encoding": {
-                        "color": {
-                            "value": "black"
-                        },
-                        "text": {
-                            "condition": {
-                                "field": "bottom_label",
-                                "test": "abs(datum.log2_bayes_factor) > 1",
-                                "type": "nominal"
-                            },
-                            "value": ""
-                        },
-                        "x": {
-                            "axis": {
-                                "labelAngle": 0,
-                                "title": "Column"
-                            },
-                            "field": "column_name",
-                            "sort": null,
-                            "type": "nominal"
                         },
-                        "y": {
-                            "field": "sum_bottom",
+                        "y2": {
                             "type": "quantitative"
                         }
                     },
                     "mark": {
-                        "baseline": "top",
-                        "dy": 5,
-                        "fontWeight": "bold",
-                        "type": "text"
-                    }
+                        "opacity": 0.5,
+                        "strokeWidth": 2,
+                        "type": "rule"
+                    },
+                    "transform": [
+                        {
+                            "filter": "datum.gamma == gamma_sel"
+                        }
+                    ]
                 }
-            ]
+            ],
+            "transform": [
+                {
+                    "filter": "datum.gamma == gamma_sel"
+                }
+            ],
+            "width": {
+                "step": 20
+            }
         },
         {
+            "data": {
+                "name": "hist"
+            },
             "encoding": {
+                "color": {
+                    "field": "log2_bf_tf",
+                    "legend": null,
+                    "scale": {
+                        "domain": [
+                            -2.5,
+                            2.5
+                        ],
+                        "scheme": "redyellowgreen"
+                    },
+                    "title": "TF adjustment weight",
+                    "type": "quantitative"
+                },
+                "tooltip": [
+                    {
+                        "field": "log2_bf_desc",
+                        "title": "Match weight"
+                    },
+                    {
+                        "field": "count",
+                        "title": "Number of values"
+                    }
+                ],
                 "x": {
                     "axis": {
-                        "labelAngle": 0,
-                        "title": "Column"
+                        "domain": false,
+                        "gridOpacity": 0.5,
+                        "labelAlign": "center",
+                        "labelFontSize": 12,
+                        "labelOpacity": 0.5,
+                        "labelOverlap": true,
+                        "ticks": false,
+                        "title": "Count of values",
+                        "titleFontSize": 12,
+                        "titleOpacity": 0.5
                     },
-                    "field": "column_name",
-                    "sort": null,
-                    "type": "nominal"
-                },
-                "x2": {
-                    "field": "lead"
+                    "field": "count",
+                    "type": "quantitative"
                 },
                 "y": {
-                    "axis": {
-                        "labelExpr": "format(1 / (1 + pow(2, -1*datum.value)), '.2r')",
-                        "orient": "right",
-                        "title": "Probability"
-                    },
-                    "field": "sum",
-                    "scale": {
-                        "zero": false
+                    "axis": null,
+                    "bin": {
+                        "step": 0.5
                     },
+                    "field": "log2_bf_final",
                     "type": "quantitative"
                 }
             },
             "mark": {
-                "color": "black",
-                "strokeWidth": 2,
-                "type": "rule",
-                "x2Offset": 30,
-                "xOffset": -30
-            }
+                "fillOpacity": 0.8,
+                "filled": true,
+                "stroke": "black",
+                "strokeWidth": 1,
+                "type": "bar"
+            },
+            "transform": [
+                {
+                    "filter": {
+                        "or": [
+                            "datum.gamma == gamma_sel",
+                            {
+                                "field": "gamma",
+                                "valid": false
+                            }
+                        ]
+                    }
+                }
+            ],
+            "view": {
+                "stroke": "transparent"
+            },
+            "width": 100
         }
     ],
     "resolve": {
-        "axis": {
-            "y": "independent"
+        "scale": {
+            "color": "shared",
+            "y": "shared"
         }
     },
+    "spacing": 10,
     "title": {
-        "subtitle": "How each comparison column contributes to the final match score",
-        "text": "Bayes factor intuition chart"
-    },
-    "transform": [
-        {
-            "filter": "(datum.bayes_factor !== 1.0)"
-        },
-        {
-            "frame": [
-                null,
-                0
-            ],
-            "window": [
-                {
-                    "as": "sum",
-                    "field": "log2_bayes_factor",
-                    "op": "sum"
-                },
-                {
-                    "as": "lead",
-                    "field": "column_name",
-                    "op": "lead"
-                }
-            ]
-        },
-        {
-            "as": "sum",
-            "calculate": "datum.column_name === \"Final score\" ? datum.sum - datum.log2_bayes_factor : datum.sum"
-        },
-        {
-            "as": "lead",
-            "calculate": "datum.lead === null ? datum.column_name : datum.lead"
-        },
-        {
-            "as": "previous_sum",
-            "calculate": "datum.column_name === \"Final score\" || datum.column_name === \"Prior lambda\" ? 0 : datum.sum - datum.log2_bayes_factor"
-        },
-        {
-            "as": "top_label",
-            "calculate": "datum.sum > datum.previous_sum ? datum.column_name : \"\""
-        },
-        {
-            "as": "bottom_label",
-            "calculate": "datum.sum < datum.previous_sum ? datum.column_name : \"\""
-        },
-        {
-            "as": "sum_top",
-            "calculate": "datum.sum > datum.previous_sum ? datum.sum : datum.previous_sum"
-        },
-        {
-            "as": "sum_bottom",
-            "calculate": "datum.sum < datum.previous_sum ? datum.sum : datum.previous_sum"
-        },
-        {
-            "as": "center",
-            "calculate": "(datum.sum + datum.previous_sum) / 2"
-        },
-        {
-            "as": "text_log2_bayes_factor",
-            "calculate": "(datum.log2_bayes_factor > 0 ? \"+\" : \"\") + datum.log2_bayes_factor"
-        },
-        {
-            "as": "dy",
-            "calculate": "datum.sum < datum.previous_sum ? 4 : -4"
-        },
-        {
-            "as": "baseline",
-            "calculate": "datum.sum < datum.previous_sum ? \"top\" : \"bottom\""
-        },
-        {
-            "as": "prob",
-            "calculate": "1. / (1 + pow(2, -1.*datum.sum))"
-        },
-        {
-            "as": "zero",
-            "calculate": "0*datum.sum"
-        }
-    ],
-    "width": {
-        "step": 75
+        "anchor": "middle",
+        "fontSize": 16,
+        "subtitle": "For selected values, incl. the lowest and highest frequency",
+        "text": "Term frequency adjusted match weights"
     }
 }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json` & `splink-3.9.2/splink/files/chart_defs/match_weight_histogram.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4147916666666667%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{'title': {replace: OrderedDict([('fontSize', 14)])}, delete: ['view', 'mark', "*

 * *             "'header']}",*

 * * "'data'": "{'values': []}",*

 * * "'encoding'": "{'tooltip': {0: {'field': 'count_rows', 'title': 'Count in bin', delete: "*

 * *               "['format']}, delete: [4, 3, 2, 1, 0]}, 'x': {'field': 'splink_score_bin_low', "*

 * *               "'axis': {'title': 'Match weight'}, 'bin': 'binned'}, 'y': {'type': 'quantitative', "*

 * *   […]*

```diff
@@ -1,90 +1,55 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
-        "header": {
-            "title": null
-        },
-        "mark": {
-            "tooltip": null
-        },
         "title": {
-            "anchor": "middle"
-        },
-        "view": {
-            "height": 300,
-            "width": 400
+            "fontSize": 14
         }
     },
     "data": {
-        "values": null
+        "values": []
     },
     "encoding": {
-        "row": {
-            "field": "column_name",
-            "header": {
-                "labelAlign": "left",
-                "labelAnchor": "middle",
-                "labelAngle": 0
-            },
-            "sort": {
-                "field": "gamma_index"
-            },
-            "type": "nominal"
-        },
         "tooltip": [
             {
-                "field": "column_name",
-                "type": "nominal"
-            },
-            {
-                "field": "level_name",
-                "type": "ordinal"
-            },
-            {
-                "field": "level_proportion",
-                "format": ".2%",
-                "title": "Percentage of record comparisons in this level",
-                "type": "nominal"
-            },
-            {
-                "field": "bayes_factor",
-                "format": ".4f",
-                "type": "quantitative"
-            },
-            {
-                "field": "sql_expr",
-                "type": "nominal"
-            },
-            {
-                "field": "log2_bayes_factor",
-                "format": ".4f",
+                "field": "count_rows",
+                "title": "Count in bin",
                 "type": "quantitative"
             }
         ],
         "x": {
             "axis": {
-                "title": "proportion of comparisons"
+                "title": "Match weight"
             },
-            "field": "level_proportion",
+            "bin": "binned",
+            "field": "splink_score_bin_low",
             "type": "quantitative"
         },
+        "x2": {
+            "field": "splink_score_bin_high"
+        },
         "y": {
             "axis": {
-                "title": null
+                "title": "Count of record comparisons in bin"
             },
-            "field": "level_name",
-            "type": "nominal"
+            "field": "count_rows",
+            "type": "quantitative"
         }
     },
-    "height": 50,
     "mark": "bar",
-    "resolve": {
-        "scale": {
-            "y": "independent"
+    "params": [
+        {
+            "bind": "scales",
+            "name": "mouse_zoom",
+            "select": {
+                "encodings": [
+                    "y"
+                ],
+                "type": "interval"
+            }
         }
-    },
+    ],
     "title": {
-        "text": "Proportion of (non-null) comparisons in each level"
-    },
-    "width": 150
+        "subtitle": "Use mousewheel to zoom",
+        "text": "Histogram of match weights"
+    }
 }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/del/score_histogram.json` & `splink-3.9.2/splink/files/chart_defs/phonetic_match_chart.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.14772727272727273%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{'view': {replace: OrderedDict([('discreteWidth', 300), ('discreteHeight', 600)])}, "*

 * *             "delete: ['title']}",*

 * * "'data'": "{replace: OrderedDict([('name', 'data-phonetic')])}",*

 * * "'datasets'": "OrderedDict([('data-phonetic', [])])",*

 * * "'layer'": "[OrderedDict([('mark', OrderedDict([('type', 'rect')])), ('encoding', "*

 * *            "OrderedDict([('color', OrderedDict([('field', 'match'), ('scale', "*

 * *            "Ordere […]*

```diff
@@ -1,58 +1,71 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
-        "title": {
-            "fontSize": 14
-        },
         "view": {
-            "continuousHeight": 300,
-            "continuousWidth": 400
+            "discreteHeight": 600,
+            "discreteWidth": 300
         }
     },
     "data": {
-        "values": null
+        "name": "data-phonetic"
+    },
+    "datasets": {
+        "data-phonetic": []
     },
-    "encoding": {
-        "tooltip": [
-            {
-                "field": "count_rows",
-                "title": "count",
-                "type": "quantitative"
-            }
-        ],
-        "x": {
-            "axis": {
-                "title": "splink score"
+    "layer": [
+        {
+            "encoding": {
+                "color": {
+                    "field": "match",
+                    "scale": {
+                        "range": [
+                            "red",
+                            "green"
+                        ]
+                    },
+                    "type": "ordinal"
+                },
+                "x": {
+                    "field": "phonetic",
+                    "type": "ordinal"
+                },
+                "y": {
+                    "field": "strings_to_compare",
+                    "type": "ordinal"
+                }
             },
-            "bin": "binned",
-            "field": "splink_score_bin_low",
-            "type": "quantitative"
-        },
-        "x2": {
-            "field": "splink_score_bin_high"
+            "mark": {
+                "type": "rect"
+            },
+            "title": "Heatmap of Phonetic Matches"
         },
-        "y": {
-            "axis": {
-                "title": "probability density"
+        {
+            "encoding": {
+                "color": {
+                    "condition": {
+                        "test": "(datum.quantity > 3)",
+                        "value": "white"
+                    },
+                    "value": "black"
+                },
+                "text": {
+                    "field": "transform",
+                    "type": "ordinal"
+                },
+                "x": {
+                    "field": "phonetic",
+                    "type": "ordinal"
+                },
+                "y": {
+                    "field": "strings_to_compare",
+                    "type": "ordinal"
+                }
             },
-            "field": "normalised",
-            "type": "quantitative"
-        }
-    },
-    "height": 200,
-    "mark": "bar",
-    "selection": {
-        "selector076": {
-            "bind": "scales",
-            "encodings": [
-                "y"
-            ],
-            "type": "interval"
+            "mark": {
+                "baseline": "middle",
+                "type": "text"
+            },
+            "title": "Heatmap of Phonetic Matches"
         }
-    },
-    "title": {
-        "subtitle": "Use mousewheel to zoom",
-        "text": "Histogram of splink scores"
-    },
-    "width": 700
+    ]
 }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.9.2/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8988095238095238%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{'view': {replace: OrderedDict([('discreteWidth', 400), ('discreteHeight', 300)])}}",*

 * * "'params'": "{0: {delete: ['description']}}"}*

```diff
@@ -1,20 +1,20 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "header": {
             "title": null
         },
         "title": {
             "anchor": "middle",
             "offset": 10
         },
         "view": {
-            "height": 300,
-            "width": 400
+            "discreteHeight": 300,
+            "discreteWidth": 400
         }
     },
     "data": {
         "values": null
     },
     "hconcat": [
         {
@@ -226,15 +226,14 @@
         {
             "bind": {
                 "input": "range",
                 "max": 10,
                 "min": 0,
                 "step": 1
             },
-            "description": "Filter by the interation number",
             "name": "iteration_number",
             "value": 0
         }
     ],
     "title": {
         "subtitle": "(m and u probabilities)",
         "text": "Proportion of record comparisons in each comparison level by match status"
```

### Comparing `splink-3.9.1/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.9.2/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4869791666666667%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{replace: OrderedDict([('mark', OrderedDict([('tooltip', None)]))])}",*

 * * "'encoding'": "{'tooltip': {2: {'field': 'iteration', 'title': 'EM iteration', 'type': "*

 * *               "'ordinal'}, insert: [(0, OrderedDict([('type', 'quantitative'), ('field', "*

 * *               "'probability_two_random_records_match'), ('title', '% of record comparisons "*

 * *               "estimated to be matches within block'), ('format', '.4g')])), (1 […]*

```diff
@@ -1,54 +1,48 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
-        "title": {
-            "fontSize": 14
+        "mark": {
+            "tooltip": null
         }
     },
     "data": {
         "values": []
     },
     "encoding": {
         "tooltip": [
             {
-                "field": "count_rows",
-                "title": "Count in bin",
+                "field": "probability_two_random_records_match",
+                "format": ".4g",
+                "title": "% of record comparisons estimated to be matches within block",
                 "type": "quantitative"
+            },
+            {
+                "field": "probability_two_random_records_match_reciprocal",
+                "format": ",.2f",
+                "title": "Reciprocal of % matches in block",
+                "type": "quantitative"
+            },
+            {
+                "field": "iteration",
+                "title": "EM iteration",
+                "type": "ordinal"
             }
         ],
         "x": {
-            "axis": {
-                "title": "Match weight"
-            },
-            "bin": "binned",
-            "field": "splink_score_bin_low",
-            "type": "quantitative"
-        },
-        "x2": {
-            "field": "splink_score_bin_high"
+            "field": "iteration",
+            "type": "ordinal"
         },
         "y": {
             "axis": {
-                "title": "Count of record comparisons in bin"
+                "format": ".2f",
+                "title": "Estimated proportion of matches within block"
             },
-            "field": "count_rows",
+            "field": "probability_two_random_records_match",
             "type": "quantitative"
         }
     },
-    "height": 200,
     "mark": "bar",
-    "selection": {
-        "selector076": {
-            "bind": "scales",
-            "encodings": [
-                "y"
-            ],
-            "type": "interval"
-        }
-    },
     "title": {
-        "subtitle": "Use mousewheel to zoom",
-        "text": "Histogram of match weights"
-    },
-    "width": 200
+        "text": "Estimated probability two random records match matches by iteration"
+    }
 }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.9.2/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7953042328042328%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{'view': {replace: OrderedDict([('discreteWidth', 400), ('discreteHeight', 60)])}}",*

 * * "'params'": "{0: {delete: ['description']}}",*

 * * "'vconcat'": "{0: {'params': [OrderedDict([('name', 'mouse_zoom'), ('select', "*

 * *              "OrderedDict([('type', 'interval'), ('encodings', ['x'])])), ('bind', 'scales')])], "*

 * *              "delete: ['selection']}, 1: {'params': [OrderedDict([('name', 'mouse_zoom'), "*

 * *              "('sele […]*

```diff
@@ -1,57 +1,47 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v5.2.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "header": {
             "title": null
         },
         "mark": {
             "tooltip": null
         },
         "title": {
             "anchor": "middle"
         },
         "view": {
-            "height": 60,
-            "width": 400
+            "discreteHeight": 60,
+            "discreteWidth": 400
         }
     },
     "data": {
         "values": []
     },
     "params": [
         {
             "bind": {
                 "input": "range",
                 "max": 10,
                 "min": 0,
                 "step": 1
             },
-            "description": "Filter by the iteration number",
             "name": "iteration_number",
             "value": 0
         }
     ],
     "resolve": {
         "axis": {
             "y": "independent"
         },
         "scale": {
             "y": "independent"
         }
     },
-    "selection": {
-        "zoom_selector": {
-            "bind": "scales",
-            "encodings": [
-                "x"
-            ],
-            "type": "interval"
-        }
-    },
     "title": {
         "subtitle": "Use mousewheel to zoom",
         "text": "Model parameters (components of final match weight)"
     },
     "transform": [
         {
             "filter": "(datum.iteration == iteration_number)"
@@ -134,23 +124,26 @@
             },
             "height": 20,
             "mark": {
                 "clip": true,
                 "height": 15,
                 "type": "bar"
             },
-            "selection": {
-                "zoom_selector": {
+            "params": [
+                {
                     "bind": "scales",
-                    "encodings": [
-                        "x"
-                    ],
-                    "type": "interval"
+                    "name": "mouse_zoom",
+                    "select": {
+                        "encodings": [
+                            "x"
+                        ],
+                        "type": "interval"
+                    }
                 }
-            },
+            ],
             "transform": [
                 {
                     "filter": "(datum.comparison_name == 'probability_two_random_records_match')"
                 }
             ]
         },
         {
@@ -258,31 +251,34 @@
             "height": {
                 "step": 12
             },
             "mark": {
                 "clip": true,
                 "type": "bar"
             },
+            "params": [
+                {
+                    "bind": "scales",
+                    "name": "mouse_zoom",
+                    "select": {
+                        "encodings": [
+                            "x"
+                        ],
+                        "type": "interval"
+                    }
+                }
+            ],
             "resolve": {
                 "axis": {
                     "y": "independent"
                 },
                 "scale": {
                     "y": "independent"
                 }
             },
-            "selection": {
-                "zoom_selector": {
-                    "bind": "scales",
-                    "encodings": [
-                        "x"
-                    ],
-                    "type": "interval"
-                }
-            },
             "transform": [
                 {
                     "filter": "(datum.comparison_name != 'probability_two_random_records_match')"
                 }
             ]
         }
     ]
```

### Comparing `splink-3.9.1/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.9.2/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9374593098958334%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'layer'": "{0: {'layer': {2: {'encoding': {'x': {'axis': {'labelAngle': -20}}}}, 3: {'encoding': "*

 * *            "{'x': {'axis': {'labelAngle': -20}}}}, 4: {'encoding': {'x': {'axis': {'labelAngle': "*

 * *            "-20}}}}, 5: {'encoding': {'x': {'axis': {'labelAngle': -20}}}}}}, 1: {'encoding': "*

 * *            "{'x': {'axis': {'labelAngle': -20}}}}}",*

 * * "'params'": "{0: {delete: ['description']}}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v5.2.0.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "view": {
             "continuousHeight": 300,
             "continuousWidth": 400
         }
     },
     "data": {
@@ -146,15 +146,15 @@
                                 "test": "abs(datum.log2_bayes_factor) > 1",
                                 "type": "nominal"
                             },
                             "value": ""
                         },
                         "x": {
                             "axis": {
-                                "labelAngle": 0,
+                                "labelAngle": -20,
                                 "title": "Column"
                             },
                             "field": "column_name",
                             "sort": {
                                 "field": "bar_sort_order",
                                 "order": "ascending"
                             },
@@ -180,15 +180,15 @@
                         },
                         "text": {
                             "field": "column_name",
                             "type": "nominal"
                         },
                         "x": {
                             "axis": {
-                                "labelAngle": 0,
+                                "labelAngle": -20,
                                 "title": "Column"
                             },
                             "field": "column_name",
                             "sort": {
                                 "field": "bar_sort_order",
                                 "order": "ascending"
                             },
@@ -213,15 +213,15 @@
                         },
                         "text": {
                             "field": "value_l",
                             "type": "nominal"
                         },
                         "x": {
                             "axis": {
-                                "labelAngle": 0,
+                                "labelAngle": -20,
                                 "title": "Column"
                             },
                             "field": "column_name",
                             "sort": {
                                 "field": "bar_sort_order",
                                 "order": "ascending"
                             },
@@ -246,15 +246,15 @@
                         },
                         "text": {
                             "field": "value_r",
                             "type": "nominal"
                         },
                         "x": {
                             "axis": {
-                                "labelAngle": 0,
+                                "labelAngle": -20,
                                 "title": "Column"
                             },
                             "field": "column_name",
                             "sort": {
                                 "field": "bar_sort_order",
                                 "order": "ascending"
                             },
@@ -274,15 +274,15 @@
                 }
             ]
         },
         {
             "encoding": {
                 "x": {
                     "axis": {
-                        "labelAngle": 0,
+                        "labelAngle": -20,
                         "title": "Column"
                     },
                     "field": "column_name",
                     "sort": {
                         "field": "bar_sort_order",
                         "order": "ascending"
                     },
@@ -317,15 +317,14 @@
         {
             "bind": {
                 "input": "range",
                 "max": 10,
                 "min": 0,
                 "step": 1
             },
-            "description": "Filter by the interation number",
             "name": "record_number",
             "value": 0
         }
     ],
     "resolve": {
         "axis": {
             "y": "independent"
```

### Comparing `splink-3.9.1/splink/files/chart_defs/missingness.json` & `splink-3.9.2/splink/files/chart_defs/missingness.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8916666666666666%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'config'": "{'view': {delete: ['width']}}"}*

```diff
@@ -1,17 +1,16 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "axis": {
             "labelFontSize": 11
         },
         "view": {
             "continuousHeight": 300,
-            "continuousWidth": 400,
-            "width": 400
+            "continuousWidth": 400
         }
     },
     "data": {
         "name": "data-0e7bce5a1d2f132e282789d6ef7780fe",
         "values": ""
     },
     "layer": [
```

### Comparing `splink-3.9.1/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.9.2/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'params'": "[OrderedDict([('name', 'mouse_zoom'), ('select', OrderedDict([('type', 'interval'), "*

 * *             "('encodings', ['x'])])), ('bind', 'scales')])]",*

 * * 'delete': "['selection']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v5.2.0.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "title": {
             "anchor": "middle",
             "fontSize": 18,
             "subtitleFontSize": 14
         },
         "view": {
@@ -116,29 +116,31 @@
     },
     "mark": {
         "filled": false,
         "opacity": 0.7,
         "size": 100,
         "type": "point"
     },
+    "params": [
+        {
+            "bind": "scales",
+            "name": "mouse_zoom",
+            "select": {
+                "encodings": [
+                    "x"
+                ],
+                "type": "interval"
+            }
+        }
+    ],
     "resolve": {
         "scale": {
             "y": "independent"
         }
     },
-    "selection": {
-        "selection_zoom": {
-            "bind": "scales",
-            "encodings": [
-                "x",
-                "column"
-            ],
-            "type": "interval"
-        }
-    },
     "title": {
         "subtitle": "Use mousewheel to zoom",
         "text": "Comparison of parameter estimates across training sessions"
     },
     "transform": [
         {
             "as": "col_header",
```

### Comparing `splink-3.9.1/splink/files/chart_defs/precision_recall.json` & `splink-3.9.2/splink/files/chart_defs/precision_recall.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'params'": "[OrderedDict([('name', 'mouse_zoom'), ('select', OrderedDict([('type', 'interval'), "*

 * *             "('encodings', ['x', 'y'])])), ('bind', 'scales')])]"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "data": {
         "values": []
     },
     "encoding": {
         "color": {
             "field": "curve_label",
             "type": "nominal"
@@ -90,9 +90,22 @@
         }
     },
     "mark": {
         "clip": true,
         "point": true,
         "type": "line"
     },
+    "params": [
+        {
+            "bind": "scales",
+            "name": "mouse_zoom",
+            "select": {
+                "encodings": [
+                    "x",
+                    "y"
+                ],
+                "type": "interval"
+            }
+        }
+    ],
     "title": "Precision-recall curve"
 }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/profile_data.json` & `splink-3.9.2/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/chart_defs/roc.json` & `splink-3.9.2/splink/files/chart_defs/roc.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7222222222222222%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'params'": "[OrderedDict([('name', 'mouse_zoom'), ('select', OrderedDict([('type', 'interval'), "*

 * *             "('encodings', ['x'])])), ('bind', 'scales')])]",*

 * * 'delete': "['selection']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "data": {
         "values": []
     },
     "encoding": {
         "color": {
             "field": "curve_label",
             "type": "nominal"
@@ -91,19 +91,22 @@
     },
     "height": 600,
     "mark": {
         "clip": true,
         "point": true,
         "type": "line"
     },
-    "selection": {
-        "selector076": {
+    "params": [
+        {
             "bind": "scales",
-            "encodings": [
-                "x"
-            ],
-            "type": "interval"
+            "name": "mouse_zoom",
+            "select": {
+                "encodings": [
+                    "x"
+                ],
+                "type": "interval"
+            }
         }
-    },
+    ],
     "title": "Receiver operating characteristic curve",
     "width": 600
 }
```

### Comparing `splink-3.9.1/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.9.2/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7879720052083333%*

 * *Differences: {"'$schema'": "'https://vega.github.io/schema/vega-lite/v5.9.3.json'",*

 * * "'layer'": "{0: {'mark': {replace: OrderedDict([('type', 'line')])}}, 1: {'mark': {replace: "*

 * *            "OrderedDict([('type', 'point')])}, 'encoding': {'opacity': {'condition': {'param': "*

 * *            "'x_match_weight_y_cum_prop_coords_of_mouse', 'empty': False, delete: ['selection']}}, "*

 * *            "'tooltip': [OrderedDict([('type', 'quantitative'), ('field', 'match_weight'), "*

 * *            "('format', '+.5'), ('title', 'Match weigh […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "config": {
         "view": {
             "continuousHeight": 300,
             "continuousWidth": 400
         }
     },
     "data": {
@@ -26,19 +26,26 @@
                         "format": "%",
                         "title": "Percentage of unlinkable records"
                     },
                     "field": "cum_prop",
                     "type": "quantitative"
                 }
             },
-            "mark": "line"
+            "mark": {
+                "type": "line"
+            }
         },
         {
             "encoding": {
                 "opacity": {
+                    "condition": {
+                        "empty": false,
+                        "param": "x_match_weight_y_cum_prop_coords_of_mouse",
+                        "value": 1
+                    },
                     "value": 0
                 },
                 "tooltip": [
                     {
                         "field": "match_weight",
                         "format": "+.5",
                         "title": "Match weight",
@@ -54,46 +61,14 @@
                         "field": "cum_prop",
                         "format": ".3%",
                         "title": "Proportion of unlinkable records",
                         "type": "quantitative"
                     }
                 ],
                 "x": {
-                    "field": "match_weight",
-                    "type": "quantitative"
-                },
-                "y": {
-                    "field": "cum_prop",
-                    "type": "quantitative"
-                }
-            },
-            "mark": "point",
-            "selection": {
-                "selector112": {
-                    "empty": "none",
-                    "fields": [
-                        "match_weight",
-                        "cum_prop"
-                    ],
-                    "nearest": true,
-                    "on": "mouseover",
-                    "type": "single"
-                }
-            }
-        },
-        {
-            "encoding": {
-                "opacity": {
-                    "condition": {
-                        "selection": "selector112",
-                        "value": 1
-                    },
-                    "value": 0
-                },
-                "x": {
                     "axis": {
                         "title": "Threshold match weight"
                     },
                     "field": "match_weight",
                     "type": "quantitative"
                 },
                 "y": {
@@ -101,15 +76,18 @@
                         "format": "%",
                         "title": "Percentage of unlinkable records"
                     },
                     "field": "cum_prop",
                     "type": "quantitative"
                 }
             },
-            "mark": "point"
+            "mark": {
+                "type": "point"
+            },
+            "name": "mouse_coords"
         },
         {
             "encoding": {
                 "x": {
                     "field": "match_weight",
                     "type": "quantitative"
                 }
@@ -117,15 +95,16 @@
             "mark": {
                 "color": "gray",
                 "type": "rule"
             },
             "transform": [
                 {
                     "filter": {
-                        "selection": "selector112"
+                        "empty": false,
+                        "param": "x_match_weight_y_cum_prop_coords_of_mouse"
                     }
                 }
             ]
         },
         {
             "encoding": {
                 "y": {
@@ -136,19 +115,37 @@
             "mark": {
                 "color": "gray",
                 "type": "rule"
             },
             "transform": [
                 {
                     "filter": {
-                        "selection": "selector112"
+                        "empty": false,
+                        "param": "x_match_weight_y_cum_prop_coords_of_mouse"
                     }
                 }
             ]
         }
     ],
+    "params": [
+        {
+            "name": "x_match_weight_y_cum_prop_coords_of_mouse",
+            "select": {
+                "fields": [
+                    "match_weight",
+                    "cum_prop"
+                ],
+                "nearest": true,
+                "on": "mouseover",
+                "type": "point"
+            },
+            "views": [
+                "mouse_coords"
+            ]
+        }
+    ],
     "title": {
         "subtitle": "Records with insufficient information to exceed a given match threshold",
         "text": "Unlinkable records"
     },
     "width": 400
 }
```

### Comparing `splink-3.9.1/splink/files/external_js/vega-embed@6.20.2` & `splink-3.9.2/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/external_js/vega-lite@5.2.0` & `splink-3.9.2/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/external_js/vega@5.21.0` & `splink-3.9.2/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/settings_jsonschema.json` & `splink-3.9.2/splink/files/settings_jsonschema.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998958333333333%*

 * *Differences: {"'properties'": "{'sql_dialect': {'examples': {insert: [(4, 'postgres')]}, 'enum': {insert: [(4, "*

 * *                 "'postgres')]}}}"}*

```diff
@@ -268,21 +268,23 @@
         },
         "sql_dialect": {
             "default": null,
             "enum": [
                 "spark",
                 "duckdb",
                 "presto",
-                "sqlite"
+                "sqlite",
+                "postgres"
             ],
             "examples": [
                 "spark",
                 "duckdb",
                 "presto",
-                "sqlite"
+                "sqlite",
+                "postgres"
             ],
             "title": "The SQL dialect in which sql_conditions are written.  Must be a valid sqlglot dialect",
             "type": "string"
         },
         "term_frequency_adjustment_column_prefix": {
             "default": "tf_",
             "examples": [
```

### Comparing `splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-3.9.2/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.9.2/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/splink_cluster_studio/custom.css` & `splink-3.9.2/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/splink_comparison_viewer/custom.css` & `splink-3.9.2/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/splink_comparison_viewer/template.j2` & `splink-3.9.2/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.9.2/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/input_column.py` & `splink-3.9.2/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/linker.py` & `splink-3.9.2/splink/linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             input_table_aliases (Union[str, list], optional): Labels assigned to
                 input tables in Splink outputs.  If the names of the tables in the
                 input database are long or unspecific, this argument can be used
                 to attach more easily readable/interpretable names. Defaults to None.
         """
-
+        self._db_schema = "splink"
         if set_up_basic_logging:
             logging.basicConfig(
                 format="%(message)s",
             )
             splink_logger = logging.getLogger("splink")
             splink_logger.setLevel(logging.INFO)
 
@@ -372,14 +372,19 @@
 
     @property
     def _infinity_expression(self):
         raise NotImplementedError(
             f"infinity sql expression not available for {type(self)}"
         )
 
+    def _random_sample_sql(
+        self, proportion, sample_size, seed=None, table=None, unique_id=None
+    ):
+        raise NotImplementedError("Random sample sql not implemented for this linker")
+
     @property
     def _verify_link_only_job(self):
         cache = self._intermediate_table_cache
         if "__splink__df_concat_with_tf" not in cache:
             return
 
         if self._settings_obj._link_type == "link_only":
@@ -639,15 +644,16 @@
                 ).sql(pretty=True)
                 # if sqlglot produces any errors, just report the raw SQL
             except Exception:
                 pass
 
             raise SplinkException(
                 f"Error executing the following sql for table "
-                f"`{templated_name}` ({physical_name}):\n{final_sql}"
+                f"`{templated_name}`({physical_name}):\n{final_sql}"
+                f"\n\nError was: {e}"
             ) from e
 
     def register_table(self, input, table_name, overwrite=False):
         """
         Register a table to your backend database, to be used in one of the
         splink methods, or simply to allow querying.
 
@@ -1285,15 +1291,15 @@
 
         Deterministic linkage, however, is likely to result in missed links
         (false negatives).
 
         Examples:
             === "DuckDB"
             ```py
-            from splink.duckdb.duckdb_linker import DuckDBLinker
+            from splink.duckdb.linker import DuckDBLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
                     "l.surname = r.surname",
                 ],
@@ -1301,15 +1307,15 @@
             }
             >>>
             linker = DuckDBLinker(df, settings)
             df = linker.deterministic_link()
             ```
             === "Spark"
             ```py
-            from splink.spark.spark_linker import SparkLinker
+            from splink.spark.linker import SparkLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
                     "l.surname = r.surname",
                 ],
@@ -1317,15 +1323,15 @@
             }
             >>>
             linker = SparkLinker(df, settings)
             df = linker.deterministic_link()
             ```
             === "Athena"
             ```py
-            from splink.athena.athena_linker import AthenaLinker
+            from splink.athena.linker import AthenaLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
                     "l.surname = r.surname",
                 ],
@@ -1333,15 +1339,15 @@
             }
             >>>
             linker = AthenaLinker(df, settings)
             df = linker.deterministic_link()
             ```
             === "SQLite"
             ```py
-            from splink.sqlite.sqlite_linker import SQLiteLinker
+            from splink.sqlite.linker import SQLiteLinker
 
             settings = {
                 "link_type": "dedupe_only",
                 "blocking_rules_to_generate_predictions": [
                     "l.first_name = r.first_name",
                     "l.surname = r.surname",
                 ],
@@ -2178,17 +2184,15 @@
                 ```py
                 labels = spark.read.csv("my_labels.csv", header=True)
                 labels.createDataFrame("labels")
                 linker.roc_chart_from_labels_table("labels")
                 ```
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
         labels_tablename = self._get_labels_tablename_from_input(
             labels_splinkdataframe_or_table_name
         )
 
         self._raise_error_if_necessary_accuracy_columns_not_computed()
         df_truth_space = truth_space_table_from_labels_table(
@@ -2244,17 +2248,15 @@
                 ```py
                 labels = spark.read.csv("my_labels.csv", header=True)
                 labels.createDataFrame("labels")
                 linker.precision_recall_chart_from_labels_table("labels")
                 ```
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
         labels_tablename = self._get_labels_tablename_from_input(
             labels_splinkdataframe_or_table_name
         )
         self._raise_error_if_necessary_accuracy_columns_not_computed()
         df_truth_space = truth_space_table_from_labels_table(
             self,
@@ -2356,17 +2358,15 @@
 
         Examples:
             ```py
             linker.roc_chart_from_labels_column("labels")
             ```
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
 
         df_truth_space = truth_space_table_from_labels_column(
             self,
             labels_column_name,
             threshold_actual=threshold_actual,
             match_weight_round_to_nearest=match_weight_round_to_nearest,
@@ -2395,17 +2395,15 @@
                 the number of points plotted on the ROC chart. Defaults to None.
         Examples:
             ```py
             linker.precision_recall_chart_from_labels_column("ground_truth")
             ```
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
 
         df_truth_space = truth_space_table_from_labels_column(
             self,
             labels_column_name,
             threshold_actual=threshold_actual,
             match_weight_round_to_nearest=match_weight_round_to_nearest,
@@ -2454,17 +2452,15 @@
             target_bins (int, optional): Target number of bins in histogram. Defaults to
                 30.
             width (int, optional): Width of output. Defaults to 600.
             height (int, optional): Height of output chart. Defaults to 250.
 
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
 
         """
         df = histogram_data(self, df_predict, target_bins)
         recs = df.as_record_dict()
         return match_weights_histogram(recs, width=width, height=height)
 
     def waterfall_chart(self, records: list[dict], filter_nulls=True):
@@ -2486,17 +2482,15 @@
                 where `df` is a SplinkDataFrame.
             filter_nulls (bool, optional): Whether the visualiation shows null
                 comparisons, which have no effect on final match weight. Defaults to
                 True.
 
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
 
         """
         self._raise_error_if_necessary_waterfall_columns_not_computed()
 
         return waterfall_chart(records, self._settings_obj, filter_nulls)
 
     def unlinkables_chart(
@@ -2527,17 +2521,15 @@
             linker.load_settings("saved_settings.json")
             linker.unlinkables_chart()
             ```
             For more complex code pipelines, you can run an entire pipeline
             that estimates your m and u values, before `unlinkables_chart().
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
 
         # Link our initial df on itself and calculate the % of unlinkable entries
         records = unlinkables_data(self)
         return unlinkables_chart(records, x_col, source_dataset, as_dict)
 
     def comparison_viewer_dashboard(
@@ -2645,14 +2637,17 @@
             save_offline_chart(c.spec, "test_chart.html")
             ```
             View resultant html file in Jupyter (or just load it in your browser)
             ```py
             from IPython.display import IFrame
             IFrame(src="./test_chart.html", width=1000, height=500
             ```
+
+        Returns:
+            altair.Chart: An altair chart
         """
         records = missingness_data(self, input_dataset)
         return missingness_chart(records)
 
     def completeness_chart(self, input_dataset: str = None, cols: list[str] = None):
         """Generate a summary chart of the completeness (proportion of non-nulls) of
         columns in each of the input datasets. By default, completeness is assessed for
@@ -2801,17 +2796,15 @@
             >>>
             linker_settings.cumulative_num_comparisons_from_blocking_rules_chart(
                 blocking_rules
              )
             ```
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
 
         if blocking_rules:
             blocking_rules = ensure_is_list(blocking_rules)
 
         records = cumulative_comparisons_generated_by_blocking_rules(
             self, blocking_rules, output_chart=True
@@ -2869,17 +2862,15 @@
             View resultant html file in Jupyter (or just load it in your browser)
             ```py
             from IPython.display import IFrame
             IFrame(src="./test_chart.html", width=1000, height=500)
             ```
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
         return self._settings_obj.match_weights_chart()
 
     def tf_adjustment_chart(
         self,
         output_column_name: str,
         n_most_freq: int = 10,
@@ -2901,17 +2892,15 @@
                 this or `n_most_freq` set to None, all values will be shown.
                 Default to 10.
             vals_to_include (list, optional): Specific values for which to show term
                 sfrequency adjustments.
                 Defaults to None.
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
 
         # Comparisons with TF adjustments
         tf_comparisons = [
             c._output_column_name
             for c in self._settings_obj.comparisons
             if any([cl._has_tf_adjustments for cl in c.comparison_levels])
@@ -2949,17 +2938,15 @@
             View resultant html file in Jupyter (or just load it in your browser)
             ```py
             from IPython.display import IFrame
             IFrame(src="./test_chart.html", width=1000, height=500)
             ```
 
         Returns:
-            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
-                The vegalite spec is available as a dictionary using the `spec`
-                attribute.
+            altair.Chart: An altair chart
         """
 
         return self._settings_obj.m_u_parameters_chart()
 
     def cluster_studio_dashboard(
         self,
         df_predict: SplinkDataFrame,
```

### Comparing `splink-3.9.1/splink/lower_id_on_lhs.py` & `splink-3.9.2/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/m_from_labels.py` & `splink-3.9.2/splink/m_from_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         linker._enqueue_sql(sql["sql"], sql["output_table_name"])
 
     sql = compute_comparison_vector_values_sql(linker._settings_obj)
 
     linker._enqueue_sql(sql, "__splink__df_comparison_vectors")
 
     sql = """
-    select *, cast(1.0 as double) as match_probability
+    select *, cast(1.0 as float8) as match_probability
     from __splink__df_comparison_vectors
     """
     linker._enqueue_sql(sql, "__splink__df_predict")
 
     sql = compute_new_parameters_sql(linker._settings_obj)
     linker._enqueue_sql(sql, "__splink__m_u_counts")
```

### Comparing `splink-3.9.1/splink/m_training.py` & `splink-3.9.2/splink/m_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     training_linker._enqueue_sql(sql, "__splink__df_blocked")
 
     sql = compute_comparison_vector_values_sql(settings_obj)
 
     training_linker._enqueue_sql(sql, "__splink__df_comparison_vectors")
 
     sql = """
-    select *, cast(1.0 as double) as match_probability
+    select *, cast(1.0 as float8) as match_probability
     from __splink__df_comparison_vectors
     """
     training_linker._enqueue_sql(sql, "__splink__df_predict")
 
     sql = compute_new_parameters_sql(settings_obj)
     training_linker._enqueue_sql(sql, "__splink__m_u_counts")
```

### Comparing `splink-3.9.1/splink/m_u_records_to_parameters.py` & `splink-3.9.2/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/match_key_analysis.py` & `splink-3.9.2/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/match_weights_histogram.py` & `splink-3.9.2/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/misc.py` & `splink-3.9.2/splink/misc.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/missingness.py` & `splink-3.9.2/splink/missingness.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/parse_sql.py` & `splink-3.9.2/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/pipeline.py` & `splink-3.9.2/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/predict.py` & `splink-3.9.2/splink/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     if probability_two_random_records_match == 1.0:
         bayes_factor_expr = sql_infinity_expression
         match_prob_expr = "1.0"
     else:
         bayes_factor = prob_to_bayes_factor(probability_two_random_records_match)
 
         bayes_factor_expr = " * ".join(mult)
-        bayes_factor_expr = f"cast({bayes_factor} as double) * {bayes_factor_expr}"
+        bayes_factor_expr = f"cast({bayes_factor} as float8) * {bayes_factor_expr}"
 
         # if any BF is Infinity then we need to adjust expression,
         # as arithmetic won't go through directly
         any_bf_inf = " OR ".join(
             map(lambda col: f"{col} = {sql_infinity_expression}", mult)
         )
         bayes_factor_expr = (
```

### Comparing `splink-3.9.1/splink/profile_data.py` & `splink-3.9.2/splink/profile_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from copy import deepcopy
 
-from .charts import load_chart_definition, vegalite_or_json
+from .charts import altair_or_json, load_chart_definition
 from .misc import ensure_is_list
 
 
 def _group_name(cols_or_expr):
     cols_or_expr = re.sub(r"[^0-9a-zA-Z_]", " ", cols_or_expr)
     cols_or_expr = re.sub(r"\s+", "_", cols_or_expr)
     return cols_or_expr
@@ -21,15 +21,15 @@
 
     return e
 
 
 _outer_chart_spec_freq = {
     "config": {"view": {"continuousWidth": 400, "continuousHeight": 300}},
     "vconcat": [],
-    "$schema": "https://vega.github.io/schema/vega-lite/v4.8.1.json",
+    "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
 }
 
 chart_path = "profile_data.json"
 _inner_chart_spec_freq = load_chart_definition(chart_path)
 
 
 def _get_inner_chart_spec_freq(percentile_data, top_n_data, bottom_n_data, col_name):
@@ -243,8 +243,8 @@
             percentile_rows, top_n_rows, bottom_n_rows, expression
         )
         inner_charts.append(inner_chart)
     outer_spec = deepcopy(_outer_chart_spec_freq)
 
     outer_spec["vconcat"] = inner_charts
 
-    return vegalite_or_json(outer_spec)
+    return altair_or_json(outer_spec)
```

### Comparing `splink-3.9.1/splink/settings.py` & `splink-3.9.2/splink/settings.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/spark/linker.py` & `splink-3.9.2/splink/spark/linker.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,17 @@
             input = pd.DataFrame.from_records(input)
             input = self.spark.createDataFrame(input)
         elif isinstance(input, pd.DataFrame):
             input = self.spark.createDataFrame(input)
 
         input.createOrReplaceTempView(table_name)
 
-    def _random_sample_sql(self, proportion, sample_size, seed=None):
+    def _random_sample_sql(
+        self, proportion, sample_size, seed=None, table=None, unique_id=None
+    ):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         if seed:
             return f" ORDER BY rand({seed}) LIMIT {round(sample_size)}"
         else:
             return f" TABLESAMPLE ({percent} PERCENT) "
```

### Comparing `splink-3.9.1/splink/spark/spark_helpers/custom_spark_dialect.py` & `splink-3.9.2/splink/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/spark/spark_helpers/spark_base.py` & `splink-3.9.2/splink/spark/spark_helpers/spark_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/spark/spark_helpers/spark_comparison_imports.py` & `splink-3.9.2/splink/spark/spark_helpers/spark_comparison_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ...comparison_level_library import (
     ArrayIntersectLevelBase,
     ColumnsReversedLevelBase,
+    DamerauLevenshteinLevelBase,
     DateDiffLevelBase,
     DistanceFunctionLevelBase,
     DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
     JaccardLevelBase,
     JaroLevelBase,
@@ -23,14 +24,15 @@
     JaccardAtThresholdsComparisonBase,
     JaroAtThresholdsComparisonBase,
     JaroWinklerAtThresholdsComparisonBase,
     LevenshteinAtThresholdsComparisonBase,
 )
 from ...comparison_template_library import (
     DateComparisonBase,
+    EmailComparisonBase,
     ForenameSurnameComparisonBase,
     NameComparisonBase,
     PostcodeComparisonBase,
 )
 from .spark_base import (
     SparkBase,
 )
@@ -114,15 +116,15 @@
     pass
 
 
 class levenshtein_level(SparkBase, LevenshteinLevelBase):
     pass
 
 
-class damerau_levenshtein_level(SparkBase, LevenshteinLevelBase):
+class damerau_levenshtein_level(SparkBase, DamerauLevenshteinLevelBase):
     pass
 
 
 class jaro_level(SparkBase, JaroLevelBase):
     pass
 
 
@@ -242,7 +244,13 @@
     @property
     def _distance_level(self):
         return distance_function_level
 
 
 class postcode_comparison(SparkComparisonProperties, PostcodeComparisonBase):
     pass
+
+
+class email_comparison(SparkComparisonProperties, EmailComparisonBase):
+    @property
+    def _distance_level(self):
+        return distance_function_level
```

### Comparing `splink-3.9.1/splink/splink_comparison_viewer.py` & `splink-3.9.2/splink/splink_comparison_viewer.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/splink_dataframe.py` & `splink-3.9.2/splink/splink_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,28 @@
     Uses methods like `as_pandas_dataframe()` and `as_record_dict()` to retrieve data
     """
 
     def __init__(self, templated_name: str, physical_name: str, linker: Linker):
         self.templated_name = templated_name
         self.physical_name = physical_name
         self.linker = linker
+        self._target_schema = "splink"
 
     @property
     def columns(self):
         pass
 
     @property
     def columns_escaped(self):
         cols = self.columns
         return [c.name() for c in cols]
 
     def validate():
         pass
 
-    def _random_sample_sql(percent):
-        raise NotImplementedError("Random sample sql not implemented for this linker")
-
     @property
     def physical_and_template_names_equal(self):
         return self.templated_name == self.physical_name
 
     def _check_drop_table_created_by_splink(self, force_non_splink_table=False):
         if not self.physical_name.startswith("__splink__"):
             if not force_non_splink_table:
```

### Comparing `splink-3.9.1/splink/sql_transform.py` & `splink-3.9.2/splink/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py` & `splink-3.9.2/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 from ...comparison_level_library import (
     ColumnsReversedLevelBase,
+    DamerauLevenshteinLevelBase,
     DistanceFunctionLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
+    JaroLevelBase,
+    JaroWinklerLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
 from ...comparison_library import (
+    DamerauLevenshteinAtThresholdsComparisonBase,
     DistanceFunctionAtThresholdsComparisonBase,
     ExactMatchBase,
+    JaroAtThresholdsComparisonBase,
+    JaroWinklerAtThresholdsComparisonBase,
     LevenshteinAtThresholdsComparisonBase,
 )
+from ...comparison_template_library import (
+    ForenameSurnameComparisonBase,
+    NameComparisonBase,
+)
 from .sqlite_base import (
     SqliteBase,
 )
 
 
 # Class used to feed our comparison_library classes
 class SqliteComparisonProperties(SqliteBase):
@@ -36,14 +46,26 @@
         return distance_function_level
 
     @property
     def _levenshtein_level(self):
         return levenshtein_level
 
     @property
+    def _damerau_levenshtein_level(self):
+        return damerau_levenshtein_level
+
+    @property
+    def _jaro_level(self):
+        return jaro_level
+
+    @property
+    def _jaro_winkler_level(self):
+        return jaro_winkler_level
+
+    @property
     def _columns_reversed_level(self):
         return columns_reversed_level
 
 
 #########################
 ### COMPARISON LEVELS ###
 #########################
@@ -59,14 +81,26 @@
     pass
 
 
 class levenshtein_level(SqliteBase, LevenshteinLevelBase):
     pass
 
 
+class damerau_levenshtein_level(SqliteBase, DamerauLevenshteinLevelBase):
+    pass
+
+
+class jaro_level(SqliteBase, JaroLevelBase):
+    pass
+
+
+class jaro_winkler_level(SqliteBase, JaroWinklerLevelBase):
+    pass
+
+
 class columns_reversed_level(SqliteBase, ColumnsReversedLevelBase):
     pass
 
 
 class distance_function_level(SqliteBase, DistanceFunctionLevelBase):
     pass
 
@@ -90,7 +124,46 @@
 
 class levenshtein_at_thresholds(
     SqliteComparisonProperties, LevenshteinAtThresholdsComparisonBase
 ):
     @property
     def _distance_level(self):
         return self._levenshtein_level
+
+
+class damerau_levenshtein_at_thresholds(
+    SqliteComparisonProperties, DamerauLevenshteinAtThresholdsComparisonBase
+):
+    @property
+    def _distance_level(self):
+        return self._damerau_levenshtein_level
+
+
+class jaro_at_thresholds(SqliteComparisonProperties, JaroAtThresholdsComparisonBase):
+    @property
+    def _distance_level(self):
+        return self._jaro_level
+
+
+class jaro_winkler_at_thresholds(
+    SqliteComparisonProperties, JaroWinklerAtThresholdsComparisonBase
+):
+    @property
+    def _distance_level(self):
+        return self._jaro_winkler_level
+
+
+###################################
+### COMPARISON TEMPLATE LIBRARY ###
+###################################
+class name_comparison(SqliteComparisonProperties, NameComparisonBase):
+    @property
+    def _distance_level(self):
+        return distance_function_level
+
+
+class forename_surname_comparison(
+    SqliteComparisonProperties, ForenameSurnameComparisonBase
+):
+    @property
+    def _distance_level(self):
+        return distance_function_level
```

### Comparing `splink-3.9.1/splink/term_frequencies.py` & `splink-3.9.2/splink/term_frequencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import warnings
 from typing import TYPE_CHECKING
 
 from numpy import arange, ceil, floor, log2
 from pandas import concat, cut
 
-from .charts import load_chart_definition, vegalite_or_json
+from .charts import altair_or_json, load_chart_definition
 from .input_column import InputColumn, remove_quotes_from_identifiers
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 logger = logging.getLogger(__name__)
@@ -31,15 +31,15 @@
 def term_frequencies_for_single_column_sql(
     input_column: InputColumn, table_name="__splink__df_concat"
 ):
     col_name = input_column.name()
 
     sql = f"""
     select
-    {col_name}, cast(count(*) as double) / (select
+    {col_name}, cast(count(*) as float8) / (select
         count({col_name}) as total from {table_name})
             as {input_column.tf_name()}
     from {table_name}
     where {col_name} is not null
     group by {col_name}
     """
 
@@ -282,30 +282,18 @@
 
     # Complete chart schema
     tf_levels = [cl["comparison_vector_value"] for cl in c]
     labels = [
         f'{cl["label_for_charts"]} (TF col: {cl["tf_adjustment_column"]})' for cl in c
     ]
 
-    width_dict = df.groupby("gamma").count()["value"].to_dict()
-    width_expression = (
-        " ".join(
-            [
-                f"gamma_sel == {lev} ? {width_dict[lev] * 20 + 150} :"
-                for lev in tf_levels[:-1]
-            ]
-        )
-        + f" {width_dict[tf_levels[-1]] * 20 + 150}"
-    )
-
     df = df[df["gamma"].isin(tf_levels)].sort_values("least_freq_rank")
 
     chart["datasets"]["data"] = df.to_dict("records")
     chart["datasets"]["hist"] = binned_df.to_dict("records")
-    chart["config"]["width"]["signal"] = width_expression
     chart["config"]["params"][0]["value"] = max(tf_levels)
     chart["config"]["params"][0]["bind"]["options"] = tf_levels
     chart["config"]["params"][0]["bind"]["labels"] = labels
 
     # filters = [
     #     f"datum.most_freq_rank < {n_most_freq}",
     #     f"datum.least_freq_rank < {n_least_freq}",
@@ -316,8 +304,8 @@
     # chart["hconcat"][0]["layer"][2]["transform"][2]["filter"] = filter_text
 
     # PLACEHOLDER (until we work out adding a dynamic title based on the filtered data)
     chart["hconcat"][0]["layer"][0]["encoding"]["x"]["title"] = "TF column value"
     chart["hconcat"][0]["layer"][-1]["encoding"]["x"]["title"] = "TF column value"
     chart["hconcat"][0]["layer"][0]["encoding"]["tooltip"][0]["title"] = "Value"
 
-    return vegalite_or_json(chart, as_dict=as_dict)
+    return altair_or_json(chart, as_dict=as_dict)
```

### Comparing `splink-3.9.1/splink/unique_id_concat.py` & `splink-3.9.2/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/unlinkables.py` & `splink-3.9.2/splink/unlinkables.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/validate_jsonschema.py` & `splink-3.9.2/splink/validate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/vertically_concatenate.py` & `splink-3.9.2/splink/vertically_concatenate.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/splink/waterfall_chart.py` & `splink-3.9.2/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.1/PKG-INFO` & `splink-3.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.9.1
+Version: 3.9.2
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.3)
-Requires-Dist: altair (>=4.2.0)
+Requires-Dist: altair (>=5.0.1,<6.0.0)
 Requires-Dist: duckdb (>=0.6.0)
 Requires-Dist: jsonschema (>=3.2,<5.0)
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: phonetics (>=1.0.5,<2.0.0)
-Requires-Dist: sqlglot (>=5.1.0)
+Requires-Dist: sqlglot (>=5.1.0,<11.4.2)
 Project-URL: Repository, https://github.com/moj-analytical-services/splink
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/7570107/85285114-3969ac00-b488-11ea-88ff-5fca1b34af1f.png" alt="Splink Logo" height="150px">
 </p>
 
@@ -100,17 +100,17 @@
 ## Quickstart
 
 The following code demonstrates how to estimate the parameters of a deduplication model, use it to identify duplicate records, and then use clustering to generate an estimated unique person ID.
 
 For more detailed tutorials, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
-from splink.duckdb.duckdb_linker import DuckDBLinker
-import splink.duckdb.duckdb_comparison_library as cl
-import splink.duckdb.duckdb_comparison_template_library as ctl
+from splink.duckdb.linker import DuckDBLinker
+import splink.duckdb.comparison_library as cl
+import splink.duckdb.comparison_template_library as ctl
 
 import pandas as pd
 
 df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
 
 settings = {
     "link_type": "dedupe_only",
@@ -119,15 +119,15 @@
         "l.surname = r.surname",
     ],
     "comparisons": [
         ctl.name_comparison("first_name"),
         ctl.name_comparison("surname"),
         ctl.date_comparison("dob", cast_strings_to_date=True),
         cl.exact_match("city", term_frequency_adjustments=True),
-        cl.levenshtein_at_thresholds("email", 2),
+        ctl.email_comparison("email"),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
 blocking_rule_for_training = "l.first_name = r.first_name and l.surname = r.surname"
```

