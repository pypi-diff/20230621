# Comparing `tmp/dfcx-scrapi-1.6.3.tar.gz` & `tmp/dfcx-scrapi-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/pmarlow/eng/scrapi-github/dfcx-scrapi/dist/tmp9nwhs6bd/dfcx-scrapi-1.6.3.tar", last modified: Fri Apr 14 18:18:03 2023, max compression
+gzip compressed data, was "/Users/pmarlow/eng/scrapi-github/dfcx-scrapi/dist/tmp2p1p79yn/dfcx-scrapi-1.7.0.tar", last modified: Wed Jun 21 02:43:30 2023, max compression
```

## Comparing `dfcx-scrapi-1.6.3.tar` & `dfcx-scrapi-1.7.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13860 2022-09-29 22:10:42.000000 dfcx-scrapi-1.6.3/.pylintrc
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      248 2022-09-29 15:38:40.000000 dfcx-scrapi-1.6.3/requirements.txt
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/images/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    56107 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/images/logo.png
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      735 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/Makefile
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      776 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/pyproject.toml
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/tests/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1504 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/conftest.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/tests/license/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1030 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/license/license_check.sh
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/tests/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1405 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/test_search_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4767 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/test_agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      766 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/config.yaml
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9290 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/README.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1803 2023-04-14 18:17:28.000000 dfcx-scrapi-1.6.3/setup.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      765 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/.gitignore
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1103 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/CONTRIBUTING.md
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11982 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/scrapi_prebuilt.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/misc/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5080 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/misc/agent_backups.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/nlu_analysis_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10106 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10420 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5426 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/sheets_to_cx.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5246 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6414 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6769 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/custom_entities_to_sheets.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3634 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7555 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10505 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/builders_101.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9284 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/template.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/copy_paste_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12067 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/copy_paste_series/copy_paste_pages.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/.github/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/.github/workflows/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/.github/workflows/linter.yml
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      831 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1115 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1810 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/pull-request.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/setup.cfg
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/LICENSE.txt
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/data/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      535 2022-09-06 20:35:13.000000 dfcx-scrapi-1.6.3/data/intent_sample_with_parts.csv
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       11 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/requirements.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2215 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/main.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    92746 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/example_agent_ccai_sk.blob
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4079 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/sample_test_cases.blob
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      359 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/sample_intent_tp.csv
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      120 2022-09-06 20:35:13.000000 dfcx-scrapi-1.6.3/data/intent_sample_params.csv
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    29501 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/sample_agent.blob
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7606 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/maker_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    39988 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/dataframe_functions.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8789 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/semantic_clustering.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      559 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    36759 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/search_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7304 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/levenshtein.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14610 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/utterance_generator_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5178 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/webhook_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11855 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/nlu_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    50537 2023-04-03 20:10:57.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/copy_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6967 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/validation_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4869 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/stats_util.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10396 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/sessions.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12405 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/transition_route_groups.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    24678 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11979 2023-04-14 18:06:49.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/scrapi_base.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    23425 2023-04-14 18:06:49.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/conversation.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7082 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/security_settings.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14779 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    16662 2023-04-14 17:27:13.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2168 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/operations.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3048 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/experiments.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7425 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14793 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/environments.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7632 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/changelogs.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14556 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8770 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/versions.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7173 2023-03-27 14:44:33.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/webhooks.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15320 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/session_entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14575 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/test_cases.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4048 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/project.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11394 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/builders_common.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6402 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/transition_route_groups.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    23961 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10092 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/fulfillments.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8045 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    26689 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    20285 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9812 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/response_messages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13551 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/routes.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4649 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/utterance_generator.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/__init__.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14237 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/test_cases.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/agent_assist/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    18850 2023-04-03 20:04:03.000000 dfcx-scrapi-1.6.3/src/agent_assist/agent_assist.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-12-10 02:15:04.000000 dfcx-scrapi-1.6.3/src/agent_assist/__init__.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3537 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/SOURCES.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       27 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/requires.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       25 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/top_level.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/dependency_links.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13860 2022-09-29 22:10:42.000000 dfcx-scrapi-1.7.0/.pylintrc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      246 2023-06-17 20:22:26.000000 dfcx-scrapi-1.7.0/requirements.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/images/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    56107 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/images/logo.png
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      735 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/Makefile
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      776 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/pyproject.toml
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/tests/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1504 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/tests/conftest.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/tests/license/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1030 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/tests/license/license_check.sh
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/tests/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1405 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/tests/test_search_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4767 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/tests/test_agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      766 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/config.yaml
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9290 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/README.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1803 2023-06-21 02:35:09.000000 dfcx-scrapi-1.7.0/setup.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      765 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/.gitignore
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1103 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/CONTRIBUTING.md
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/examples/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11982 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/scrapi_prebuilt.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/examples/misc/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5080 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/misc/agent_backups.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/examples/nlu_analysis_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10106 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10420 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/examples/google_sheets_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5426 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/google_sheets_series/sheets_to_cx.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5246 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/google_sheets_series/cx_to_sheets.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6414 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6769 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/google_sheets_series/custom_entities_to_sheets.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/examples/bot_building_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3634 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_101.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7555 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10505 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_101.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/bot_building_series/builders_101.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9284 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/template.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/examples/copy_paste_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12067 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/examples/copy_paste_series/copy_paste_pages.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/.github/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/.github/workflows/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/.github/workflows/linter.yml
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      831 2022-02-04 04:14:34.000000 dfcx-scrapi-1.7.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1115 2022-02-04 04:14:34.000000 dfcx-scrapi-1.7.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1810 2022-02-04 04:14:34.000000 dfcx-scrapi-1.7.0/.github/ISSUE_TEMPLATE/pull-request.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/setup.cfg
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/LICENSE.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/data/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      535 2022-09-06 20:35:13.000000 dfcx-scrapi-1.7.0/data/intent_sample_with_parts.csv
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/data/ccai_service_kit/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/data/ccai_service_kit/conf_score_cfx/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       11 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/data/ccai_service_kit/conf_score_cfx/requirements.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2215 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/data/ccai_service_kit/conf_score_cfx/main.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    92746 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/data/ccai_service_kit/example_agent_ccai_sk.blob
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4079 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/data/sample_test_cases.blob
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      359 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/data/sample_intent_tp.csv
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      120 2022-09-06 20:35:13.000000 dfcx-scrapi-1.7.0/data/intent_sample_params.csv
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    29501 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/data/sample_agent.blob
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7606 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/maker_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    39988 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/dataframe_functions.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8789 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/semantic_clustering.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      559 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    36759 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/search_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7304 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/levenshtein.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14610 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/utterance_generator_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5178 2023-03-27 20:57:04.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/webhook_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11855 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/nlu_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    50537 2023-04-03 20:10:57.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/copy_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6967 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/validation_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4869 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/stats_util.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10397 2023-06-21 02:20:07.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/sessions.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12581 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/transition_route_groups.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    24899 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13532 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/scrapi_base.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    22800 2023-06-21 02:32:53.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/conversation.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7302 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/security_settings.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15460 2023-06-17 20:58:53.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    16955 2023-06-17 20:58:53.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2215 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/operations.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3112 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/experiments.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8298 2023-06-21 02:18:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15171 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/environments.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7721 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/changelogs.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14952 2023-06-21 02:18:27.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9034 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/versions.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7349 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/webhooks.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15540 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/session_entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15596 2023-06-17 20:27:52.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/test_cases.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4049 2023-06-17 20:27:42.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/project.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11394 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/builders_common.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6402 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/transition_route_groups.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    23961 2023-03-27 20:57:04.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10092 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/fulfillments.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8045 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    26689 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    20285 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9812 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/response_messages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13551 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/routes.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_ml/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_ml/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4649 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_ml/utterance_generator.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/__init__.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_async/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_async/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14237 2023-03-27 13:37:45.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_async/test_cases.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/agent_assist/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    18850 2023-04-03 20:04:03.000000 dfcx-scrapi-1.7.0/src/agent_assist/agent_assist.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-12-10 02:15:04.000000 dfcx-scrapi-1.7.0/src/agent_assist/__init__.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3537 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       27 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/requires.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       25 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/top_level.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-06-21 02:43:30.000000 dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/dependency_links.txt
```

### Comparing `dfcx-scrapi-1.6.3/PKG-INFO` & `dfcx-scrapi-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcx-scrapi
-Version: 1.6.3
+Version: 1.7.0
 Summary: A high level scripting API for bot builders, developers, and      maintainers.
 Home-page: https://github.com/GoogleCloudPlatform/dfcx-scrapi
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,intent,dfcx,entity
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.6.3 Summary: A high level
+Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.7.0 Summary: A high level
 scripting API for bot builders, developers, and maintainers. Home-page: https:/
 /github.com/GoogleCloudPlatform/dfcx-scrapi Author: Patrick Marlow Author-
 email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,intent,dfcx,entity Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

### Comparing `dfcx-scrapi-1.6.3/.pylintrc` & `dfcx-scrapi-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/images/logo.png` & `dfcx-scrapi-1.7.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/Makefile` & `dfcx-scrapi-1.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/pyproject.toml` & `dfcx-scrapi-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/tests/conftest.py` & `dfcx-scrapi-1.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/tests/license/license_check.sh` & `dfcx-scrapi-1.7.0/tests/license/license_check.sh`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/tests/test_search_util.py` & `dfcx-scrapi-1.7.0/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/tests/test_agents.py` & `dfcx-scrapi-1.7.0/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/config.yaml` & `dfcx-scrapi-1.7.0/config.yaml`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/README.md` & `dfcx-scrapi-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/setup.py` & `dfcx-scrapi-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dfcx-scrapi',
-    version='1.6.3',
+    version='1.7.0',
     description='A high level scripting API for bot builders, developers, and\
       maintainers.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/dfcx-scrapi',
     author='Patrick Marlow',
     author_email='pmarlow@google.com',
```

### Comparing `dfcx-scrapi-1.6.3/.gitignore` & `dfcx-scrapi-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/CONTRIBUTING.md` & `dfcx-scrapi-1.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/scrapi_prebuilt.ipynb` & `dfcx-scrapi-1.7.0/examples/scrapi_prebuilt.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/misc/agent_backups.ipynb` & `dfcx-scrapi-1.7.0/examples/misc/agent_backups.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb` & `dfcx-scrapi-1.7.0/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb` & `dfcx-scrapi-1.7.0/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/google_sheets_series/sheets_to_cx.ipynb` & `dfcx-scrapi-1.7.0/examples/google_sheets_series/sheets_to_cx.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets.ipynb` & `dfcx-scrapi-1.7.0/examples/google_sheets_series/cx_to_sheets.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb` & `dfcx-scrapi-1.7.0/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/google_sheets_series/custom_entities_to_sheets.ipynb` & `dfcx-scrapi-1.7.0/examples/google_sheets_series/custom_entities_to_sheets.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.py` & `dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_101.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb` & `dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.ipynb` & `dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_101.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py` & `dfcx-scrapi-1.7.0/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/bot_building_series/builders_101.ipynb` & `dfcx-scrapi-1.7.0/examples/bot_building_series/builders_101.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/template.ipynb` & `dfcx-scrapi-1.7.0/examples/template.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/examples/copy_paste_series/copy_paste_pages.ipynb` & `dfcx-scrapi-1.7.0/examples/copy_paste_series/copy_paste_pages.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/.github/workflows/linter.yml` & `dfcx-scrapi-1.7.0/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/feature-request.md` & `dfcx-scrapi-1.7.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/bug-report.md` & `dfcx-scrapi-1.7.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/pull-request.md` & `dfcx-scrapi-1.7.0/.github/ISSUE_TEMPLATE/pull-request.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/LICENSE.txt` & `dfcx-scrapi-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/data/intent_sample_with_parts.csv` & `dfcx-scrapi-1.7.0/data/intent_sample_with_parts.csv`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/main.py` & `dfcx-scrapi-1.7.0/data/ccai_service_kit/conf_score_cfx/main.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/data/ccai_service_kit/example_agent_ccai_sk.blob` & `dfcx-scrapi-1.7.0/data/ccai_service_kit/example_agent_ccai_sk.blob`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/data/sample_test_cases.blob` & `dfcx-scrapi-1.7.0/data/sample_test_cases.blob`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/data/sample_agent.blob` & `dfcx-scrapi-1.7.0/data/sample_agent.blob`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/maker_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/maker_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/dataframe_functions.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/semantic_clustering.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/semantic_clustering.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/__init__.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/search_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/search_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/levenshtein.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/levenshtein.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/utterance_generator_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/utterance_generator_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/webhook_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/webhook_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/nlu_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/nlu_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/copy_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/copy_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/validation_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/validation_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/stats_util.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/tools/stats_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/sessions.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 
 import logging
 import uuid
 from typing import Dict, List
 from google.cloud.dialogflowcx_v3beta1 import services
 from google.cloud.dialogflowcx_v3beta1 import types
 
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+from dfcx_scrapi.core import scrapi_base
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
-class Sessions(ScrapiBase):
+class Sessions(scrapi_base.ScrapiBase):
     """Core Class for CX Session Resource functions."""
 
     def __init__(
         self,
         creds_path: str = None,
         creds_dict: Dict = None,
         scope=False,
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/transition_route_groups.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/transition_route_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
             pages_dict = {
                 page.name: page.display_name
                 for page in self.list_transition_route_groups(flow_id)
             }
 
         return pages_dict
 
+    @scrapi_base.api_call_counter_decorator
     def list_transition_route_groups(self, flow_id: str = None):
         """Exports List of all Route Groups in the specified CX Flow ID.
 
         Args:
           flow_id: The formatted CX Flow ID to list the route groups from
 
         Returns:
@@ -160,14 +161,15 @@
         cx_route_groups = []
         for page in response.pages:
             for cx_route_group in page.transition_route_groups:
                 cx_route_groups.append(cx_route_group)
 
         return cx_route_groups
 
+    @scrapi_base.api_call_counter_decorator
     def get_transition_route_group(self, route_group_id):
         """Get a single Transition Route Group object.
 
         Args:
           route_group_id: the formatted CX Route Group ID to retrieve.
 
         Returns:
@@ -179,14 +181,15 @@
         client = services.transition_route_groups.TransitionRouteGroupsClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.get_transition_route_group(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_transition_route_group(
         self,
         flow_id: str = None,
         obj: types.TransitionRouteGroup = None,
         **kwargs,
     ):
         """Create a single Transition Route Group resource.
@@ -218,14 +221,15 @@
         )
         response = client.create_transition_route_group(
             parent=flow_id, transition_route_group=trg
         )
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def update_transition_route_group(
         self,
         route_group_id: str = None,
         obj: types.TransitionRouteGroup = None,
         language_code: str = None,
         **kwargs,
     ):
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/intents.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/intents.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 from typing import Dict, List, Tuple
 import pandas as pd
 
 from google.cloud.dialogflowcx_v3beta1 import services
 from google.cloud.dialogflowcx_v3beta1 import types
 from google.protobuf import field_mask_pb2
 
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+from dfcx_scrapi.core import scrapi_base
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
-class Intents(ScrapiBase):
+class Intents(scrapi_base.ScrapiBase):
     """Core Class for CX Intent Resource functions."""
 
     def __init__(
         self,
         creds_path: str = None,
         creds_dict: Dict = None,
         creds=None,
@@ -405,14 +405,15 @@
             intents_dict = {
                 intent.name: intent.display_name
                 for intent in self.list_intents(agent_id)
             }
 
         return intents_dict
 
+    @scrapi_base.api_call_counter_decorator
     def list_intents(
         self,
         agent_id: str = None,
         language_code: str = None) -> List[types.Intent]:
         """Exports List of all intents in specific CX Agent.
 
         Args:
@@ -441,14 +442,15 @@
         intents = []
         for page in response.pages:
             for intent in page.intents:
                 intents.append(intent)
 
         return intents
 
+    @scrapi_base.api_call_counter_decorator
     def get_intent(
         self,
         intent_id: str = None,
         language_code: str = None) -> types.Intent:
         """Get a single Intent object based on specific CX Intent ID.
 
         Args:
@@ -473,14 +475,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.get_intent(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_intent(
         self,
         agent_id: str,
         obj: types.Intent = None,
         display_name: str = None,
         language_code: str = None,
         **kwargs) -> types.Intent:
@@ -527,14 +530,15 @@
             client_options=client_options, credentials=self.creds
         )
 
         response = client.create_intent(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def update_intent(
         self,
         intent_id: str = None,
         obj: types.Intent = None,
         language_code: str = None,
         **kwargs) -> types.Intent:
         """Updates a single Intent object based on provided arguments.
@@ -578,14 +582,15 @@
         if language_code:
             request.language_code = language_code
 
         response = client.update_intent(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def delete_intent(self, intent_id: str, obj: types.Intent = None) -> None:
         """Deletes an intent by Intent ID.
 
         Args:
           intent_id: intent to delete
         """
         if obj:
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/scrapi_base.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/scrapi_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import json
 import re
-
+import functools
+from collections import defaultdict
 from typing import Dict
+
 from google.oauth2 import service_account
 from google.auth.transport.requests import Request
 from google.protobuf import json_format  # type: ignore
 
 from proto.marshal.collections import repeated
 from proto.marshal.collections import maps
 
@@ -67,14 +69,16 @@
         else:
             self.creds = None
             self.token = None
 
         if agent_id:
             self.agent_id = agent_id
 
+        self.api_calls_dict = defaultdict(int)
+
     @staticmethod
     def _set_region(resource_id: str):
         """Different regions have different API endpoints
 
         Args:
           item_id: agent/flow/page - any type of long path id like
             `projects/<GCP PROJECT ID>/locations/<LOCATION ID>
@@ -271,7 +275,52 @@
             if isinstance(v, maps.MapComposite):
                 v = self.recurse_proto_marshal_to_dict(v)
             elif isinstance(v, repeated.RepeatedComposite):
                 v = self.recurse_proto_repeated_composite(v)
             new_dict[k] = v
 
         return new_dict
+
+    def get_api_calls_details(self) -> Dict[str, int]:
+        """The number of API calls corresponding to each method.
+
+        Returns:
+          A dictionary with keys as the method names
+          and values as the number of calls.
+        """
+        this_class_methods, sub_class_apis_dict = {}, {}
+
+        for attr_name in dir(self):
+            attr = getattr(self, attr_name)
+            if callable(attr) and hasattr(attr, "calls_api"):
+                this_class_methods[attr_name] = 0
+            if any(
+                isinstance(attr, sub_class)
+                for sub_class in ScrapiBase.__subclasses__()
+            ):
+                sub_class_apis_dict.update(attr.get_api_calls_details())
+
+        if hasattr(self, "api_calls_dict"):
+            this_class_methods.update(getattr(self, "api_calls_dict"))
+
+        return {**this_class_methods, **sub_class_apis_dict}
+
+    def get_api_calls_count(self) -> int:
+        """Show the total number of API calls for this resource.
+
+        Returns:
+          Total calls to the API so far as an int.
+        """
+        return sum(self.get_api_calls_details().values())
+
+
+def api_call_counter_decorator(func):
+    """Counts the number of API calls for the function `func`."""
+
+    @functools.wraps(func)
+    def wrapper(self, *args, **kwargs):
+        self.api_calls_dict[func.__name__] += 1
+        return func(self, *args, **kwargs)
+
+    wrapper.calls_api = True
+
+    return wrapper
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/conversation.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,14 +391,15 @@
         else:
             start_time = self.start_time
         duration = round((time.perf_counter() - start_time), 2)
         if duration > 2:
             if msg:
                 print(f"{duration:0.2f}s {msg}")
 
+    @scrapi_base.api_call_counter_decorator
     def reply(
         self,
         send_obj: Dict[str, str],
         restart: bool = False,
         retries: int = 0,
         current_page: str = None,
         checkpoints: bool = False,
@@ -418,15 +419,15 @@
           current_page: Specify the page id to start the conversation from
           checkpoints: Boolean flag to enable/disable Checkpoint timer
             debugging. Defaults to False.
 
         Returns:
           A dictionary for the agent reply to to the submitted text.
             Includes keys response_messages, confidence, page_name,
-            intent_name, match_type, match, other_intents, and params.
+            intent_name, match_type, match, and params.
         """
         text = send_obj.get("text")
         send_params = send_obj.get("params")
 
         if not text:
             logging.warning(f"Input Text is empty. {send_obj}")
 
@@ -538,43 +539,20 @@
         reply["confidence"] = query_result.intent_detection_confidence
         reply["page_name"] = query_result.current_page.display_name
         reply["intent_name"] = query_result.intent.display_name
         reply["match_type"] = self._get_match_type_from_map(
             query_result.match.match_type
         )
         reply["match"] = query_result.match
-        reply["other_intents"] = self.format_other_intents(query_result)
         reply["params"] = params
 
         logging.debug("reply %s", reply)
 
         return reply
 
-    def format_other_intents(self, query_result):
-        """Unwind protobufs into more friendly dict"""
-        other_intents = query_result.diagnostic_info.get(
-            "Alternative Matched Intents"
-        )
-        items = []
-        rank = 0
-        for alt in other_intents:
-            items.append(
-                {
-                    "name": alt.get("DisplayName"),
-                    "score": alt.get("Score"),
-                    "rank": rank,
-                }
-            )
-            rank += 1
-
-        if self:
-            return items
-
-        return None
-
     def getpath(self, obj, xpath, default=None):
         """Get data at a pathed location out of object internals"""
         elem = obj
         try:
             for xpitem in xpath.strip("/").split("/"):
                 try:
                     xpitem = int(xpitem)
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/security_settings.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/security_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
         if agent_id:
             self.agent_id = agent_id
 
         self.ss_service = services.security_settings_service
         self.ss_types = types.security_settings
 
+    @scrapi_base.api_call_counter_decorator
     def list_security_settings(self, location_id: str):
         """List Security Settings for a given Project and Region.
 
         Args:
           location_id: CX Agent ID string in the following format
             projects/<PROJECT ID>/locations/<LOCATION ID>/
 
@@ -79,14 +80,15 @@
         for page in response.pages:
             for ss in page.security_settings:
                 security_settings.append(ss)
 
         return security_settings
 
 
+    @scrapi_base.api_call_counter_decorator
     def get_security_settings(self, security_setting_id: str):
         """Get specified CCAI Security Setting.
 
         Args:
           security_setting_id: Security Setting ID string in the following
             format: projects/<PROJECT ID>/locations/<LOCATION ID>/
             securitySettings/<SECURITY SETTINGS ID>
@@ -103,14 +105,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.get_security_settings(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_security_settings(
         self,
         location_id: str,
         obj: types.SecuritySettings = None,
         security_settings_dict: Dict[str,str] = None):
         """Create CCAI Security Settings profile in the specified project.
 
@@ -154,14 +157,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.create_security_settings(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def update_security_settings(self, security_setting_id: str, **kwargs):
         """Update specified CCAI Security Setting.
 
         Args:
           security_setting_id: Security Setting ID string in the following
             format: projects/<PROJECT ID>/locations/<LOCATION ID>/
             securitySettings/<SECURITY SETTINGS ID>
@@ -188,14 +192,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.update_security_settings(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def delete_security_settings(self, security_setting_id: str):
         """Delete the specified CCAI Security Setting.
 
         Args:
           security_setting_id: Security Setting ID string in the following
             format: projects/<PROJECT ID>/locations/<LOCATION ID>/
             securitySettings/<SECURITY SETTINGS ID>
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/entity_types.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/entity_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,45 +18,47 @@
 from typing import Dict, List
 
 import pandas as pd
 from google.cloud.dialogflowcx_v3beta1 import services
 from google.cloud.dialogflowcx_v3beta1 import types
 from google.protobuf import field_mask_pb2
 
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+from dfcx_scrapi.core import scrapi_base
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
-class EntityTypes(ScrapiBase):
+class EntityTypes(scrapi_base.ScrapiBase):
     """Core Class for CX Entity Type Resource functions."""
 
     def __init__(
         self,
         creds_path: str = None,
         creds_dict: Dict = None,
         creds=None,
         scope=False,
         entity_id: str = None,
         agent_id: str = None,
+        language_code: str = "en"
     ):
         super().__init__(
             creds_path=creds_path,
             creds_dict=creds_dict,
             creds=creds,
             scope=scope,
         )
 
         self.entity_id = entity_id
         self.agent_id = agent_id
+        self.language_code = language_code
 
 
     @staticmethod
     def entity_type_proto_to_dataframe(
         obj: types.EntityType, mode: str = "basic"
     ):
         """Converts an EntityType protobuf object to a Pandas Dataframe.
@@ -239,28 +241,31 @@
             entities_dict = {
                 entity.name: entity.display_name
                 for entity in self.list_entity_types(agent_id)
             }
 
         return entities_dict
 
-    def list_entity_types(self, agent_id: str = None):
+    @scrapi_base.api_call_counter_decorator
+    def list_entity_types(self, agent_id: str, language_code: str = "en"):
         """Returns a list of Entity Type objects.
 
         Args:
           agent_id: the formatted CX Agent ID to use
+          language_code: Specifies the language of the Entity Types listed
 
         Returns:
           List of Entity Type objects
         """
         if not agent_id:
             agent_id = self.agent_id
 
         request = types.entity_type.ListEntityTypesRequest()
         request.parent = agent_id
+        request.language_code = language_code
 
         client_options = self._set_region(agent_id)
         client = services.entity_types.EntityTypesClient(
             credentials=self.creds, client_options=client_options
         )
 
         response = client.list_entity_types(request)
@@ -268,34 +273,41 @@
         entities = []
         for page in response.pages:
             for entity in page.entity_types:
                 entities.append(entity)
 
         return entities
 
-    def get_entity_type(self, entity_id: str = None):
+    @scrapi_base.api_call_counter_decorator
+    def get_entity_type(self, entity_id: str = None, language_code: str = "en"):
         """Returns a single Entity Type object.
 
         Args:
           entity_id: the formatted CX Entity ID to get
+          language_code: Specifies the language of the Entity Types listed
 
         Returns:
           The single Entity Type object
         """
         if not entity_id:
             entity_id = self.entity_id
 
         client_options = self._set_region(entity_id)
         client = services.entity_types.EntityTypesClient(
             credentials=self.creds, client_options=client_options
         )
-        response = client.get_entity_type(name=entity_id)
+        request = types.entity_type.GetEntityTypeRequest()
+        request.name = entity_id
+        request.language_code = language_code
+
+        response = client.get_entity_type(request=request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_entity_type(
         self,
         agent_id: str = None,
         display_name: str = None,
         language_code: str = None,
         obj: types.EntityType = None,
         **kwargs
@@ -349,14 +361,15 @@
 
         response = client.create_entity_type(
             request=request
         )
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def update_entity_type(
         self,
         entity_type_id: str = None,
         obj: types.EntityType = None,
         language_code: str = None,
         **kwargs):
         """Update a single CX Entity Type object.
@@ -403,14 +416,15 @@
         if language_code:
             request.language_code = language_code
 
         response = client.update_entity_type(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def delete_entity_type(self, entity_id: str = None, obj=None) -> None:
         """Deletes a single Entity Type resouce object.
 
         Args:
           entity_id: the formatted CX Entity ID to delete
 
         Returns:
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/agents.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/agents.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,50 +49,63 @@
             scope=scope,
         )
 
         if agent_id:
             self.agent_id = agent_id
             self.client_options = self._set_region(agent_id)
 
-    def _build_list_agents_client_request(self, location_id):
-        """Builds the List Agents Request object."""
+    @scrapi_base.api_call_counter_decorator
+    def _list_agents_client_request(self, location_id) -> List[
+        types.agent.Agent
+    ]:
+        """Builds the List Agents Request object.
+
+        Args:
+          location_id: The GCP Location ID in the following format:
+            `projects/<project_id>/locations/<location>`
+
+        Returns:
+          List of types.agent.Agent"""
 
         request = types.agent.ListAgentsRequest()
         request.parent = location_id
 
         client_options = self._set_region(location_id)
         client = services.agents.AgentsClient(
             credentials=self.creds, client_options=client_options
         )
 
-        return client, request
+        response = client.list_agents(request)
+
+        agents = []
+        for page in response.pages:
+            for agent in page.agents:
+                agents.append(agent)
+
+        return agents
 
     def list_agents(
         self,
-        location_id: str = None,
-        project_id: str = None) -> List[types.Agent]:
+        project_id: str,
+        location: str = None) -> List[types.Agent]:
         """Get list of all CX agents in a given GCP Region or Project.
 
-        This method allows you to provide a specific Location ID consisting of
-        a GCP Project ID and Location ID (i.e. GCP Region Name) to retrieve all
-        of the CX agents associated with that Project/Region. Optionally, you
-        can provide just the Project ID and the funciton will traverse ALL
-        available GCP regions to list ALL agents across the regions.
+        This method allows you to provide a GCP Project ID to retrieve all of
+        the CX agents across ALL available GCP region. If the optional location
+        ID is provided, the method will only pull the agents for that region.
 
         Args:
-          location_id: The GCP Project/Location ID in the following format
-              `projects/<GCP PROJECT ID>/locations/<LOCATION ID>`
-              `projects/my-gcp-project/locations/us-central1`
-          project_id: The GCP Project ID as a string
+          project_id: The GCP Project ID. Ex: `my-cool-gcp-project`
+          location_id: The GCP Location ID. Ex: `global`, `us-central1`, etc.
 
         Returns:
           List of Agent objects
         """
 
-        if project_id:
+        if not location:
             region_list = [
                 "global",
                 "us-central1",
                 "us-east1",
                 "us-west1",
                 "asia-northeast1",
                 "asia-south1",
@@ -101,34 +114,23 @@
                 "europe-west1",
                 "europe-west2",
             ]
 
             agents = []
             for region in region_list:
                 location_path = f"projects/{project_id}/locations/{region}"
-                client, request = self._build_list_agents_client_request(
-                    location_path
-                )
-
-                agents += self.list_agents(location_id=location_path)
+                agents += self._list_agents_client_request(location_path)
 
         else:
-            client, request = self._build_list_agents_client_request(
-                location_id
-            )
-
-            response = client.list_agents(request)
-
-            agents = []
-            for page in response.pages:
-                for agent in page.agents:
-                    agents.append(agent)
+            location_path = f"projects/{project_id}/locations/{location}"
+            agents = self._list_agents_client_request(location_path)
 
         return agents
 
+    @scrapi_base.api_call_counter_decorator
     def get_agent(self, agent_id: str) -> types.Agent:
         """Retrieves a single CX Agent resource object.
 
         Args:
           agent_id: The formatted CX Agent ID
 
         Returns:
@@ -174,22 +176,20 @@
               https://cloud.google.com/dialogflow/cx/docs/concept/region#avail
 
         Returns:
           CX agent resource object. If no agent is found, returns None.
         """
 
         if location_id:
-            agent_list = self.list_agents(
-                location_id=location_id
-                )
+            agent_list = self._list_agents_client_request(location_id)
 
         elif region:
-            agent_list = self.list_agents(
-                location_id=f"projects/{project_id}/locations/{region}"
-            )
+            agent_list = self._list_agents_client_request(
+                f"projects/{project_id}/locations/{region}"
+                )
         else:
             agent_list = self.list_agents(project_id=project_id)
 
         possible_agent = None
         matched_agent = None
 
         for agent in agent_list:
@@ -212,14 +212,15 @@
                  ambiguity.''',
                 possible_agent.display_name
             )
             matched_agent = None
 
         return matched_agent
 
+    @scrapi_base.api_call_counter_decorator
     def create_agent(
         self,
         project_id: str,
         display_name: str = None,
         gcp_region: str = "global",
         obj: types.Agent = None,
         **kwargs,
@@ -269,17 +270,19 @@
             credentials=self.creds, client_options=client_options
         )
         response = client.create_agent(parent=parent, agent=agent_obj)
 
         return response
 
 
+    @scrapi_base.api_call_counter_decorator
     def validate_agent(
         self,
-        agent_id: str = None,
+        agent_id: str,
+        language_code: str = "en",
         timeout: float = None) -> Dict:
         """Initiates the Validation of the CX Agent or Flow.
 
         This function will start the Validation feature for the given Agent
         and then return the results as a Dict.
 
         Args:
@@ -292,27 +295,29 @@
         """
 
         if not agent_id:
             agent_id = self.agent_id
 
         request = types.agent.ValidateAgentRequest()
         request.name = agent_id
+        request.language_code = language_code
 
         client_options = self._set_region(agent_id)
         client = services.agents.AgentsClient(
             credentials=self.creds, client_options=client_options
         )
 
         response = client.validate_agent(request, timeout=timeout)
 
         val_dict = self.cx_object_to_dict(response)
 
         return val_dict
 
 
+    @scrapi_base.api_call_counter_decorator
     def get_validation_result(
         self,
         agent_id: str = None,
         timeout: float = None) -> Dict:
         """Extract Validation Results from CX Validation feature.
 
         This function will get the LATEST validation result run for the given
@@ -350,14 +355,15 @@
         )
 
         val_results_dict = self.cx_object_to_dict(response)
 
         return val_results_dict
 
 
+    @scrapi_base.api_call_counter_decorator
     def export_agent(
         self,
         agent_id: str,
         gcs_bucket_uri: str,
         environment_display_name: str = None
     ) -> str:
         """Exports the specified CX agent to Google Cloud Storage bucket.
@@ -398,14 +404,15 @@
             credentials=self.creds, client_options=client_options
         )
         response = client.export_agent(request)
 
         return response.operation.name
 
 
+    @scrapi_base.api_call_counter_decorator
     def restore_agent(self, agent_id: str, gcs_bucket_uri: str) -> str:
         """Restores a CX agent from a gcs_bucket location.
 
         Currently there is no way to restore back to default
         settings via the api. The feature request for this is logged.
 
         Args:
@@ -429,14 +436,15 @@
         client = services.agents.AgentsClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.restore_agent(request)
 
         return response.operation.name
 
+    @scrapi_base.api_call_counter_decorator
     def update_agent(
         self, agent_id: str, obj: types.Agent = None, **kwargs
     ) -> types.Agent:
         """Updates a single Agent object based on provided kwargs.
 
         Args:
           agent_id: CX Agent ID string in the following format
@@ -466,14 +474,15 @@
         client = services.agents.AgentsClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.update_agent(agent=agent, update_mask=mask)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def delete_agent(self, agent_id: str) -> str:
         """Deletes the specified Dialogflow CX Agent.
 
         Args:
           agent_id: CX Agent ID string in the following format
             projects/<PROJECT ID>/locations/<LOCATION ID>/agents/<AGENT ID>
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/operations.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from typing import Dict
+
 from google.api_core import operations_v1, grpc_helpers
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+
+from dfcx_scrapi.core import scrapi_base
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
-class Operations(ScrapiBase):
+class Operations(scrapi_base.ScrapiBase):
     """Core class for Operations functions, primarily used to
     extract LRO information on long running jobs for CX.
     """
 
     def __init__(
         self,
         creds_path: str = None,
@@ -41,14 +43,15 @@
         super().__init__(
             creds_path=creds_path,
             creds_dict=creds_dict,
             creds=creds,
             scope=scope
         )
 
+    @scrapi_base.api_call_counter_decorator
     def get_lro(self, lro: str):
         """Used to retrieve the status of LROs for Dialogflow CX.
 
         Args:
           lro: The Long Running Operation(LRO) ID in the following format
               'projects/<project-name>/locations/<locat>/operations/
                 <operation-uuid>'
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/experiments.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/experiments.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 # limitations under the License.
 
 import json
 import logging
 from typing import Dict
 from google.cloud.dialogflowcx_v3beta1 import services
 from google.cloud.dialogflowcx_v3beta1 import types
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+from dfcx_scrapi.core import scrapi_base
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 SCOPES = [
     "https://www.googleapis.com/auth/cloud-platform",
     "https://www.googleapis.com/auth/dialogflow",
 ]
 
 
-class ScrapiExperiments(ScrapiBase):
+class ScrapiExperiments(scrapi_base.ScrapiBase):
     """Wrapper for working with Experiments"""
 
     def __init__(
         self,
         creds_path: str = None,
         creds_dict: Dict = None,
         creds=None,
@@ -51,15 +51,16 @@
             creds=creds,
             scope=scope,
             agent_id=agent_id,
         )
 
         logging.info("created %s", self.agent_id)
 
-    def list_experiments(self, environment_id=None):
+    @scrapi_base.api_call_counter_decorator
+    def list_experiments(self, environment_id: str = None):
         """List out experiments.
 
         Args:
           environment_id: (Optional) The ID for the environment from which
             the list of experiments will be retrieved.
 
         Returns:
@@ -71,15 +72,15 @@
         request = types.experiment.ListExperimentsRequest()
         request.parent = environment_path
         client_options = self._set_region(environment_path)
         client = services.experiments.ExperimentsClient(
             client_options=client_options, credentials=self.creds
         )
         response = client.list_experiments(request)
-        blob = ScrapiBase.cx_object_to_json(response)
+        blob = scrapi_base.ScrapiBase.cx_object_to_json(response)
 
         if len(blob) < 1:
             logging.warning(
                 "no experiments found for environment: %s", environment_id
             )
             return None
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/pages.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/pages.py`

 * *Files 19% similar despite different names*

```diff
@@ -108,39 +108,49 @@
 
         pages_dict = self._add_generic_pages_to_map(
             flow_id, pages_dict, reverse
         )
 
         return pages_dict
 
-    def list_pages(self, flow_id: str = None) -> List[gcdc_page.Page]:
+    @scrapi_base.api_call_counter_decorator
+    def list_pages(
+        self,
+        flow_id: str = None,
+        language_code: str = "en") -> List[gcdc_page.Page]:
         """Get a List of all pages for the specified Flow ID.
 
         Args:
           flow_id: the properly formatted Flow ID string
+          language_code: Specifies the language of the Pages listed. While the
+            majority of contents of a Page is language agnostic, the contents
+            in the "Agent Says" and similar parts of a Page are affected by
+            language code.
 
         Returns:
           A List of CX Page objects for the specific Flow ID
         """
         request = gcdc_page.ListPagesRequest()
         request.parent = flow_id
+        request.language_code = language_code
 
         client_options = self._set_region(flow_id)
         client = pages.PagesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.list_pages(request)
 
         cx_pages = []
         for page in response.pages:
             for cx_page in page.pages:
                 cx_pages.append(cx_page)
 
         return cx_pages
 
+    @scrapi_base.api_call_counter_decorator
     def get_page(self, page_id: str = None) -> gcdc_page.Page:
         """Get a single CX Page object based on the provided Page ID.
 
         Args:
           page_id: a properly formatted CX Page ID
 
         Returns:
@@ -154,14 +164,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.get_page(name=page_id)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_page(
         self, flow_id: str = None, obj: gcdc_page.Page = None, **kwargs
     ) -> gcdc_page.Page:
         """Create a single CX Page object in the specified Flow ID.
 
         Args:
           flow_id: the CX Flow ID where the Page object will be created
@@ -187,14 +198,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.create_page(parent=flow_id, page=page)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def update_page(
         self, page_id: str = None, obj: gcdc_page.Page = None, **kwargs
     ) -> gcdc_page.Page:
         """Update a single CX Page object.
 
         Args:
           page_id: the CX Page ID to update
@@ -221,25 +233,30 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.update_page(page=page, update_mask=mask)
 
         return response
 
-    def delete_page(self, page_id: str = None) -> str:
+    @scrapi_base.api_call_counter_decorator
+    def delete_page(self, page_id: str = None, force: bool = False) -> str:
         """Deletes the specified Page.
 
         Args:
           page_id: CX Page ID string in the following Format:
             ``projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>/
               flows/<Flow ID>/pages/<Page ID>``
+          force: (Optional) This field has no effect for pages with no incoming
+            transitions. If set to True, Dialogflow will remove the page,
+            as well as any transitions to the page.
 
         Returns:
           String "Page `{page_id}` successfully deleted."
         """
         client_options = self._set_region(page_id)
         client = pages.PagesClient(
             credentials=self.creds, client_options=client_options
         )
-        client.delete_page(name=page_id)
+        req = gcdc_page.DeletePageRequest(name=page_id, force=force)
+        client.delete_page(request=req)
 
         return f"Page `{page_id}` successfully deleted."
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/environments.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/environments.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 class Environments(scrapi_base.ScrapiBase):
     """Core Class for CX Environments Resource functions."""
 
     def __init__(
         self,
         creds_path: str = None,
-        creds_dict: Dict[str,str] = None,
+        creds_dict: Dict[str, str] = None,
         creds: service_account.Credentials = None,
         agent_id: str = None,
     ):
         super().__init__(
             creds_path=creds_path,
             creds_dict=creds_dict,
             creds=creds,
@@ -125,15 +125,16 @@
             environments_dict = {
                 environment.name: environment.display_name
                 for environment in self.list_environments(agent_id)
             }
 
         return environments_dict
 
-    def list_environments(self, agent_id:str=None):
+    @scrapi_base.api_call_counter_decorator
+    def list_environments(self, agent_id: str = None):
         """List all Versions for a given Flow"""
 
         if not agent_id:
             agent_id = self.agent_id
 
         request = types.environment.ListEnvironmentsRequest()
 
@@ -148,17 +149,18 @@
         environments = []
         for page in response.pages:
             for environment in page.environments:
                 environments.append(environment)
 
         return environments
 
+    @scrapi_base.api_call_counter_decorator
     def get_environment(
         self,
-        environment_id:str) -> types.environment.Environment:
+        environment_id: str) -> types.environment.Environment:
         """Get Environment object for specified environment ID.
 
         Args:
           environment_id: Unique environment ID of the target to get. Format:
             projects/<Project ID>/locations/<Location ID>/agents/
             <Agent ID>/environments/<Environment ID>
 
@@ -174,16 +176,16 @@
 
         response = client.get_environment(request)
 
         return response
 
     def get_environment_by_display_name(
         self,
-        display_name:str,
-        agent_id:str) -> types.environment.Environment:
+        display_name: str,
+        agent_id: str) -> types.environment.Environment:
         """Get Environment object for specific environment by its display name.
 
         Args:
           display_name: Human readable display name of the target to get.
           agent_id: The agent for the operation. format:
             projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>
 
@@ -197,18 +199,19 @@
         environment_list = self.list_environments(agent_id)
         for environment_obj in environment_list:
             if environment_obj.display_name == display_name:
                 result = environment_obj
 
         return result
 
+    @scrapi_base.api_call_counter_decorator
     def create_environment(
         self,
-        environment:types.environment.Environment,
-        agent_id:str=None):
+        environment: types.environment.Environment,
+        agent_id: str = None):
         """Create a new environment for a specified agent.
         Args:
           environment: The environment to create.
             type google.cloud.dialogflowcx_v3beta1.types.Environment
           agent_id: The targeted agent for the operation. format:
             projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>
 
@@ -231,18 +234,18 @@
         response = client.create_environment(request)
 
         return response
 
 
     def create_environment_by_display_name(
         self,
-        display_name:str,
-        version_configs:List[Tuple[str,str]],
-        description:str=None,
-        agent_id:str=None):
+        display_name: str,
+        version_configs: List[Tuple[str, str]],
+        description: str = None,
+        agent_id: str = None):
         """Create a new environment for a specified agent.
         Args:
           display_name: The display name of the Environment to create
           version_configs: A List of Tuples, containing the Flow Display
             Names and Version IDs to include in the Environment creation.
             Ex:
               [('Default Start Flow', 2), ('Confidence Demo', 3), ('FlowC', 1)]
@@ -282,18 +285,19 @@
         )
 
         response = client.create_environment(request)
 
         return response
 
 
+    @scrapi_base.api_call_counter_decorator
     def update_environment(
         self,
         environment_id: str,
-        environment_obj:types.Environment = None,
+        environment_obj: types.Environment = None,
         **kwargs):
         """Update an existing environment for a specified agent.
 
         Args:
           environment_id: The specified environment to update.
           environment_obj: Optional Environment object of types.Environment
             that can be provided when you are planning to replace the full
@@ -326,15 +330,16 @@
         request.update_mask = mask
 
         response = client.update_environment(request)
 
         return response
 
 
-    def delete_environment(self, environment_id:str):
+    @scrapi_base.api_call_counter_decorator
+    def delete_environment(self, environment_id: str):
         """Delete a specified environment.
 
         Args:
           environment_id: unique ID associated with target environment. Format:
             projects/<Project ID>/locations/<Location ID>/agents/
             <Agent ID>/environments/<Environment ID>.
         """
@@ -346,18 +351,19 @@
         client = services.environments.EnvironmentsClient(
             credentials=self.creds, client_options=client_options
         )
 
         client.delete_environment(request)
 
 
+    @scrapi_base.api_call_counter_decorator
     def deploy_flow_to_environment(
         self,
-        environment_id:str,
-        flow_version:str):
+        environment_id: str,
+        flow_version: str):
         """Deploys a flow to the specified environment.
 
          Args:
           environment_id: unique ID associated with target environment. Format:
             projects/<Project ID>/locations/<Location ID>/agents/
             <Agent ID>/environments/<Environment ID>.
           flow_version: Required. The flow version to deploy. Format:
@@ -378,17 +384,18 @@
         )
 
         response = client.deploy_flow(request)
 
         return response
 
 
+    @scrapi_base.api_call_counter_decorator
     def lookup_environment_history(
         self,
-        environment_id:str) -> List[types.Environment]:
+        environment_id: str) -> List[types.Environment]:
         """Looks up the history of the specified environment.
 
         Args:
           environment_id: unique ID associated with target environment. Format:
             projects/<Project ID>/locations/<Location ID>/agents/
             <Agent ID>/environments/<Environment ID>.
 
@@ -409,15 +416,16 @@
         history = []
         for page in response.pages:
             for environment in page.environments:
                 history.append(environment)
 
         return history
 
-    def list_continuous_test_results(self, environment_id:str):
+    @scrapi_base.api_call_counter_decorator
+    def list_continuous_test_results(self, environment_id: str):
         """Fetches a list of continuous test results for a given environment.
 
         Args:
           environment_id: unique ID associated with target environment. Format:
             projects/<Project ID>/locations/<Location ID>/agents/
             <Agent ID>/environments/<Environment ID>.
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/changelogs.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/changelogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 
 from typing import Dict
 
 import pandas as pd
 
 from google.cloud.dialogflowcx_v3beta1 import services
 from google.cloud.dialogflowcx_v3beta1 import types
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+from dfcx_scrapi.core import scrapi_base
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
-class Changelogs(ScrapiBase):
+class Changelogs(scrapi_base.ScrapiBase):
     """Tools class that contains methods to support Change History feature."""
 
     def __init__(
         self,
         creds_path: str = None,
         creds_dict: Dict = None,
         creds=None,
@@ -72,14 +72,15 @@
             datetime.datetime.fromtimestamp(int(create_time_epoch_seconds))
         except ValueError as err:
             print("Create Time should be valid Unix Timestamp")
             raise ValueError from err
         else:
             return True
 
+    @scrapi_base.api_call_counter_decorator
     def list_changelogs(self, agent_id: str = None, **kwargs):
         """Lists all Change History logs for a CX Agent.
 
         This method supports log filtering via **kwargs input. The filters
         currently supported are: user_email, resource, display_name, type,
         action, and create_time.
         See https://github.com/googleapis/python-dialogflow-cx/blob/main/
@@ -143,14 +144,15 @@
         changelogs = []
         for page in response.pages:
             for log in page.changelogs:
                 changelogs.append(log)
 
         return changelogs
 
+    @scrapi_base.api_call_counter_decorator
     def get_changelog(self, changelog_id: str):
         """Get a single changelog resource object.
 
         Args:
           changelog_id: The ID of the changelog to get. Format: `projects/
             <Project ID>/locations/<Location ID>/agents/<Agent ID>/changelogs/
             <Changelog ID>`
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/flows.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/flows.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,14 +125,15 @@
             flows_dict = {
                 flow.name: flow.display_name
                 for flow in self.list_flows(agent_id=agent_id)
             }
 
         return flows_dict
 
+    @scrapi_base.api_call_counter_decorator
     def train_flow(self, flow_id: str) -> str:
         """Trains the specified flow.
 
         Args:
           flow_id: CX flow ID string in the following format
             projects/<PROJECT ID>/locations/<LOCATION ID>/agents/<AGENT ID>/
               flows/<FLOW ID>
@@ -151,14 +152,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.train_flow(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def list_flows(self, agent_id: str) -> List[types.Flow]:
         """Get a List of all Flows in the current Agent.
 
         Args:
           agent_id: CX Agent ID string in the proper format
             projects/<PROJECT ID>/locations/<LOCATION ID>/agents/<AGENT ID>
 
@@ -204,14 +206,15 @@
                 f"does not exist in the specified agent."
             )
 
         flow = self.get_flow(flow_id=flow_id)
 
         return flow
 
+    @scrapi_base.api_call_counter_decorator
     def get_flow(self, flow_id: str) -> types.Flow:
         """Get a single CX Flow object.
 
         Args:
           flow_id: CX Flow ID in the proper format
 
         Returns:
@@ -222,14 +225,15 @@
         client = services.flows.FlowsClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.get_flow(name=flow_id)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_flow(
         self,
         agent_id: str,
         display_name: str = None,
         language_code: str = "en",
         obj: types.Flow = None,
         **kwargs,
@@ -270,14 +274,15 @@
         client = services.flows.FlowsClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.create_flow(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def update_flow(
         self, flow_id: str, obj: types.Flow = None, **kwargs
     ) -> types.Flow:
         """Update a single specific CX Flow object.
 
         Args:
           flow_id: CX Flow ID in the proper format
@@ -321,14 +326,15 @@
 
         flow = self.get_flow(flow_id)
         current_settings = flow.nlu_settings
         for key, value in kwargs.items():
             setattr(current_settings, key, value)
         self.update_flow(flow_id=flow_id, nlu_settings=current_settings)
 
+    @scrapi_base.api_call_counter_decorator
     def export_flow(
         self, flow_id: str, gcs_path: str, ref_flows: bool = True
     ) -> Dict[str, str]:
         """Exports DFCX Flow(s) into GCS bucket.
 
         Args:
           flow_id: the formatted CX Flow ID to export
@@ -351,14 +357,15 @@
         client = services.flows.FlowsClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.export_flow(request)
 
         return response.result()
 
+    @scrapi_base.api_call_counter_decorator
     def export_flow_inline(self, flow_id: str, ref_flows: bool = True) -> bytes:
         """Export a Flow, returning uncompressed raw byte content for flow.
 
         Args:
           flow_id: the formatted CX Flow ID to export
           ref_flows: Whether to export flows referenced by the specified flow.
 
@@ -373,14 +380,15 @@
         client = services.flows.FlowsClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.export_flow(request)
 
         return (response.result()).flow_content
 
+    @scrapi_base.api_call_counter_decorator
     def import_flow(
         self,
         agent_id: str,
         gcs_path: str = None,
         flow_content: bytes = None,
         import_option: str = "KEEP",
     ) -> Dict[str, str]:
@@ -421,14 +429,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.import_flow(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def delete_flow(self, flow_id: str, force: bool = False):
         """Deletes a single CX Flow Object resource.
 
         Args:
           flow_id: flow to delete
           force: False means a flow will not be deleted if a route to the flow
             exists, True means the flow will be deleted as well as all the
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/versions.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             creds_dict=creds_dict,
             creds=creds,
         )
 
         if flow_id:
             self.flow_id = flow_id
 
+    @scrapi_base.api_call_counter_decorator
     def list_versions(self, flow_id:str):
         """List all Versions for a given Flow.
 
         Args:
           flow_id: Required. The targeted flow for the operation. Format:
             projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>
               /flows/<Flow ID>
@@ -75,14 +76,15 @@
         versions = []
         for page in response.pages:
             for version in page.versions:
                 versions.append(version)
 
         return versions
 
+    @scrapi_base.api_call_counter_decorator
     def get_version(
         self,
         version_id:str=None,
         display_name:str=None,
         flow_id:str=None):
         """Get Version object for specific version.
 
@@ -136,14 +138,15 @@
         versions_list = self.list_versions(flow_id)
         for version_obj in versions_list:
             if version_obj.display_name == display_name:
                 return version_obj
 
         return None
 
+    @scrapi_base.api_call_counter_decorator
     def load_version(
         self,
         version:types.version.Version,
         allow_override:bool = False,
         flow_id:str = None):
         """Switch a flow to the specified version.
 
@@ -172,14 +175,15 @@
         client = services.versions.VersionsClient(
             client_options=client_options, credentials=self.creds
         )
 
         response = client.load_version(request)
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_version(
         self,
         flow_id:str,
         display_name:str,
         description:str=None):
         """Create a Version for the specified Flow ID.
 
@@ -208,14 +212,15 @@
         request.parent = flow_id
         request.version = version
 
         response = client.create_version(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def delete_version(self, version_id:str):
         """Delete a specified Version.
 
         Args:
           version_name: Unique Version ID of the target to delete. Format:
             projects/<Project ID>/locations/<Location ID>/agents/
             <Agent ID>/flows/<Flow ID>/versions/<Version ID>
@@ -225,14 +230,15 @@
         client = services.versions.VersionsClient(
             client_options=self._set_region(version_id),
             credentials=self.creds
         )
 
         return client.delete_version(request)
 
+    @scrapi_base.api_call_counter_decorator
     def compare_versions(
         self,
         base_version_id:str,
         target_version_id:str,
         flow_id:str = None):
         """Compares the specified base version with target version.
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/webhooks.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/webhooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,14 +84,15 @@
                 webhook.name: webhook.display_name
                 for webhook in self.list_webhooks(agent_id)
             }
 
         return webhooks_dict
 
 
+    @scrapi_base.api_call_counter_decorator
     def list_webhooks(self, agent_id: str = None):
         """List all Webhooks in the specified CX Agent.
 
         Args:
           agent_id: the formated CX Agent ID to use
 
         Returns:
@@ -112,14 +113,15 @@
         cx_webhooks = []
         for page in response.pages:
             for cx_webhook in page.webhooks:
                 cx_webhooks.append(cx_webhook)
 
         return cx_webhooks
 
+    @scrapi_base.api_call_counter_decorator
     def create_webhook(
         self,
         agent_id: str,
         obj: types.Webhook = None,
         **kwargs):
         """Create a single webhook resource on a given CX Agent.
 
@@ -145,14 +147,15 @@
         client = services.webhooks.WebhooksClient(
             client_options=client_options, credentials=self.creds)
         response = client.create_webhook(parent=agent_id, webhook=webhook)
 
         return response
 
 
+    @scrapi_base.api_call_counter_decorator
     def get_webhook(self, webhook_id:str):
         """Retrieves the specified webhook.
 
         Args:
           webhook_id: The ID of the webhook. Format:
             projects/<Project ID>/locations/<Location ID>/agents/
             <Agent ID>/webhooks/<Webhook
@@ -198,14 +201,15 @@
                 f"Webhook \"{webhook_display_name}\" does not exist in the \
                     specified Agent."
                 )
 
         return webhook_obj
 
 
+    @scrapi_base.api_call_counter_decorator
     def update_webhook(
         self,
         webhook_id:str,
         webhook_obj:types.Webhook = None,
         **kwargs):
         """Update the values of an existing webhook.
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/session_entity_types.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/session_entity_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,15 @@
             ent.synonyms = v
             entity_list.append(ent)
 
         st.entities = entity_list
 
         return st
 
+    @scrapi_base.api_call_counter_decorator
     def list_session_entity_types(
         self, session_id: str, environment_id: str = None
     ) -> List[types.SessionEntityType]:
         """Lists all Session Entities currently active in the Session.
 
         Args:
           session_id, The session to list all session entity types from.
@@ -232,14 +233,15 @@
         for page in response.pages:
             print(page)
             # for entity in page.entity_types:
             #     session_entities.append(entity)
 
         return session_entities
 
+    @scrapi_base.api_call_counter_decorator
     def get_session_entity_type(
         self, session_entity_type_id: str, environment_id: str = None
     ) -> types.SessionEntityType:
         """Retrieves the specified Session Entity Type.
 
         Args:
           session_entity_type_id, The Session Entity Type ID to retrieve.
@@ -268,14 +270,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.get_session_entity_type(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_session_entity_type(
         self, session_id: str, session_entity_type: types.SessionEntityType
     ) -> types.SessionEntityType:
         """Creates a Session Entity Type object from provided inputs.
         Args:
           session_id, The session to list all session entity types from.
             Format:
@@ -295,14 +298,15 @@
             credentials=self.creds, client_options=client_options
         )
 
         response = client.create_session_entity_type(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def update_session_entity_type(
         self,
         session_entity_type_id: str,
         environment_id: str = None,
         obj: types.SessionEntityType = None,
         **kwargs,
     ) -> types.SessionEntityType:
@@ -357,14 +361,15 @@
         request.session_entity_type = parent_id
         request.update_mask = mask
 
         response = client.update_session_entity_type(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def delete_session_entity_type(
         self, session_entity_type_id: str, environment_id: str = None
     ) -> str:
         """Deletes the specified Session Entity Type.
 
         Args:
           session_entity_type_id, the ID of the Session Entity Type to update
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/test_cases.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/test_cases.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 import logging
 from typing import Dict, List
 
 from google.cloud.dialogflowcx_v3beta1 import services
 from google.cloud.dialogflowcx_v3beta1 import types
 from google.protobuf import field_mask_pb2
 
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+from dfcx_scrapi.core import scrapi_base
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
-class TestCases(ScrapiBase):
+class TestCases(scrapi_base.ScrapiBase):
     """Core Class for CX Test Cases."""
 
     def __init__(
         self,
         creds_path: str = None,
         creds_dict: Dict = None,
         creds=None,
@@ -55,30 +55,42 @@
             self.agent_id = agent_id
             self.client_options = self._set_region(self.agent_id)
 
         if test_case_id:
             self.test_case_id = test_case_id
             self.client_options = self._set_region(self.test_case_id)
 
-    def list_test_cases(self, agent_id: str = None):
+    @scrapi_base.api_call_counter_decorator
+    def list_test_cases(
+        self, agent_id: str = None, include_conversation_turns: bool = False
+    ):
         """List test cases from an agent.
 
         Args:
-          agent_id: The agent to list all pages for.
+          agent_id: The agent to list all test cases for.
             `projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>`
+          include_conversation_turns: Either to include the conversation turns
+            in the test cases or not. Default is False
+            which shows only the basic metadata about the test cases.
 
         Returns:
           List of test cases from an agent.
         """
 
         if not agent_id:
             agent_id = self.agent_id
 
-        request = types.test_case.ListTestCasesRequest()
-        request.parent = agent_id
+        if include_conversation_turns:
+            test_case_view = types.ListTestCasesRequest.TestCaseView.FULL
+        else:
+            test_case_view = types.ListTestCasesRequest.TestCaseView.BASIC
+
+        request = types.test_case.ListTestCasesRequest(
+            parent=agent_id, view=test_case_view
+        )
 
         client_options = self._set_region(agent_id)
 
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
 
@@ -87,14 +99,15 @@
         test_cases = []
         for page in response.pages:
             for test_case in page.test_cases:
                 test_cases.append(test_case)
 
         return test_cases
 
+    @scrapi_base.api_call_counter_decorator
     def export_test_cases(
         self,
         gcs_uri: str,
         agent_id: str = None,
         data_format: str = None,
         data_filter: str = None,
     ):
@@ -133,14 +146,15 @@
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.export_test_cases(request)
 
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def create_test_case(self, test_case: types.TestCase, agent_id: str = None):
         """Create a new Test Case in the specified CX Agent.
 
         Args:
           test_case: The test case to create.
           agent_id: The agent to create the test case for. Format:
               `projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>`
@@ -158,14 +172,15 @@
         client_options = self._set_region(agent_id)
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.create_test_case(request)
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def get_test_case(self, test_case_id: str):
         """Get test case object from CX Agent.
 
         Args:
           test_case_id: The name of the test case. Format:
             `projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>/
               testCases/<TestCase ID>`
@@ -180,14 +195,15 @@
         client_options = self._set_region(test_case_id)
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.get_test_case(request)
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def import_test_cases(self, gcs_uri: str, agent_id: str = None):
         """Import test cases from cloud storage.
 
         Args:
           gcs_uri: The GCS URI to import test cases from. The format of this
             URI must be `gs://<bucket-name>/<object-name>`
           agent_id: The agent to import test cases to. Format:
@@ -208,14 +224,15 @@
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.import_test_cases(request)
         result = response.result()
         return result
 
+    @scrapi_base.api_call_counter_decorator
     def batch_delete_test_cases(
         self,
         test_case_ids: List[str],
         agent_id: str = None):
         """Delete a set of test cases from an agent.
 
         Args:
@@ -238,14 +255,15 @@
 
         client_options = self._set_region(agent_id)
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         client.batch_delete_test_cases(request)
 
+    @scrapi_base.api_call_counter_decorator
     def list_test_case_results(self, test_case_id: str):
         """List the results from a specific Test Case.
 
         Args:
           test_case_id: The test case to list results for. Format:
             `projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>/
               testCases/<TestCase ID>`
@@ -268,14 +286,15 @@
         test_case_results = []
         for page in response.pages:
             for result in page.test_case_results:
                 test_case_results.append(result)
 
         return test_case_results
 
+    @scrapi_base.api_call_counter_decorator
     def batch_run_test_cases(
         self,
         test_cases: List[str],
         agent_id: str = None,
         environment: str = None):
         """Run a set of test cases to get their latest results.
 
@@ -305,14 +324,15 @@
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.batch_run_test_cases(request)
         results = response.result()
         return results
 
+    @scrapi_base.api_call_counter_decorator
     def update_test_case(
         self,
         test_case_id: str = None,
         obj: types.TestCase = None,
         **kwargs) -> types.TestCase:
         """Update Test Case attributes for a specified Test Case.
 
@@ -344,14 +364,15 @@
         client_options = self._set_region(test_case_id)
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.update_test_case(request)
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def run_test_case(self, test_case_id: str, environment: str = None):
         """Run test case and get result for a specified test case.
 
         Args:
           test_case_id: Test Case ID in the following format:
             `projects/<Project ID>/locations/ <Location ID>/agents/<AgentID>/
               testCases/<TestCase ID>`
@@ -371,14 +392,15 @@
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.run_test_case(request)
         results = response.result()
         return results
 
+    @scrapi_base.api_call_counter_decorator
     def get_test_case_result(self, test_case_result_id: str):
         """Get test case result for a specified run on a specified test case.
 
         Args:
           test_case_result_id: The Test Case Result ID to retrieve.
             projects/<Project ID>/locations/<Location ID>/agents/<Agent ID>/
               testCases/<TestCase ID>/results/<TestCaseResult ID>
@@ -392,14 +414,15 @@
         client_options = self._set_region(test_case_result_id)
         client = services.test_cases.TestCasesClient(
             credentials=self.creds, client_options=client_options
         )
         response = client.get_test_case_result(request)
         return response
 
+    @scrapi_base.api_call_counter_decorator
     def calculate_coverage(self, coverage_type: int, agent_id: str = None):
         """Calculate coverage of different resources in the test case set.
 
         Args:
           coverage_type: The type of coverage requested.
             INTENT = 1
             PAGE_TRANSITION = 2
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/project.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import time
 from typing import Dict
 
-from dfcx_scrapi.core.scrapi_base import ScrapiBase
+from dfcx_scrapi.core import scrapi_base
 from dfcx_scrapi.core.agents import Agents
 
 # logging config
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(levelname)-8s %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
-class Project(ScrapiBase):
+class Project(scrapi_base.ScrapiBase):
     """Top Level class representing the Project level resources
     when working on a Dialogflow CX project. This Class will allow you to
     extract information about your GCP project as a whole in relation to
     your CX agents.
     """
     def __init__(
         self,
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/builders_common.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/builders_common.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/transition_route_groups.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/transition_route_groups.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/intents.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/intents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/fulfillments.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/fulfillments.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/entity_types.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/entity_types.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/agents.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/agents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/pages.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/pages.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/flows.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/flows.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/response_messages.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/response_messages.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/routes.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/builders/routes.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/utterance_generator.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_ml/utterance_generator.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/test_cases.py` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi/core_async/test_cases.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/agent_assist/agent_assist.py` & `dfcx-scrapi-1.7.0/src/agent_assist/agent_assist.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/PKG-INFO` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcx-scrapi
-Version: 1.6.3
+Version: 1.7.0
 Summary: A high level scripting API for bot builders, developers, and      maintainers.
 Home-page: https://github.com/GoogleCloudPlatform/dfcx-scrapi
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,intent,dfcx,entity
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.6.3 Summary: A high level
+Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.7.0 Summary: A high level
 scripting API for bot builders, developers, and maintainers. Home-page: https:/
 /github.com/GoogleCloudPlatform/dfcx-scrapi Author: Patrick Marlow Author-
 email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,intent,dfcx,entity Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

### Comparing `dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/SOURCES.txt` & `dfcx-scrapi-1.7.0/src/dfcx_scrapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

