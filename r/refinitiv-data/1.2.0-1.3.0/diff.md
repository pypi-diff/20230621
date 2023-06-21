# Comparing `tmp/refinitiv-data-1.2.0.tar.gz` & `tmp/refinitiv-data-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refinitiv-data-1.2.0.tar", last modified: Tue May  2 10:11:28 2023, max compression
+gzip compressed data, was "refinitiv-data-1.3.0.tar", last modified: Wed Jun 21 15:15:09 2023, max compression
```

## Comparing `refinitiv-data-1.2.0.tar` & `refinitiv-data-1.3.0.tar`

### file list

```diff
@@ -1,1033 +1,1040 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.921840 refinitiv-data-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     9338 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9778 2023-05-02 10:11:28.921840 refinitiv-data-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9061 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.797839 refinitiv-data-1.2.0/changes/
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/changes/template.jinja
--rw-rw-rw-   0 root         (0) root         (0)    21868 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/python
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.797839 refinitiv-data-1.2.0/refinitiv/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.797839 refinitiv-data-1.2.0/refinitiv/data/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)    16562 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_config_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_config_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    15270 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_configure.py
--rw-rw-rw-   0 root         (0) root         (0)     4036 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_content_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.797839 refinitiv-data-1.2.0/refinitiv/data/_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1810 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/log_reporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.801840 refinitiv-data-1.2.0/refinitiv/data/_core/session/
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_dacs_params.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_default_session_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4908 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_desktop_session.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_platform_session.py
--rw-rw-rw-   0 root         (0) root         (0)    11808 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_retry_transport.py
--rw-rw-rw-   0 root         (0) root         (0)    14681 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_cxn_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_cxn_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10054 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_provider.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3632 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/access_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/auth_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    10563 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/event.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/event_code.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/global_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/grant_password.py
--rw-rw-rw-   0 root         (0) root         (0)    12612 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/http_service.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/null_session.py
--rw-rw-rw-   0 root         (0) root         (0)     4281 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/refresh_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3990 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_core/session/updater.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.801840 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.801840 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    26229 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11923 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     7238 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py
--rw-rw-rw-   0 root         (0) root         (0)     5845 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.805840 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5334 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_containers.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_data_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12224 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4588 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_history_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1500 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_intervals_consts.py
--rw-rw-rw-   0 root         (0) root         (0)     4195 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_mixed_streams.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_ohlc_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_pricing_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)     5290 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_recording_control.py
--rw-rw-rw-   0 root         (0) root         (0)     3110 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_stream_update_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.805840 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2993 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_context.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4950 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.805840 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2482 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     3621 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)     4581 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py
--rw-rw-rw-   0 root         (0) root         (0)     3836 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/get_data_func.py
--rw-rw-rw-   0 root         (0) root         (0)     7418 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/get_history_func.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/get_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.805840 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/news/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/news/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/session.py
--rw-rw-rw-   0 root         (0) root         (0)    12927 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_log.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_open_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.809840 refinitiv-data-1.2.0/refinitiv/data/_qpl/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_bid_ask.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_fx_spot_quote.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_fx_swap_points.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_fx_swp_to_swp.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_tenor_bid_ask.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_qpl/_tenor_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.809840 refinitiv-data-1.2.0/refinitiv/data/_tools/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_common.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6623 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)     4171 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_datetime.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_debug.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_params.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_patterns.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_repr.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_specification.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5257 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_tools/templates.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/_types.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-02 10:11:28.000000 refinitiv-data-1.2.0/refinitiv/data/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.813840 refinitiv-data-1.2.0/refinitiv/data/content/
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_content_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_content_data_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_content_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_content_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_content_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_df_build_type.py
--rw-rw-rw-   0 root         (0) root         (0)    17783 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     8514 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_df_builder_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    18264 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_entire_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_error_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_historical_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     6441 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_historical_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6937 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_historical_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_historical_raw_transf.py
--rw-rw-rw-   0 root         (0) root         (0)     3209 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_historical_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3064 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_intervals.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_universe_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     8436 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_universe_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    18431 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/_universe_streams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.813840 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15389 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     6061 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_instrument_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12907 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    18090 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_manage.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_search.py
--rw-rw-rw-   0 root         (0) root         (0)     8665 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_stream_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_summaries.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/events.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/manage.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/search.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/summaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.817840 refinitiv-data-1.2.0/refinitiv/data/content/esg/
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_base_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1785 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_basic_overview_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_esg_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_full_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_full_scores_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_standard_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_standard_scores_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/_universe_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/basic_overview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.817840 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     9784 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_db_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7363 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_file_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3264 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_package_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_package_manager_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/full_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/full_scores.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/standard_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/standard_scores.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/esg/universe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.817840 refinitiv-data-1.2.0/refinitiv/data/content/estimates/
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/_enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.817840 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.821840 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.821840 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2369 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2327 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2218 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2248 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2198 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/annual.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_non_periodic_measures.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_annual.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_interim.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_recommendations.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/interim.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/non_periodic_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/recommendations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.821840 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1785 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/historical_snapshots_kpi.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.825840 refinitiv-data-1.2.0/refinitiv/data/content/filings/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/_feed_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4584 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/_filing_query.py
--rw-rw-rw-   0 root         (0) root         (0)    20076 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/_retrieval_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/_retrieval_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8827 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/_search_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4866 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/_search_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/retrieval.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/filings/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.825840 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3970 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    10662 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2746 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.825840 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_events_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3471 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_summaries_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/events.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/summaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.825840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5727 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_content_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.829840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.829840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.829840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)    11462 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    28196 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.833840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_basis_spline_smooth_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calendar_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calibration_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py
--rw-rw-rw-   0 root         (0) root         (0)     8933 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_issuer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating_scale_source.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_reference_entity_type.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_seniority.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.833840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.833840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4482 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     9677 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.837840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_risk_type.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_constituent_override_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_type.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     1356 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5766 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     3719 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7749 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     6772 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     4477 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.837840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py
--rw-rw-rw-   0 root         (0) root         (0)     3593 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3716 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_quotation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_standard_turn_period.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2164 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py
--rw-rw-rw-   0 root         (0) root         (0)     3621 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7044 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2871 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8742 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_risk_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.841840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     8503 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_curves_builder_df.py
--rw-rw-rw-   0 root         (0) root         (0)    22286 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_curves_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.845840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_calendar_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_compounding_type.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_constituent_override_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_forward_curves_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_market_data_access_denied_fallback.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_swap_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_zc_curves_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2774 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3441 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_forward_curve_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.845840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_convexity.py
--rw-rw-rw-   0 root         (0) root         (0)     3881 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_curve.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_curve_point.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)    13718 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_turn.py
--rw-rw-rw-   0 root         (0) root         (0)     3014 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_shift_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)    10434 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    19745 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4204 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12838 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    19456 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2988 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.857840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/
--rw-rw-rw-   0 root         (0) root         (0)     3130 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_adjust_interest_to_payment_date.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_american_monte_carlo_method.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_amortization_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_amortization_type.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_average_type.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_axis.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_barrier_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_barrier_style.py
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_barrier_type.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_benchmark_yield_selection_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_buy_sell.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_calibration_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_call_put.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_cds_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_common_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_credit_spread_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_dates_calendars_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_day_of_week.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_direction.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_discounting_type.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_dividend_extrapolation.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_dividend_type.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_doc_clause.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_double_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_end_of_month_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_equity_dividend_type.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_eti_input_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_exercise_schedule_type.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_exercise_style.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_extrapolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_fixing_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_format.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_forward_compute_method.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_forward_extrapolation.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_funding_spread_method.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_fx_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_fx_cross_type.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_fx_leg_type.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_fx_volatility_model.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_implied_deposit_date_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_in_or_out.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_average_method.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_integration_method.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_method.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_type.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_observation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_reset_type.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_spread_compounding_method.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_inflation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_input_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_interest_calculation_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_interest_type.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_local_volatility_method.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_method.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_notional_exchange.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_numeraire_type.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_option_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_period_type.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_premium_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_pricing_model_type.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_projected_index_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_repo_curve_type.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_risk_type.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_rounding.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_rounding_type.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_seniority.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_stub_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_swaption_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_swaption_type.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_swaption_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_tenor_reference_date.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_time_stamp.py
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_underlying_type.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_up_or_down.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_vol_type.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_volatility_adjustment_type.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_volatility_model.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_volatility_term_structure_type.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_yield_type.py
--rw-rw-rw-   0 root         (0) root         (0)    10539 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_ipa_content_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_ipa_content_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.861840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3841 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_amortization_item.py
--rw-rw-rw-   0 root         (0) root         (0)     2188 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_basket_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py
--rw-rw-rw-   0 root         (0) root         (0)     5046 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_day_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_fx_point.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_input_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_numerical_method.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_payout_scaling.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_pde_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     4393 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_object_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.861840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.861840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_enums/_calibration_type.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_enums/_moneyness_type.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_enums/_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_enums/_strike_type.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_enums/_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8965 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    13475 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9532 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     1214 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2290 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_surface.py
--rw-rw-rw-   0 root         (0) root         (0)     6749 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_point.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_surface_types.py
--rw-rw-rw-   0 root         (0) root         (0)    11119 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    14375 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1853 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_bond_curves/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_bond_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2737 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_arg_enums.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_base_data_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3000 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/
--rw-rw-rw-   0 root         (0) root         (0)     2037 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7302 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    11268 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/manage.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5917 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.865840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/forward_curves/
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6123 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curves/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    10019 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8278 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     1860 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)      933 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7269 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py
--rw-rw-rw-   0 root         (0) root         (0)     3486 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6928 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.869840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_base_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8331 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     3615 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.873840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22906 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    90430 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    14567 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.873840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22163 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7581 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    12450 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.873840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12059 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7555 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     7021 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    13621 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9673 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.873840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6350 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7306 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10144 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.877840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/
--rw-rw-rw-   0 root         (0) root         (0)     2174 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.877840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_base/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_info.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_underlying_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9594 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.877840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_double_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_underlying_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.877840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    13901 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4699 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.881840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4219 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    17171 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2164 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3848 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4114 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3673 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    30468 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.881840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5782 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8053 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4865 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     4384 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2984 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py
--rw-rw-rw-   0 root         (0) root         (0)     4900 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.881840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5213 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    35752 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     9941 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.881840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    11982 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.881840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7211 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    12318 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.881840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.885840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/cap/
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2921 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.885840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/eti/
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2628 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.885840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/fx/
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.885840 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/swaption/
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2994 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.885840 refinitiv-data-1.2.0/refinitiv/data/content/news/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/_content_validator_udf.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/_news_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/_news_data_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)     3276 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/_urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.885840 refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3216 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5481 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4929 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_sort_order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.885840 refinitiv-data-1.2.0/refinitiv/data/content/news/images/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/images/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/images/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/images/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2821 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/images/_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.889840 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_image_data.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_news_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.889840 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.889840 refinitiv-data-1.2.0/refinitiv/data/content/news/story/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3375 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/_data.py
--rw-rw-rw-   0 root         (0) root         (0)      788 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/_response.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/story/_udf_html_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.889840 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_top_news_headline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.889840 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_subcategory.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_top_news_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.893840 refinitiv-data-1.2.0/refinitiv/data/content/ownership/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/_org_info_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3986 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/_ownership_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.893840 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/breakdown.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/concentration.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/investors.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/recent_activity.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/shareholders_history_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/top_n_concentration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.897840 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_breakdown_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1771 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_holdings_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_investors_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3197 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/breakdown.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/concentration.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/holdings.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/investors.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/recent_activity.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/shareholders_history_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/top_n_concentration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.897840 refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2140 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3238 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/transaction_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.897840 refinitiv-data-1.2.0/refinitiv/data/content/ownership/investor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/investor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/investor/_holdings_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/investor/holdings.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/ownership/org_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.897840 refinitiv-data-1.2.0/refinitiv/data/content/pricing/
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5313 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/_pricing_content_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    18330 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.897840 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8116 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_chain_record.py
--rw-rw-rw-   0 root         (0) root         (0)     5139 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_chain_records.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    55563 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_display_template.py
--rw-rw-rw-   0 root         (0) root         (0)     8373 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     4789 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.901840 refinitiv-data-1.2.0/refinitiv/data/content/search/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11914 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/_lookup_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/_metadata_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/_views.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/lookup.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/search/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.901840 refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_asset_state.py
--rw-rw-rw-   0 root         (0) root         (0)     4444 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_country_code.py
--rw-rw-rw-   0 root         (0) root         (0)     7435 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_symbol_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.901840 refinitiv-data-1.2.0/refinitiv/data/content/trade_data_service/
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/trade_data_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/trade_data_service/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/trade_data_service/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    10810 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/content/trade_data_service/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.901840 refinitiv-data-1.2.0/refinitiv/data/delivery/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.905840 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_api_type.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3271 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    27039 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_provider_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5729 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_type.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_endpoint_data.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     5820 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_endpoint_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_parsed_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_raw_data_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5778 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3617 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_validators.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_dictionary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.909840 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11380 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_protocol_type.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_rdp_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    10068 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5401 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11913 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    11475 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     9547 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_listener.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/base_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.909840 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5529 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_offstream.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_response.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.909840 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14002 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_dictionary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_field_description.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     6746 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     9328 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    15911 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     6952 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/omm_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2773 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/omm_stream_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3929 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/proxy_info.py
--rw-rw-rw-   0 root         (0) root         (0)    10724 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rdp_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     3085 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.909840 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     5403 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/ema.py
--rw-rw-rw-   0 root         (0) root         (0)     9451 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/socket.py
--rw-rw-rw-   0 root         (0) root         (0)     4741 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream.py
--rw-rw-rw-   0 root         (0) root         (0)     4073 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    16405 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_cxn_state.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_state.py
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_state_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.909840 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/ws/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/ws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/ws/ws_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.913840 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3519 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_buckets_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_data_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1276 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_data_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_file_downloader_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     4471 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_file_sets_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2280 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_files_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4204 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_iter_object.py
--rw-rw-rw-   0 root         (0) root         (0)     3033 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_packages_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_unpacker.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/buckets.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/file_sets.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/files.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/packages.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/endpoint_request.py
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/delivery/rdp_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.913840 refinitiv-data-1.2.0/refinitiv/data/discovery/
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2471 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_convert_symbols.py
--rw-rw-rw-   0 root         (0) root         (0)     2803 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.913840 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_explorer/
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_explorer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11534 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_explorer/_dataclasses.py
--rw-rw-rw-   0 root         (0) root         (0)     8350 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_explorer/_search_explorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.913840 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12658 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8134 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/embedded.py
--rw-rw-rw-   0 root         (0) root         (0)     5282 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/manage.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/search.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.917840 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_customers.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_fetch_data.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_relationship_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_suppliers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.917840 refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_peers.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_screener.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_universe_expander.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.917840 refinitiv-data-1.2.0/refinitiv/data/early_access/
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/early_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.917840 refinitiv-data-1.2.0/refinitiv/data/early_access/discovery/
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/early_access/discovery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.917840 refinitiv-data-1.2.0/refinitiv/data/eikon/
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9549 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_data_grid.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_json_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     7401 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_news_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_streaming_prices.py
--rw-rw-rw-   0 root         (0) root         (0)     5234 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_symbology.py
--rw-rw-rw-   0 root         (0) root         (0)    13670 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     4829 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/eikon/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.917840 refinitiv-data-1.2.0/refinitiv/data/session/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/session/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/session/desktop.py
--rw-rw-rw-   0 root         (0) root         (0)     3850 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/session/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.921840 refinitiv-data-1.2.0/refinitiv/data/usage_collection/
--rw-rw-rw-   0 root         (0) root         (0)      359 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/usage_collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/usage_collection/_abstract_logger.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/usage_collection/_filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/usage_collection/_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/usage_collection/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-02 10:11:11.000000 refinitiv-data-1.2.0/refinitiv/data/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:11:28.921840 refinitiv-data-1.2.0/refinitiv_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9778 2023-05-02 10:11:28.000000 refinitiv-data-1.2.0/refinitiv_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    55166 2023-05-02 10:11:28.000000 refinitiv-data-1.2.0/refinitiv_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 10:11:28.000000 refinitiv-data-1.2.0/refinitiv_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-02 10:11:28.000000 refinitiv-data-1.2.0/refinitiv_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-02 10:11:28.000000 refinitiv-data-1.2.0/refinitiv_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 10:11:28.921840 refinitiv-data-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11615 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.650218 refinitiv-data-1.3.0/changes/
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/changes/template.jinja
+-rw-rw-rw-   0 root         (0) root         (0)    21868 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.650218 refinitiv-data-1.3.0/refinitiv/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.658218 refinitiv-data-1.3.0/refinitiv/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)    16816 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_config_defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_config_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15270 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     4036 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_content_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.658218 refinitiv-data-1.3.0/refinitiv/data/_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/log_reporter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.670218 refinitiv-data-1.3.0/refinitiv/data/_core/session/
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_dacs_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_default_session_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5004 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_desktop_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     9961 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_platform_session.py
+-rw-rw-rw-   0 root         (0) root         (0)    11808 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_retry_transport.py
+-rw-rw-rw-   0 root         (0) root         (0)    15808 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_cxn_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_cxn_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10130 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/_user_uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/access_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/auth_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    10563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/event_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/global_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/grant_password.py
+-rw-rw-rw-   0 root         (0) root         (0)    12676 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/http_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/null_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4281 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/refresh_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3990 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_core/session/updater.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.670218 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.670218 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    26229 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11923 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     7238 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     5845 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.678218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5350 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12224 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4588 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_intervals_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3454 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_mixed_streams.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_ohlc_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_pricing_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_recording_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     3110 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_stream_update_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.682218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4950 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.682218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2482 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_data_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     7418 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_history_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.682218 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    12912 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_open_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.686218 refinitiv-data-1.3.0/refinitiv/data/_qpl/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_bid_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_spot_quote.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swap_points.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swp_to_swp.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_tenor_bid_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_qpl/_tenor_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.690218 refinitiv-data-1.3.0/refinitiv/data/_tools/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6623 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)     4708 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_patterns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_repr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_specification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5257 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_tools/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/_types.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv/data/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.698217 refinitiv-data-1.3.0/refinitiv/data/content/
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_data_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_content_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_df_build_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    18497 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_df_builder_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    18264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_entire_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_error_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6441 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6937 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_raw_transf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3209 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_historical_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_intervals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_universe_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8436 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_universe_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    18431 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/_universe_streams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.706218 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14446 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     6061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12895 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    18090 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     8665 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_stream_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_summaries.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/search.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/summaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.710218 refinitiv-data-1.3.0/refinitiv/data/content/esg/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_base_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_basic_overview_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_esg_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_full_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_full_scores_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_standard_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1652 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_standard_scores_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/_universe_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/basic_overview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.710218 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9784 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_db_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7363 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_package_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_package_manager_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/full_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/full_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/standard_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/standard_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/esg/universe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.714218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/_enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.714218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.714218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.718217 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2150 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_non_periodic_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_annual.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_interim.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_recommendations.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/interim.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/non_periodic_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/recommendations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.722218 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/historical_snapshots_kpi.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.726218 refinitiv-data-1.3.0/refinitiv/data/content/filings/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_feed_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_filing_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    20076 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8827 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4866 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/retrieval.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/filings/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.726218 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3970 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    10662 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2746 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.730218 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_events_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3471 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_summaries_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/summaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.730218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5727 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_content_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.738217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.738217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.742218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)    11462 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    28240 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.746218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_basis_spline_smooth_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calendar_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calibration_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py
+-rw-rw-rw-   0 root         (0) root         (0)     8933 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_issuer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating_scale_source.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_reference_entity_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_seniority.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.746218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.754217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4482 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     9677 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.754217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_risk_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_constituent_override_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5860 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     3719 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7749 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     6772 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     4477 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     3593 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3767 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.762218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_quotation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_standard_turn_period.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7044 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8798 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_risk_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.766218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    21263 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_curves_builder_df.py
+-rw-rw-rw-   0 root         (0) root         (0)    10677 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_curves_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.770218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_calendar_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_compounding_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_constituent_override_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_forward_curves_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_market_data_access_denied_fallback.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_swap_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_zc_curves_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2832 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3441 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.774217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_convexity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_curve.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_curve_point.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)    13718 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_turn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_shift_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)    10434 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    19827 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12838 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    19563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.794217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_adjust_interest_to_payment_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_american_monte_carlo_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_amortization_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_amortization_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_average_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_axis.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_barrier_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_barrier_style.py
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_barrier_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_benchmark_yield_selection_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_buy_sell.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_calibration_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_call_put.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_cds_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_common_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_credit_spread_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_dates_calendars_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_of_week.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_direction.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_discounting_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_dividend_extrapolation.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_dividend_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_doc_clause.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_double_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_end_of_month_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_equity_dividend_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_eti_input_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_exercise_schedule_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_exercise_style.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_extrapolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fixing_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_format.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_forward_compute_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_forward_extrapolation.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_funding_spread_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_cross_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_leg_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_volatility_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_implied_deposit_date_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_in_or_out.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_average_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_integration_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_observation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_reset_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_spread_compounding_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_inflation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_input_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_interest_calculation_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_interest_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_local_volatility_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_notional_exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_numeraire_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_option_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_period_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_premium_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_pricing_model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_projected_index_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_repo_curve_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_risk_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_rounding.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_rounding_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_seniority.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_stub_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_swaption_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_swaption_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_swaption_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_tenor_reference_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_time_stamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_underlying_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_up_or_down.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_vol_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_adjustment_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_term_structure_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_yield_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    10539 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.798217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_amortization_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     2188 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_basket_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_day_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_fx_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_input_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_numerical_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_payout_scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_pde_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_object_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.806218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.806218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_calibration_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_moneyness_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_strike_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_enums/_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9016 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    13552 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9639 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py
+-rw-rw-rw-   0 root         (0) root         (0)     5195 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface.py
+-rw-rw-rw-   0 root         (0) root         (0)     6749 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surface_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    11119 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1853 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.810217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2737 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.814217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_arg_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_base_data_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.814217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.814217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11268 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6123 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.818217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    10019 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8278 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     1860 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.822218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.826218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7269 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py
+-rw-rw-rw-   0 root         (0) root         (0)     3486 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.826218 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6928 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.830217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_base_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8331 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3615 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.830217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22987 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    90634 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    14745 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.834217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22217 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7701 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    12529 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.838217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12297 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7675 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    13741 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9673 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.838217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6350 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7426 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10264 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.842217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.846217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_base/_underlying_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     9706 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.846217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_double_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_underlying_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.850217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14031 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.854217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4298 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    17334 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3848 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4201 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    30588 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.854217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5861 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8173 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4865 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4504 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.858217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5276 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    35872 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10061 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12111 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     6428 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12438 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.862217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2921 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.866217 refinitiv-data-1.3.0/refinitiv/data/content/news/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_content_validator_udf.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3276 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/_urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.870217 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5481 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_sort_order.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.870217 refinitiv-data-1.3.0/refinitiv/data/content/news/images/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/images/_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.874217 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_image_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_news_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.874217 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.874217 refinitiv-data-1.3.0/refinitiv/data/content/news/story/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      788 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/story/_udf_html_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.878217 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_top_news_headline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.878217 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_subcategory.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_top_news_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.878217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_org_info_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3986 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/_ownership_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.882217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/breakdown.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/concentration.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/investors.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/recent_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/shareholders_history_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/top_n_concentration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_breakdown_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_holdings_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_investors_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3197 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/breakdown.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/concentration.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/holdings.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/investors.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/recent_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/shareholders_history_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/top_n_concentration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3238 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/transaction_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/_holdings_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/holdings.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/ownership/org_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.890217 refinitiv-data-1.3.0/refinitiv/data/content/pricing/
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5313 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/_pricing_content_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    17807 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.894217 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    55563 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_display_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     8373 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     4789 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.898217 refinitiv-data-1.3.0/refinitiv/data/content/search/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11914 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_lookup_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_metadata_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/_views.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/search/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.902217 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     4444 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_country_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     7513 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_symbol_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.902217 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    10810 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.902217 refinitiv-data-1.3.0/refinitiv/data/delivery/
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.910217 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_api_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    26935 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     5634 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_parsed_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_raw_data_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5778 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_dictionary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.922217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12942 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_protocol_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_rdp_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    10068 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5401 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11913 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    11442 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9547 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_validator_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/base_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.922217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5529 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_offstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.926217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14643 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_dictionary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_field_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     6746 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     9811 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    15911 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3929 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/proxy_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.926217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     5403 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/ema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9506 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/socket.py
+-rw-rw-rw-   0 root         (0) root         (0)     4741 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     4073 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    16512 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_cxn_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_state_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.926217 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/ws_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.934217 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_buckets_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_sets_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_files_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_iter_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     2829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_packages_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_unpacker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/buckets.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/file_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/files.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/packages.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/endpoint_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/delivery/rdp_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.934217 refinitiv-data-1.3.0/refinitiv/data/discovery/
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2471 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_convert_symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2803 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.934217 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_buckets_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_navigator.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_property.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_property_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_search_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)     8754 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.938217 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12658 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8134 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/embedded.py
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/search.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.938217 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_customers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_fetch_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_relationship_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_suppliers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.942217 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_peers.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_screener.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_universe_expander.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.942217 refinitiv-data-1.3.0/refinitiv/data/early_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/early_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.942217 refinitiv-data-1.3.0/refinitiv/data/early_access/discovery/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/early_access/discovery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.946217 refinitiv-data-1.3.0/refinitiv/data/eikon/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9549 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_data_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_json_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     7401 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_news_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_streaming_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     5234 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_symbology.py
+-rw-rw-rw-   0 root         (0) root         (0)    13670 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/eikon/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.946217 refinitiv-data-1.3.0/refinitiv/data/session/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/session/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/session/desktop.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/session/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.946217 refinitiv-data-1.3.0/refinitiv/data/usage_collection/
+-rw-rw-rw-   0 root         (0) root         (0)      359 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_abstract_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/usage_collection/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-21 15:14:51.000000 refinitiv-data-1.3.0/refinitiv/data/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/refinitiv_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    55616 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-21 15:15:09.000000 refinitiv-data-1.3.0/refinitiv_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 15:15:09.950217 refinitiv-data-1.3.0/setup.cfg
```

### Comparing `refinitiv-data-1.2.0/CHANGELOG.md` & `refinitiv-data-1.3.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,45 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!-- towncrier release notes start -->
 
+
+## [1.3.0] - 2023-06-21
+
+### Added
+
+- `datetime` types for date measuring parameters to `refinitiv.data.content.ipa` objects ([eapi-5062](https://jira.refinitiv.com/browse/eapi-5062))
+- Fields validation option to the `contribute()` method for updating instrument(RIC) ([eapi-5213](https://jira.refinitiv.com/browse/eapi-5213))
+- `proxies` parameter to platform session ([eapi-5493](https://jira.refinitiv.com/browse/eapi-5493))
+
+### Changed
+
+- Updated docstrings for whole Delivery layer and the Content layer for the following parts: ESG, Estimates, Pricing, Symbol conversion ([eapi-5217](https://jira.refinitiv.com/browse/eapi-5217))
+- Optimising the logic of custom-instruments requests by saving `uuid` in cache ([eapi-5357](https://jira.refinitiv.com/browse/eapi-5357))
+- `Instrument` header name registered is unified for rdp/udf responses ([eapi-5387](https://jira.refinitiv.com/browse/eapi-5387))
+- Unified logic for displaying headers in `rd.get_history` DataFrame ([eapi-5454](https://jira.refinitiv.com/browse/eapi-5454))
+- `axis` parameter can be defined as `string` in `surface.get_point()` and `surface.get_curve()` methods ([eapi-5473](https://jira.refinitiv.com/browse/eapi-5473))
+
+### Fixed
+
+- `KeyError` raised if returns empty response in `cfs.packages` ([eapi-5634](https://jira.refinitiv.com/browse/eapi-5634))
+- `TypeError` raised instead of meaningful error message from response in `ipa.forward_curves` ([eapi-5631](https://jira.refinitiv.com/browse/eapi-5631))
+- `ValueError` raised if different case on duplicated fields defined in `rd.get_history` request ([eapi-5453](https://jira.refinitiv.com/browse/eapi-5453))
+- `search_explorer.get_possible_values()` is raise KeyError if no Navigators key exists ([eapi-5542](https://jira.refinitiv.com/browse/eapi-5542))
+
+### Hidden
+
+- Additional columns are added to DataFrame for customers and suppliers, renamed `fetch()` to `get_data()` ([eapi-5382](https://jira.refinitiv.com/browse/eapi-5382))
+- `Property.get_possible_values` method will not request data every call but check data in previous search response ([eapi-5490](https://jira.refinitiv.com/browse/eapi-5490))
+- `metadata` property is removed from `SearchPropertyExploreResponse` ([eapi-5491](https://jira.refinitiv.com/browse/eapi-5491))
+
+
 ## [1.2.0] - 2023-05-02
 
 ### Added
 
 - `extended_params` parameter to `Definition` classes of the following submodules of the `refinitiv.data.content.news` module: `online_reports`, `online_reports`, `top_news`, `top_news`, `story` ([eapi-4976](https://jira.refinitiv.com/browse/eapi-4976))
 - `instrument_type` parameter to the `refinitiv.data.content.ipa.financial_contracts.bond.Definition` ([eapi-5001](https://jira.refinitiv.com/browse/eapi-5001))
 - `refinitiv.data.content.ipa.surfaces.eti.VolatilitySurfacePoint` ([eapi-5020](https://jira.refinitiv.com/browse/eapi-5020))
```

### Comparing `refinitiv-data-1.2.0/LICENSE` & `refinitiv-data-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/PKG-INFO` & `refinitiv-data-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refinitiv-data
-Version: 1.2.0
+Version: 1.3.0
 Summary: Client for Refinitiv Data Platform API's
 Author: REFINITIV
 License: Apache 2.0
 Project-URL: Homepage, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python
 Project-URL: Documentation, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python/documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `refinitiv-data-1.2.0/README.md` & `refinitiv-data-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/pyproject.toml` & `refinitiv-data-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     # https://pypi.org/project/six/
     "six<=1.16.0",
     # https://pypi.org/project/tenacity/
     "tenacity>=8.0,<8.1.0",
     # https://pypi.org/project/watchdog/
     "watchdog>=0.10.2,<=2.1.9",
     # https://pypi.org/project/websocket-client/
-    "websocket-client>=0.58.0,!=1.2.2,<=1.4.1",
+    "websocket-client>=0.58.0,!=1.2.2,<=1.5.1",
     # https://pypi.org/project/pyhumps/
     "pyhumps~=3.0.2,<=3.8.0",
     # https://pypi.org/project/Jinja2/
     "jinja2>=3.0.3,<4.0.0",
     # https://pypi.org/project/simplejson/
     "simplejson~=3.15",
 ]
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_config_defaults.py` & `refinitiv-data-1.3.0/refinitiv/data/_config_defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,23 @@
                     "metadata": "/metadata/views",
                 },
             }
         },
         "streaming": {
             "pricing": {
                 "url": "/streaming/pricing/v1",
-                "endpoints": {"main": {"path": "/", "protocols": ["OMM"], "locations": []}},
+                "endpoints": {
+                    "main": {
+                        "contrib": {"field-validation": False},
+                        "metadata": {"download": False},
+                        "path": "/",
+                        "protocols": ["OMM"],
+                        "locations": [],
+                    }
+                },
             },
             "custom-instruments": {
                 "url": "/streaming/custom-instruments/v1",
                 "endpoints": {
                     "resource": {
                         "path": "/resource",
                         "protocols": ["OMM"],
@@ -346,15 +354,15 @@
                 },
             },
         },
     },
 }
 
 current_checksum = hashlib.md5(repr(data).encode()).hexdigest()  # NOSONAR
-fixed_checksum = "a8961eddd3d4cee9d87fcaf2d8b6b435"
+fixed_checksum = "a47956a749ac71d4d60fe66ea5e90358"
 
 if current_checksum != fixed_checksum:
     warnings.warn(
         "Default library config was changed. This may cause unexpected errors. "
         "Please use user config to introduce new changes. You can reinstall "
         "refinitiv-data to revert changes back."
     )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_config_functions.py` & `refinitiv-data-1.3.0/refinitiv/data/_config_functions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_configure.py` & `refinitiv-data-1.3.0/refinitiv/data/_configure.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_content_type.py` & `refinitiv-data-1.3.0/refinitiv/data/_content_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/log_reporter.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/log_reporter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_default_session_manager.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_default_session_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_desktop_session.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_desktop_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from typing import Union
 
 from ._session import Session
 from ._session_cxn_type import SessionCxnType
 from ._session_type import SessionType
 from ..._tools import urljoin
 
 
@@ -18,23 +19,25 @@
         base_url=None,
         platform_path_rdp=None,
         platform_path_udf=None,
         handshake_url=None,
         token=None,
         dacs_position=None,
         dacs_application_id=None,
+        proxies: Union[str, dict] = None,
     ):
         super().__init__(
             app_key=app_key,
             on_state=on_state,
             on_event=on_event,
             token=token,
             dacs_position=dacs_position,
             dacs_application_id=dacs_application_id,
             name=name,
+            proxies=proxies,
         )
         from os import getenv
 
         self._port = None
         self._udf_url = None
         self._timeout = self.http_request_timeout_secs
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_platform_session.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_platform_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
 from ._session import Session
 from ._session_cxn_type import SessionCxnType
 from ._session_type import SessionType
 from .event_code import EventCode
 from ..._errors import ScopeError
 from ..._tools import urljoin, cached_property, parse_url
@@ -42,23 +42,25 @@
         auto_reconnect=None,
         server_mode=None,
         base_url=None,
         auth_url=None,
         auth_authorize=None,
         auth_token=None,
         realtime_distribution_system_url=None,
+        proxies: Union[str, dict] = None,
     ):
         super().__init__(
             app_key,
             on_state=on_state,
             on_event=on_event,
             deployed_platform_username=deployed_platform_username,
             dacs_position=dacs_position,
             dacs_application_id=dacs_application_id,
             name=name,
+            proxies=proxies,
         )
 
         self._grant = grant
         self._take_signon_control = signon_control
 
         self._auto_reconnect = auto_reconnect
         self._server_mode = server_mode
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_retry_transport.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_retry_transport.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_session.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import abc
 import asyncio
 import itertools
 import logging
 import warnings
+from contextlib import AbstractContextManager, AbstractAsyncContextManager
 from threading import Lock
 from typing import Callable, TYPE_CHECKING, Union
-from contextlib import AbstractContextManager, AbstractAsyncContextManager
 
 from . import http_service
-from .event_code import EventCode
 from ._dacs_params import DacsParams
+from ._user_uuid import get_user_uuid
 from ._session_cxn_type import SessionCxnType
+from .event_code import EventCode
 from .tools import is_closed
 from ... import _configure as configure, _log as log
 from ..._open_state import OpenState
 from ..._tools import DEBUG, cached_property, create_repr
 
 if TYPE_CHECKING:
+    import httpx
     from ._session_cxn_factory import SessionConnection
     from .http_service import HTTPService
     from ..._configure import _RDPConfig
-    import httpx
     from ...delivery._data._data_provider import Request
+    from ...delivery._stream.metadata import Dictionary
 
 SESSION_IS_CLOSED = "Session is closed"
 
 
 class Session(AbstractContextManager, AbstractAsyncContextManager):
     _id_iterator = itertools.count()
     # Logger for messages outside of particular session instances
 
     __acquire_session_id_lock = Lock()
+    __acquire_stream_id_lock = Lock()
+    __acquire_metadata_load_lock = Lock()
 
     @property
     @abc.abstractmethod
     def type(self):
         pass
 
     @staticmethod
@@ -51,14 +55,15 @@
         on_state: Callable[[OpenState, str, "Session"], None] = None,
         on_event: Callable[[EventCode, Union[dict, str], "Session"], None] = None,
         token=None,
         deployed_platform_username=None,
         dacs_position=None,
         dacs_application_id=None,
         name="default",
+        proxies: Union[str, dict] = None,
     ):
         with self.__acquire_session_id_lock:
             self._session_id = next(self._id_iterator)
 
         session_type = self.type.name.lower()
         logger_name = f"sessions.{session_type}.{name}.{self.session_id}"
 
@@ -100,17 +105,19 @@
         specific_api = self._config.get(specific_api_path)
         if specific_api:
             self._config.set_param("apis", specific_api)
 
         self._config.on(configure.ConfigEvent.UPDATE, self._on_config_updated)
         # rssl/rwf stream ids always starts with 5
         self._omm_stream_counter = itertools.count(5)
-
         self._rdp_stream_counter = itertools.count(5)  # can not be 0
-        self._contrib_post_id_counter = itertools.count(5)
+
+        self._is_metadata_loaded = False
+
+        self._proxies = proxies
 
     def __enter__(self):
         self.open()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.close()
@@ -118,14 +125,18 @@
     async def __aenter__(self):
         await self.open_async()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close_async()
 
+    def _get_omm_stream_id(self) -> int:
+        with self.__acquire_stream_id_lock:
+            return next(self._omm_stream_counter)
+
     @cached_property
     def _http_service(self) -> "HTTPService":
         return http_service.get_service(self)
 
     @cached_property
     def _connection(self) -> "SessionConnection":
         from ._session_cxn_factory import get_session_cxn
@@ -260,18 +271,43 @@
     def logger(self) -> logging.Logger:
         return self._logger
 
     def _get_rdp_url_root(self) -> str:
         return ""
 
     @cached_property
+    def _user_uuid(self):
+        return get_user_uuid(self)
+
+    @cached_property
     def http_request_timeout_secs(self):
         return self._http_service.request_timeout_secs
 
     ############################################################
+    #   shared metadata
+
+    @cached_property
+    def _metadata(self) -> "Dictionary":
+        from ...delivery._dictionary import Dictionary
+
+        return Dictionary(self)
+
+    def _load_metadata(self, api: str) -> None:
+        with self.__acquire_metadata_load_lock:
+            if not self._is_metadata_loaded:
+                self._metadata.load(api=api)
+                self._is_metadata_loaded = True
+
+    def _validate_metadata(self, fields: dict) -> dict:
+        if not self._is_metadata_loaded:
+            raise ValueError("Metadata is not loaded")
+
+        return self._metadata.validate(fields)
+
+    ############################################################
     #   reconnection configuration
 
     @property
     def stream_auto_reconnection(self):
         return True
 
     @property
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_cxn_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_cxn_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/_session_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/_session_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from ..._external_libraries import python_configuration as ext_config_mod  # noqa
-
 from typing import Union
 
 from ._desktop_session import DesktopSession
-from ._session_type import SessionType
 from ._platform_session import PlatformSession
-from ... import _configure as configure
+from ._session_type import SessionType
 from .grant_password import GrantPassword
+from ... import _configure as configure
+from ..._external_libraries import python_configuration as ext_config_mod  # noqa
 
 CANNOT_FIND_APP_KEY = "Can't find 'app-key' in config object."
 
 DEPLOYED_PLATFORM_URL_CONFIG_KEY = "realtime-distribution-system.url"
 DEPLOYED_PLATFORM_USER_CONFIG_KEY = "realtime-distribution-system.dacs.username"
 DEPLOYED_PLATFORM_DACS_POS_CONFIG_KEY = "realtime-distribution-system.dacs.position"
 DEPLOYED_PLATFORM_DACS_ID_CONFIG_KEY = "realtime-distribution-system.dacs.application-id"
@@ -113,14 +112,15 @@
     app_key=None,
     signon_control=None,
     deployed_platform_host=None,
     deployed_platform_username=None,
     dacs_position=None,
     dacs_application_id=None,
     grant=None,
+    proxies=None,
 ):
     session_config = configure.get(configure.keys.platform_session(session_name), {})
     default_session_config = configure.get(configure.keys.platform_session("default"), {})
 
     if isinstance(session_config, dict) and len(session_config) == 0:
         raise ValueError(f"Session name: {session_name} is invalid or session_name object is empty")
 
@@ -150,15 +150,15 @@
     _validate_platform_session_arguments(
         app_key=app_key,
         grant=grant,
         deployed_platform_host=deployed_platform_host,
         deployed_platform_username=deployed_platform_username,
     )
 
-    return make_session_provider(SessionType.PLATFORM, merged_config, grant, session_name)
+    return make_session_provider(SessionType.PLATFORM, merged_config, grant, session_name, proxies)
 
 
 def _validate_desktop_session_app_key(session_config=None, app_key=None, session_name=None):
     if not session_config and not app_key:
         raise ValueError(f"Can't get config by name: {session_name}. Please check config name or provide app_key")
 
     if not app_key:
@@ -238,24 +238,25 @@
         deployed_platform_host=deployed_platform_host,
         deployed_platform_username=deployed_platform_username,
     )
 
     return make_session_provider(session_type, merged_config, grant, session_name)
 
 
-def make_session_provider(session_type, config=None, grant=None, session_name="default"):
+def make_session_provider(session_type, config=None, grant=None, session_name="default", proxies=None):
     config = config or {}
     session_class = session_class_by_session_type.get(session_type)
     if not session_class:
         raise ValueError(f"Cannot find session class by session type {session_type}")
     session_class = get_session_class(session_type)
 
     def session_provider():
         params = _retrieve_values_from_config(config, session_type, grant)
         params["name"] = session_name
+        params["proxies"] = proxies
         sessions_inst = session_class(**params)
         sessions_inst.debug(f" + Session created: {sessions_inst}")
         return sessions_inst
 
     return session_provider
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/access_token_updater.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/access_token_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/auth_manager.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/auth_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/connection.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/event.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/event.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/event_code.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/event_code.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/grant_password.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/grant_password.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/http_service.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/http_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
+import re
 import threading
 from typing import TYPE_CHECKING, Union
-import re
 
 import httpx
 
 from ._retry_transport import RequestRetryException, RetryAsyncTransport, RetryTransport
 from .tools import is_desktop_session
 from ..log_reporter import LogReporter
 from ... import _configure as configure
@@ -155,15 +155,15 @@
 
     def open(self):
         config = self._session.config
         limits = get_http_limits(config)
 
         # httpx has its default Accept header and
         # server wants application/json or nothing
-        self._client = httpx.Client(headers={"Accept": APPLICATION_JSON}, limits=limits)
+        self._client = httpx.Client(headers={"Accept": APPLICATION_JSON}, limits=limits, proxies=self._session._proxies)
 
         key = configure.keys.http_auto_retry_config
         auto_retry_config = config.get(key, None)
 
         if auto_retry_config:
             number_of_retries = auto_retry_config.get("number-of-retries", 3)
             retry_on_errors = auto_retry_config.get("on-errors", [])
@@ -172,15 +172,15 @@
 
             retry_transport = RetryTransport(
                 total_attempts=number_of_retries,
                 on_statuses=retry_on_errors,
                 on_methods=retry_on_methods,
                 backoff_factor=retry_backoff_factor,
             )
-            self._auto_retry_client = httpx.Client(transport=retry_transport)
+            self._auto_retry_client = httpx.Client(transport=retry_transport, proxies=self._session._proxies)
 
     def close(self):
         if self._client:
             try:
                 self._client.close()
                 self._client = None
             except RuntimeError as e:
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/null_session.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/null_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/refresh_token_updater.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/refresh_token_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/tools.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_core/session/updater.py` & `refinitiv-data-1.3.0/refinitiv/data/_core/session/updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_errors.py` & `refinitiv-data-1.3.0/refinitiv/data/_errors.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/LICENSE` & `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/LICENSE`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/configuration.py` & `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py` & `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_external_libraries/python_configuration/helpers.py` & `refinitiv-data-1.3.0/refinitiv/data/_external_libraries/python_configuration/helpers.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_containers.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 self._adc_fields.append(field)
             else:
                 self._hp_fields.append(field)
 
     @cached_property
     def _fields(self) -> "StrStrings":
         raw = fields_arg_parser.get_list(self.raw or [])
-        unique_fields = list(dict.fromkeys(raw).keys())
+        unique_fields = list(dict.fromkeys(map(str.upper, raw)).keys())
         if len(unique_fields) < len(raw):
             warnings.warn("You have duplicated fields in your input. Output will contain unique fields only.")
         return unique_fields
 
     @property
     def adc(self) -> "StrStrings":
         if self._adc_fields is None:
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_data_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_history_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_history_df_builder_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_intervals_consts.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_intervals_consts.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_mixed_streams.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,114 @@
-from typing import Dict
+from typing import Any, TYPE_CHECKING
 
-from .._tools import cached_property
-from .._content_type import ContentType
-from ..content._universe_stream import _UniverseStream
-from ..content._universe_streams import _UniverseStreams
-from ..content.custom_instruments._custom_instruments_data_provider import (
-    is_instrument_id,
-    get_user_id,
-    symbol_with_user_id,
-)
-from ..content.custom_instruments._stream_facade import uuid_from_symbol
-from ..content.pricing._stream_facade import Stream as _Stream, PricingStream
-from ..delivery._data._data_provider import DataProviderLayer
-from ..delivery._data._endpoint_data import RequestMethod
-from ..delivery._stream import StreamStateEvent
-
-
-class MixedStreams(_UniverseStreams):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs, content_type=ContentType.NONE)
-        self._uuid = None
-
-    def _get_symbol(self, universe):
-        if is_instrument_id.match(universe):
-            data_provider_layer = DataProviderLayer(
-                data_type=ContentType.CUSTOM_INSTRUMENTS_INSTRUMENTS,
-                universe=self.universe,
-            )
-            instrument_response = data_provider_layer.get_data(self._session, method=RequestMethod.GET)
-            symbol = instrument_response.data.raw.get("symbol")
-            if not self._uuid:
-                self._uuid = uuid_from_symbol(symbol)
-        else:
-            if not symbol_with_user_id.match(universe):
-                if not self._uuid:
-                    self._uuid = get_user_id(self._session)
-                symbol = f"{universe}.{self._uuid}"
-            else:
-                symbol = universe
-        return symbol
-
-    def _get_pricing_stream(self, name):
-        stream = _UniverseStream(
-            content_type=ContentType.STREAMING_PRICING,
-            session=self._session,
-            name=name,
-            fields=self.fields,
-            service=self._service,
-            on_refresh=self._on_stream_refresh,
-            on_status=self._on_stream_status,
-            on_update=self._on_stream_update,
-            on_complete=self._on_stream_complete,
-            on_error=self._on_stream_error,
-            extended_params=self._extended_params,
-            parent_id=self._id,
-        )
-        return stream
+import pandas as pd
 
-    def _get_custom_instruments_stream(self, name):
-        stream = _UniverseStream(
-            content_type=ContentType.STREAMING_CUSTOM_INSTRUMENTS,
-            session=self._session,
-            name=self._get_symbol(name),
-            fields=self.fields,
-            service=self._service,
-            on_refresh=self._on_stream_refresh,
-            on_status=self._on_stream_status,
-            on_update=self._on_stream_update,
-            on_complete=self._on_stream_complete,
-            on_error=self._on_stream_error,
-            extended_params=self._extended_params,
-            parent_id=self._id,
-        )
-        return stream
+from ...._content_type import ContentType
+from ...._tools import cached_property
+from ....delivery._stream import _RDPStream, StreamStateEvent, StreamStateManager
+from ....delivery._stream._stream_factory import create_rdp_stream
+from ....delivery._stream._stream_listener import RDPStreamListener
+
+if TYPE_CHECKING:
+    from ...._types import ExtendedParams
+    from ...._core.session import Session
+    from ....delivery._stream import StreamState
+
+
+class QuantitativeDataStream(StreamStateManager, RDPStreamListener["QuantitativeDataStream"]):
+    def __init__(
+        self,
+        universe: dict,
+        session: "Session",
+        fields: list = None,
+        extended_params: "ExtendedParams" = None,
+    ):
+        self._session = session
+
+        StreamStateManager.__init__(self, logger=self._session.logger())
+        RDPStreamListener.__init__(self, logger=self._session.logger())
+
+        self._universe = universe
+        self._fields = fields
+        self._extended_params = extended_params
+
+        if extended_params and "view" in extended_params:
+            self._column_names = extended_params["view"]
 
-    def _create_stream_by_name(self, name):
-        if name.startswith("S)"):
-            stream = self._get_custom_instruments_stream(name)
         else:
-            stream = self._get_pricing_stream(name)
-        return stream
+            self._column_names = fields or None
 
-    @cached_property
-    def _stream_by_name(self) -> Dict[str, _UniverseStream]:
-        retval = {}
-        for name in self.universe:
-            stream = self._create_stream_by_name(name)
-            stream.on(StreamStateEvent.CLOSED, self._on_stream_close)
-            retval[name] = stream
-        return retval
-
-    def add_instruments(self, *instruments):
-        instruments = [self._get_symbol(name) if name.startswith("S)") else name for name in instruments]
-        super().add_instruments(*instruments)
-
-    def remove_instruments(self, *args):
-        args = [self._get_symbol(name) if name.startswith("S)") else name for name in args]
-        super().remove_instruments(*args)
+        self._data = None
+        self._headers = None
 
+    @property
+    def universe(self):
+        return self._universe
+
+    @property
+    def session(self) -> "Session":
+        return self._session
+
+    @session.setter
+    def session(self, session: "Session"):
+        if self._session != session and not self.is_open:
+            self._session = session
+            RDPStreamListener.init_logger(self, self._session.logger())
+            self._stream.session = self._session
 
-class Stream(_Stream):
     @cached_property
-    def _stream(self) -> MixedStreams:
-        return MixedStreams(
-            item_facade_class=PricingStream,
-            universe=self._universe,
+    def _stream(self) -> _RDPStream:
+        stream = create_rdp_stream(
+            ContentType.STREAMING_CONTRACTS,
             session=self._session,
-            fields=self._fields,
-            service=self._service,
+            view=self._fields,
+            universe=self._universe,
             extended_params=self._extended_params,
         )
+        stream.on(StreamStateEvent.CLOSED, lambda *_: self.close())
+        stream.on_ack(self._on_stream_ack)
+        stream.on_response(self._on_stream_response)
+        stream.on_update(self._on_stream_update)
+        stream.on_alarm(self._on_stream_alarm)
+        return stream
+
+    def __repr__(self):
+        s = super().__repr__()
+        s = s.replace(">", f" {{name='{self._universe}', state={self._stream.state}}}>")
+        return s
+
+    @property
+    def df(self):
+        if self._data is None or self._column_names is None:
+            return pd.DataFrame([])
+        return pd.DataFrame.from_records(self._data, columns=self._column_names)
+
+    def get_snapshot(self) -> pd.DataFrame:
+        return self.df
+
+    def _do_open(self, **kwargs) -> "StreamState":
+        return self._stream.open(**kwargs)
+
+    def _do_close(self, **kwargs) -> "StreamState":
+        return self._stream.close(**kwargs)
+
+    def _do_on_stream_ack(self, stream: _RDPStream, message: dict) -> Any:
+        return message["state"]
+
+    def _do_on_stream_response(self, stream: _RDPStream, message: dict) -> Any:
+        if "data" in message:
+            self._data = message["data"]
+
+        if "headers" in message:
+            self._headers = message["headers"]
+            self._column_names = [col["name"] for col in self._headers]
+
+        return self._data, self._column_names
+
+    def _do_on_stream_update(self, stream: _RDPStream, message: dict) -> Any:
+        if "data" in message:
+            self._data = message["data"]
+
+        return self._data, self._column_names
+
+    def _do_on_stream_alarm(self, stream: _RDPStream, message: dict) -> Any:
+        return message["state"]
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_ohlc_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_ohlc_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_pricing_recorder.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_pricing_recorder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_recording_control.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_recording_control.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/_stream_update_handler.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/_stream_update_handler.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_rdp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_adc_udf_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_context_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_rdp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_cust_inst_udf_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_and_cust_inst_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/context_collection/_hp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_add_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_count_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_date_schedule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_holidays.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/dates_and_calendars/_is_working_day.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/get_data_func.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_data_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,8 +97,10 @@
         except_msg = "\n\n".join(exceptions)
         raise RDError(-1, except_msg)
 
     hp_and_cust_inst_data = HPAndCustInstDataContainer(stream_columns, stream_data, stream_df)
     adc_data = ADCDataContainer(adc_raw, adc_df, fields)
     adc.set_data(adc_data=adc_data, hp_data=hp_and_cust_inst_data)
     hp_and_cust_inst.set_data(adc_data=adc_data, hp_data=hp_and_cust_inst_data)
-    return DataDFBuilder.build_df(adc, hp_and_cust_inst)
+    df = DataDFBuilder.build_df(adc, hp_and_cust_inst)
+    df.rename(columns={"instrument": "Instrument"}, inplace=True)
+    return df
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/get_history_func.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_history_func.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/get_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/get_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/news/_news.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/news/_news.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_fin_coder_layer/session.py` & `refinitiv-data-1.3.0/refinitiv/data/_fin_coder_layer/session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_log.py` & `refinitiv-data-1.3.0/refinitiv/data/_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         "%(thread)d-%(threadName)s|"
         "%(name)s] \n"
         "%(module)s."
         "%(funcName)s "
         "%(message)s"
     )
 else:
-    fmt = "[%(asctime)s] - " "[%(levelname)s] - " "[%(name)s] - " "[%(thread)d] | " "%(threadName)s\n" "%(message)s"
+    fmt = "[%(asctime)s] - [%(levelname)s] - [%(name)s] - [%(thread)d] | %(threadName)s\n%(message)s"
 
 _stdout_formatter = RDFormatter(fmt)
 
 
 def _create_log_stdout_handler():
     handler_ = logging.StreamHandler(sys.stdout)
     handler_.setFormatter(_stdout_formatter)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_qpl/_bid_ask.py` & `refinitiv-data-1.3.0/refinitiv/data/_qpl/_bid_ask.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_qpl/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/_qpl/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_qpl/_fx_spot_quote.py` & `refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_spot_quote.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_qpl/_fx_swap_points.py` & `refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swap_points.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_qpl/_fx_swp_to_swp.py` & `refinitiv-data-1.3.0/refinitiv/data/_qpl/_fx_swp_to_swp.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_qpl/_serializer.py` & `refinitiv-data-1.3.0/refinitiv/data/_qpl/_serializer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_qpl/_tenor_bid_ask.py` & `refinitiv-data-1.3.0/refinitiv/data/_qpl/_tenor_bid_ask.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_common.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_common.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_converter.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_converter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_dataframe.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_dataframe.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_datetime.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_datetime.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,14 +71,27 @@
 
 class FundamentalAndReferenceFormatter:
     def to_str(self, date_time):
         s = date_time.isoformat()
         return s.split("T")[0]
 
 
+class IPADateTimeFormatter:
+    def to_str(self, date_time_value):
+        return date_time_value.strftime("%Y-%m-%dT%H:%M:%SZ")
+
+
+class IPADateFormatter:
+    def to_str(self, date_time_value):
+        return date_time_value.strftime("%Y-%m-%d")
+
+
+# yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g. 2021-01-01t00:00:00z)
+
+
 class NanosecondsFormatter:
     NANOSECOND_LENGTH = 9
 
     def to_str(self, date_time):
         s = date_time.isoformat(timespec="microseconds")
         # s => '2021-08-03T10:33:35.554103+00:00000Z'
         s, *_ = s.split("+", maxsplit=1)
@@ -114,25 +127,29 @@
         if isinstance(value, str) and ownership_expr.match(value):
             return value
         return self.formatter.to_str(self.convert(value))
 
 
 _nanoseconds_formatter = NanosecondsFormatter()
 _date_formatter = FundamentalAndReferenceFormatter()
+ipa_datetime_formatter = IPADateTimeFormatter()
+ipa_date_formatter = IPADateFormatter()
 _converter = Converter()
 
 _z_ends_date_time_adapter = DateTimeAdapter(_converter, _nanoseconds_formatter)
 _t_ends_date_time_adapter = DateTimeAdapter(_converter, _date_formatter)
 hp_datetime_adapter = _z_ends_date_time_adapter
 news_datetime_adapter = _z_ends_date_time_adapter
 filling_search_datetime_adapter = _z_ends_date_time_adapter
 fr_datetime_adapter = _t_ends_date_time_adapter
 add_periods_datetime_adapter = _t_ends_date_time_adapter
 qpl_datetime_adapter = _t_ends_date_time_adapter
 tds_datetime_adapter = _z_ends_date_time_adapter
 custom_inst_datetime_adapter = _z_ends_date_time_adapter
 cfs_datetime_adapter = DateTimeAdapter(_converter, CFSFormatter())
 ownership_datetime_adapter = OwnerShipDateTimeAdapter(_converter, OwnershipFormatter())
+ipa_datetime_adapter = DateTimeAdapter(_converter, ipa_datetime_formatter)
+ipa_date_adapter = DateTimeAdapter(_converter, ipa_date_formatter)
 
 
 def to_iso_format(value):
     return to_datetime(value).isoformat()
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_params.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_params.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_patterns.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_patterns.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_repr.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_repr.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_specification.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_specification.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/_utils.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/_utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_tools/templates.py` & `refinitiv-data-1.3.0/refinitiv/data/_tools/templates.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/_types.py` & `refinitiv-data-1.3.0/refinitiv/data/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_content_data_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_content_data_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_content_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_content_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_content_provider_layer.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_content_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_content_response_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_content_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_df_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -529,14 +529,32 @@
 
     @classmethod
     def is_date_column(cls, header: dict, column: str) -> bool:
         header_title = header.get("title", column)
         return cls.DATE_PATTERN in header_title.lower() and not ADC_FUNC_PATTERN_IN_FIELDS.match(header_title)
 
 
+class DFBuilderFundamentalAndReferenceRDP(DFBuilderRDP):
+    def get_date_idxs_and_columns(
+        self, headers: List[dict], use_field_names_in_headers: bool = False
+    ) -> Tuple[List[str], List[int]]:
+        header_key = self.get_header_key(use_field_names_in_headers)
+        columns = []
+        date_idxs = []
+        for idx, header in enumerate(headers):
+            col = header[header_key]
+            if col == "instrument":
+                col = col.capitalize()
+            columns.append(col)
+            if self.is_date_column(header, col):
+                date_idxs.append(idx)
+
+        return columns, date_idxs
+
+
 def build_dates_calendars_df(raw: Any, **kwargs):
     raw = deepcopy(raw)
     add_periods_data = []
 
     clean_request_items = []
     for item in raw:
         if not item.get("error"):
@@ -597,7 +615,8 @@
 
 def build_empty_df(*args, **kwargs) -> pd.DataFrame:
     return pd.DataFrame()
 
 
 dfbuilder_rdp = DFBuilderRDP()
 dfbuilder_udf = DFBuilderUDF()
+dfbuilder_fundamental_and_reference_rdp = DFBuilderFundamentalAndReferenceRDP()
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_df_builder_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_df_builder_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from .news.online_reports._df_builder import news_online_reports_build_df
 from .news.online_reports.hierarchy._df_builder import news_online_reports_hierarchy_build_df
 from .._content_type import ContentType
 from ._df_build_type import DFBuildType
 from ._df_builder import (
     dfbuilder_udf,
     dfbuilder_rdp,
+    dfbuilder_fundamental_and_reference_rdp,
     default_build_df,
     build_empty_df,
     build_dates_calendars_holidays_df,
     build_dates_calendars_df,
     build_dates_calendars_date_schedule_df,
 )
 from ._historical_df_builder import custom_insts_builder, historical_builder
 from .custom_instruments._custom_instruments_data_provider import custom_instruments_build_df
-from .ipa._curves._curves_builder_df import bond_curve_build_df, cross_currency_curves_curve_build_df
-from .ipa._curves._curves_data_provider import (
+from .ipa._curves._curves_builder_df import (
+    bond_curve_build_df,
+    cross_currency_curves_curve_build_df,
     forward_curve_build_df,
     zc_curve_definitions_build_df,
     zc_curves_build_df,
     cross_currency_curves_definitions_search_build_df,
 )
 from .ipa.financial_contracts._contracts_data_provider import financial_contracts_build_df
 from .news._tools import news_build_df_rdp, news_build_df_udf
@@ -35,15 +37,15 @@
 
 content_type_by_build_type: Dict[Union[ContentType, DataType], Callable[[Any, Dict[str, Any]], pd.DataFrame]] = {
     ContentType.CHAINS: chains_build_df,
     ContentType.CONTRACTS: financial_contracts_build_df,
     ContentType.CUSTOM_INSTRUMENTS_INSTRUMENTS: custom_instruments_build_df,
     ContentType.CUSTOM_INSTRUMENTS_SEARCH: custom_instruments_build_df,
     ContentType.DATA_GRID_RDP: {
-        DFBuildType.INDEX: dfbuilder_rdp.build_index,
+        DFBuildType.INDEX: dfbuilder_fundamental_and_reference_rdp.build_index,
         DFBuildType.DATE_AS_INDEX: dfbuilder_rdp.build_date_as_index,
     },
     ContentType.DATA_GRID_UDF: {
         DFBuildType.INDEX: dfbuilder_udf.build_index,
         DFBuildType.DATE_AS_INDEX: dfbuilder_udf.build_date_as_index,
     },
     ContentType.DEFAULT: default_build_df,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_entire_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_entire_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_error_parser.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_error_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_historical_content_validator.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_historical_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_historical_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_historical_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_historical_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_historical_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_historical_raw_transf.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_historical_raw_transf.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_historical_response_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_historical_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_intervals.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_intervals.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_universe_content_validator.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_universe_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_universe_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_universe_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/_universe_streams.py` & `refinitiv-data-1.3.0/refinitiv/data/content/_universe_streams.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,16 +40,14 @@
     Parser,
     success_http_codes,
     ContentValidator,
     ContentTypeValidator,
     ValidatorContainer,
     ParsedData,
 )
-from ...delivery._data._data_provider import _check_response as default_check_response
-from ...delivery._data._data_provider_layer import get_data_by_data_type
 from ...delivery._data._endpoint_data import RequestMethod
 
 if TYPE_CHECKING:
     import httpx
 
 content_type_by_day_interval_type = {
     DayIntervalType.INTER: ContentType.CUSTOM_INSTRUMENTS_INTERDAY_SUMMARIES,
@@ -58,17 +56,14 @@
 
 # a20140be-3648-4892-9d1b-ce78ee8617fd
 is_instrument_id = re.compile(r"[a-z0-9]{8}(-[a-z0-9]{4}){3}-[a-z0-9]{12}")
 
 # S)INST.GESG1-0000
 symbol_with_user_id = re.compile(r".*\.[A-Z0-9]+-[A-Z0-9]+")
 
-wrong_uuid_regexp = re.compile(r"(Validation Error: .UUID suffix ).*( not matched with userID)")
-wrong_symbol = "S)Instrument.UUID-0000"
-
 
 def provide_session(func):
     def _func(value, session, *args, **kwargs):
         return func(value, session)
 
     return _func
 
@@ -100,35 +95,17 @@
     dataframe.fillna(pd.NA, inplace=True)
     return dataframe
 
 
 # --------------------------------------------------------------------------------------
 #   Request factory
 # --------------------------------------------------------------------------------------
-def has_all_error_user_id(response):
-    return all(wrong_uuid_regexp.match(error.message) for error in response.errors)
-
-
-def check_response(response, config):
-    return None if has_all_error_user_id(response) else default_check_response(response, config)
-
-
 def get_user_id(session=None) -> str:
     session = get_valid_session(session)
-    response = get_data_by_data_type(ContentType.CUSTOM_INSTRUMENTS_INSTRUMENTS, session, universe=wrong_symbol)
-    check_response(response, session.config)
-    errors = response.errors
-    messages = [error.message for error in errors]
-    user_id = ""
-    for message in messages:
-        if wrong_uuid_regexp.match(message):
-            _, user_id = message.rsplit(" ", 1)
-            break
-
-    return user_id
+    return session._user_uuid
 
 
 def convert_to_symbol(symbol, session=None, uuid=""):
     # "MyNewInstrument"
     retval = symbol
     if not retval.startswith("S)"):
         retval = f"S){retval}"
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_enums.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_enums.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_events.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_instrument_class.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from refinitiv.data._tools import (
     EnumArgsParser,
     make_parse_enum,
     make_convert_to_enum,
     custom_inst_datetime_adapter,
 )
-from refinitiv.data._types import OptDateTime
+from ..._types import OptDateTime
 from refinitiv.data.content.custom_instruments._enums import (
     VolumeBasedRolloverMethod,
     DayBasedRolloverMethod,
     SpreadAdjustmentMethod,
 )
 
 volume_based_rollover_method_enum_arg_parser = EnumArgsParser(
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_manage.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_search.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_stream_facade.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/_summaries.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/_summaries.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/custom_instruments/manage.py` & `refinitiv-data-1.3.0/refinitiv/data/content/custom_instruments/manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_base_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/_base_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_basic_overview_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/_org_info_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 from typing import TYPE_CHECKING
 
 from .._content_data import Data
 from .._content_provider_layer import ContentUsageLoggerMixin
 from ..._content_type import ContentType
-from ..._tools import create_repr, validate_bool_value, try_copy_to_list
+from ..._tools import validate_bool_value, try_copy_to_list
 from ...delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ..._types import StrStrings
+    from ..._types import ExtendedParams, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve ESG basic data.
+    This class describe parameters to retrieve the organization information for the requested instrument.
 
     Parameters
     ----------
-    universe : str, list of str
-        The Universe parameter allows the user to define the company they
-        want content returned for, ESG content is delivered at the Company Level.
+    universe: str, list of str
+        The Universe parameter allows the user to define the companies for which the content is returned.
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
+    extended_params : ExtendedParams, optional
+        If necessary other parameters.
+
     Examples
     --------
-    >>> from refinitiv.data.content import esg
-    >>> definition = esg.basic_overview.Definition("IBM.N")
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.org_info.Definition("TRI.N")
     >>> response = definition.get_data()
-
-    >>> response = await definition.get_data_async()
     """
 
-    _USAGE_CLS_NAME = "ESG.BasicOverviewDefinition"
+    _USAGE_CLS_NAME = "Ownership.OrgInfoDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         use_field_names_in_headers: bool = False,
+        extended_params: "ExtendedParams" = None,
     ):
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESG_BASIC_OVERVIEW,
+            ContentType.OWNERSHIP_ORG_INFO,
             universe=universe,
             use_field_names_in_headers=use_field_names_in_headers,
-        )
-
-    def __repr__(self):
-        return create_repr(
-            self,
-            middle_path="basic_overview",
-            content=f"{{universe='{self._kwargs.get('universe')}'}}",
+            extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_esg_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/_esg_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_full_measures_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/_standard_measures_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 if TYPE_CHECKING:
     from ..._types import StrStrings, OptInt
 
 
 class Definition(BaseDefinition):
     """
-    This class describe parameters to retrieve ESG full measures data.
+    This class describe parameters to retrieve ESG standart measures data.
 
     Parameters
     ----------
     universe : str, list of str
         The Universe parameter allows the user to define the company they
         want content returned for, ESG content is delivered at the Company Level.
 
@@ -28,15 +28,15 @@
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     Examples
     --------
     >>> from refinitiv.data.content import esg
-    >>> definition = esg.full_measures.Definition("BNPP.PA")
+    >>> definition = esg.standard_measures.Definition("BNPP.PA")
     """
 
     def __init__(
         self,
         universe: "StrStrings",
         start: "OptInt" = None,
         end: "OptInt" = None,
@@ -44,17 +44,17 @@
     ):
         validate_types(start, [int, type(None)], "start")
         validate_types(end, [int, type(None)], "end")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESG_FULL_MEASURES,
+            ContentType.ESG_STANDARD_MEASURES,
             universe=universe,
             start=start,
             end=end,
             use_field_names_in_headers=use_field_names_in_headers,
         )
 
     def __repr__(self):
-        s = super().__repr__()
-        return s.replace("esg", "esg.full_measures")
+        get_repr = super().__repr__()
+        return get_repr.replace("esg", "esg.standard_measures")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_full_scores_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 from typing import TYPE_CHECKING
 
-from ._base_definition import BaseDefinition
-from ..._content_type import ContentType
-from ..._tools import validate_types, validate_bool_value, try_copy_to_list
+from ..._content_data import Data
+from ..._content_provider_layer import ContentUsageLoggerMixin
+from ...._content_type import ContentType
+from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ..._types import StrStrings, OptInt
+    from ...._types import ExtendedParams, StrStrings
 
 
-class Definition(BaseDefinition):
+class Definition(
+    ContentUsageLoggerMixin[BaseResponse[Data]],
+    DataProviderLayer[BaseResponse[Data]],
+):
     """
-    This class describe parameters to retrieve ESG full scores data.
+    This class describe parameters to retrieve the calculated concentration data
+    by top 10, 20, 50, 100 consolidated investors.
 
     Parameters
     ----------
-    universe : str, list of str
-        The Universe parameter allows the user to define the company they
-        want content returned for, ESG content is delivered at the Company Level.
-
-    start : int, optional
-        Start & End parameter allows the user to request
-         the number of Financial Years they would like returned.
-
-    end : int, optional
-        Start & End parameter allows the user to request
-        the number of Financial Years they would like returned.
+    universe: str, list of str
+        The Universe parameter allows the user to define the companies for which the content is returned.
+
+    count: int
+        Number of records
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
+    extended_params : ExtendedParams, optional
+        If necessary other parameters.
+
     Examples
     --------
-    >>> from refinitiv.data.content import esg
-    >>> definition = esg.full_scores.Definition(universe="4295904307", start=0, end=-5)
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.consolidated.top_n_concentration.Definition("TRI.N", 30)
+    >>> response = definition.get_data()
     """
 
+    _USAGE_CLS_NAME = "Ownership.Consolidated.TopNConcentrationDefinition"
+
     def __init__(
         self,
         universe: "StrStrings",
-        start: "OptInt" = None,
-        end: "OptInt" = None,
+        count: int,
         use_field_names_in_headers: bool = False,
+        extended_params: "ExtendedParams" = None,
     ):
-        validate_types(start, [int, type(None)], "start")
-        validate_types(end, [int, type(None)], "end")
+        validate_types(count, [int], "count")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESG_FULL_SCORES,
+            ContentType.OWNERSHIP_CONSOLIDATED_TOP_N_CONCENTRATION,
             universe=universe,
-            start=start,
-            end=end,
+            count=count,
             use_field_names_in_headers=use_field_names_in_headers,
+            extended_params=extended_params,
         )
-
-    def __repr__(self):
-        get_repr = super().__repr__()
-        return get_repr.replace("esg", "esg.full_scores")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_standard_measures_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 from typing import TYPE_CHECKING
 
-from ._base_definition import BaseDefinition
-from ..._content_type import ContentType
-from ..._tools import validate_types, validate_bool_value, try_copy_to_list
+from ..._content_data import Data
+from ..._content_provider_layer import ContentUsageLoggerMixin
+from ...._content_type import ContentType
+from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ..._types import StrStrings, OptInt
+    from ...._types import ExtendedParams, StrStrings
 
 
-class Definition(BaseDefinition):
+class Definition(
+    ContentUsageLoggerMixin[BaseResponse[Data]],
+    DataProviderLayer[BaseResponse[Data]],
+):
     """
-    This class describe parameters to retrieve ESG standart measures data.
+    This class describe parameters to retrieve the calculated concentration data
+    by top 10, 20, 50, 100 fund investors.
 
     Parameters
     ----------
-    universe : str, list of str
-        The Universe parameter allows the user to define the company they
-        want content returned for, ESG content is delivered at the Company Level.
-
-    start : int, optional
-        Start & End parameter allows the user to request
-         the number of Financial Years they would like returned.
-
-    end : int, optional
-        Start & End parameter allows the user to request
-        the number of Financial Years they would like returned.
+    universe: str, list of str
+        The Universe parameter allows the user to define the companies for which the content is returned.
+
+    count: int
+        Number of records
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
+    extended_params : ExtendedParams, optional
+        If necessary other parameters.
+
     Examples
     --------
-    >>> from refinitiv.data.content import esg
-    >>> definition = esg.standard_measures.Definition("BNPP.PA")
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.fund.top_n_concentration.Definition("TRI.N", 30)
+    >>> response = definition.get_data()
     """
 
+    _USAGE_CLS_NAME = "Ownership.Fund.TopNConcentrationDefinition"
+
     def __init__(
         self,
         universe: "StrStrings",
-        start: "OptInt" = None,
-        end: "OptInt" = None,
+        count: int,
         use_field_names_in_headers: bool = False,
+        extended_params: "ExtendedParams" = None,
     ):
-        validate_types(start, [int, type(None)], "start")
-        validate_types(end, [int, type(None)], "end")
+        validate_types(count, [int], "count")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESG_STANDARD_MEASURES,
+            ContentType.OWNERSHIP_FUND_TOP_N_CONCENTRATION,
             universe=universe,
-            start=start,
-            end=end,
+            count=count,
             use_field_names_in_headers=use_field_names_in_headers,
+            extended_params=extended_params,
         )
-
-    def __repr__(self):
-        get_repr = super().__repr__()
-        return get_repr.replace("esg", "esg.standard_measures")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_standard_scores_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_breakdown_definition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,71 @@
-from typing import TYPE_CHECKING
+from typing import Union, TYPE_CHECKING
 
-from ._base_definition import BaseDefinition
-from ..._content_type import ContentType
-from ..._tools import validate_types, validate_bool_value, try_copy_to_list
+from .._enums import StatTypes
+from ..._content_data import Data
+from ..._content_provider_layer import ContentUsageLoggerMixin
+from ...._content_type import ContentType
+from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ..._types import StrStrings, OptInt
+    from ...._types import ExtendedParams, StrStrings
 
 
-class Definition(BaseDefinition):
+class Definition(
+    ContentUsageLoggerMixin[BaseResponse[Data]],
+    DataProviderLayer[BaseResponse[Data]],
+):
     """
-    This class describe parameters to retrieve ESG standart scores data.
+    This class describe parameters to retrieve holdings data breakdown by Investors Types,
+    Styles, Region, Countries, Rotations and Turnovers.
 
     Parameters
     ----------
-    universe : str, list of str
-        The Universe parameter allows the user to define the company they
-        want content returned for, ESG content is delivered at the Company Level.
-
-    start : int, optional
-        Start & End parameter allows the user to request
-         the number of Financial Years they would like returned.
-
-    end : int, optional
-        Start & End parameter allows the user to request
-        the number of Financial Years they would like returned.
+    universe: str, list of str
+        The Universe parameter allows the user to define the companies for which the content is returned.
+
+    stat_type: int, StatTypes
+        The statType parameter specifies which statistics type to be returned.
+        The types available are:
+            - Investor Type (1)
+            - Investment Style (2)
+            - Region (3)
+            - Rotation (4)
+            - Country (5)
+            - Metro Area (6)
+            - Investor Type Parent (7)
+            - Invest Style Parent (8)
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
+    extended_params : ExtendedParams, optional
+        If necessary other parameters.
+
     Examples
     --------
-    >>> from refinitiv.data.content import esg
-    >>> definition = esg.standard_scores.Definition("6758.T")
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.fund.breakdown.Definition("TRI.N", ownership.StatTypes.INVESTOR_TYPE)
+    >>> response = definition.get_data()
     """
 
+    _USAGE_CLS_NAME = "Ownership.Fund.BreakdownDefinition"
+
     def __init__(
         self,
         universe: "StrStrings",
-        start: "OptInt" = None,
-        end: "OptInt" = None,
+        stat_type: Union[int, StatTypes],
         use_field_names_in_headers: bool = False,
+        extended_params: "ExtendedParams" = None,
     ):
-        validate_types(start, [int, type(None)], "start")
-        validate_types(end, [int, type(None)], "end")
+        validate_types(stat_type, [int, StatTypes], "stat_type")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESG_STANDARD_SCORES,
+            ContentType.OWNERSHIP_FUND_BREAKDOWN,
             universe=universe,
-            start=start,
-            end=end,
+            stat_type=stat_type,
             use_field_names_in_headers=use_field_names_in_headers,
+            extended_params=extended_params,
         )
-
-    def __repr__(self):
-        get_repr = super().__repr__()
-        return get_repr.replace("esg", "esg.standard_scores")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/_universe_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/_universe_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from ..._content_type import ContentType
 from ..._tools import create_repr, validate_bool_value
 from ...delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 
 class Definition(DataProviderLayer[BaseResponse[Data]]):
     """
-    This class describe parameters to retrieve data for ESG universe.
+    Defines the ESG data for all available instruments.
 
     Parameters
     ----------
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
+        Boolean that indicates whether or not to display field names in the headers.
 
     Examples
     --------
     >>> from refinitiv.data.content import esg
     >>> definition = esg.universe.Definition()
     >>> response = definition.get_data()
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_actions.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_actions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_db_manager.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_db_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,24 @@
 
 class Response:
     pass
 
 
 class Definition:
     """
-    This class describe parameters to retrieve ESG data.
+    Defines the ESG full measures data to retrieve.
 
     Parameters
     ----------
     package_name : str
-
+        Name of the package to download.
     universe : str, list of str
-        The Universe parameter allows the user to define the company they
-        want content returned for, ESG content is delivered at the Company Level.
-
+        Single instrument or list of instruments.
     fields : list, optional
-        The list of fields that are to be returned in the response
+        List of fields to return.
 
     Examples
     --------
     >>> import refinitiv.data.content.esg.bulk as bulk
     >>> definition = bulk.Definition(
     ...     package_name='standard_scores',
     ...     universe=['4295875817', '4295889298'],
@@ -54,15 +52,15 @@
         self._fields = fields and fields_arg_parser.get_list(fields)
         universe = try_copy_to_list(universe)
         self._universe = universe_arg_parser.get_list(universe)
         self._db_manager: DBManager = create_db_manager_by_package_name(package_name)
 
     def get_db_data(self) -> Response:
         """
-        Returns a response to the data platform
+        Sends a request to the previously created database to retrieve the defined ESG data.
 
         Returns
         -------
         Response
 
         """
         data = self._db_manager.get_data(universe=self._universe, fields=self._fields)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_file_manager.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_file_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_package_manager.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_package_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/esg/bulk/_tools.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/bulk/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,54 +12,48 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves estimates actuals values for reported annual periods.
+    Describes the parameters used to retrieve the estimated actuals interim values for the reported annual periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
-
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_actuals.annual.Definition(
-    ...     universe="IBM.N",
-    ...     package=estimates.Package.BASIC
-    ... )
+    >>> definition = estimates.view_actuals.annual.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Actuals.AnnualDefinition"
+    _USAGE_CLS_NAME = "Estimates.Actuals.InterimDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_ACTUALS_ANNUAL,
+            ContentType.ESTIMATES_VIEW_ACTUALS_INTERIM,
             universe=universe,
             package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,51 +12,51 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves estimates actuals values for reported interim periods.
+    Describes the parameters to retrieve the estimated actuals values for the reported annual periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
-
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_actuals.annual.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> definition = estimates.view_actuals.annual.Definition(
+    ...     universe="IBM.N",
+    ...     package=estimates.Package.BASIC
+    ... )
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Actuals.InterimDefinition"
+    _USAGE_CLS_NAME = "Estimates.Actuals.AnnualDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_ACTUALS_INTERIM,
+            ContentType.ESTIMATES_VIEW_ACTUALS_ANNUAL,
             universe=universe,
             package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,52 +3,51 @@
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
 from ...._tools import validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import StrStrings, ExtendedParams
+    from ...._types import ExtendedParams, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves estimates actuals values for KPI Measures for reported annual periods.
+    Describes the parameters used to retrieve the estimated actuals values for KPI Measures for the reported interim
+    periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_actuals_kpi.annual.Definition(universe="BNPP.PA")
+    >>> definition = estimates.view_actuals_kpi.interim.Definition(universe="BNPP.PA")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.ActualsKPI.AnnualDefinition"
+    _USAGE_CLS_NAME = "Estimates.ActualsKPI.InterimDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_ACTUALS_KPI_ANNUAL,
+            ContentType.ESTIMATES_VIEW_ACTUALS_KPI_INTERIM,
             universe=universe,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,44 +11,44 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves estimates actuals values for KPI Measures for reported interim periods.
+    This class describe parameters to retrieve the calculated concentration data by all consolidated investors.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
-    extended_params: ExtendedParams, optional
+    extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
-    >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_actuals_kpi.interim.Definition(universe="BNPP.PA")
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.consolidated.concentration.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.ActualsKPI.InterimDefinition"
+    _USAGE_CLS_NAME = "Ownership.Consolidated.ConcentrationDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_ACTUALS_KPI_INTERIM,
+            ContentType.OWNERSHIP_CONSOLIDATED_CONCENTRATION,
             universe=universe,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from typing import Union, TYPE_CHECKING
 
-from .._enums import Package
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
+from .._enums import Package
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
     from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves the annual estimates summary data for periodic estimates measures.
+    Describes the parameters used to retrieve recommendation summary.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
-
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary.annual.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> definition = estimates.view_summary.recommendations.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Summary.AnnualDefinition"
+    _USAGE_CLS_NAME = "Estimates.Summary.RecommendationsDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_ANNUAL,
+            ContentType.ESTIMATES_VIEW_SUMMARY_RECOMMENDATIONS,
             universe=universe,
             package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 from typing import Union, TYPE_CHECKING
 
+from .._enums import Package
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
-from .._enums import Package
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
     from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves the estimates monthly historical snapshot value for non periodic estimates measures for the last 12 months.
+    Describes parameters to retrieve the estimates monthly historical snapshot value for last 12 months for all
+    interim period estimates measures.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
-
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary.historical_snapshots_non_periodic_measures.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> definition = estimates.view_summary.historical_snapshots_periodic_measures_interim.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Summary.HistoricalSnapshotsNonPeriodicMeasuresDefinition"
+    _USAGE_CLS_NAME = "Estimates.Summary.HistoricalSnapshotsPeriodicMeasuresInterimDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_HISTORICAL_SNAPSHOTS_NON_PERIODIC_MEASURES,
+            ContentType.ESTIMATES_VIEW_SUMMARY_HISTORICAL_SNAPSHOTS_PERIODIC_MEASURES_INTERIM,
             universe=universe,
             package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from typing import Union, TYPE_CHECKING
 
-from .._enums import Package
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
+from .._enums import Package
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, StrStrings
+    from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves the estimates monthly historical snapshot value for last 12 months for all annual period estimates measures.
+    Describes the parameters used to retrieve the estimated summary values for the reported interim periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
-
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary.historical_snapshots_periodic_measures_annual.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> definition = estimates.view_summary.interim.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Summary.HistoricalSnapshotsPeriodicMeasuresAnnualDefinition"
+    _USAGE_CLS_NAME = "Estimates.Summary.InterimDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_HISTORICAL_SNAPSHOTS_PERIODIC_MEASURES_ANNUAL,
+            ContentType.ESTIMATES_VIEW_SUMMARY_INTERIM,
             universe=universe,
             package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 from typing import Union, TYPE_CHECKING
 
-from .._enums import Package
+from .._enums import StatTypes
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import StrStrings, ExtendedParams
+    from ...._types import ExtendedParams, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves the estimates monthly historical snapshot value for last 12 months for all interim period estimates measures.
+    This class describe parameters to retrieve holdings data breakdown by Investor Types,
+    Styles, Region, Countries, Rotations and Turnovers.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
-    package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
+    stat_type: int, StatTypes
+        The statType parameter specifies which statistics type to be returned.
+        The types available are:
+            - Investor Type (1)
+            - Investment Style (2)
+            - Region (3)
+            - Rotation (4)
+            - Country (5)
+            - Metro Area (6)
+            - Investor Type Parent (7)
+            - Invest Style Parent (8)
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     extended_params: ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
-    >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary.historical_snapshots_periodic_measures_interim.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.consolidated.breakdown.Definition("TRI.N", ownership.StatTypes.INVESTOR_TYPE)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Summary.HistoricalSnapshotsPeriodicMeasuresInterimDefinition"
+    _USAGE_CLS_NAME = "Ownership.Consolidated.BreakdownDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        package: Union[str, Package],
+        stat_type: Union[int, StatTypes],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(package, [str, Package], "package")
+        validate_types(stat_type, [int, StatTypes], "stat_type")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_HISTORICAL_SNAPSHOTS_PERIODIC_MEASURES_INTERIM,
+            ContentType.OWNERSHIP_CONSOLIDATED_BREAKDOWN,
             universe=universe,
-            package=package,
+            stat_type=stat_type,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves the estimates monthly historical snapshot value for recommendations for the last 12 months.
+    Describes the parameters used to retrieve the estimates monthly historical snapshot value for recommendations for
+    the last 12 months.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
-
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
     >>> definition = estimates.view_summary.historical_snapshots_recommendations.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from typing import Union, TYPE_CHECKING
 
+from .._enums import Package
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
-from .._enums import Package
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
     from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves the interim estimates summary data for periodic estimates measures.
+    Describes the parameters used to retrieve the estimated summary values for the reported annual periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
-
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary.interim.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> definition = estimates.view_summary.annual.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Summary.InterimDefinition"
+    _USAGE_CLS_NAME = "Estimates.Summary.AnnualDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_INTERIM,
+            ContentType.ESTIMATES_VIEW_SUMMARY_ANNUAL,
             universe=universe,
             package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 from typing import Union, TYPE_CHECKING
 
-from .._enums import Package
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
-from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ...._tools import validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import StrStrings, ExtendedParams
+    from ...._types import ExtendedParams, StrStrings
+    from .._enums import SortOrder
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrives estimates summary for all non-periodic estimates measures.
+    This class describe parameters to retrieve the latest 5 buy or sell activities for the requested company.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
-    package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
+    sort_order: str, SortOrder
+        The sortOrder parameter specifies ascending (asc) or descending (desc) Sort Order.
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
-    extended_params: ExtendedParams, optional
+    extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
-    >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary.non_periodic_measures.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.consolidated.recent_activity.Definition("TRI.N", "asc")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Summary.NonPeriodicMeasuresDefinition"
+    _USAGE_CLS_NAME = "Ownership.Consolidated.RecentActivityDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        package: Union[str, Package],
+        sort_order: Union[str, "SortOrder"],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_NON_PERIODIC_MEASURES,
+            ContentType.OWNERSHIP_CONSOLIDATED_RECENT_ACTIVITY,
             universe=universe,
-            package=package,
+            sort_order=sort_order,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_investors_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from typing import Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
-from .._enums import Package
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import StrStrings, ExtendedParams
+    from ...._types import ExtendedParams, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves recommendation summary.
+    This class describe parameters to retrieve company ownership details. Also, information on
+    the top 20 fund shareholders invested in the requested company.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
-    package: str, Package
-        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
-        the overall content set. Types of packages: basic, standard, professional
+    limit: int, optional
+        The limit parameter is used for paging. It allows users to select the number of records to be returned.
+        Default page size is 100 or 20 (depending on the operation).
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
-    extended_params: ExtendedParams, optional
+    extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
-    >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary.recommendations.Definition(universe="IBM.N", package=estimates.Package.BASIC)
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.fund.investors.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.Summary.RecommendationsDefinition"
+    _USAGE_CLS_NAME = "Ownership.Fund.InvestorsDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        package: Union[str, Package],
+        limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(package, [str, Package], "package")
+        validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_RECOMMENDATIONS,
+            ContentType.OWNERSHIP_FUND_INVESTORS,
             universe=universe,
-            package=package,
+            limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,44 +11,42 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves estimates summary values for KPI measures for annual periods.
+    Describes the parameters used to retrieve the estimated monthly historical snapshot value for all KPI measures for the last 12 months.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary_kpi.annual.Definition(universe="ORCL.N")
+    >>> definition = estimates.view_summary_kpi.historical_snapshots_kpi.Definition(universe="BNPP.PA")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.SummaryKPI.AnnualDefinition"
+    _USAGE_CLS_NAME = "Estimates.SummaryKPI.HistoricalSnapshotsKPIDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_KPI_ANNUAL,
+            ContentType.ESTIMATES_VIEW_SUMMARY_KPI_HISTORICAL_SNAPSHOTS_KPI,
             universe=universe,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,44 +11,42 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieves the Estimates monthly historical snapshot value for all KPI measures for the last 12 months.
+    Describes the parameters used to retrieve the estimated summary values for KPI measures for annual periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
+        Boolean that indicates whether or not to display field names in the headers.
     extended_params: ExtendedParams, optional
-        If necessary other parameters.
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary_kpi.historical_snapshots_kpi.Definition(universe="BNPP.PA")
+    >>> definition = estimates.view_summary_kpi.annual.Definition(universe="ORCL.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.SummaryKPI.HistoricalSnapshotsKPIDefinition"
+    _USAGE_CLS_NAME = "Estimates.SummaryKPI.AnnualDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_KPI_HISTORICAL_SNAPSHOTS_KPI,
+            ContentType.ESTIMATES_VIEW_SUMMARY_KPI_ANNUAL,
             universe=universe,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,62 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
-from ...._tools import validate_bool_value, try_copy_to_list
+from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import StrStrings, ExtendedParams
+    from ...._types import ExtendedParams, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
+
     """
-    This class describe parameters to retrieves estimates summary values for KPI measures for interim periods.
+    This class describe parameters to retrieve the latest fund shareholders
+    investment information for the requested company.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
+    limit: int, optional
+        The limit parameter is used for paging. It allows users to select the number of records to be returned.
+
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
-    extended_params: ExtendedParams, optional
+    extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
-    >>> from refinitiv.data.content import estimates
-    >>> definition = estimates.view_summary_kpi.interim.Definition(universe="BNPP.PA")
+    >>> from refinitiv.data.content import ownership
+    >>> definition = ownership.fund.shareholders_report.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Estimates.SummaryKPI.InterimDefinition"
+    _USAGE_CLS_NAME = "Ownership.Fund.ShareholdersReportDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
+        limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
+        validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.ESTIMATES_VIEW_SUMMARY_KPI_INTERIM,
+            ContentType.OWNERSHIP_FUND_SHAREHOLDERS_REPORT,
             universe=universe,
+            limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/filings/_filing_query.py` & `refinitiv-data-1.3.0/refinitiv/data/content/filings/_filing_query.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/filings/_retrieval_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/filings/_retrieval_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/filings/_retrieval_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/filings/_search_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/filings/_search_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/filings/_search_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py` & `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_enums.py` & `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_enums.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_events_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_events_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/historical_pricing/_summaries_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/historical_pricing/_summaries_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_content_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_content_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     InterestCalculationMethod,
     InterpolationMode,
     PriceSide,
 )
 
 
 if TYPE_CHECKING:
-    from ......_types import OptStrings, OptInt, OptBool, OptStr
+    from ......_types import OptStrings, OptInt, OptBool, OptStr, OptDateTime
 
 
 class CreditCurveParameters(ObjectDefinition):
     """
     Generates the credit curves for the definition provided
 
     Parameters
@@ -156,15 +156,15 @@
         sometimes creates a zero coupon curve which does not accurately reprice the
         input instruments used to build it. the multi-dimensional solver is recommended
         when cubic interpolation methods are used in building the curve (in other cases,
         performance might be inferior to the regular bootstrapping method). when use for
         credit curve it is only used when the calibrationmodel is set to 'bootstrap'.
         the possible values are:   * true: the multi-dimensional solver is used,   *
         false: the multi-dimensional solver is not used. the default value is 'true'.
-    valuation_date : str, optional
+    valuation_date : str or date or timedelta, optional
         Valuation date for this curve, that means the data at which instrument market
         data is retrieved.
     """
 
     def __init__(
         self,
         interest_calculation_method: Optional[InterestCalculationMethod] = None,
@@ -177,15 +177,15 @@
         interpolation_mode: Optional[InterpolationMode] = None,
         price_side: Optional[PriceSide] = None,
         basis_spline_knots: "OptInt" = None,
         return_calibrated_parameters: "OptBool" = None,
         use_delayed_data_if_denied: "OptBool" = None,
         use_duration_weighted_minimization: "OptBool" = None,
         use_multi_dimensional_solver: "OptBool" = None,
-        valuation_date: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.interest_calculation_method = interest_calculation_method
         self.basis_spline_smooth_model = basis_spline_smooth_model
         self.calendar_adjustment = calendar_adjustment
         self.calendars = try_copy_to_list(calendars)
         self.calibration_model = calibration_model
@@ -483,8 +483,8 @@
         data is retrieved.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_date_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Optional, TYPE_CHECKING
 
 from ..._models import ValuationTime
 from ...._enums._extrapolation_mode import ExtrapolationMode
 from ...._enums._interpolation_mode import InterpolationMode
 from ...._object_definition import ObjectDefinition
 
-
 if TYPE_CHECKING:
-    from ......_types import OptStr, OptBool
+    from ......_types import OptBool, OptDateTime
 
 
 class FxForwardCurveParameters(ObjectDefinition):
     """
     Generates the Cross Currency curves for the definitions provided
 
     Parameters
@@ -27,33 +26,33 @@
         are invlide, the curve is not calculated and an error is returned.  the default
         value is 'true'.
     ignore_pivot_currency_holidays : bool, optional
 
     use_delayed_data_if_denied : bool, optional
         Use delayed ric to retrieve data when not permissioned on constituent ric. the
         default value is 'false'.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
 
-    valuation_date_time : str, optional
+    valuation_date_time : str or date or datetime or timedelta, optional
         The date and time at which the zero coupon curve is generated. the value is
         expressed in iso 8601 format: yyyy-mm-ddt00:00:00z (e.g., '2021-01-01t14:00:00z'
         or '2021-01-01t14:00:00+02:00'). only one parameter of valuationdate and
         valuationdatetime must be specified.
     """
 
     def __init__(
         self,
         extrapolation_mode: Optional[ExtrapolationMode] = None,
         interpolation_mode: Optional[InterpolationMode] = None,
         valuation_time: Optional[ValuationTime] = None,
         ignore_invalid_instrument: "OptBool" = None,
         ignore_pivot_currency_holidays: "OptBool" = None,
         use_delayed_data_if_denied: "OptBool" = None,
-        valuation_date: "OptStr" = None,
-        valuation_date_time: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
+        valuation_date_time: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.extrapolation_mode = extrapolation_mode
         self.interpolation_mode = interpolation_mode
         self.valuation_time = valuation_time
         self.ignore_invalid_instrument = ignore_invalid_instrument
         self.ignore_pivot_currency_holidays = ignore_pivot_currency_holidays
@@ -138,23 +137,23 @@
         """
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_date_parameter("valuationDate", value)
 
     @property
     def valuation_date_time(self):
         """
         The date and time at which the zero coupon curve is generated. the value is
         expressed in iso 8601 format: yyyy-mm-ddt00:00:00z (e.g., '2021-01-01t14:00:00z'
         or '2021-01-01t14:00:00+02:00'). only one parameter of valuationdate and
         valuationdatetime must be specified.
         :return: str
         """
         return self._get_parameter("valuationDateTime")
 
     @valuation_date_time.setter
     def valuation_date_time(self, value):
-        self._set_parameter("valuationDateTime", value)
+        self._set_datetime_parameter("valuationDateTime", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     @property
     def definition_expiry_date(self):
         return self._get_parameter("definitionExpiryDate")
 
     @definition_expiry_date.setter
     def definition_expiry_date(self, value):
-        self._set_parameter("definitionExpiryDate", value)
+        self._set_date_parameter("definitionExpiryDate", value)
 
     @property
     def is_fallback_for_fx_curve_definition(self):
         return self._get_parameter("isFallbackForFxCurveDefinition")
 
     @is_fallback_for_fx_curve_definition.setter
     def is_fallback_for_fx_curve_definition(self, value):
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING
 
 from .._base_definition_mixin import BaseDefinitionMixin
 
 
 if TYPE_CHECKING:
     from ..._types import OptMainConstituentAssetClass, OptRiskType
-    from ......._types import OptStr, OptBool
+    from ......._types import OptStr, OptBool, OptDateTime
 
 
 class CrossCurrencyCurveCreateDefinition(BaseDefinitionMixin):
     """
     Create a cross currency curve definition
 
     Parameters
@@ -21,15 +21,15 @@
         The risk type to which the generated cross currency curve is sensitive. the
         possible value is:   * 'crosscurrency'
     base_currency : str, optional
         The base currency in the fxcross currency pair. it is expressed in iso 4217
         alphabetical format (e.g., 'eur').
     base_index_name : str, optional
         The name of the floating rate index (e.g., 'estr') applied to the base currency.
-    definition_expiry_date : str, optional
+    definition_expiry_date : str or date or datetime or timedelta, optional
         The date after which curvedefinitions can not be used. the value is expressed in
         iso 8601 format: yyyy-mm-dd (e.g., '2021-01-01').
     is_fallback_for_fx_curve_definition : bool, optional
         The indicator used to define the fallback logic for the fx curve definition. the
         possible values are:   * true: there's a fallback logic to use cross currency
         curve definition for fx curve definition,   * false: there's no fallback logic
         to use cross currency curve definition for fx curve definition.
@@ -54,15 +54,15 @@
 
     def __init__(
         self,
         main_constituent_asset_class: "OptMainConstituentAssetClass" = None,
         risk_type: "OptRiskType" = None,
         base_currency: "OptStr" = None,
         base_index_name: "OptStr" = None,
-        definition_expiry_date: "OptStr" = None,
+        definition_expiry_date: "OptDateTime" = None,
         is_fallback_for_fx_curve_definition: "OptBool" = None,
         is_non_deliverable: "OptBool" = None,
         name: "OptStr" = None,
         quoted_currency: "OptStr" = None,
         quoted_index_name: "OptStr" = None,
         source: "OptStr" = None,
     ) -> None:
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 
 from ._constituents_description import (
     CrossCurrencyConstituentsDescription,
 )
 from ._curve_parameters import CrossCurrencyCurveParameters
 from ...._object_definition import ObjectDefinition
 
-
 if TYPE_CHECKING:
-    from ......_types import OptStr
+    from ......_types import OptDateTime
 
 
 class CrossCurrencyInstrumentsSegment(ObjectDefinition):
     """
     Creates the Cross Currency curve definition with the definition provided.
 
     Parameters
     ----------
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
 
     constituents : CrossCurrencyConstituentsDescription, optional
 
     curve_parameters : CrossCurrencyCurveParameters, optional
 
     """
 
     def __init__(
         self,
-        start_date: "OptStr" = None,
+        start_date: "OptDateTime" = None,
         constituents: Optional[CrossCurrencyConstituentsDescription] = None,
         curve_parameters: Optional[CrossCurrencyCurveParameters] = None,
     ) -> None:
         super().__init__()
         self.start_date = start_date
         self.constituents = constituents
         self.curve_parameters = curve_parameters
@@ -63,8 +62,8 @@
         """
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import Optional, TYPE_CHECKING
 
 from ._override_bid_ask_fields import OverrideBidAskFields
 from ...._object_definition import ObjectDefinition
 
 if TYPE_CHECKING:
-    from ......_types import OptStr
+    from ......_types import OptStr, OptDateTime
 
 
 class OverrideBidAsk(ObjectDefinition):
     """
     Creates the Cross Currency curve definition with the definition provided.
 
     Parameters
     ----------
     instrument_code : str, optional
         Reuters instrument code (ric)
     fields : OverrideBidAskFields, optional
 
-    date : str, optional
+    date : str or date or datetime or timedelta, optional
         Overridden date
     """
 
     def __init__(
         self,
         instrument_code: "OptStr" = None,
         fields: Optional[OverrideBidAskFields] = None,
-        date: "OptStr" = None,
+        date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.instrument_code = instrument_code
         self.fields = fields
         self.date = date
 
     @property
@@ -49,15 +49,15 @@
         Overridden date
         :return: str
         """
         return self._get_parameter("date")
 
     @date.setter
     def date(self, value):
-        self._set_parameter("date", value)
+        self._set_date_parameter("date", value)
 
     @property
     def instrument_code(self):
         """
         Reuters instrument code (ric)
         :return: str
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from typing import Optional, TYPE_CHECKING
 
 from ._fx_forward_turn_fields import FxForwardTurnFields
 from ...._object_definition import ObjectDefinition
 
 if TYPE_CHECKING:
-    from ......_types import OptStr
+    from ......_types import OptStr, OptDateTime
 
 
 class OverrideFxForwardTurn(ObjectDefinition):
     """
     Creates the Cross Currency curve definition with the definition provided.
 
     Parameters
     ----------
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
 
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
 
     fields : FxForwardTurnFields, optional
 
-    date : str, optional
+    date : "OptDateTime"
 
     turn_tag : str, optional
 
     """
 
     def __init__(
         self,
-        start_date: "OptStr" = None,
-        end_date: "OptStr" = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         fields: Optional[FxForwardTurnFields] = None,
-        date: "OptStr" = None,
+        date: "OptDateTime" = None,
         turn_tag: "OptStr" = None,
     ) -> None:
         super().__init__()
         self.start_date = start_date
         self.end_date = end_date
         self.fields = fields
         self.date = date
@@ -56,37 +56,37 @@
         """
         :return: str
         """
         return self._get_parameter("date")
 
     @date.setter
     def date(self, value):
-        self._set_parameter("date", value)
+        self._set_date_parameter("date", value)
 
     @property
     def end_date(self):
         """
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_date_parameter("endDate", value)
 
     @property
     def start_date(self):
         """
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_date_parameter("startDate", value)
 
     @property
     def turn_tag(self):
         """
         :return: str
         """
         return self._get_parameter("turnTag")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ....._object_definition import ObjectDefinition
 from ..._enums import MainConstituentAssetClass, RiskType
 
 
 if TYPE_CHECKING:
     from ..._types import OptMainConstituentAssetClass, OptRiskType
-    from ......._types import OptStr, OptBool
+    from ......._types import OptStr, OptBool, OptDateTime
 
 
 class CrossCurrencyCurveGetDefinitionItem(ObjectDefinition):
     """
     Returns the definitions of the available commodity and energy forward curves for
     the filters selected (e.g. currency, source…).
 
@@ -46,15 +46,15 @@
         alphabetical format (e.g., 'usd').
     quoted_index_name : str, optional
         The name of the floating rate index (e.g., 'sofr') applied to the quoted
         currency.
     source : str, optional
         A user-defined string that is provided by the creator of a curve. curves created
         by refinitiv have the 'refinitiv' source.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date used to define a list of curves or a unique cross currency curve that
         can be priced at this date. the value is expressed in iso 8601 format:
         yyyy-mm-dd (e.g., '2021-01-01').
     """
 
     def __init__(
         self,
@@ -65,15 +65,15 @@
         curve_tag: "OptStr" = None,
         id: "OptStr" = None,
         is_non_deliverable: "OptBool" = None,
         name: "OptStr" = None,
         quoted_currency: "OptStr" = None,
         quoted_index_name: "OptStr" = None,
         source: "OptStr" = None,
-        valuation_date: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.main_constituent_asset_class = main_constituent_asset_class
         self.risk_type = risk_type
         self.base_currency = base_currency
         self.base_index_name = base_index_name
         self.curve_tag = curve_tag
@@ -237,8 +237,8 @@
         yyyy-mm-dd (e.g., '2021-01-01').
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_date_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING
 
 from .._base_definition_mixin import BaseWithIdDefinitionMixin
 
 if TYPE_CHECKING:
     from ..._types import OptMainConstituentAssetClass, OptRiskType
-    from ......._types import OptStr, OptBool
+    from ......._types import OptStr, OptBool, OptDateTime
 
 
 class CrossCurrencyCurveUpdateDefinition(BaseWithIdDefinitionMixin):
     """
     Update an existing cross currency curve definition
 
     Parameters
@@ -22,15 +22,15 @@
         The risk type to which the generated cross currency curve is sensitive. the
         possible value is:   * 'crosscurrency'
     base_currency : str, optional
         The base currency in the fxcross currency pair. it is expressed in iso 4217
         alphabetical format (e.g., 'eur').
     base_index_name : str, optional
         The name of the floating rate index (e.g., 'estr') applied to the base currency.
-    definition_expiry_date : str, optional
+    definition_expiry_date : str or date or datetime or timedelta, optional
         The date after which curvedefinitions can not be used. the value is expressed in
         iso 8601 format: yyyy-mm-dd (e.g., '2021-01-01').
     is_fallback_for_fx_curve_definition : bool, optional
         The indicator used to define the fallback logic for the fx curve definition. the
         possible values are:   * true: there's a fallback logic to use cross currency
         curve definition for fx curve definition,   * false: there's no fallback logic
         to use cross currency curve definition for fx curve definition.
@@ -56,15 +56,15 @@
     def __init__(
         self,
         id: str,
         main_constituent_asset_class: "OptMainConstituentAssetClass" = None,
         risk_type: "OptRiskType" = None,
         base_currency: "OptStr" = None,
         base_index_name: "OptStr" = None,
-        definition_expiry_date: "OptStr" = None,
+        definition_expiry_date: "OptDateTime" = None,
         is_fallback_for_fx_curve_definition: "OptBool" = None,
         is_non_deliverable: "OptBool" = None,
         name: "OptStr" = None,
         quoted_currency: "OptStr" = None,
         quoted_index_name: "OptStr" = None,
         source: "OptStr" = None,
     ) -> None:
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING
 
 from ...._object_definition import ObjectDefinition
 
 if TYPE_CHECKING:
-    from ......_types import OptStr
+    from ......_types import OptStr, OptDateTime
 
 
 class RequestItem(ObjectDefinition):
     """
     Gets the Cross Currency curve definitions who can be used with provided criterias.
 
     Parameters
@@ -20,26 +20,28 @@
         A user-defined string to identify the interest rate curve. it can be used to
         link output results to the curve definition. limited to 40 characters. only
         alphabetic, numeric and '- _.#=@' characters are supported.
     quoted_currency : str, optional
 
     quoted_index_name : str, optional
 
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
+        The date used to define a list of curves or a unique curve that can be priced
+        at this date. The value is expressed in ISO 8601 format: YYYY-MM-DD
 
     """
 
     def __init__(
         self,
         base_currency: "OptStr" = None,
         base_index_name: "OptStr" = None,
         curve_tag: "OptStr" = None,
         quoted_currency: "OptStr" = None,
         quoted_index_name: "OptStr" = None,
-        valuation_date: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.base_currency = base_currency
         self.base_index_name = base_index_name
         self.curve_tag = curve_tag
         self.quoted_currency = quoted_currency
         self.quoted_index_name = quoted_index_name
@@ -108,8 +110,8 @@
         """
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_date_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_curves_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_curves_builder_df.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,228 @@
-from dataclasses import dataclass
-from typing import Any, Callable, List, TYPE_CHECKING
+from itertools import product
 
-import numpy as np
 import pandas as pd
-from numpy import iterable
+from ...._tools._dataframe import convert_df_columns_to_datetime, convert_dtypes, convert_df_columns_to_datetime_by_idx
 
-from ._models._curve import Curve, ForwardCurve, ZcCurve
-from .._content_provider import (
-    CrossCurrencyCurvesDefinitionsRequestFactory,
-    CurvesAndSurfacesRequestFactory,
-    get_type_by_axis,
-)
-from .._ipa_content_validator import IPAContentValidator
-from ..curves._cross_currency_curves.definitions._data_classes import (
-    CurveDefinitionData,
-)
-from ..curves._cross_currency_curves.triangulate_definitions._data_provider import (
-    TriangulateDefinitionsData,
-)
-from ..._content_data import Data
-from ..._content_data_provider import ContentDataProvider
-from ..._content_response_factory import ContentResponseFactory
-from ...._content_type import ContentType
-from ...._tools import cached_property
-from ...._tools._dataframe import convert_df_columns_to_datetime, convert_dtypes
-from ....delivery._data._data_provider import DataProvider, ValidatorContainer
-from ....delivery._data._response_factory import ResponseFactory
-
-if TYPE_CHECKING:
-    from ....delivery._data._data_provider import ParsedData
-
-
-# ---------------------------------------------------------------------------
-#   ContentValidator
-# ---------------------------------------------------------------------------
-
-
-class CurvesContentValidator(IPAContentValidator):
-    @cached_property
-    def validators(self) -> List[Callable[["ParsedData"], bool]]:
-        return [self.content_data_is_not_none, self.any_element_have_no_error]
-
-
-class CurveDefinitionContentValidator(CurvesContentValidator):
-    _NAME_DATA = "curveDefinition"
-
-
-# ---------------------------------------------------------------------------
-#   Content data
-# ---------------------------------------------------------------------------
+
+def bond_curve_build_df(raw, **kwargs):
+    """
+    Parameters
+    ----------
+    raw : dict
+
+    Returns
+    -------
+    DataFrame
+
+    Examples
+    -------
+    >>> raw
+    ... {
+    ...     "data": [
+    ...         {
+    ...             "error": {
+    ...                 "id": "b6f9797d-72c8-4baa-84eb-6a079fc40ec5/b6f9797d-72c8-4baa-84eb-6a079fc40ec5",
+    ...                 "code": "QPS-Curves.6",
+    ...                 "message": "Invalid input: curveDefinition is missing",
+    ...             }
+    ...         },
+    ...         {
+    ...             "curveTag": "test_curve",
+    ...             "curveParameters": {
+    ...                 "interestCalculationMethod": "Dcb_Actual_Actual",
+    ...                 "priceSide": "Mid",
+    ...                 "calendarAdjustment": "Calendar",
+    ...                 "calendars": ["EMU_FI"],
+    ...                 "compoundingType": "Compounded",
+    ...                 "useConvexityAdjustment": True,
+    ...                 "useSteps": False,
+    ...                 "valuationDate": "2022-02-09",
+    ...             },
+    ...             "curveDefinition": {
+    ...                 "availableTenors": ["OIS", "1M", "3M", "6M", "1Y"],
+    ...                 "availableDiscountingTenors": ["OIS", "1M", "3M", "6M", "1Y"],
+    ...                 "currency": "EUR",
+    ...                 "mainConstituentAssetClass": "Swap",
+    ...                 "riskType": "InterestRate",
+    ...                 "indexName": "EURIBOR",
+    ...                 "source": "Refinitiv",
+    ...                 "name": "EUR EURIBOR Swap ZC Curve",
+    ...                 "id": "9d619112-9ab3-45c9-b83c-eb04cbec382e",
+    ...                 "discountingTenor": "OIS",
+    ...                 "ignoreExistingDefinition": False,
+    ...                 "owner": "Refinitiv",
+    ...             },
+    ...             "curvePoints": [
+    ...                 {
+    ...                     "endDate": "2021-02-01",
+    ...                     "startDate": "2021-02-01",
+    ...                     "discountFactor": 1.0,
+    ...                     "ratePercent": 7.040811073443143,
+    ...                     "tenor": "0D",
+    ...                 },
+    ...                 {
+    ...                     "endDate": "2021-02-04",
+    ...                     "startDate": "2021-02-01",
+    ...                     "discountFactor": 0.999442450671571,
+    ...                     "ratePercent": 7.040811073443143,
+    ...                     "tenor": "1D",
+    ...                 },
+    ...             ],
+    ...         },
+    ...     ]
+    ... }
+    """
+    datas = raw.get("data", [])
+    datas = datas or []
+    dfs = []
+    for data in datas:
+        error = data.get("error")
+        if error:
+            continue
+
+        curve_points = data.get("curvePoints")
+
+        for curve_point in curve_points:
+            d = {}
+            for key, value in curve_point.items():
+                values = d.setdefault(key, [])
+                values.append(value)
+
+            df = pd.DataFrame(d)
+            df = df.convert_dtypes()
+            dfs.append(df)
+
+    df = pd.concat(dfs, ignore_index=True)
+    df = convert_df_columns_to_datetime(df, "Date", utc=True, delete_tz=True)
+    df = convert_dtypes(df)
+    return df
+
+
+def cross_currency_curves_curve_build_df(raw, **kwargs):
+    """
+    Parameters
+    ----------
+    raw : dict
+
+    Returns
+    -------
+    DataFrame
+
+    Examples
+    -------
+    >>> raw
+    ... {
+    ... 'data':
+    ...    [
+    ...        {
+    ...            "error": {
+    ...                "id": "b6f9797d-72c8-4baa-84eb-6a079fc40ec5/b6f9797d-72c8-4baa-84eb-6a079fc40ec5",
+    ...                "code": "QPS-Curves.6",
+    ...                "message": "Invalid input: curveDefinition is missing",
+    ...            }
+    ...        },
+    ...        {
+    ...            'curveDefinition': {
+    ...                'baseCurrency': 'EUR', 'baseIndexName': 'ESTR',
+    ...                'quotedCurrency': 'USD', 'quotedIndexName': 'SOFR',
+    ...                'crossCurrencyDefinitions': [
+    ...                    {
+    ...                        'baseCurrency': 'EUR', 'baseIndexName': 'ESTR',
+    ...                        'name': 'EUR ESTR/USD SOFR FxCross',
+    ...                        'quotedCurrency': 'USD', 'quotedIndexName': 'SOFR',
+    ...                        'source': 'Refinitiv', 'isNonDeliverable': False,
+    ...                        'mainConstituentAssetClass': 'Swap',
+    ...                        'riskType': 'CrossCurrency',
+    ...                        'id': 'c9f2e9fb-b04b-4140-8377-8b7e47391486',
+    ...                        'ignoreExistingDefinition': False
+    ...                    }
+    ...                ]
+    ...            },
+    ...            'curveParameters': {
+    ...                'valuationDate': '2021-10-06',
+    ...                'interpolationMode': 'Linear',
+    ...                'extrapolationMode': 'Constant', 'turnAdjustments': {},
+    ...                'ignorePivotCurrencyHolidays': False,
+    ...                'useDelayedDataIfDenied': False,
+    ...                'ignoreInvalidInstrument': True,
+    ...                'marketDataLookBack': {'value': 10, 'unit': 'CalendarDay'}
+    ...            },
+    ...            'curve': {
+    ...                'fxCrossScalingFactor': 1.0, 'fxSwapPointScalingFactor': 10000.0,
+    ...                'curvePoints': [
+    ...                    {
+    ...                        'tenor': 'SPOT', 'startDate': '2021-10-08',
+    ...                        'endDate': '2021-10-08',
+    ...                        'swapPoint': {'bid': 0.0, 'ask': 0.0, 'mid': 0.0},
+    ...                        'outright': {'bid': 1.1556, 'ask': 1.156, 'mid': 1.1558}
+    ...                    },
+    ...                    {
+    ...                        'tenor': 'SN', 'startDate': '2021-10-08',
+    ...                        'endDate': '2021-10-12',
+    ...                        'instruments': [{'instrumentCode': 'EURSN='}],
+    ...                        'swapPoint': {
+    ...                            'bid': 0.8399999999997299,
+    ...                            'ask': 0.8800000000008801,
+    ...                            'mid': 0.860000000000305
+    ...                        },
+    ...                        'outright': {'bid': 1.155684, 'ask': 1.156088,
+    ...                                     'mid': 1.155886}
+    ...                    }
+    ...                ]
+    ...            }
+    ...        }
+    ...    ]
+    ... }
+    """
+    datas = raw.get("data", [])
+    datas = datas or []
+    get_curve = (data["curve"] for data in datas if "curve" in data)
+    columns_have_level_1 = ("swapPoint", "outright")
+    level_1 = ("bid", "ask", "mid")
+
+    curve = next(get_curve, {})
+    curve_points = curve.get("curvePoints", [])
+    curve_point = max(curve_points, key=lambda x: len(x))
+    columns = [key for key in curve_point]
+    data_df = _create_data_for_df(curve_points, columns, columns_have_level_1, level_1)
+
+    allcolumns = []
+    for name in columns:
+        if name in columns_have_level_1:
+            allcolumns.extend(list(product([name], level_1)))
+        else:
+            allcolumns.append((name, ""))
+
+    columns_date_idxs = [index for index, value in enumerate(allcolumns) if "date" in value[0].lower()]
+    columns = pd.MultiIndex.from_tuples(allcolumns)
+    df = pd.DataFrame(data_df, columns=columns)
+    df = convert_df_columns_to_datetime_by_idx(df, columns_date_idxs, utc=True, delete_tz=True)
+    df = convert_dtypes(df)
+    return df
+
+
+def _create_data_for_df(curve_points, columns, columns_have_level_1, columns_level_1):
+    data_df = []
+
+    for curve_point in curve_points:
+        row_data = []
+        for name in columns:
+            value = curve_point.get(name, pd.NA)
+            if name == "instruments" and not pd.isna(value):
+                value = [v["instrumentCode"] for v in value if "instrumentCode" in v]
+                value = value.pop() if len(value) == 1 else value
+            if name in columns_have_level_1:
+                value = [value.get(i, pd.NA) for i in columns_level_1]
+                row_data.extend(value)
+            else:
+                row_data.append(value)
+        data_df.append(row_data)
+
+    return data_df
 
 
 def zc_curves_build_df(raw, **kwargs):
     """
 
     Parameters
     ----------
@@ -317,36 +487,43 @@
     ...     ]
     ... }
     """
     datas = raw.get("data", [])
     datas = datas or []
     dfs = []
     for data in datas:
-        error = data.get("error")
-        if error:
+        if data.get("error"):
             continue
 
         forward_curves = data.get("forwardCurves")
 
         for forward_curve in forward_curves:
+            if forward_curve.get("error"):
+                continue
+
             curve_points = forward_curve.get("curvePoints")
 
             d = {}
             for curve_point in curve_points:
                 for key, value in curve_point.items():
                     values = d.setdefault(key, [])
                     values.append(value)
 
             df = pd.DataFrame(d)
             df = df.convert_dtypes()
             dfs.append(df)
 
-    df = pd.concat(dfs, ignore_index=True)
-    df = convert_df_columns_to_datetime(df, "Date", utc=True, delete_tz=True)
-    df = convert_dtypes(df)
+    if not dfs:
+        df = pd.DataFrame()
+
+    else:
+        df = pd.concat(dfs, ignore_index=True)
+        df = convert_df_columns_to_datetime(df, "Date", utc=True, delete_tz=True)
+        df = convert_dtypes(df)
+
     return df
 
 
 def zc_curve_definitions_build_df(raw, **kwargs):
     data = raw.get("data", [])
     data = data or []
     curve_definitions = [d for d in data if d for d in d.get("curveDefinitions")]
@@ -356,275 +533,7 @@
         df = convert_df_columns_to_datetime(df, "Date", utc=True, delete_tz=True)
         df = convert_dtypes(df)
     return df
 
 
 def cross_currency_curves_definitions_search_build_df(raw, **kwargs):
     return zc_curve_definitions_build_df(raw)
-
-
-@dataclass
-class OneCurveData(Data):
-    _create_curves: Callable = None
-    _curve: Curve = None
-
-    @property
-    def curve(self) -> Curve:
-        if self._curve is None:
-            curve = self._create_curves(self.raw)
-            self._curve = curve[0]
-        return self._curve
-
-
-@dataclass
-class CurvesData(Data):
-    _create_curves: Callable = None
-    _curves: List[Curve] = None
-
-    @property
-    def curves(self) -> List[Curve]:
-        if self._curves is None:
-            self._curves = self._create_curves(self.raw)
-        return self._curves
-
-
-def make_create_forward_curves(x_axis: str, y_axis: str) -> Callable:
-    """
-    Parameters
-    ----------
-    x_axis: str
-        Name of key in curve point data for build X axis
-    y_axis: str
-        Name of key in curve point data for build Y axis
-
-    Returns
-    -------
-    Callable
-    """
-
-    def create_forward_curves(raw: dict) -> list:
-        """
-        Curve point in "curvePoints":
-        {
-            "discountFactor": 1.0,
-            "endDate": "2021-02-01",
-            "ratePercent": -2.330761285491212,
-            "startDate": "2021-02-01",
-            "tenor": "0D"
-        }
-        Parameters
-        ----------
-        raw
-
-        Returns
-        -------
-        list of ForwardCurve
-        """
-        curves = []
-        for data in raw.get("data", []):
-            for forward_curve in data.get("forwardCurves", []):
-                x, y = [], []
-                for point in forward_curve.get("curvePoints"):
-                    end_date = point.get(x_axis)
-                    x.append(end_date)
-                    discount_factor = point.get(y_axis)
-                    y.append(discount_factor)
-
-                x = np.array(x, dtype=get_type_by_axis(x_axis))
-                y = np.array(y, dtype=get_type_by_axis(y_axis))
-                curve = ForwardCurve(x, y, **forward_curve)
-                curves.append(curve)
-
-        return curves
-
-    return create_forward_curves
-
-
-def make_create_bond_curves(x_axis: str, y_axis: str) -> Callable:
-    """
-    Parameters
-    ----------
-    x_axis: str
-        Name of key in curve point data for build X axis
-    y_axis: str
-        Name of key in curve point data for build Y axis
-
-    Returns
-    -------
-    Callable
-    """
-
-    def create_bond_curves(raw: dict) -> list:
-        """
-        Curve point in "curvePoints":
-        {
-            "discountFactor": 1.0,
-            "endDate": "2021-02-01",
-            "ratePercent": -2.330761285491212,
-            "startDate": "2021-02-01",
-            "tenor": "0D"
-        }
-        Parameters
-        ----------
-        raw
-
-        Returns
-        -------
-        list of Curve
-        """
-        curves = []
-        for data in raw.get("data", []):
-            x, y = [], []
-            for point in data.get("curvePoints"):
-                end_date = point.get(x_axis)
-                x.append(end_date)
-                discount_factor = point.get(y_axis)
-                y.append(discount_factor)
-
-            x = np.array(x, dtype=get_type_by_axis(x_axis))
-            y = np.array(y, dtype=get_type_by_axis(y_axis))
-            curve = Curve(x, y)
-            curves.append(curve)
-
-        return curves
-
-    return create_bond_curves
-
-
-def make_create_zc_curves(x_axis: str, y_axis: str) -> Callable:
-    """
-    Parameters
-    ----------
-    x_axis: str
-        Name of key in curve point data for build X axis
-    y_axis: str
-        Name of key in curve point data for build Y axis
-
-    Returns
-    -------
-    Callable
-    """
-
-    def create_zc_curves(raw: dict) -> list:
-        """
-        Curve point in "curvePoints":
-        {
-            "discountFactor": 1.0,
-            "endDate": "2021-07-27",
-            "ratePercent": -0.7359148312458879,
-            "startDate": "2021-07-27",
-            "tenor": "ON",
-            "instruments": [
-                {
-                    "instrumentCode": "SARON.S"
-                }
-            ]
-        }
-        Parameters
-        ----------
-        raw
-
-        Returns
-        -------
-        list of ZcCurve
-        """
-        curves = []
-        for data in raw.get("data", []):
-            for index_tenor, zc_curve in data.get("curves", {}).items():
-                x, y = [], []
-                for point in zc_curve.get("curvePoints"):
-                    end_date = point.get(x_axis)
-                    x.append(end_date)
-                    discount_factor = point.get(y_axis)
-                    y.append(discount_factor)
-
-                x = np.array(x, dtype=get_type_by_axis(x_axis))
-                y = np.array(y, dtype=get_type_by_axis(y_axis))
-                curve = ZcCurve(x, y, index_tenor, **zc_curve)
-                curves.append(curve)
-
-        return curves
-
-    return create_zc_curves
-
-
-curves_maker_by_content_type = {
-    ContentType.FORWARD_CURVE: make_create_forward_curves(x_axis="endDate", y_axis="discountFactor"),
-    ContentType.BOND_CURVE: make_create_bond_curves(x_axis="endDate", y_axis="discountFactor"),
-    ContentType.ZC_CURVES: make_create_zc_curves(x_axis="endDate", y_axis="discountFactor"),
-}
-
-
-def get_curves_maker(content_type):
-    curves_maker = curves_maker_by_content_type.get(content_type)
-
-    if not curves_maker:
-        raise ValueError(f"Cannot find curves_maker for content_type={content_type}")
-
-    return curves_maker
-
-
-# ---------------------------------------------------------------------------
-#   Response factory
-# ---------------------------------------------------------------------------
-
-
-class CurvesResponseFactory(ContentResponseFactory):
-    def create_data_success(self, raw: Any, **kwargs) -> Data:
-        return self._do_create_data(raw, **kwargs)
-
-    def create_data_fail(self, raw: Any, **kwargs) -> Data:
-        return self._do_create_data({}, **kwargs)
-
-    def _do_create_data(self, raw: Any, universe=None, **kwargs):
-        content_type = kwargs.get("__content_type__")
-        dfbuilder = self.get_dfbuilder(content_type, **kwargs)
-
-        if content_type is ContentType.ZC_CURVE_DEFINITIONS:
-            data = Data(raw, _dfbuilder=dfbuilder)
-
-        else:
-            curves_maker = get_curves_maker(content_type)
-            if iterable(universe):
-                data = CurvesData(
-                    raw=raw,
-                    _dfbuilder=dfbuilder,
-                    _create_curves=curves_maker,
-                )
-
-            else:
-                data = OneCurveData(raw=raw, _dfbuilder=dfbuilder, _create_curves=curves_maker)
-
-        return data
-
-
-# ---------------------------------------------------------------------------
-#   Data provider
-# ---------------------------------------------------------------------------
-
-curves_data_provider = ContentDataProvider(
-    request=CurvesAndSurfacesRequestFactory(),
-    response=CurvesResponseFactory(),
-    validator=ValidatorContainer(content_validator=CurvesContentValidator()),
-)
-
-curve_data_provider = ContentDataProvider(
-    request=CurvesAndSurfacesRequestFactory(),
-    validator=ValidatorContainer(content_validator=CurvesContentValidator()),
-)
-
-
-cross_currency_curves_triangulate_definitions_data_provider = DataProvider(
-    request=CurvesAndSurfacesRequestFactory(),
-    response=ResponseFactory(data_class=TriangulateDefinitionsData),
-    validator=ValidatorContainer(content_validator=CurvesContentValidator()),
-)
-
-cross_currency_curves_definitions_data_provider = DataProvider(
-    request=CrossCurrencyCurvesDefinitionsRequestFactory(),
-    response=ResponseFactory(data_class=CurveDefinitionData),
-    validator=ValidatorContainer(content_validator=CurveDefinitionContentValidator()),
-)
-
-cross_currency_curves_definitions_delete_data_provider = DataProvider(
-    request=CrossCurrencyCurvesDefinitionsRequestFactory(),
-)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_instrument_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_enums/_zc_interpolation_mode.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding: utf8
 
 from .._object_definition import ObjectDefinition
 from ...._tools import try_copy_to_list
-from ...._types import OptStr, OptStrings
+from ...._types import OptStr, OptStrings, OptDateTime
 
 
 class ForwardCurveDefinition(ObjectDefinition):
     """
     Parameters
     ----------
     index_tenor : str, optional
 
     forward_curve_tenors : list of str, optional
         Defines expected forward rate surface tenor/slices
     forward_curve_tag : str, optional
 
-    forward_start_date : str, optional
+    forward_start_date : str or date or datetime or timedelta, optional
         Defines the forward start date by date format
     forward_start_tenor : str, optional
         Defines the forward start date by tenor format: "Spot" / "1M" / ...
     """
 
     def __init__(
         self,
         index_tenor: OptStr = None,
         forward_curve_tag: OptStr = None,
         forward_curve_tenors: OptStrings = None,
-        forward_start_date: OptStr = None,
+        forward_start_date: "OptDateTime" = None,
         forward_start_tenor: OptStr = None,
     ) -> None:
         super().__init__()
         self.index_tenor = index_tenor
         self.forward_curve_tenors = try_copy_to_list(forward_curve_tenors)
         self.forward_curve_tag = forward_curve_tag
         self.forward_start_date = forward_start_date
@@ -65,15 +65,15 @@
         Defines the forward start date by date format
         :return: str
         """
         return self._get_parameter("forwardStartDate")
 
     @forward_start_date.setter
     def forward_start_date(self, value):
-        self._set_parameter("forwardStartDate", value)
+        self._set_date_parameter("forwardStartDate", value)
 
     @property
     def forward_start_tenor(self):
         """
         Defines the forward start date by tenor format: "Spot" / "1M" / ...
         :return: str
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_forward_curve_types.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_forward_curve_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_convexity.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_convexity.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_curve.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     @property
     def y(self):
         return self._y
 
     def get_point(
         self,
         value: Union[str, float, np.datetime64],
-        axis: Axis,
+        axis: Union[Axis, str],
     ) -> CurvePoint:
         """
         Parameters
         ----------
         value: str, float, np.datetime64
 
         axis: Axis
@@ -90,16 +90,16 @@
         Raises
         -------
         ValueError
             If cannot identify axis
         """
         value = value_arg_parser.parse(value)
 
-        is_value_on_axis_x = axis is Axis.X
-        is_value_on_axis_y = axis is Axis.Y
+        is_value_on_axis_x = axis == Axis.X
+        is_value_on_axis_y = axis == Axis.Y
 
         value_as_float = value_arg_parser.get_float(value)
 
         if is_value_on_axis_x:
             f = interpolate.interp1d(
                 x=self._x.astype(float),
                 y=self._y.astype(float),
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_instrument.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_instrument.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_interest_rate_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_par_rate_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_step.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_step.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # coding: utf8
 from ..._object_definition import ObjectDefinition
-from ....._types import OptStr
+from ....._types import OptDateTime
 
 
 class Step(ObjectDefinition):
     """
     Parameters
     ----------
-    effective_date : str, optional
+    effective_date : str or date or datetime or timedelta, optional
 
-    meeting_date : str, optional
+    meeting_date : str or date or datetime or timedelta, optional
 
     """
 
     def __init__(
         self,
-        effective_date: OptStr = None,
-        meeting_date: OptStr = None,
+        effective_date: "OptDateTime" = None,
+        meeting_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.effective_date = effective_date
         self.meeting_date = meeting_date
 
     @property
     def effective_date(self):
         """
         :return: str
         """
         return self._get_parameter("effectiveDate")
 
     @effective_date.setter
     def effective_date(self, value):
-        self._set_parameter("effectiveDate", value)
+        self._set_date_parameter("effectiveDate", value)
 
     @property
     def meeting_date(self):
         """
         :return: str
         """
         return self._get_parameter("meetingDate")
 
     @meeting_date.setter
     def meeting_date(self, value):
-        self._set_parameter("meetingDate", value)
+        self._set_date_parameter("meetingDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_turn.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_turn.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_models/_valuation_time.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_shift_scenario.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_shift_scenario.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_swap_zc_curve_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ExtrapolationMode,
 )
 from ._models import (
     ConvexityAdjustment,
     Step,
     Turn,
 )
-from ...._types import Strings, OptBool, OptStr
+from ...._types import Strings, OptBool, OptStr, OptDateTime
 from ...._tools import create_repr, try_copy_to_list
 
 if TYPE_CHECKING:
     from ._forward_curve_types import Steps, Turns
 
 
 class SwapZcCurveParameters(ObjectDefinition):
@@ -87,15 +87,15 @@
          - true: to use multi-dimensional solver for yield curve bootstrapping
          - false: not to use multi-dimensional solver for yield curve bootstrapping
     use_steps : bool, optional
         false / true
         Default value is: false.
         It indicates if the system needs to retrieve the overnight index
         stepped dates or/and rates
-    valuation_date : str, optional
+    valuation_date : str or date, optional
         The valuation date
         Default value is the current date
     market_data_access_denied_fallback : MarketDataAccessDeniedFallback, optional
         If at leat one constituent access is denied:
             * returnerror: dont price the surface and return an error (default value)
             * ignoreconstituents: price the surface without the error market data
             * usedelayeddata: use delayed market data if possible
@@ -112,15 +112,15 @@
     ignore_invalid_instrument : bool, optional
         Ignore invalid instrument to calculate the curve.
         If false and some instrument are invlide, the curve is not calculated
         and an error is returned.  the default value is 'True'.
     use_delayed_data_if_denied : bool, optional
         Use delayed ric to retrieve data when not permissioned on constituent ric. The
         default value is 'False'.
-    valuation_date_time : str, optional
+    valuation_date_time : str or date or datetime or timedelta, optional
         The date and time at which the zero coupon curve is generated.
         The value is expressed in iso 8601 format: yyyy-mm-ddt00:00:00z
         (e.g., '2021-01-01t14:00:00z' or '2021-01-01t14:00:00+02:00').
         Only one parameter of valuation_date and valuation_date_time must be specified.
     """
 
     _ignore_existing_definition = None
@@ -138,22 +138,22 @@
         steps: "Steps" = None,
         turns: "Turns" = None,
         ignore_existing_definition: OptBool = None,
         reference_tenor: OptStr = None,
         use_convexity_adjustment: OptBool = None,
         use_multi_dimensional_solver: OptBool = None,
         use_steps: OptBool = None,
-        valuation_date: OptStr = None,
+        valuation_date: "OptDateTime" = None,
         market_data_access_denied_fallback: Optional[MarketDataAccessDeniedFallback] = None,
         pivot_curve_parameters: Optional[InterestRateCurveParameters] = None,
         reference_curve_parameters: Optional[InterestRateCurveParameters] = None,
         valuation_time: Optional[ValuationTime] = None,
         ignore_invalid_instrument: OptBool = None,
         use_delayed_data_if_denied: OptBool = None,
-        valuation_date_time: OptStr = None,
+        valuation_date_time: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.interest_calculation_method = interest_calculation_method
         self.calendar_adjustment = calendar_adjustment
         self.calendars = try_copy_to_list(calendars)
         self.compounding_type = compounding_type
         self.convexity_adjustment = convexity_adjustment
@@ -403,15 +403,15 @@
         Default value is the current date
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_date_parameter("valuationDate", value)
 
     @property
     def market_data_access_denied_fallback(self):
         """
         If at leat one constituent access is denied:
             * returnerror: dont price the surface and return an error (default value)
             * ignoreconstituents: price the surface without the error market data
@@ -500,8 +500,8 @@
         Only one parameter of valuation_date and valuation_date_time must be specified.
         :return: str
         """
         return self._get_parameter("valuationDateTime")
 
     @valuation_date_time.setter
     def valuation_date_time(self, value):
-        self._set_parameter("valuationDateTime", value)
+        self._set_datetime_parameter("valuationDateTime", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definition_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         """
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_date_parameter("valuationDate", value)
 
     @property
     def market_data_location(self):
         """
         The identifier of the market place from which constituents come from. currently
         the following values are supported: 'onshore' and 'emea'. the list of values can
         be extended by a user when creating a curve.
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_definitions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import Optional, TYPE_CHECKING
-from ...._tools import create_repr, try_copy_to_list
 
-from .._object_definition import ObjectDefinition
 from ._enums import (
     CalendarAdjustment,
     CompoundingType,
     ExtrapolationMode,
     DayCountBasis,
     MarketDataAccessDeniedFallback,
     SwapPriceSide,
@@ -14,15 +12,17 @@
 from ._models import (
     Step,
     Turn,
     InterestRateCurveParameters,
     ConvexityAdjustment,
     ValuationTime,
 )
-from ...._types import OptBool, OptStr, Strings
+from .._object_definition import ObjectDefinition
+from ...._tools import create_repr, try_copy_to_list
+from ...._types import OptBool, OptStr, Strings, OptDateTime
 
 if TYPE_CHECKING:
     from ._zc_curve_types import Steps, Turns
 
 
 class ZcCurveParameters(ObjectDefinition):
     """
@@ -95,27 +95,27 @@
         interpolation methods are used in building the curve (in other cases,
         performance might be inferior to the regular bootstrapping method). When use for
         Credit Curve it is only used when the calibrationModel is set to Bootstrap.
         - true: to use multi-dimensional solver for yield curve bootstrapping
         - false: not to use multi-dimensional solver for yield curve bootstrapping
     use_steps : bool, optional
 
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The valuation date. The default value is the current date.
     valuation_time : ValuationTime, optional
         The time identified by offsets at which the zero coupon curve is generated.
     ignore_invalid_instrument : bool, optional
         Ignore invalid instrument to calculate the curve.
         if False and some instrument are invlide, the curve is not calculated and an
         error is returned.
         The default value is 'True'.
     use_delayed_data_if_denied : bool, optional
         Use delayed ric to retrieve data when not permissioned on constituent ric.
         The default value is 'False'.
-    valuation_date_time : str, optional
+    valuation_date_time : str or date or datetime or timedelta, optional
         The date and time at which the zero coupon curve is generated. the value is
         expressed in iso 8601 format: yyyy-mm-ddt00:00:00z (e.g., '2021-01-01t14:00:00z'
         or '2021-01-01t14:00:00+02:00'). Only one parameter of valuation_date and
         valuation_date_time must be specified.
     """
 
     _ignore_existing_definition = None
@@ -136,19 +136,19 @@
         steps: "Steps" = None,
         turns: "Turns" = None,
         ignore_existing_definition: OptBool = None,
         reference_tenor: OptStr = None,
         use_convexity_adjustment: OptBool = None,
         use_multi_dimensional_solver: OptBool = None,
         use_steps: OptBool = None,
-        valuation_date: OptStr = None,
+        valuation_date: "OptDateTime" = None,
         valuation_time: Optional[ValuationTime] = None,
         ignore_invalid_instrument: OptBool = None,
         use_delayed_data_if_denied: OptBool = None,
-        valuation_date_time: OptStr = None,
+        valuation_date_time: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.interest_calculation_method = interest_calculation_method
         self.calendar_adjustment = calendar_adjustment
         self.calendars = try_copy_to_list(calendars)
         self.compounding_type = compounding_type
         self.convexity_adjustment = convexity_adjustment
@@ -427,15 +427,15 @@
         The valuation date. The default value is the current date.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_date_parameter("valuationDate", value)
 
     @property
     def valuation_time(self):
         """
         The time identified by offsets at which the zero coupon curve is generated.
         :return: object ValuationTime
         """
@@ -481,8 +481,8 @@
         valuation_date_time must be specified.
         :return: str
         """
         return self._get_parameter("valuationDateTime")
 
     @valuation_date_time.setter
     def valuation_date_time(self, value):
-        self._set_parameter("valuationDateTime", value)
+        self._set_datetime_parameter("valuationDateTime", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_curves/_zc_curve_types.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_curves/_zc_curve_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_common_tools.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_common_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_day_of_week.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_day_of_week.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_direction.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_direction.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_exercise_style.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_exercise_style.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_frequency.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_frequency.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_period_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_period_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_seniority.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_seniority.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_stub_rule.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_stub_rule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_enums/_yield_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_enums/_yield_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_ipa_content_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_ipa_content_validator.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_ipa_content_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import TYPE_CHECKING
 
-from ...delivery._data._data_provider import (
-    ContentValidator,
-)
+from ...delivery._data._data_provider import ContentValidator
 
 if TYPE_CHECKING:
     from ...delivery._data._data_provider import ParsedData
 
 
 class IPAContentValidator(ContentValidator):
     _NAME_DATA = "data"
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_amortization_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_amortization_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # coding: utf8
 
 __all__ = ["AmortizationItem"]
 
 from typing import Optional, Union
 
+from ...._types import OptDateTime
 from .._object_definition import ObjectDefinition
 from .._enums import (
     AmortizationType,
     AmortizationFrequency,
 )
 
 
 class AmortizationItem(ObjectDefinition):
     """
     Parameters
     ----------
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         Start Date of an amortization section/window, or stepped rate
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         End Date of an amortization section/window, or stepped rate
     amortization_frequency : AmortizationFrequency, optional
         Frequency of the Amortization
     amortization_type : AmortizationType or str, optional
         Amortization type Annuity, Schedule, Linear, ....
     remaining_notional : float, optional
         The Remaining Notional Amount after Amortization
@@ -38,16 +39,16 @@
     ... )
     >>> amortization_item
 
     """
 
     def __init__(
         self,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         amortization_frequency: Optional[AmortizationFrequency] = None,
         amortization_type: Union[AmortizationType, str] = None,
         remaining_notional: Optional[float] = None,
         amount: Optional[float] = None,
     ) -> None:
         super().__init__()
         self.start_date = start_date
@@ -99,15 +100,15 @@
         End Date of an amortization section/window, or stepped rate
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def remaining_notional(self):
         """
         The Remaining Notional Amount after Amortization
         :return: float
         """
@@ -123,8 +124,8 @@
         Start Date of an amortization section/window, or stepped rate
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_basket_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_basket_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_day_weight.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_day_weight.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         """
         :return: str
         """
         return self._get_parameter("date")
 
     @date.setter
     def date(self, value):
-        self._set_parameter("date", value)
+        self._set_date_parameter("date", value)
 
     @property
     def weight(self):
         """
         :return: float
         """
         return self._get_parameter("weight")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_fx_point.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_fx_point.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_input_flow.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_input_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf8
 
 
 from typing import Optional
 
+from ...._types import OptDateTime
 from .._enums import PremiumSettlementType
 from .._object_definition import ObjectDefinition
 
 
 class InputFlow(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
@@ -16,24 +17,24 @@
     ----------
     amount : float, optional
 
     premium_settlement_type : PremiumSettlementType, optional
         The cash settlement type of the option premium -spot -forward
     currency : str, optional
 
-    date : str, optional
+    date : str or date or datetime or timedelta, optional
 
     """
 
     def __init__(
         self,
         amount: Optional[float] = None,
         premium_settlement_type: Optional[PremiumSettlementType] = None,
         currency: Optional[str] = None,
-        date: Optional[str] = None,
+        date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.amount = amount
         self.premium_settlement_type = premium_settlement_type
         self.currency = currency
         self.date = date
 
@@ -76,8 +77,8 @@
         """
         :return: str
         """
         return self._get_parameter("date")
 
     @date.setter
     def date(self, value):
-        self._set_parameter("date", value)
+        self._set_date_parameter("date", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_numerical_method.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_numerical_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_payout_scaling.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_payout_scaling.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_models/_pde_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_models/_pde_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_object_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_object_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 import abc
 
+from ..._tools import ipa_datetime_adapter, ipa_date_adapter
 from ..._tools._common import is_all_same_type
 
 
 class ObjectDefinition(abc.ABC):
     """
     This class is designed to represent the instrument definition templates for QPS request.
     """
@@ -86,14 +87,24 @@
     def _set_parameter(self, name, value):
         if value or isinstance(value, int):
             self._dict[name] = value
 
         elif self._dict.get(name):
             self._dict.pop(name)
 
+    def _set_datetime_parameter(self, name, value):
+        if value is not None:
+            value = ipa_datetime_adapter.get_str(value)
+        self._set_parameter(name, value)
+
+    def _set_date_parameter(self, name, value):
+        if value is not None:
+            value = ipa_date_adapter.get_str(value)
+        self._set_parameter(name, value)
+
     def _set_enum_parameter(self, enum_type, name, value):
         if value is None:
             self._dict.pop(name, False)
             return None
 
         result = None
         if isinstance(value, enum_type):
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_cap_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Optional, TYPE_CHECKING, Iterable
 
-from .._object_definition import ObjectDefinition
-
+from ._enums import Axis
 from ._enums import EtiInputVolatilityType
-from ._enums import VolatilityModel
+from ._enums import MoneynessType
 from ._enums import PriceSide
 from ._enums import TimeStamp
-from ._enums import MoneynessType
-from ._enums import Axis
+from ._enums import VolatilityModel
 from ._models import MoneynessWeight
 from ._models import SurfaceFilters
+from .._object_definition import ObjectDefinition
 from ...._tools import try_copy_to_list
 
 if TYPE_CHECKING:
-    from ...._types import OptStr, OptBool
+    from ...._types import OptBool, OptDateTime
 
 
 class EtiSurfaceParameters(ObjectDefinition):
     """
     This class property contains the properties that may be used to control the
     calculation. It mainly covers dates, market data assumptions (e.g. interpolation),
     and pricing model preferences. Some Parameters are common to all volatility surfaces
@@ -56,15 +55,15 @@
         The list of calibration weights that should be applied to different
         MoneynessWeight.
     x_axis : Axis, optional
         Specifies the unit for the x axis (e.g. date, tenor)
     y_axis : Axis, optional
         Specifies the unit for the y axis (e.g. strike, delta). this may depend on the
         asset class. for fx volatility surface, we support both delta and strike.
-    calculation_date : str, optional
+    calculation_date : str or date or datetime or timedelta, optional
         The date the volatility surface is generated.
     svi_alpha_extrapolation : bool, optional
         Svi alpha extrapolation for building the surface default value : true
     """
 
     def __init__(
         self,
@@ -73,15 +72,15 @@
         moneyness_type: Optional[MoneynessType] = None,
         price_side: Optional[PriceSide] = None,
         time_stamp: Optional[TimeStamp] = None,
         volatility_model: Optional[VolatilityModel] = None,
         weights: Optional[Iterable[MoneynessWeight]] = None,
         x_axis: Optional[Axis] = None,
         y_axis: Optional[Axis] = None,
-        calculation_date: "OptStr" = None,
+        calculation_date: "OptDateTime" = None,
         svi_alpha_extrapolation: "OptBool" = None,
     ):
         super().__init__()
         self.filters = filters
         self.input_volatility_type = input_volatility_type
         self.moneyness_type = moneyness_type
         self.price_side = price_side
@@ -222,15 +221,15 @@
         The date the volatility surface is generated.
         :return: str
         """
         return self._get_parameter("calculationDate")
 
     @calculation_date.setter
     def calculation_date(self, value):
-        self._set_parameter("calculationDate", value)
+        self._set_datetime_parameter("calculationDate", value)
 
     @property
     def svi_alpha_extrapolation(self):
         """
         Svi Alpha Extrapolation for building the surface
         Default value : TRUE
         :return: bool
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_eti_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_statistics_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 
+from ...._types import OptDateTime
 from .._object_definition import ObjectDefinition
 
 from ._enums import FxVolatilityModel
 from ._enums import FxSwapCalculationMethod
 from ._enums import PriceSide
 from ._enums import TimeStamp
 from ._enums import Axis
@@ -65,15 +66,15 @@
         on the asset class. for fx volatility surface, we currently support the svi
         model.
     x_axis : Axis, optional
         Specifies the unit for the x axis (e.g. date, tenor)
     y_axis : Axis, optional
         Specifies the unit for the y axis (e.g. strike, delta). this may depend on the
         asset class. for fx volatility surface, we support both delta and strike.
-    calculation_date : str, optional
+    calculation_date : str or date or datetime or timedelta, optional
         The date the volatility surface is generated.
     cutoff_time : str, optional
         The cutoff time
     cutoff_time_zone : str, optional
         The cutoff time zone
     """
 
@@ -92,15 +93,15 @@
         price_side: Optional[PriceSide] = None,
         risk_reversal10_d_object: Optional[BidAskMid] = None,
         risk_reversal25_d_object: Optional[BidAskMid] = None,
         time_stamp: Optional[TimeStamp] = None,
         volatility_model: Optional[FxVolatilityModel] = None,
         x_axis: Optional[Axis] = None,
         y_axis: Optional[Axis] = None,
-        calculation_date: Optional[str] = None,
+        calculation_date: "OptDateTime" = None,
         cutoff_time: Optional[str] = None,
         cutoff_time_zone: Optional[str] = None,
     ):
         super().__init__()
         self.atm_volatility_object = atm_volatility_object
         self.butterfly10_d_object = butterfly10_d_object
         self.butterfly25_d_object = butterfly25_d_object
@@ -344,15 +345,15 @@
         The date the volatility surface is generated.
         :return: str
         """
         return self._get_parameter("calculationDate")
 
     @calculation_date.setter
     def calculation_date(self, value):
-        self._set_parameter("calculationDate", value)
+        self._set_datetime_parameter("calculationDate", value)
 
     @property
     def cutoff_time(self):
         """
         The cutoff time
         :return: str
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_fx_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_i_ir_vol_model_pricing_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ._enums import InputVolatilityType
 from ._models import SurfaceFilters
 from .._enums import PriceSide, TimeStamp
 from .._object_definition import ObjectDefinition
 
 
 if TYPE_CHECKING:
-    from ...._types import OptStr, OptFloat
+    from ...._types import OptStr, OptFloat, OptDateTime
 
 
 class IIrVolModelPricingParameters(ObjectDefinition):
     # new name CapletsStrippingSurfaceParameters in version 1.0.130
     """
     This class property contains the properties that may be used to control the
     calculation. It mainly covers dates, market data assumptions (e.g. interpolation),
@@ -42,30 +42,30 @@
         expressed in percentages. the default value is selected based oninstrumentcode
     source : str, optional
         Requested volatility data contributor.
     stripping_shift_percent : float, optional
         Shift value applied to strikes allowing the stripped caplets surface to include
         volatility even when some strikes are negative. the value is expressed in
         percentages. the default value is '0.0'.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date at which the instrument is valued. the value is expressed in iso 8601
         format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). by default,
         marketdatadate is used. if marketdatadate is not specified, the default value is
         today.
     filters : SurfaceFilters, optional
     price_side : PriceSide, optional
         Specifies whether bid, ask, mid or settle is used to build the surface. if not
         precised, default to mid.
     time_stamp : TimeStamp, optional
         Define how the timestamp is selected:
         - open: the opening value of the valuationdate or if not available the close of
           the previous day is used.
         - default: the latest snapshot is used when valuationdate is today, the close
           price when valuationdate is in the past.
-    calculation_date : str, optional
+    calculation_date : str or date or datetime or timedelta, optional
         The date the volatility surface is generated.
     """
 
     _market_data_date = None
 
     def __init__(
         self,
@@ -74,19 +74,19 @@
         x_axis: Optional[Axis] = None,
         y_axis: Optional[Axis] = None,
         z_axis: Optional[Axis] = None,
         market_data_date=None,
         shift_percent: "OptFloat" = None,
         source: "OptStr" = None,
         stripping_shift_percent: "OptFloat" = None,
-        valuation_date: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
         filters: Optional[SurfaceFilters] = None,
         price_side: Optional[PriceSide] = None,
         time_stamp: Optional[TimeStamp] = None,
-        calculation_date: "OptStr" = None,
+        calculation_date: "OptDateTime" = None,
     ):
         super().__init__()
         self.input_volatility_type = input_volatility_type
         self.volatility_adjustment_type = volatility_adjustment_type
         self.x_axis = x_axis
         self.y_axis = y_axis
         self.z_axis = z_axis
@@ -209,15 +209,15 @@
         """
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
 
     @property
     def filters(self):
         """
         :return: object SurfaceFilters
         """
         return self._get_object_parameter(SurfaceFilters, "filters")
@@ -261,8 +261,8 @@
         The date the volatility surface is generated.
         :return: str
         """
         return self._get_parameter("calculationDate")
 
     @calculation_date.setter
     def calculation_date(self, value):
-        self._set_parameter("calculationDate", value)
+        self._set_datetime_parameter("calculationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_maturity_filter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_moneyness_weight.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_strike_filter_range.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_surface.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     @property
     def z(self):
         return self._matrix
 
     def get_curve(
         self,
         value: Union[str, float, int, np.datetime64],
-        axis: Axis,
+        axis: Union[Axis, str],
     ) -> Curve:
         """
         Get curve
 
         Parameters
         ----------
         value: str, float, int, np.datetime64
@@ -118,17 +118,17 @@
         """
         values = self._values_by_axis.get(axis, [])
 
         value = value_arg_parser.parse(value)
 
         axis_x, axis_y = [], []
 
-        is_axis_x = axis is Axis.X
-        is_axis_y = axis is Axis.Y
-        is_axis_z = axis is Axis.Z
+        is_axis_x = axis == Axis.X
+        is_axis_y = axis == Axis.Y
+        is_axis_z = axis == Axis.Z
 
         # interpolate
         if value not in values and not is_axis_z:
             value = value_arg_parser.get_float(value)
 
             if is_axis_x:
                 axis_x = self._column
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_filters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_surface_output.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_models/_volatility_surface_point.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_surfaces_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_calculation_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ._enums import Axis
 from ._enums import InputVolatilityType
 from .._enums import PriceSide, TimeStamp
 from .._object_definition import ObjectDefinition
 
 
 if TYPE_CHECKING:
-    from ...._types import OptStr, OptFloat, OptBool
+    from ...._types import OptStr, OptFloat, OptBool, OptDateTime
 
 
 class SwaptionCalculationParams(ObjectDefinition):
     # new name VolatilityCubeSurfaceParameters in version 1.0.130
     """
     This class property contains the properties that may be used to control the
     calculation. It mainly covers dates, market data assumptions (e.g. interpolation),
@@ -46,15 +46,15 @@
         expressed in percentages. the default value is selected based oninstrumentcode.
     source : str, optional
         Requested volatility data contributor.
     stripping_shift_percent : float, optional
         Shift value applied to strikes allowing the stripped caplets surface to include
         volatility even when some strikes are negative. the value is expressed in
         percentages. the default value is '0.0'.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date at which the instrument is valued. the value is expressed in iso 8601
         format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). by default,
         marketdatadate is used. if marketdatadate is not specified, the default value is
         today.
     filters : DEPRECATED
         This attribute doesn't use anymore.
     price_side : PriceSide, optional
@@ -62,15 +62,15 @@
         precised, default to mid.
     time_stamp : TimeStamp, optional
         Define how the timestamp is selected:
         - open: the opening value of the valuationdate or if not available the close of
           the previous day is used.
         - default: the latest snapshot is used when valuationdate is today, the close
           price when valuationdate is in the past.
-    calculation_date : str, optional
+    calculation_date : str or date or datetime or timedelta, optional
         The date the volatility surface is generated.
     calibration_type : CalibrationType, optional
         The calibration type defines the solver used during calibration (i.e. sabr model
         calibration optimization method). the default value is selected based
         oninstrumentcode.
     output_volatility_type : VolatilityType, optional
         The sabr volatility can be expressed as lognormal volatility (%) or normal
@@ -104,19 +104,19 @@
         x_axis: Optional[Axis] = None,
         y_axis: Optional[Axis] = None,
         z_axis: Optional[Axis] = None,
         market_data_date=None,
         shift_percent: "OptFloat" = None,
         source: "OptStr" = None,
         stripping_shift_percent: "OptFloat" = None,
-        valuation_date: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
         filters=None,
         price_side: Optional[PriceSide] = None,
         time_stamp: Optional[TimeStamp] = None,
-        calculation_date: "OptStr" = None,
+        calculation_date: "OptDateTime" = None,
         calibration_type: Optional[CalibrationType] = None,
         output_volatility_type: Optional[VolatilityType] = None,
         strike_type: Optional[StrikeType] = None,
         beta: "OptFloat" = None,
         include_caplets_volatility: "OptBool" = None,
         use_smart_params: "OptBool" = None,
     ):
@@ -252,15 +252,15 @@
         """
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
 
     @property
     def filters(self):
         return self._filters
 
     @filters.setter
     def filters(self, value):
@@ -301,15 +301,15 @@
         The date the volatility surface is generated.
         :return: str
         """
         return self._get_parameter("calculationDate")
 
     @calculation_date.setter
     def calculation_date(self, value):
-        self._set_parameter("calculationDate", value)
+        self._set_datetime_parameter("calculationDate", value)
 
     @property
     def calibration_type(self):
         """
         The calibration type defines the solver used during calibration (i.e. sabr model
         calibration optimization method). the default value is selected based
         oninstrumentcode.
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/_surfaces/_swaption_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING
 
 from .._arg_enums import main_constituent_asset_class_arg_parser, risk_type_arg_parser
 from .._base_data_class import BaseData
 from ......delivery._data._endpoint_data import EndpointData
 
 if TYPE_CHECKING:
-    from ......_types import OptStr, OptBool
+    from ......_types import OptStr, OptBool, OptDateTime
     from ...._curves._cross_currency_curves._types import (
         OptMainConstituentAssetClass,
         OptRiskType,
     )
 
 
 curve_info_camel_to_snake = {
@@ -90,15 +90,15 @@
         The risk type to which the generated cross currency curve is sensitive. the
         possible value is:   * 'crosscurrency'
     base_currency : str, optional
         The base currency in the fxcross currency pair. it is expressed in iso 4217
         alphabetical format (e.g., 'eur').
     base_index_name : str, optional
         The name of the floating rate index (e.g., 'estr') applied to the base currency.
-    definition_expiry_date : str, optional
+    definition_expiry_date : str or date or datetime or timedelta, optional
         The date after which curvedefinitions can not be used. the value is expressed in
         iso 8601 format: yyyy-mm-dd (e.g., '2021-01-01').
     first_historical_availability_date : str, optional
         The date starting from which cross currency curve definition can be used. the
         value is expressed in iso 8601 format: yyyy-mm-dd (e.g., '2021-01-01').
     id : str, optional
         The identifier of the cross currency curve.
@@ -128,15 +128,15 @@
 
     def __init__(
         self,
         main_constituent_asset_class: "OptMainConstituentAssetClass" = None,
         risk_type: "OptRiskType" = None,
         base_currency: "OptStr" = None,
         base_index_name: "OptStr" = None,
-        definition_expiry_date: "OptStr" = None,
+        definition_expiry_date: "OptDateTime" = None,
         first_historical_availability_date: "OptStr" = None,
         id: "OptStr" = None,
         is_fallback_for_fx_curve_definition: "OptBool" = None,
         is_non_deliverable: "OptBool" = None,
         name: "OptStr" = None,
         quoted_currency: "OptStr" = None,
         quoted_index_name: "OptStr" = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         alphabetical format (e.g., 'usd').
     quoted_index_name : str, optional
         The name of the floating rate index (e.g., 'sofr') applied to the quoted
         currency.
     source : str, optional
         A user-defined string that is provided by the creator of a curve. curves created
         by refinitiv have the 'refinitiv' source.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date used to define a list of curves or a unique cross currency curve that
         can be priced at this date. the value is expressed in iso 8601 format:
         yyyy-mm-dd (e.g., '2021-01-01').
     extended_params : dict, optional
         If necessary other parameters.
 
     Examples
@@ -89,15 +89,15 @@
         curve_tag: "OptStr" = None,
         id: "OptStr" = None,
         is_non_deliverable: "OptBool" = None,
         name: "OptStr" = None,
         quoted_currency: "OptStr" = None,
         quoted_index_name: "OptStr" = None,
         source: "OptStr" = None,
-        valuation_date: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
         extended_params: "ExtendedParams" = None,
     ) -> None:
         request_item = CrossCurrencyCurveGetDefinitionItem(
             main_constituent_asset_class=main_constituent_asset_class,
             risk_type=risk_type,
             base_currency=base_currency,
             base_index_name=base_index_name,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..._curves._zc_curve_definition_request import ZcCurveDefinitionRequest
 from ...._content_provider_layer import ContentProviderLayer
 from ....._content_type import ContentType
 from ....._tools import create_repr, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import OptStr, ExtendedParams
+    from ....._types import OptStr, ExtendedParams, OptDateTime
     from ..._enums._risk_type import RiskType
     from ..._enums._asset_class import AssetClass
 
 
 class Definition(ContentProviderLayer):
     """
 
@@ -34,15 +34,15 @@
     id : str, optional
         Id of the curve definition
     name : str, optional
         The name of the interest rate curve.
     source : str, optional
         Example:
             "Refinitiv"
-    valuation_date: str, optional
+    valuation_date: str or date, optional
         Example:
             "2019-08-21"
     extended_params : dict, optional
         If necessary other parameters.
     market_data_location : str, optional
         The identifier of the market place from which constituents come from.
         Currently the following values are supported: 'onshore' and 'emea'.
@@ -74,15 +74,15 @@
         main_constituent_asset_class: Optional["AssetClass"] = None,
         risk_type: Optional["RiskType"] = None,
         currency: "OptStr" = None,
         curve_tag: "OptStr" = None,
         id: "OptStr" = None,
         name: "OptStr" = None,
         source: "OptStr" = None,
-        valuation_date: "OptStr" = None,
+        valuation_date: "OptDateTime" = None,
         extended_params: "ExtendedParams" = None,
         market_data_location: "OptStr" = None,
     ) -> None:
         request_item = ZcCurveDefinitionRequest(
             index_name=index_name,
             main_constituent_asset_class=main_constituent_asset_class,
             risk_type=risk_type,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_base_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_base_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_contracts_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,114 +1,137 @@
-from typing import Any, TYPE_CHECKING
+from typing import Any, Callable, TYPE_CHECKING
 
-import pandas as pd
-
-from ...._content_type import ContentType
-from ...._tools import cached_property
-from ....delivery._stream import _RDPStream, StreamStateEvent, StreamStateManager
-from ....delivery._stream._stream_factory import create_rdp_stream
-from ....delivery._stream._stream_listener import RDPStreamListener
+from ._quantitative_data_stream import QuantitativeDataStream
+from ...._core.session import get_valid_session
+from ...._tools import cached_property, create_repr, make_callback
+from ....delivery._stream.base_stream import StreamOpenMixin
 
 if TYPE_CHECKING:
     from ...._types import ExtendedParams
+    from pandas import DataFrame
     from ...._core.session import Session
-    from ....delivery._stream import StreamState
 
 
-class QuantitativeDataStream(StreamStateManager, RDPStreamListener["QuantitativeDataStream"]):
+class Stream(StreamOpenMixin):
+    """
+    Open a streaming quantitative analytic service subscription.
+
+    Parameters
+    ----------
+    universe: dict
+
+    fields: list
+
+    extended_params: dict
+        Default: None
+
+    Methods
+    -------
+    open()
+        Open the QuantitativeDataStream connection
+
+    close()
+        Close the QuantitativeDataStream connection, releases resources
+
+    get_snapshot()
+        Get DataFrame with stream
+
+    """
+
     def __init__(
         self,
         universe: dict,
-        session: "Session",
         fields: list = None,
+        session: "Session" = None,
         extended_params: "ExtendedParams" = None,
-    ):
-        self._session = session
-
-        StreamStateManager.__init__(self, logger=self._session.logger())
-        RDPStreamListener.__init__(self, logger=self._session.logger())
-
+    ) -> None:
         self._universe = universe
         self._fields = fields
+        self._session = get_valid_session(session)
+        self._always_use_default_session = session is None
         self._extended_params = extended_params
 
-        if extended_params and "view" in extended_params:
-            self._column_names = extended_params["view"]
-
-        else:
-            self._column_names = fields or None
-
-        self._data = None
-        self._headers = None
-
-    @property
-    def universe(self):
-        return self._universe
-
-    @property
-    def session(self) -> "Session":
-        return self._session
-
-    @session.setter
-    def session(self, session: "Session"):
-        if self._session != session and not self.is_open:
-            self._session = session
-            RDPStreamListener.init_logger(self, self._session.logger())
-            self._stream.session = self._session
-
     @cached_property
-    def _stream(self) -> _RDPStream:
-        stream = create_rdp_stream(
-            ContentType.STREAMING_CONTRACTS,
-            session=self._session,
-            view=self._fields,
+    def _stream(self) -> QuantitativeDataStream:
+        stream = QuantitativeDataStream(
             universe=self._universe,
+            fields=self._fields,
+            session=self._session,
             extended_params=self._extended_params,
         )
-        stream.on(StreamStateEvent.CLOSED, lambda *_: self.close())
-        stream.on_ack(self._on_stream_ack)
-        stream.on_response(self._on_stream_response)
-        stream.on_update(self._on_stream_update)
-        stream.on_alarm(self._on_stream_alarm)
         return stream
 
-    def __repr__(self):
-        s = super().__repr__()
-        s = s.replace(">", f" {{name='{self._universe}', state={self._stream.state}}}>")
-        return s
-
-    @property
-    def df(self):
-        if self._data is None or self._column_names is None:
-            return pd.DataFrame([])
-        return pd.DataFrame.from_records(self._data, columns=self._column_names)
-
-    def get_snapshot(self) -> pd.DataFrame:
-        return self.df
+    def get_snapshot(self) -> "DataFrame":
+        """
+        Returns DataFrame snapshot a streaming quantitative analytic service
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        return self._stream.get_snapshot()
+
+    def on_response(self, func: Callable[[list, list, "Stream"], Any]) -> "Stream":
+        """
+        This callback is called with the reference to the stream object,
+        the instrument name and the instrument response
+
+        Parameters
+        ----------
+        func : Callable
+            Called when the stream has response
+
+        Returns
+        -------
+        current instance
+        """
+        self._stream.on_response(make_fin_callback(func))
+        return self
+
+    def on_update(self, func: Callable[[list, list, "Stream"], Any]) -> "Stream":
+        """
+        This callback is called with the reference to the stream object,
+        the instrument name and the instrument update
+
+        Parameters
+        ----------
+        func : Callable
+            Called when the stream has a new update
+
+        Returns
+        -------
+        current instance
+        """
+        self._stream.on_update(make_fin_callback(func))
+        return self
+
+    def on_state(self, func: Callable[[list, "Stream"], Any]) -> "Stream":
+        """
+        This callback is called with the reference to the stream object,
+        when the stream has new state
+
+        Parameters
+        ----------
+        func : Callable
+            Called when the stream has a new state
+
+        Returns
+        -------
+        current instance
+        """
+        self._stream.on_alarm(make_callback(func))
+        return self
 
-    def _do_open(self, **kwargs) -> "StreamState":
-        return self._stream.open(**kwargs)
-
-    def _do_close(self, **kwargs) -> "StreamState":
-        return self._stream.close(**kwargs)
-
-    def _do_on_stream_ack(self, stream: _RDPStream, message: dict) -> Any:
-        return message["state"]
-
-    def _do_on_stream_response(self, stream: _RDPStream, message: dict) -> Any:
-        if "data" in message:
-            self._data = message["data"]
-
-        if "headers" in message:
-            self._headers = message["headers"]
-            self._column_names = [col["name"] for col in self._headers]
+    def __repr__(self):
+        return create_repr(
+            self,
+            class_name=self.__class__.__name__,
+        )
 
-        return self._data, self._column_names
 
-    def _do_on_stream_update(self, stream: _RDPStream, message: dict) -> Any:
-        if "data" in message:
-            self._data = message["data"]
+def make_fin_callback(func: Callable[["Stream", list, list], Any]) -> Callable:
+    """Return a callback functions with correct arguments order."""
 
-        return self._data, self._column_names
+    def callback(stream, *args):
+        func(*args, stream)
 
-    def _do_on_stream_alarm(self, stream: _RDPStream, message: dict) -> Any:
-        return message["state"]
+    return callback
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/_definition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,106 @@
-from typing import Any, Callable, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
-from ._quantitative_data_stream import QuantitativeDataStream
-from ...._core.session import get_valid_session
-from ...._tools import cached_property, create_repr, make_callback
-from ....delivery._stream.base_stream import StreamOpenMixin
+from ._pricing_content_provider import PricingData
+from ._stream_facade import Stream
+from .._content_provider_layer import ContentUsageLoggerMixin
+from ..._content_type import ContentType
+from ..._core.session import Session
+from ..._tools import create_repr, try_copy_to_list
+from ..._tools._common import universe_arg_parser, fields_arg_parser
+from ...delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams
-    from pandas import DataFrame
-    from ...._core.session import Session
+    from ..._types import OptStr, ExtendedParams, StrStrings, OptStrStrs
 
 
-class Stream(StreamOpenMixin):
+class Definition(
+    ContentUsageLoggerMixin[BaseResponse[PricingData]],
+    DataProviderLayer[BaseResponse[PricingData]],
+):
     """
-    Open a streaming quantitative analytic service subscription.
+    Creates a definition of information about the specific Pricing data.
 
     Parameters
     ----------
-    universe: dict
-
-    fields: list
-
-    extended_params: dict
-        Default: None
-
-    Methods
-    -------
-    open()
-        Open the QuantitativeDataStream connection
-
-    close()
-        Close the QuantitativeDataStream connection, releases resources
-
-    get_snapshot()
-        Get DataFrame with stream
+    universe : str or list of str
+        Single instrument or list of instruments.
+    fields : str or list of str, optional
+        Single field or list of fields to return.
+    service : str, optional
+        Name of the streaming service publishing the instruments.
+    api: str, optional
+        Specifies the data source for the further retrieval of data.
+    extended_params : dict, optional
+        Specifies the parameters that will be merged with the request.
+
+    Examples
+    --------
+    >>> from refinitiv.data.content import pricing
+    >>> definition = pricing.Definition("EUR=")
+    >>> response = definition.get_data()
 
     """
 
+    _USAGE_CLS_NAME = "Pricing.PricingDefinition"
+
     def __init__(
         self,
-        universe: dict,
-        fields: list = None,
-        session: "Session" = None,
+        universe: "StrStrings",
+        fields: "OptStrStrs" = None,
+        service: "OptStr" = None,
+        api: "OptStr" = None,
         extended_params: "ExtendedParams" = None,
     ) -> None:
+        extended_params = extended_params or {}
+        universe = extended_params.pop("universe", universe)
+        universe = try_copy_to_list(universe)
+        universe = universe_arg_parser.get_list(universe)
+        fields = extended_params.pop("fields", fields)
+        fields = try_copy_to_list(fields)
+        fields = fields_arg_parser.get_unique(fields or [])
+        super().__init__(
+            data_type=ContentType.PRICING,
+            universe=universe,
+            fields=fields,
+            extended_params=extended_params,
+        )
         self._universe = universe
         self._fields = fields
-        self._session = get_valid_session(session)
-        self._always_use_default_session = session is None
+        self._service = service
+        self._api = api
         self._extended_params = extended_params
 
-    @cached_property
-    def _stream(self) -> QuantitativeDataStream:
-        stream = QuantitativeDataStream(
-            universe=self._universe,
-            fields=self._fields,
-            session=self._session,
-            extended_params=self._extended_params,
+    def __repr__(self) -> str:
+        return create_repr(
+            self,
+            content=f"{{name={self._universe}}}",
         )
-        return stream
 
-    def get_snapshot(self) -> "DataFrame":
+    def get_stream(self, session: Session = None) -> Stream:
         """
-        Returns DataFrame snapshot a streaming quantitative analytic service
-
-        Returns
-        -------
-        pd.DataFrame
-        """
-        return self._stream.get_snapshot()
-
-    def on_response(self, func: Callable[[list, list, "Stream"], Any]) -> "Stream":
-        """
-        This callback is called with the reference to the stream object,
-        the instrument name and the instrument response
+        Creates and returns the pricing stream that allows you to get streaming data for previously defined instruments.
 
         Parameters
         ----------
-        func : Callable
-            Called when the stream has response
+        session : Session, optional
+            Session object. If it's not passed the default session will be used.
 
         Returns
         -------
-        current instance
-        """
-        self._stream.on_response(make_fin_callback(func))
-        return self
+        pricing.Stream
 
-    def on_update(self, func: Callable[[list, list, "Stream"], Any]) -> "Stream":
+        Examples
+        --------
+        >>> from refinitiv.data.content import pricing
+        >>> definition = pricing.Definition("IBM")
+        >>> stream = definition.get_stream()
+        >>> stream.open()
         """
-        This callback is called with the reference to the stream object,
-        the instrument name and the instrument update
-
-        Parameters
-        ----------
-        func : Callable
-            Called when the stream has a new update
-
-        Returns
-        -------
-        current instance
-        """
-        self._stream.on_update(make_fin_callback(func))
-        return self
-
-    def on_state(self, func: Callable[[list, "Stream"], Any]) -> "Stream":
-        """
-        This callback is called with the reference to the stream object,
-        when the stream has new state
-
-        Parameters
-        ----------
-        func : Callable
-            Called when the stream has a new state
-
-        Returns
-        -------
-        current instance
-        """
-        self._stream.on_alarm(make_callback(func))
-        return self
-
-    def __repr__(self):
-        return create_repr(
-            self,
-            class_name=self.__class__.__name__,
+        return Stream(
+            universe=self._universe,
+            session=session,
+            fields=self._fields,
+            service=self._service,
+            api=self._api,
+            extended_params=self._extended_params,
         )
-
-
-def make_fin_callback(func: Callable[["Stream", list, list], Any]) -> Callable:
-    """Return a callback functions with correct arguments order."""
-
-    def callback(stream, *args):
-        func(*args, stream)
-
-    return callback
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from ..._enums import (
     DateRollingConvention,
     DayCountBasis,
     InterestType,
     StubRule,
     Frequency,
     AdjustInterestToPaymentDate,
@@ -18,39 +19,39 @@
 
 
 class BondInstrumentDefinition(InstrumentDefinition):
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
         instrument_code: Optional[str] = None,
-        end_date: Optional[str] = None,
+        end_date: "OptDateTime" = None,
         direction: Union[Direction, str] = None,
         interest_type: Union[InterestType, str] = None,
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         fixed_rate_percent: Optional[float] = None,
         spread_bp: Optional[float] = None,
         interest_payment_frequency: Union[Frequency, str] = None,
         interest_calculation_method: Union[DayCountBasis, str] = None,
         accrued_calculation_method: Union[DayCountBasis, str] = None,
         payment_business_day_convention: Union[BusinessDayConvention, str] = None,
         payment_roll_convention: Union[DateRollingConvention, str] = None,
         index_reset_frequency: Union[Frequency, str] = None,
         index_fixing_lag: Optional[int] = None,
-        first_regular_payment_date: Optional[str] = None,
-        last_regular_payment_date: Optional[str] = None,
+        first_regular_payment_date: "OptDateTime" = None,
+        last_regular_payment_date: "OptDateTime" = None,
         amortization_schedule: Optional[AmortizationItem] = None,
         payment_business_days: Optional[str] = None,
         adjust_interest_to_payment_date: Union[AdjustInterestToPaymentDate, str] = None,
         index_compounding_method: Union[IndexCompoundingMethod, str] = None,
         interest_payment_delay: Optional[int] = None,
         stub_rule: Union[StubRule, str] = None,
-        issue_date: Optional[str] = None,
+        issue_date: "OptDateTime" = None,
         index_average_method: Union[IndexAverageMethod, str] = None,
-        first_accrual_date: Optional[str] = None,
+        first_accrual_date: "OptDateTime" = None,
         floor_strike_percent: Optional[float] = None,
         index_fixing_ric: Optional[str] = None,
         is_perpetual: Optional[bool] = None,
         template: Optional[str] = None,
         index_observation_method: Union[IndexObservationMethod, str] = None,
         fixed_rate_percent_schedule: Optional[dict] = None,
         instrument_type: Optional[str] = "Bond",
@@ -319,42 +320,42 @@
         has been defined, value comes from bond reference data.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def first_accrual_date(self):
         """
         Date at which bond starts accruing. Optional. In case an instrument code has
         been defined, value comes from bond reference data. Otherwise default value is
         the issue date of the bond.
         :return: str
         """
         return self._get_parameter("firstAccrualDate")
 
     @first_accrual_date.setter
     def first_accrual_date(self, value):
-        self._set_parameter("firstAccrualDate", value)
+        self._set_datetime_parameter("firstAccrualDate", value)
 
     @property
     def first_regular_payment_date(self):
         """
         The first regular coupon payment date for leg with an odd first coupon.
         Optional.
         :return: str
         """
         return self._get_parameter("firstRegularPaymentDate")
 
     @first_regular_payment_date.setter
     def first_regular_payment_date(self, value):
-        self._set_parameter("firstRegularPaymentDate", value)
+        self._set_datetime_parameter("firstRegularPaymentDate", value)
 
     @property
     def fixed_rate_percent(self):
         """
         The fixed coupon rate in percentage. It is mandatory in case of a single leg
         instrument. Otherwise, in case of multi leg instrument, it can be computed as
         the Par rate.
@@ -470,27 +471,27 @@
         reference data.
         :return: str
         """
         return self._get_parameter("issueDate")
 
     @issue_date.setter
     def issue_date(self, value):
-        self._set_parameter("issueDate", value)
+        self._set_datetime_parameter("issueDate", value)
 
     @property
     def last_regular_payment_date(self):
         """
         The last regular coupon payment date for leg with an odd last coupon. Optional.
         :return: str
         """
         return self._get_parameter("lastRegularPaymentDate")
 
     @last_regular_payment_date.setter
     def last_regular_payment_date(self, value):
-        self._set_parameter("lastRegularPaymentDate", value)
+        self._set_datetime_parameter("lastRegularPaymentDate", value)
 
     @property
     def notional_amount(self):
         """
         The notional amount of the leg at the period start date. Optional. By default
         1,000,000 is used.
         :return: float
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,25 @@
     BenchmarkYieldSelectionMode,
     YieldType,
     QuoteFallbackLogic,
     InflationMode,
 )
 from ..._models import BondRoundingParameters
 from ..._object_definition import ObjectDefinition
+from ....._types import OptDateTime
 
 
 class PricingParameters(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
     Parameters
     ----------
-    trade_date : str, optional
+    trade_date : str or date or datetime or timedelta, optional
         Trade date of the bond. The trade_date is used to compute the default
         valuation_date : By default the rule is that valuation_date = trade_date +
         settlement_convention. Optional. By default, it is equal to market_data_date.
     benchmark_yield_selection_mode : BenchmarkYieldSelectionMode or str, optional
         The benchmark yield.
         Default value is "Interpolate".
     credit_spread_type : CreditSpreadType or str, optional
@@ -246,15 +247,15 @@
         spread. No override is applied by default and yield is computed or retrieved
         from market data.
     issuer_spread_bp : float, optional
         Spread of issuer benchmark to override and that will be used as pricing analysis
         input to compute the bond price. This spread is computed is for coprorate bonds.
         Optional. No override is applied by default. Note that only one pricing anlysis
         input should be defined.
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The market data date for pricing.
         By default, the market_data_date date is the valuation_date or Today
     market_value_in_deal_ccy : float, optional
         Market value in deal currency. This field can be used to compute notionalAmount
         to apply to get this market value. Optional. By default the value is computed
         from notional amount. NotionalAmount field, market_value_in_deal_ccy field and
         market_value_in_report_ccy field cannot be set at defined at the same time.
@@ -304,15 +305,15 @@
         Yield of rating benchmark to override and that will be used to compute rating
         spread. No override is applied by default and yield is computed or retrieved
         from market data.
     rating_spread_bp : float, optional
         Spread of rating benchmark to override and that will be used as pricing analysis
         input to compute the bond price. No override is applied by default.
         Note that only one pricing anlysis input should be defined.
-    redemption_date : str, optional
+    redemption_date : str or date or datetime or timedelta, optional
         Redemption date that defines the end date for yield and price computation. Used
         only if redemption date type is set to "RedemptionAtCustomDate"
     sector_rating_benchmark_curve_yield_percent : float, optional
         Yield of sector rating benchmark to override and that will be used to compute
         sector rating spread. No override is applied by default and yield is computed
         or retrieved from market data.
     sector_rating_spread_bp : float, optional
@@ -375,15 +376,15 @@
         Yield of user defined instrument to override and that will be used to compute
         user defined spread. No override is applied by default and yield is computed
         or retrieved from market data.
     user_defined_spread_bp : float, optional
         Spread of user defined instrument to override and that will be used as pricing
         analysis input to compute the bond price. No override is applied by default.
         Note that only one pricing analysis input should be defined.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The valuation date for pricing. If not set the valuation date is equal
         to market_data_date or Today. For assets that contains a settlement_convention,
         the default valuation date is equal to the settlementdate of the Asset that
         is usually the trade_date+settlement_convention.
     yield_percent : float, optional
         Yield (expressed in percent) to override and that will be used as pricing
         analysis input. No override is applied by default. Note that only one pricing
@@ -405,15 +406,15 @@
     ...    fields=["InstrumentDescription", "MarketDataDate", "Price", "YieldPercent", "ZSpreadBp"]
     ...)
     >>> response = definition.get_data()
     """
 
     def __init__(
         self,
-        trade_date: Optional[str] = None,
+        trade_date: "OptDateTime" = None,
         benchmark_yield_selection_mode: Union[BenchmarkYieldSelectionMode, str] = None,
         credit_spread_type: Union[CreditSpreadType, str] = None,
         dividend_type: Union[DividendType, str] = None,
         fx_price_side: Union[PriceSide, str] = None,
         inflation_mode: Union[InflationMode, str] = None,
         price_side: Union[PriceSide, str] = None,
         projected_index_calculation_method: Union[ProjectedIndexCalculationMethod, str] = None,
@@ -463,29 +464,29 @@
         gov_country_spread_bp: Optional[float] = None,
         government_benchmark_curve_price: Optional[float] = None,
         government_benchmark_curve_yield_percent: Optional[float] = None,
         government_spread_bp: Optional[float] = None,
         is_coupon_payment_adjustedfor_leap_year: Optional[bool] = None,
         issuer_benchmark_curve_yield_percent: Optional[float] = None,
         issuer_spread_bp: Optional[float] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         market_value_in_deal_ccy: Optional[float] = None,
         market_value_in_report_ccy: Optional[float] = None,
         net_price: Optional[float] = None,
         neutral_yield_percent: Optional[float] = None,
         next_coupon_rate_percent: Optional[float] = None,
         ois_zc_benchmark_curve_yield_percent: Optional[float] = None,
         ois_zc_spread_bp: Optional[float] = None,
         option_adjusted_spread_bp: Optional[float] = None,
         price: Optional[float] = None,
         projected_index_percent: Optional[float] = None,
         quoted_price: Optional[float] = None,
         rating_benchmark_curve_yield_percent: Optional[float] = None,
         rating_spread_bp: Optional[float] = None,
-        redemption_date: Optional[str] = None,
+        redemption_date: "OptDateTime" = None,
         report_ccy: Optional[str] = None,
         sector_rating_benchmark_curve_yield_percent: Optional[float] = None,
         sector_rating_spread_bp: Optional[float] = None,
         settlement_convention: Optional[str] = None,
         simple_margin_bp: Optional[float] = None,
         stock_borrow_rate_percent: Optional[float] = None,
         stock_flat_volatility_percent: Optional[float] = None,
@@ -498,15 +499,15 @@
         tax_on_coupon_percent: Optional[float] = None,
         tax_on_price_percent: Optional[float] = None,
         tax_on_yield_percent: Optional[float] = None,
         use_settlement_date_from_quote: Optional[bool] = None,
         user_defined_benchmark_price: Optional[float] = None,
         user_defined_benchmark_yield_percent: Optional[float] = None,
         user_defined_spread_bp: Optional[float] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
         yield_percent: Optional[float] = None,
         z_spread_bp: Optional[float] = None,
     ) -> None:
         super().__init__()
         self.trade_date = trade_date
         self.benchmark_yield_selection_mode = benchmark_yield_selection_mode
         self.credit_spread_type = credit_spread_type
@@ -1446,15 +1447,15 @@
         date is the valuation_date or Today
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def market_value_in_deal_ccy(self):
         """
         Market value in deal currency. This field can be used to compute notionalAmount
         to apply to get this market value. Optional. By default the value is computed
         from notional amount. NotionalAmount field, market_value_in_deal_ccy field and
@@ -1654,15 +1655,15 @@
         only if redemption date type is set to "RedemptionAtCustomDate"
         :return: str
         """
         return self._get_parameter("redemptionDate")
 
     @redemption_date.setter
     def redemption_date(self, value):
-        self._set_parameter("redemptionDate", value)
+        self._set_datetime_parameter("redemptionDate", value)
 
     @property
     def report_ccy(self):
         """
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
@@ -1886,15 +1887,15 @@
         settlement_convention. Optional. By default, it is equal to market_data_date.
         :return: str
         """
         return self._get_parameter("tradeDate")
 
     @trade_date.setter
     def trade_date(self, value):
-        self._set_parameter("tradeDate", value)
+        self._set_datetime_parameter("tradeDate", value)
 
     @property
     def use_settlement_date_from_quote(self):
         """
         Specify whether to use the settlment date of the quote or the one computed from
         the MarketData Date
         :return: bool
@@ -1957,15 +1958,15 @@
         trade_date+settlement_convention.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
 
     @property
     def yield_percent(self):
         """
         Yield (expressed in percent) to override and that will be used as pricing
         analysis input. Optional. No override is applied by default. Note that only one
         pricing analysis input should be defined.
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ..._models import AmortizationItem
 from .._base_definition import BaseDefinition
 from .._contracts_data_provider import bond_instrument_code_arg_parser
 from ..._enums import IndexObservationMethod
 from ....._tools import validate_types, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
 
 
 class Definition(BaseDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
@@ -33,15 +33,15 @@
     ----------
     instrument_code : str, optional
         Code to define the bond instrument.
     instrument_tag : str, optional
         User defined string to identify the instrument. It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         Maturity date of the bond to override. Mandatory if instrument code has not been
         defined and is_perpetual flag has been set to false. In case an instrument code
         has been defined, value comes from bond reference data.
     direction : Direction or str, optional
         The direction of the leg. Optional for a single leg instrument (like a bond),
         in that case default value is Received. It is mandatory for a multi-instrument
         leg instrument (like Swap or CDS leg).
@@ -81,17 +81,17 @@
     index_reset_frequency : Frequency or str, optional
         The reset frequency in case the leg Type is Float.
         By default, the IndexTenor is used.
     index_fixing_lag : int, optional
         Defines the number of working days between the fixing date and the start of the
         coupon period ('InAdvance') or the end of the coupon period ('InArrears').
         By default 0 is used.
-    first_regular_payment_date : str, optional
+    first_regular_payment_date : str or date or datetime or timedelta, optional
         The first regular coupon payment date for leg with an odd first coupon.
-    last_regular_payment_date : str, optional
+    last_regular_payment_date : str or date or datetime or timedelta, optional
         The last regular coupon payment date for leg with an odd last coupon.
     amortization_schedule : AmortizationItem, optional
         Definition of amortizations.
     payment_business_days : str, optional
         A list of coma-separated calendar codes to adjust dates (e.g. 'EMU' or 'USA').
         By default the calendar associated to notional_ccy is used.
     adjust_interest_to_payment_date : AdjustInterestToPaymentDate or str, optional
@@ -106,22 +106,22 @@
         The number of working days between the end of coupon period and the actual
         interest payment date.
         By default, no delay (0) is applied.
     stub_rule : StubRule or str, optional
         The rule that defines whether coupon roll dates are aligned on the  maturity or
         the issue date.
         By default, 'Maturity' is used.
-    issue_date : str, optional
+    issue_date : str or date or datetime or timedelta, optional
         Date of issuance of the bond to override. Mandatory if instrument code has not
         been defined. In case an instrument code has been defined, value comes from bond
         reference data.
     index_average_method :  or str, optional
         The value of the average index calculation method. The possible values are:
         ArithmeticAverage, CompoundedActual, CompoundedAverageRate, DailyCompoundedAverage
-    first_accrual_date : str, optional
+    first_accrual_date : str or date or datetime or timedelta, optional
         Date at which bond starts accruing. In case an instrument code has
         been defined, value comes from bond reference data. Otherwise, default value is
         the issue date of the bond.
     floor_strike_percent : float, optional
         The contractual strike rate of the floor. The value is expressed in percentages.
         If this parameter is set, the floor will apply to the leg with the same
         parameters set in the swapLegDefinition (e.g.maturity, frequency, index,
@@ -199,39 +199,39 @@
     >>> response = definition.get_stream()
     """
 
     def __init__(
         self,
         instrument_code: Optional[str] = None,
         instrument_tag: Optional[str] = None,
-        end_date: Optional[str] = None,
+        end_date: "OptDateTime" = None,
         direction: Union[Direction, str] = None,
         interest_type: Union[InterestType, str] = None,
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         fixed_rate_percent: Optional[float] = None,
         spread_bp: Optional[float] = None,
         interest_payment_frequency: Union[Frequency, str] = None,
         interest_calculation_method: Union[DayCountBasis, str] = None,
         accrued_calculation_method: Union[DayCountBasis, str] = None,
         payment_business_day_convention: Union[BusinessDayConvention, str] = None,
         payment_roll_convention: Union[DateRollingConvention, str] = None,
         index_reset_frequency: Union[Frequency, str] = None,
         index_fixing_lag: Optional[int] = None,
-        first_regular_payment_date: Optional[str] = None,
-        last_regular_payment_date: Optional[str] = None,
+        first_regular_payment_date: "OptDateTime" = None,
+        last_regular_payment_date: "OptDateTime" = None,
         amortization_schedule: Optional[AmortizationItem] = None,
         payment_business_days: Optional[str] = None,
         adjust_interest_to_payment_date: Union[AdjustInterestToPaymentDate, str] = None,
         index_compounding_method: Union[IndexCompoundingMethod, str] = None,
         interest_payment_delay: Optional[int] = None,
         stub_rule: Union[StubRule, str] = None,
-        issue_date: Optional[str] = None,
+        issue_date: "OptDateTime" = None,
         index_average_method: Union[IndexAverageMethod, str] = None,
-        first_accrual_date: Optional[str] = None,
+        first_accrual_date: "OptDateTime" = None,
         floor_strike_percent: Optional[float] = None,
         index_fixing_ric: Optional[str] = None,
         is_perpetual: Optional[bool] = None,
         template: Optional[str] = None,
         fields: "OptStrStrs" = None,
         pricing_parameters: Optional[PricingParameters] = None,
         extended_params: "ExtendedParams" = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
+from .._instrument_definition import InstrumentDefinition
 from ..._enums import (
     AdjustInterestToPaymentDate,
     BusinessDayConvention,
     BuySell,
     DateRollingConvention,
     DayCountBasis,
     Frequency,
@@ -15,23 +17,22 @@
     PriceSide,
 )
 from ..._models import (
     AmortizationItem,
     BarrierDefinitionElement,
     InputFlow,
 )
-from .._instrument_definition import InstrumentDefinition
 
 
 class CapFloorInstrumentDefinition(InstrumentDefinition):
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         index_name: Optional[str] = None,
         index_tenor: Optional[str] = None,
         interest_payment_frequency: Union[Frequency, str] = None,
         interest_calculation_method: Union[DayCountBasis, str] = None,
@@ -351,15 +352,15 @@
         forward by tenor.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def floor_digital_payout_percent(self):
         """
         A percentage of notionalamount that is received (paid) by the option buyer
         (seller) if the option expires on or below the floor strike. no default value
         applies.
@@ -544,15 +545,15 @@
         valuationdate shifted forward by a month using market conventions.
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def tenor(self):
         """
         The code indicating the tenor of the instrument (e.g. '5m'). mandatory if
         enddate is not provided. no default value applies.
         :return: str
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from ..._enums import (
     IndexConvexityAdjustmentIntegrationMethod,
     IndexConvexityAdjustmentMethod,
     PriceSide,
 )
 from ..._object_definition import ObjectDefinition
 
@@ -19,27 +20,27 @@
     ----------
     index_convexity_adjustment_integration_method : IndexConvexityAdjustmentIntegrationMethod, optional
 
     index_convexity_adjustment_method : IndexConvexityAdjustmentMethod, optional
 
     price_side : PriceSide or str, optional
         The quoted price side of the instrument. optional. default value is 'mid'.
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The market data date for pricing. Optional. By default, the marketDataDate date
         is the ValuationDate or Today
     market_value_in_deal_ccy : float, optional
         MarketValueInDealCcy to override and that will be used as pricing analysis input
         to compute VolatilityPercent. Optional. No override is applied by default. Note
         that Premium takes priority over Volatility input.
     report_ccy : str, optional
         Valuation is performed in deal currency. If a report currency is set, valuation
         is done in that report currency.
     skip_first_cap_floorlet : bool, optional
         Indicates whether to take in consideration the first caplet
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The valuation date for pricing.  Optional. If not set the valuation date is
         equal to MarketDataDate or Today. For assets that contains a
         settlementConvention, the default valuation date  is equal to the settlementdate
         of the Asset that is usually the TradeDate+SettlementConvention.
     implied_volatility_bp : float, optional
         User defined implied normal volatility, expressed in basis points.
     implied_volatility_percent : float, optional
@@ -47,19 +48,19 @@
     """
 
     def __init__(
         self,
         index_convexity_adjustment_integration_method: Optional[IndexConvexityAdjustmentIntegrationMethod] = None,
         index_convexity_adjustment_method: Optional[IndexConvexityAdjustmentMethod] = None,
         price_side: Union[PriceSide, str] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         market_value_in_deal_ccy: Optional[float] = None,
         report_ccy: Optional[str] = None,
         skip_first_cap_floorlet: Optional[bool] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
         implied_volatility_bp: Optional[float] = None,
         implied_volatility_percent: Optional[float] = None,
     ) -> None:
         super().__init__()
         self.index_convexity_adjustment_integration_method = index_convexity_adjustment_integration_method
         self.index_convexity_adjustment_method = index_convexity_adjustment_method
         self.price_side = price_side
@@ -119,15 +120,15 @@
         is the ValuationDate or Today
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def market_value_in_deal_ccy(self):
         """
         MarketValueInDealCcy to override and that will be used as pricing analysis input
         to compute VolatilityPercent. Optional. No override is applied by default. Note
         that Premium takes priority over Volatility input.
@@ -173,15 +174,15 @@
         of the Asset that is usually the TradeDate+SettlementConvention.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
 
     @property
     def implied_volatility_bp(self):
         return self._get_parameter("impliedVolatilityBp")
 
     @implied_volatility_bp.setter
     def implied_volatility_bp(self, value):
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 )
 from .._base_definition import BaseDefinition
 from ..._enums import InterestCalculationConvention
 from ..._models import InputFlow
 from ....._tools import validate_types, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
 
 
 class Definition(BaseDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
     Parameters
     ----------
     instrument_tag : str, optional
         User defined string to identify the instrument.It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported. Optional.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         The option start date
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity date of the CapFloor
     tenor : str, optional
         Tenor of the option
     notional_ccy : str, optional
         The ISO code of the notional currency. Mandatory if instrument code or
         instrument style has not been defined. In case an instrument code/style has been
         defined, value may comes from the reference data.
@@ -184,16 +184,16 @@
 
     >>> response = definition.get_stream()
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         index_name: Optional[str] = None,
         index_tenor: Optional[str] = None,
         interest_payment_frequency: Union[Frequency, str] = None,
         interest_calculation_method: Union[DayCountBasis, str] = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from .._instrument_definition import InstrumentDefinition
 from ..._enums import (
     BusinessDayConvention,
     CdsConvention,
 )
 from ._premium_leg_definition import PremiumLegDefinition
 from ._protection_leg_definition import ProtectionLegDefinition
@@ -23,23 +24,23 @@
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported. Optional.
     instrument_code : str, optional
         A cds RIC that is used to retrieve the description of the cds contract.
         Optional. If null, the protection_leg and the premium_leg  must be provided.
     cds_convention : CdsConvention or str, optional
         Define the cds convention. Optional. Defaults to 'ISDA'.
-    trade_date : str, optional
+    trade_date : str or date or datetime or timedelta, optional
         The date the cds contract was created. Optional. By default the valuation date.
-    step_in_date : str, optional
+    step_in_date : str or date or datetime or timedelta, optional
         The effective protection date. Optional. By default the trade_date + 1 calendar.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         The date the cds starts accruing interest. Its effective date. Optional. By
         default it is the accrued_begin_date (the last IMM date before trade_date) if
         cds_convention is ISDA, else it is the step_in_date.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity date of the cds contract. Mandatory if instrument_code is null.
         Either the end_date or the tenor must be provided.
     tenor : str, optional
         The period code that represents the time between the start date and end date the
         contract. Mandatory if instrument_code is null. Either the end_date or the tenor
         must be provided.
     start_date_moving_convention : BusinessDayConvention or str, optional
@@ -56,34 +57,34 @@
           is ISDA, else false is used.
     protection_leg : ProtectionLegDefinition, optional
         The Protection Leg of the CDS. It is the default leg. Mandatory if
         instrument_code is null. Optional if instrument_code not null.
     premium_leg : PremiumLegDefinition, optional
         The Premium Leg of the CDS. It is a swap leg paying a fixed coupon. Mandatory if
         instrument_code is null. Optional if instrument_code not null.
-    accrued_begin_date : str, optional
+    accrued_begin_date : str or date or datetime or timedelta, optional
         The last cashflow date. Optional. By default it is the last cashflow date.
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
         instrument_code: Optional[str] = None,
         cds_convention: Union[CdsConvention, str] = None,
-        trade_date: Optional[str] = None,
-        step_in_date: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        trade_date: "OptDateTime" = None,
+        step_in_date: "OptDateTime" = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         start_date_moving_convention: Union[BusinessDayConvention, str] = None,
         end_date_moving_convention: Union[BusinessDayConvention, str] = None,
         adjust_to_isda_end_date: Optional[bool] = None,
         protection_leg: Optional[ProtectionLegDefinition] = None,
         premium_leg: Optional[PremiumLegDefinition] = None,
-        accrued_begin_date: Optional[str] = None,
+        accrued_begin_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.instrument_tag = instrument_tag
         self.instrument_code = instrument_code
         self.cds_convention = cds_convention
         self.trade_date = trade_date
         self.step_in_date = step_in_date
@@ -192,15 +193,15 @@
         The last cashflow date. Optional. By default it is the last cashflow date.
         :return: str
         """
         return self._get_parameter("accruedBeginDate")
 
     @accrued_begin_date.setter
     def accrued_begin_date(self, value):
-        self._set_parameter("accruedBeginDate", value)
+        self._set_datetime_parameter("accruedBeginDate", value)
 
     @property
     def adjust_to_isda_end_date(self):
         """
         The way the end_date is adjusted if computed from tenor input.    The possible
         values are:
         - true ( the end_date is an IMM date computed from start_date according to ISDA
@@ -223,15 +224,15 @@
         Either the end_date or the tenor must be provided.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def instrument_code(self):
         """
         A cds RIC that is used to retrieve the description of the cds contract.
         Optional. If null, the protection_leg and the premium_leg  must be provided.
         :return: str
@@ -250,27 +251,27 @@
         cds_convention is ISDA, else it is the step_in_date.
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def step_in_date(self):
         """
         The effective protection date. Optional. By default the trade_date + 1 calendar.
         :return: str
         """
         return self._get_parameter("stepInDate")
 
     @step_in_date.setter
     def step_in_date(self, value):
-        self._set_parameter("stepInDate", value)
+        self._set_date_parameter("stepInDate", value)
 
     @property
     def tenor(self):
         """
         The period code that represents the time between the start date and end date the
         contract. Mandatory if instrument_code is null. Either the end_date or the tenor
         must be provided.
@@ -288,8 +289,8 @@
         The date the cds contract was created. Optional. By default the valuation date.
         :return: str
         """
         return self._get_parameter("tradeDate")
 
     @trade_date.setter
     def trade_date(self, value):
-        self._set_parameter("tradeDate", value)
+        self._set_date_parameter("tradeDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional
 
+from ....._types import OptDateTime
 from ..._object_definition import ObjectDefinition
 
 
 class PricingParameters(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
@@ -20,46 +21,46 @@
         clean_price_percent to override and that will be used as pricing analysis input
         to compute the cds other outputs. Optional. No override is applied by default.
         Note that only one pricing analysis input should be defined.
     conventional_spread_bp : float, optional
         conventional_spread_bp to override and that will be used as pricing analysis
         input to compute the cds other outputs. Optional. No override is applied by
         default. Note that only one pricing analysis input should be defined.
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The market data date for pricing. Optional. By default, the market_data_date
         date is the valuation_date or Today
     report_ccy : str, optional
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
     upfront_amount_in_deal_ccy : float, optional
         upfront_amount_in_deal_ccy to override and that will be used as pricing analysis
         input to compute the cds other outputs. Optional. No override is applied by
         default. Note that only one pricing analysis input should be defined.
     upfront_percent : float, optional
         upfront_percent to override and that will be used as pricing analysis input to
         compute the cds other outputs. Optional. No override is applied by default. Note
         that only one pricing analysis input should be defined.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The valuation date for pricing.  Optional. If not set the valuation date is
         equal to market_data_date or Today. For assets that contains a
         settlementConvention, the default valuation date  is equal to the settlementdate
         of the Asset that is usually the TradeDate+SettlementConvention.
     """
 
     def __init__(
         self,
         cash_amount_in_deal_ccy: Optional[float] = None,
         clean_price_percent: Optional[float] = None,
         conventional_spread_bp: Optional[float] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         report_ccy: Optional[str] = None,
         upfront_amount_in_deal_ccy: Optional[float] = None,
         upfront_percent: Optional[float] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.cash_amount_in_deal_ccy = cash_amount_in_deal_ccy
         self.clean_price_percent = clean_price_percent
         self.conventional_spread_bp = conventional_spread_bp
         self.market_data_date = market_data_date
         self.report_ccy = report_ccy
@@ -116,15 +117,15 @@
         date is the valuation_date or Today
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def report_ccy(self):
         """
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). It is set for the fields ending with 'xxxinreportccy'. Optional. The
         default value is the notional currency.
@@ -173,8 +174,8 @@
         of the Asset that is usually the TradeDate+SettlementConvention.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from ._premium_leg_definition import PremiumLegDefinition
 from ._protection_leg_definition import ProtectionLegDefinition
 from .._base_definition import BaseDefinition
 from ....._tools import try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
 
 
 class Definition(BaseDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
@@ -29,23 +29,23 @@
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported. Optional.
     instrument_code : str, optional
         A cds RIC that is used to retrieve the description of the cds contract.
         Optional. If null, the protection_leg and the premium_leg  must be provided.
     cds_convention : CdsConvention, optional
         Define the cds convention. Optional. Defaults to 'ISDA'.
-    trade_date : str, optional
+    trade_date : str or date, optional
         The date the cds contract was created. Optional. By default the valuation date.
-    step_in_date : str, optional
+    step_in_date : str or date, optional
         The effective protection date. Optional. By default the trade_date + 1 calendar.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         The date the cds starts accruing interest. Its effective date. Optional. By
         default it is the accrued_begin_date (the last IMM date before trade_date) if
         cds_convention is ISDA, else it is the step_in_date.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity date of the cds contract. Mandatory if instrument_code is null.
         Either the end_date or the tenor must be provided.
     tenor : str, optional
         The period code that represents the time between the start date and end date the
         contract. Mandatory if instrument_code is null. Either the end_date or the tenor
         must be provided.
     start_date_moving_convention : BusinessDayConvention, optional
@@ -118,25 +118,25 @@
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
         instrument_code: Optional[str] = None,
         cds_convention: Optional[CdsConvention] = None,
-        trade_date: Optional[str] = None,
-        step_in_date: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        trade_date: "OptDateTime" = None,
+        step_in_date: "OptDateTime" = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         start_date_moving_convention: Optional[BusinessDayConvention] = None,
         end_date_moving_convention: Optional[BusinessDayConvention] = None,
         adjust_to_isda_end_date: Optional[bool] = None,
         protection_leg: Optional[ProtectionLegDefinition] = None,
         premium_leg: Optional[PremiumLegDefinition] = None,
-        accrued_begin_date: Optional[str] = None,
+        accrued_begin_date: "OptDateTime" = None,
         fields: "OptStrStrs" = None,
         pricing_parameters: Optional[PricingParameters] = None,
         extended_params: "ExtendedParams" = None,
     ):
         fields = try_copy_to_list(fields)
         definition = CdsInstrumentDefinition(
             cds_convention=cds_convention,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from .._instrument_definition import ObjectDefinition
 from ..._enums import (
     BusinessDayConvention,
     DayCountBasis,
     Direction,
     Frequency,
     StubRule,
@@ -42,18 +43,18 @@
     accrued_calculation_method : DayCountBasis or str, optional
         The Day Count Basis method used to calculate the accrued interest payments.
         Optional. By default, the same value than interest_calculation_method is used.
     payment_business_day_convention : BusinessDayConvention or str, optional
         The method to adjust dates to a working day. Optional.
         In case an instrument code/style has been defined, value comes from
         bond reference data. Otherwise 'ModifiedFollowing' is used.
-    first_regular_payment_date : str, optional
+    first_regular_payment_date : str or date or datetime or timedelta, optional
         The first regular coupon payment date for leg with an odd first coupon.
         Optional.
-    last_regular_payment_date : str, optional
+    last_regular_payment_date : str or date or datetime or timedelta, optional
         The last regular coupon payment date for leg with an odd last coupon. Optional.
     payment_business_days : str, optional
         A list of coma-separated calendar codes to adjust dates (e.g. 'EMU' or 'USA').
         Optional. By default the calendar associated to notional_ccy is used.
     stub_rule : StubRule or str, optional
         The rule that defines whether coupon roll dates are aligned on the  maturity or
         the issue date. Optional. By default 'Maturity' is used.
@@ -73,16 +74,16 @@
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         fixed_rate_percent: Optional[float] = None,
         interest_payment_frequency: Union[Frequency, str] = None,
         interest_calculation_method: Union[DayCountBasis, str] = None,
         accrued_calculation_method: Union[DayCountBasis, str] = None,
         payment_business_day_convention: Union[BusinessDayConvention, str] = None,
-        first_regular_payment_date: Optional[str] = None,
-        last_regular_payment_date: Optional[str] = None,
+        first_regular_payment_date: "OptDateTime" = None,
+        last_regular_payment_date: "OptDateTime" = None,
         payment_business_days: Optional[str] = None,
         stub_rule: Union[StubRule, str] = None,
         accrued_paid_on_default: Optional[bool] = None,
         interest_payment_ccy: Optional[str] = None,
     ) -> None:
         super().__init__()
         self.direction = direction
@@ -232,15 +233,15 @@
         Optional.
         :return: str
         """
         return self._get_parameter("firstRegularPaymentDate")
 
     @first_regular_payment_date.setter
     def first_regular_payment_date(self, value):
-        self._set_parameter("firstRegularPaymentDate", value)
+        self._set_datetime_parameter("firstRegularPaymentDate", value)
 
     @property
     def fixed_rate_percent(self):
         """
         The fixed coupon rate in percentage. It is mandatory in case of a single leg
         instrument. Otherwise, in case of multi leg instrument, it can be computed as
         the Par rate.
@@ -270,15 +271,15 @@
         The last regular coupon payment date for leg with an odd last coupon. Optional.
         :return: str
         """
         return self._get_parameter("lastRegularPaymentDate")
 
     @last_regular_payment_date.setter
     def last_regular_payment_date(self, value):
-        self._set_parameter("lastRegularPaymentDate", value)
+        self._set_datetime_parameter("lastRegularPaymentDate", value)
 
     @property
     def notional_amount(self):
         """
         The notional amount of the leg at the period start date. Optional. By default
         1,000,000 is used.
         :return: float
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from .._instrument_definition import ObjectDefinition
 from ..._enums import (
     FxLegType,
     BuySell,
 )
 
 
 class LegDefinition(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
     Parameters
     ----------
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
 
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity date of the contract that is the date the amounts are exchanged.
         Either the end_date or the tenor must be provided.
     tenor : str, optional
         The tenor representing the maturity date of the contract (e.g. '1Y' or '6M' ).
         Either the end_date or the tenor must be provided.
     leg_tag : str, optional
         A user defined string to identify the leg. Optional.
@@ -49,16 +50,16 @@
         The tenor representing the Starting of maturity period of the contract (e.g.
         '1Y' or '6M' ). Either the start_date or the start_tenor must be provided for
         TimeOptionForward.
     """
 
     def __init__(
         self,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         leg_tag: Optional[str] = None,
         deal_ccy_buy_sell: Union[BuySell, str] = None,
         fx_leg_type: Union[FxLegType, str] = None,
         contra_amount: Optional[float] = None,
         contra_ccy: Optional[str] = None,
         deal_amount: Optional[float] = None,
@@ -165,15 +166,15 @@
         Either the end_date or the tenor must be provided.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def leg_tag(self):
         """
         A user defined string to identify the leg. Optional.
         :return: str
         """
@@ -188,15 +189,15 @@
         """
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def start_tenor(self):
         """
         The tenor representing the Starting of maturity period of the contract (e.g.
         '1Y' or '6M' ). Either the start_date or the Starttenor must be provided for
         TimeOptionForward.
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from ..._enums import PriceSide, FxSwapCalculationMethod, ImpliedDepositDateConvention
 from ..._object_definition import ObjectDefinition
 
 
 class PricingParameters(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
@@ -38,47 +39,47 @@
           optional. defaults to 'false'.
     ignore_ref_ccy_holidays : bool, optional
         An indicator if holidays of the reference currency are included or not in the
         pricing when dates are computed. by default, the reference currency is usd. the
         possible values are:
         - true: holidays are ignored,
         - false: holidays are included in pricing. optional. defaults to 'false'.
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The date at which the market data is retrieved. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). it
         should be less or equal tovaluationdate). optional. by
         default,marketdatadateisvaluationdateor today.
     report_ccy : str, optional
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
     use_direct_quote : bool, optional
         An indicator if the spot and the swap points should be retrieved without a pivot
         currency
         - true: the market data is retrieved directly
         - false: unmodified market data is returned. optional. defaults to 'false'.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The valuation date for pricing.  Optional. If not set the valuation date is
         equal to market_data_date or Today. For assets that contains a
         settlementConvention, the default valuation date  is equal to the settlementdate
         of the Asset that is usually the TradeDate+SettlementConvention.
     """
 
     def __init__(
         self,
         fx_swap_calculation_method: Union[FxSwapCalculationMethod, str] = None,
         implied_deposit_date_convention: Union[ImpliedDepositDateConvention, str] = None,
         price_side: Union[PriceSide, str] = None,
         adjust_all_deposit_points_to_cross_calendars: Optional[bool] = None,
         adjust_all_swap_points_to_cross_calendars: Optional[bool] = None,
         ignore_ref_ccy_holidays: Optional[bool] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         report_ccy: Optional[str] = None,
         use_direct_quote: Optional[bool] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.fx_swap_calculation_method = fx_swap_calculation_method
         self.implied_deposit_date_convention = implied_deposit_date_convention
         self.price_side = price_side
         self.adjust_all_deposit_points_to_cross_calendars = adjust_all_deposit_points_to_cross_calendars
         self.adjust_all_swap_points_to_cross_calendars = adjust_all_swap_points_to_cross_calendars
@@ -182,15 +183,15 @@
         date is the valuation_date or Today
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def report_ccy(self):
         """
         :return: str
         """
         return self._get_parameter("reportCcy")
@@ -223,8 +224,8 @@
         of the Asset that is usually the TradeDate+SettlementConvention.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 from ._option_instrument_definition import OptionInstrumentDefinition
 from ._option_pricing_parameters import PricingParameters
 from .._base_definition import BaseDefinition
 from ..._models import InputFlow
 from ....._tools import validate_types, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
     from ...financial_contracts._stream_facade import Stream
     from ....._core.session import Session
 
 
 class Definition(BaseDefinition):
     """
     Parameters
     ----------
     instrument_tag : str, optional
         User defined string to identify the instrument.It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported. Optional.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         Expiry date of the option
     buy_sell : BuySell or str, optional
         The side of the deal.
     call_put : CallPut or str, optional
         Tells if the option is a call or a put.
     exercise_style : ExerciseStyle or str, optional
         EURO or AMER
@@ -73,27 +73,27 @@
         Details for double binary option.
     dual_currency_definition : FxDualCurrencyDefinition, optional
         Details for dual currency option.
     forward_start_definition : FxOptionForwardStart, optional
         Details for Forward Start option.
     underlying_definition : FxUnderlyingDefinition, EtiUnderlyingDefinition, optional
         Details of the underlying. Can be used to override some data of the underlying.
-    delivery_date : str, optional
+    delivery_date : str or date or datetime or timedelta, optional
         Expiry date of the option
     instrument_code : str, optional
         An option RIC that is used to retrieve the description of the
         EtiOptionDefinition contract. Optional.If null, the instrument_code of
         underlying_definition must be provided.
     cbbc_definition : EtiOptionCbbcDefinition, optional
         Details for CBBC (Call Bear/Bull Contract) option.
     double_barriers_definition : EtiOptionDoubleBarriersDefinition, optional
         Details for double barriers option.
     deal_contract : int, optional
         deal_contract. It is the number of contracts bought or sold in the deal.
-    end_date_time : str, optional
+    end_date_time : str or date or datetime or timedelta, optional
         Expiry date time of the option
     lot_size : float, optional
         The lot size. It is the number of options bought or sold in one transaction.
     offset : int, optional
         offset. The offset in minutes between the time UTC and the time of the exchange
         where the contract is traded.
     fields: list of str, optional
@@ -143,32 +143,32 @@
         asian_definition: Union[EtiFixingInfo, FxAverageInfo] = None,
         barrier_definition: Union[FxBarrierDefinition, EtiBarrierDefinition] = None,
         binary_definition: Union[FxBinaryDefinition, EtiBinaryDefinition] = None,
         buy_sell: Union[BuySell, str] = None,
         call_put: Union[CallPut, str] = None,
         cbbc_definition: Optional[EtiCbbcDefinition] = None,
         deal_contract: Optional[int] = None,
-        delivery_date: Optional[str] = None,
+        delivery_date: "OptDateTime" = None,
         double_barrier_definition: Optional[FxDoubleBarrierDefinition] = None,
         double_barriers_definition: Optional[EtiDoubleBarriersDefinition] = None,
         double_binary_definition: Union[FxDoubleBinaryDefinition] = None,
         dual_currency_definition: Optional[FxDualCurrencyDefinition] = None,
-        end_date: Optional[str] = None,
-        end_date_time: Optional[str] = None,
+        end_date: "OptDateTime" = None,
+        end_date_time: "OptDateTime" = None,
         exercise_style: Union[ExerciseStyle, str] = None,
         forward_start_definition: Optional[FxForwardStart] = None,
         instrument_code: Optional[str] = None,
         instrument_tag: Optional[str] = None,
         lot_size: Optional[float] = None,
         notional_amount: Optional[float] = None,
         notional_ccy: Optional[str] = None,
         payments: Optional[InputFlow] = None,
         settlement_ccy: Optional[str] = None,
         settlement_type: Union[SettlementType, str] = None,
-        start_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
         strike: Optional[float] = None,
         tenor: Optional[str] = None,
         time_zone_offset: Optional[int] = None,
         underlying_definition: Union[FxUnderlyingDefinition, EtiUnderlyingDefinition] = None,
         underlying_type: Union[UnderlyingType, str] = None,
         fields: "OptStrStrs" = None,
         pricing_parameters: Optional[PricingParameters] = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_enums/_fx_binary_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_cbbc_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ......_types import OptDateTime
 from .._base import UnderlyingDefinition
 from ..._instrument_definition import InstrumentDefinition
 from .._enums import (
     BuySell,
     CallPut,
     ExerciseStyle,
     UnderlyingType,
@@ -26,15 +27,15 @@
         User defined string to identify the instrument.It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported. Optional.
     instrument_code : str, optional
         An option RIC that is used to retrieve the description of the
         EtiOptionDefinition contract. Optional.If null, the instrument_code of
         underlying_definition must be provided.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         Expiry date of the option
     asian_definition : EtiOptionFixingInfo, optional
         Fixing details for asian options
     barrier_definition : EtiOptionBarrierDefinition, optional
         Details for barrier option.
     binary_definition : EtiOptionBinaryDefinition, optional
         Details for binary option.
@@ -50,43 +51,43 @@
         EURO or AMER
     underlying_definition : EtiUnderlyingDefinition, optional
         Details of the underlying. Can be used to override some data of the underlying.
     underlying_type : UnderlyingType or str, optional
         Underlying type of the option.
     deal_contract : int, optional
         deal_contract. It is the number of contracts bought or sold in the deal.
-    end_date_time : str, optional
+    end_date_time : str or date or datetime or timedelta, optional
         Expiry date time of the option
     lot_size : float, optional
         The lot size. It is the number of options bought or sold in one transaction.
     offset : int, optional
         offset. The offset in minutes between the time UTC and the time of the exchange
         where the contract is traded.
     strike : float, optional
         strike of the option
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
         instrument_code: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         asian_definition: Optional[EtiFixingInfo] = None,
         barrier_definition: Optional[EtiBarrierDefinition] = None,
         binary_definition: Optional[EtiBinaryDefinition] = None,
         buy_sell: Union[BuySell, str] = None,
         call_put: Union[CallPut, str] = None,
         cbbc_definition: Optional[EtiCbbcDefinition] = None,
         double_barriers_definition: Optional[EtiDoubleBarriersDefinition] = None,
         exercise_style: Union[ExerciseStyle, str] = None,
         underlying_definition: Optional[EtiUnderlyingDefinition] = None,
         underlying_type: Union[UnderlyingType, str] = None,
         deal_contract: Optional[int] = None,
-        end_date_time: Optional[str] = None,
+        end_date_time: "OptDateTime" = None,
         lot_size: Optional[float] = None,
         strike: Optional[float] = None,
         time_zone_offset: Optional[int] = None,
         **kwargs,
     ) -> None:
         super().__init__(instrument_tag, **kwargs)
         self.instrument_tag = instrument_tag
@@ -264,29 +265,29 @@
         instrument reference data.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def end_date_time(self):
         """
         The expiry date and time of the instrument at the exchange where it is traded.
         the value is expressed in iso 8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g.,
         '2021-01-01t00:00:00z'). optional. no default value applies.
         :return: str
         """
         return self._get_parameter("endDateTime")
 
     @end_date_time.setter
     def end_date_time(self, value):
-        self._set_parameter("endDateTime", value)
+        self._set_datetime_parameter("endDateTime", value)
 
     @property
     def instrument_code(self):
         """
         The code (an option ric) used to define the instrument. optional. mandatory for
         listed eti options. for otc eti options instrumentcode of the underlying asset
         must be provided. no default value applies.
@@ -333,15 +334,15 @@
         Start date of the option
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def strike(self):
         """
         The set price at which the owner of the option can buy or sell the underlying
         asset. the value is expressed according to the market convention linked to the
         underlying asset. optional. mandatory for otc eti options and fx options. if
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_double_barriers_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ......_types import OptDateTime
 from .._base import Info
 from .._enums import (
     AverageType,
     FixingFrequency,
 )
 
 
-class EtiFixingInfo(Info):
+class FxAverageInfo(Info):
     """
     Parameters
     ----------
     average_type : AverageType or str, optional
         The type of average used to compute.
     fixing_frequency : FixingFrequency or str, optional
         The fixing's frequency.
     average_so_far : float, optional
         The value of the average_type
-    fixing_calendar : str, optional
-        The calendar of the underlying's currency.
-    fixing_end_date : str, optional
-        The end date of the fixing period. Should be less or equal to the expiry.
-    fixing_start_date : str, optional
+    fixing_ric_source : str, optional
+        The fixing's RIC source. Default value: the first available source RIC of the Fx
+        Cross Code
+    fixing_start_date : str or date or datetime or timedelta, optional
         The beginning date of the fixing period.
     include_holidays : bool, optional
         Include the holidays in the list of fixings
     include_week_ends : bool, optional
         Include the week-ends in the list of fixings
     """
 
     def __init__(
         self,
         average_type: Union[AverageType, str] = None,
         fixing_frequency: Union[FixingFrequency, str] = None,
         average_so_far: Optional[float] = None,
-        fixing_calendar: Optional[str] = None,
-        fixing_end_date: Optional[str] = None,
-        fixing_start_date: Optional[str] = None,
+        fixing_ric: Optional[str] = None,
+        fixing_start_date: "OptDateTime" = None,
         include_holidays: Optional[bool] = None,
         include_week_ends: Optional[bool] = None,
     ) -> None:
         super().__init__()
         self.average_type = average_type
         self.fixing_frequency = fixing_frequency
         self.average_so_far = average_so_far
-        self.fixing_calendar = fixing_calendar
-        self.fixing_end_date = fixing_end_date
+        self.fixing_ric = fixing_ric
         self.fixing_start_date = fixing_start_date
         self.include_holidays = include_holidays
         self.include_week_ends = include_week_ends
 
     @property
     def average_type(self):
         """
@@ -96,48 +94,37 @@
         return self._get_parameter("averageSoFar")
 
     @average_so_far.setter
     def average_so_far(self, value):
         self._set_parameter("averageSoFar", value)
 
     @property
-    def fixing_calendar(self):
+    def fixing_ric(self):
         """
-        The calendar of the underlying's currency.
+        The fixing's ric source. default value: the first available source ric of the fx
+        cross code
         :return: str
         """
-        return self._get_parameter("fixingCalendar")
+        return self._get_parameter("fixingRic")
 
-    @fixing_calendar.setter
-    def fixing_calendar(self, value):
-        self._set_parameter("fixingCalendar", value)
-
-    @property
-    def fixing_end_date(self):
-        """
-        The end date of the fixing period. Should be less or equal to the expiry.
-        :return: str
-        """
-        return self._get_parameter("fixingEndDate")
-
-    @fixing_end_date.setter
-    def fixing_end_date(self, value):
-        self._set_parameter("fixingEndDate", value)
+    @fixing_ric.setter
+    def fixing_ric(self, value):
+        self._set_parameter("fixingRic", value)
 
     @property
     def fixing_start_date(self):
         """
         The beginning date of the fixing period.
         :return: str
         """
         return self._get_parameter("fixingStartDate")
 
     @fixing_start_date.setter
     def fixing_start_date(self, value):
-        self._set_parameter("fixingStartDate", value)
+        self._set_datetime_parameter("fixingStartDate", value)
 
     @property
     def include_holidays(self):
         """
         Include the holidays in the list of fixings
         :return: bool
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_underlying_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_average_info.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_eti/_eti_fixing_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from refinitiv.data._types import OptDateTime
 from .._base import Info
 from .._enums import (
     AverageType,
     FixingFrequency,
 )
 
 
-class FxAverageInfo(Info):
+class EtiFixingInfo(Info):
     """
     Parameters
     ----------
     average_type : AverageType or str, optional
         The type of average used to compute.
     fixing_frequency : FixingFrequency or str, optional
         The fixing's frequency.
     average_so_far : float, optional
         The value of the average_type
-    fixing_ric_source : str, optional
-        The fixing's RIC source. Default value: the first available source RIC of the Fx
-        Cross Code
-    fixing_start_date : str, optional
+    fixing_calendar : str, optional
+        The calendar of the underlying's currency.
+    fixing_end_date : str or date or datetime or timedelta, optional
+        The end date of the fixing period. Should be less or equal to the expiry.
+    fixing_start_date : str or date or datetime or timedelta, optional
         The beginning date of the fixing period.
     include_holidays : bool, optional
         Include the holidays in the list of fixings
     include_week_ends : bool, optional
         Include the week-ends in the list of fixings
     """
 
     def __init__(
         self,
         average_type: Union[AverageType, str] = None,
         fixing_frequency: Union[FixingFrequency, str] = None,
         average_so_far: Optional[float] = None,
-        fixing_ric: Optional[str] = None,
-        fixing_start_date: Optional[str] = None,
+        fixing_calendar: Optional[str] = None,
+        fixing_end_date: "OptDateTime" = None,
+        fixing_start_date: "OptDateTime" = None,
         include_holidays: Optional[bool] = None,
         include_week_ends: Optional[bool] = None,
     ) -> None:
         super().__init__()
         self.average_type = average_type
         self.fixing_frequency = fixing_frequency
         self.average_so_far = average_so_far
-        self.fixing_ric = fixing_ric
+        self.fixing_calendar = fixing_calendar
+        self.fixing_end_date = fixing_end_date
         self.fixing_start_date = fixing_start_date
         self.include_holidays = include_holidays
         self.include_week_ends = include_week_ends
 
     @property
     def average_type(self):
         """
@@ -93,37 +97,48 @@
         return self._get_parameter("averageSoFar")
 
     @average_so_far.setter
     def average_so_far(self, value):
         self._set_parameter("averageSoFar", value)
 
     @property
-    def fixing_ric(self):
+    def fixing_calendar(self):
         """
-        The fixing's ric source. default value: the first available source ric of the fx
-        cross code
+        The calendar of the underlying's currency.
         :return: str
         """
-        return self._get_parameter("fixingRic")
+        return self._get_parameter("fixingCalendar")
 
-    @fixing_ric.setter
-    def fixing_ric(self, value):
-        self._set_parameter("fixingRic", value)
+    @fixing_calendar.setter
+    def fixing_calendar(self, value):
+        self._set_parameter("fixingCalendar", value)
+
+    @property
+    def fixing_end_date(self):
+        """
+        The end date of the fixing period. Should be less or equal to the expiry.
+        :return: str
+        """
+        return self._get_parameter("fixingEndDate")
+
+    @fixing_end_date.setter
+    def fixing_end_date(self, value):
+        self._set_datetime_parameter("fixingEndDate", value)
 
     @property
     def fixing_start_date(self):
         """
         The beginning date of the fixing period.
         :return: str
         """
         return self._get_parameter("fixingStartDate")
 
     @fixing_start_date.setter
     def fixing_start_date(self, value):
-        self._set_parameter("fixingStartDate", value)
+        self._set_datetime_parameter("fixingStartDate", value)
 
     @property
     def include_holidays(self):
         """
         Include the holidays in the list of fixings
         :return: bool
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_barrier_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ......_types import OptDateTime
 from .._base import BarrierDefinition
 from .._enums import (
     BarrierMode,
     InOrOut,
     UpOrDown,
 )
 
@@ -20,29 +21,29 @@
         In/Out property of the barrier option
     up_or_down : UpOrDown or str, optional
         Up/Down property of the barrier option
     level : float, optional
         Barrier of the barrier option
     rebate_amount : float, optional
         Rebate of the barrier option
-    window_end_date : str, optional
+    window_end_date : str or date or datetime or timedelta, optional
         Window Start date of the barrier option
-    window_start_date : str, optional
+    window_start_date : str or date or datetime or timedelta, optional
         Window Start date of the barrier option
     """
 
     def __init__(
         self,
         barrier_mode: Union[BarrierMode, str] = None,
         in_or_out: Union[InOrOut, str] = None,
         up_or_down: Union[UpOrDown, str] = None,
         level: Optional[float] = None,
         rebate_amount: Optional[float] = None,
-        window_end_date: Optional[str] = None,
-        window_start_date: Optional[str] = None,
+        window_end_date: "OptDateTime" = None,
+        window_start_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.barrier_mode = barrier_mode
         self.in_or_out = in_or_out
         self.up_or_down = up_or_down
         self.level = level
         self.rebate_amount = rebate_amount
@@ -115,20 +116,20 @@
         Window Start date of the barrier option
         :return: str
         """
         return self._get_parameter("windowEndDate")
 
     @window_end_date.setter
     def window_end_date(self, value):
-        self._set_parameter("windowEndDate", value)
+        self._set_datetime_parameter("windowEndDate", value)
 
     @property
     def window_start_date(self):
         """
         Window Start date of the barrier option
         :return: str
         """
         return self._get_parameter("windowStartDate")
 
     @window_start_date.setter
     def window_start_date(self, value):
-        self._set_parameter("windowStartDate", value)
+        self._set_datetime_parameter("windowStartDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, List, Union
 
+from ......_types import OptDateTime
 from ...._models import InputFlow
 from .._base import UnderlyingDefinition
 from ..._instrument_definition import InstrumentDefinition
 from .._enums import (
     BuySell,
     CallPut,
     ExerciseStyle,
@@ -28,17 +29,17 @@
     """
     Parameters
     ----------
     instrument_tag : str, optional
         User defined string to identify the instrument.it can be used to link output
         results to the instrument definition. only alphabetic, numeric and '- _.#=@'
         characters are supported. optional.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         Start date of the option
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity or expiry date of the instrument. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z').
         optional. mandatory for otc eti options and fx options(if tenor is not defined).
         if instrumentcode of listed eti option is defined, the value comes from the
         instrument reference data.
     tenor : str, optional
         The code indicating the period between startdate and enddate of the instrument
@@ -77,15 +78,15 @@
         An array of payments
     settlement_type : SettlementType or str, optional
         The settlement method for options when exercised.
     underlying_definition : FxUnderlyingDefinition, optional
 
     underlying_type : UnderlyingType or str, optional
         The type of the option based on the underlying asset. Mandatory. No default value applies.
-    delivery_date : str, optional
+    delivery_date : str or date or datetime or timedelta, optional
         The date when the underlylng asset is delivered. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g. '2021-01-01t00:00:00z').
     settlement_ccy : str, optional
         The currency of the instrument's settlement. the value is expressed in iso 4217
         alphabetical format (e.g. 'usd'). if the option is a eurgbp call option,
         settlementccy can be expressed in eur or gbp
     strike : float, optional
@@ -95,16 +96,16 @@
         instrumentcode of listed eti option is defined, the value comes from the
         instrument reference data.
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         asian_definition: Optional[FxAverageInfo] = None,
         barrier_definition: Optional[FxBarrierDefinition] = None,
         binary_definition: Optional[FxBinaryDefinition] = None,
         buy_sell: Union[BuySell, str] = None,
@@ -114,15 +115,15 @@
         dual_currency_definition: Optional[FxDualCurrencyDefinition] = None,
         exercise_style: Union[ExerciseStyle, str] = None,
         forward_start_definition: Optional[FxForwardStart] = None,
         payments: Optional[List[InputFlow]] = None,
         settlement_type: Union[SettlementType, str] = None,
         underlying_definition: Optional[FxUnderlyingDefinition] = None,
         underlying_type: Union[UnderlyingType, str] = None,
-        delivery_date: Optional[str] = None,
+        delivery_date: "OptDateTime" = None,
         settlement_ccy: Optional[str] = None,
         strike: Optional[float] = None,
         **kwargs,
     ) -> None:
         super().__init__(instrument_tag, **kwargs)
         self.instrument_tag = instrument_tag
         self.start_date = start_date
@@ -335,15 +336,15 @@
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g. '2021-01-01t00:00:00z').
         :return: str
         """
         return self._get_parameter("deliveryDate")
 
     @delivery_date.setter
     def delivery_date(self, value):
-        self._set_parameter("deliveryDate", value)
+        self._set_datetime_parameter("deliveryDate", value)
 
     @property
     def end_date(self):
         """
         The maturity or expiry date of the instrument. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z').
         optional. mandatory for otc eti options and fx options(if tenor is not defined).
@@ -351,15 +352,15 @@
         instrument reference data.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def instrument_tag(self):
         """
         User defined string to identify the instrument.it can be used to link output
         results to the instrument definition. only alphabetic, numeric and '- _.#=@'
         characters are supported. optional.
@@ -418,15 +419,15 @@
         Start date of the option
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def strike(self):
         """
         The set price at which the owner of the option can buy or sell the underlying
         asset. the value is expressed according to the market convention linked to the
         underlying asset. optional. mandatory for otc eti options and fx options. if
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_barrier_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_double_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_dual_currency_definition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # coding: utf8
 
 from typing import Optional
 
+from ......_types import OptDateTime
 from ..._instrument_definition import ObjectDefinition
 
 
 class FxDualCurrencyDefinition(ObjectDefinition):
     """
     Parameters
     ----------
-    deposit_start_date : str, optional
+    deposit_start_date : str or date or datetime or timedelta, optional
         Deposit Start Date for the DualCurrencyDeposit option
     margin_percent : float, optional
         Margin for the DualCurrencyDeposit option
     """
 
     def __init__(
         self,
-        deposit_start_date: Optional[str] = None,
+        deposit_start_date: "OptDateTime" = None,
         margin_percent: Optional[float] = None,
     ) -> None:
         super().__init__()
         self.deposit_start_date = deposit_start_date
         self.margin_percent = margin_percent
 
     @property
@@ -30,15 +31,15 @@
         Deposit Start Date for the DualCurrencyDeposit option
         :return: str
         """
         return self._get_parameter("depositStartDate")
 
     @deposit_start_date.setter
     def deposit_start_date(self, value):
-        self._set_parameter("depositStartDate", value)
+        self._set_date_parameter("depositStartDate", value)
 
     @property
     def margin_percent(self):
         """
         Margin for the DualCurrencyDeposit option
         :return: float
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_forward_start.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # coding: utf8
 
 from typing import Optional
 
+from ......_types import OptDateTime
 from ..._instrument_definition import ObjectDefinition
 
 
 class FxForwardStart(ObjectDefinition):
     """
     Parameters
     ----------
-    forward_start_date : str, optional
+    forward_start_date : str or date or datetime or timedelta, optional
         Expiry date of the Forward Start option
     forward_start_tenor : str, optional
         Tenor of the Forward Start option
     strike_percent : float, optional
         Strike Percent of the Forward Start date of the option
     """
 
     def __init__(
         self,
-        forward_start_date: Optional[str] = None,
+        forward_start_date: "OptDateTime" = None,
         forward_start_tenor: Optional[str] = None,
         strike_percent: Optional[float] = None,
     ) -> None:
         super().__init__()
         self.forward_start_date = forward_start_date
         self.forward_start_tenor = forward_start_tenor
         self.strike_percent = strike_percent
@@ -34,15 +35,15 @@
         Expiry date of the Forward Start option
         :return: str
         """
         return self._get_parameter("forwardStartDate")
 
     @forward_start_date.setter
     def forward_start_date(self, value):
-        self._set_parameter("forwardStartDate", value)
+        self._set_datetime_parameter("forwardStartDate", value)
 
     @property
     def forward_start_tenor(self):
         """
         Tenor of the Forward Start option
         :return: str
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_fx/_fx_underlying_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # coding: utf8
 
 from typing import Optional, Union
 
-from .._instrument_definition import InstrumentDefinition
+from ....._types import OptDateTime
 from ._enums import (
     BuySell,
     CallPut,
     ExerciseStyle,
     UnderlyingType,
 )
+from .._instrument_definition import InstrumentDefinition
 
 
 class OptionDefinition(InstrumentDefinition):
     """
     Parameters
     ----------
     instrument_tag : str, optional
         User defined string to identify the instrument.It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported. Optional.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         Expiry date of the option.
     buy_sell : BuySell or str, optional
         The side of the deal.
     call_put : CallPut or str, optional
         Tells if the option is a call or a put.
     exercise_style : ExerciseStyle or str, optional
         The option style based on its exercise restrictions.
@@ -32,16 +33,16 @@
     strike : float, optional
         strike of the option
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         buy_sell: Union[BuySell, str] = None,
         call_put: Union[CallPut, str] = None,
         exercise_style: Union[ExerciseStyle, str] = None,
         underlying_type: Union[UnderlyingType, str] = None,
         strike: Optional[float] = None,
         **kwargs,
     ) -> None:
@@ -118,27 +119,27 @@
         Expiry date of the option
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def start_date(self):
         """
         Start date of the option
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def strike(self):
         """
         strike of the option
         :return: float
         """
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional
 
+from ....._types import OptDateTime
 from ._enums import BuySell, CallPut, ExerciseStyle, UnderlyingType, SettlementType
 from ._eti import (
     EtiUnderlyingDefinition,
     EtiBinaryDefinition,
     EtiBarrierDefinition,
     EtiDefinition,
     EtiCbbcDefinition,
@@ -29,32 +30,32 @@
         asian_definition: Optional[EtiFixingInfo] = None,
         barrier_definition: Optional[EtiBarrierDefinition] = None,
         binary_definition: Optional[EtiBinaryDefinition] = None,
         buy_sell: Optional[BuySell] = None,
         call_put: Optional[CallPut] = None,
         cbbc_definition: Optional[EtiCbbcDefinition] = None,
         deal_contract: Optional[int] = None,
-        delivery_date: Optional[str] = None,
+        delivery_date: "OptDateTime" = None,
         double_barrier_definition: Optional[FxDoubleBarrierDefinition] = None,
         double_barriers_definition: Optional[EtiDoubleBarriersDefinition] = None,
         double_binary_definition: Optional[FxDoubleBinaryDefinition] = None,
         dual_currency_definition: Optional[FxDualCurrencyDefinition] = None,
-        end_date: Optional[str] = None,
-        end_date_time: Optional[str] = None,
+        end_date: "OptDateTime" = None,
+        end_date_time: "OptDateTime" = None,
         exercise_style: Optional[ExerciseStyle] = None,
         forward_start_definition: Optional[FxForwardStart] = None,
         instrument_code: Optional[str] = None,
         instrument_tag: Optional[str] = None,
         lot_size: Optional[float] = None,
         notional_amount: Optional[float] = None,
         notional_ccy: Optional[str] = None,
         payments: Optional[InputFlow] = None,
         settlement_ccy: Optional[str] = None,
         settlement_type: Optional[SettlementType] = None,
-        start_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
         strike: Optional[float] = None,
         tenor: Optional[str] = None,
         time_zone_offset: Optional[int] = None,
         underlying_definition: Optional[EtiUnderlyingDefinition] = None,
         underlying_type: Optional[UnderlyingType] = None,
     ):
         super().__init__(
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     VolatilityModel,
 )
 from ..._models import (
     BidAskMid,
     InterpolationWeight,
     PayoutScaling,
 )
+from ....._types import OptDateTime
 
 
 class PricingParameters(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
@@ -89,15 +90,15 @@
         Define whether the payout chart must be computed or not
     compute_volatility_payout : bool, optional
         Define whether the volatility payout chart must be computed or not
     cutoff_time : str, optional
         The cutoff time
     cutoff_time_zone : str, optional
         The cutoff time zone
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The date at which the market data is retrieved. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). it
         should be less or equal tovaluationdate). optional. by
         default,marketdatadateisvaluationdateor today.
     market_value_in_deal_ccy : float, optional
         The market value (premium) of the instrument. the value is expressed in the deal
         currency. it is used to define optionprice and compute volatilitypercent. if
@@ -128,15 +129,15 @@
         Tells if payoff-linked cashflow should be returned. possible values:
         - true
         - false
     underlying_price : float, optional
         The price of the underlying asset. the value is expressed in the deal currency.
         if underlyingprice is defined, underlyingpriceside is not taken into account.
         optional. by default, the value is retrieved from the market data.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date at which the instrument is valued. the value is expressed in iso 8601
         format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). by default,
         marketdatadate is used. if marketdatadate is not specified, the default value is
         today.
     volatility : float, optional
         Volatility(without unity) to override and that will be used as pricing analysis
         input to compute marketvalueindealccy. introduced due to bachelier model, for
@@ -176,23 +177,23 @@
         underlying_time_stamp: Optional[TimeStamp] = None,
         volatility_model: Union[VolatilityModel, str] = None,
         volatility_type: Optional[OptionVolatilityType] = None,
         compute_payout_chart: Optional[bool] = None,
         compute_volatility_payout: Optional[bool] = None,
         cutoff_time: Optional[str] = None,
         cutoff_time_zone: Optional[str] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         market_value_in_deal_ccy: Optional[float] = None,
         market_value_in_report_ccy: Optional[float] = None,
         report_ccy: Optional[str] = None,
         report_ccy_rate: Optional[float] = None,
         risk_free_rate_percent: Optional[float] = None,
         simulate_exercise: Optional[bool] = None,
         underlying_price: Optional[float] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
         volatility: Optional[float] = None,
         volatility_percent: Optional[float] = None,
     ) -> None:
         super().__init__()
         self.atm_volatility_object = atm_volatility_object
         self.butterfly10_d_object = butterfly10_d_object
         self.butterfly25_d_object = butterfly25_d_object
@@ -599,15 +600,15 @@
         default,marketdatadateisvaluationdateor today.
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def market_value_in_deal_ccy(self):
         """
         The market value (premium) of the instrument. the value is expressed in the deal
         currency. it is used to define optionprice and compute volatilitypercent. if
         marketvalueindealccy is defined, optionpriceside and volatilitypercent are not
@@ -718,15 +719,15 @@
         today.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
 
     @property
     def volatility(self):
         """
         Volatility(without unity) to override and that will be used as pricing analysis
         input to compute marketvalueindealccy. introduced due to bachelier model, for
         more details please have a look at apqps-13558 optional. no override is applied
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 from ._repo_pricing_parameters import PricingParameters
 from ._repo_underlying_contract import UnderlyingContract
 from .._base_definition import BaseDefinition
 from ..._enums import DayCountBasis, BuySell
 from ....._tools import create_repr, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
 
 
 class Definition(BaseDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
     Parameters
     ----------
     instrument_tag : str, optional
         User defined string to identify the instrument.It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         Start date of the repo, that means when the the underlying security is
         exchanged.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         End date of the repo, that means when the borrower repurchases the security
         back. Either end_date or tenor field are requested.
     tenor : str, optional
         tenor that defines the duration of the Repo in case no end_date has been
         provided. In that case, end_date is computed from start_date and tenor. Either
         end_date or tenor field are requested.
      buy_sell : BuySell or str, optional
@@ -92,16 +92,16 @@
     >>> stream = definition.get_stream()
     >>> stream.open()
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         buy_sell: Union[BuySell, str] = None,
         day_count_basis: Union[DayCountBasis, str] = None,
         underlying_instruments: Optional[List[UnderlyingContract]] = None,
         is_coupon_exchanged: Optional[bool] = None,
         repo_rate_percent: Optional[float] = None,
         fields: "OptStrStrs" = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from .._instrument_definition import InstrumentDefinition
 from ..._enums import (
     BuySell,
     DayCountBasis,
 )
 from ._repo_underlying_contract import UnderlyingContract
 
@@ -17,18 +18,18 @@
 
     Parameters
     ----------
     instrument_tag : str, optional
         User defined string to identify the instrument.it can be used to link output
         results to the instrument definition. only alphabetic, numeric and '- _.#=@'
         characters are supported. optional.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         Start date of the repo, that means when the underlying security is exchanged.
         mandatory.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         End date of the repo, that means when the borrower repurchases the security
         back. either enddate or tenor field are requested.
     tenor : str, optional
         Tenor that defines the duration of the repo in case no enddate has been
         provided. in that case, enddate is computed from startdate and tenor. either
         enddate or tenor field are requested.
     buy_sell : BuySell or str, optional
@@ -54,16 +55,16 @@
         Custom repo rate in percentage. if not provided in the request, it will be
         computed by interpolating/extrapolating a repo curve. optional.
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         buy_sell: Union[BuySell, str] = None,
         day_count_basis: Union[DayCountBasis, str] = None,
         underlying_instruments: Optional[UnderlyingContract] = None,
         is_coupon_exchanged: Optional[bool] = None,
         repo_rate_percent: Optional[float] = None,
     ) -> None:
@@ -127,15 +128,15 @@
         back. either enddate or tenor field are requested.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def instrument_tag(self):
         """
         User defined string to identify the instrument.it can be used to link output
         results to the instrument definition. only alphabetic, numeric and '- _.#=@'
         characters are supported. optional.
@@ -187,15 +188,15 @@
         mandatory.
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def tenor(self):
         """
         Tenor that defines the duration of the repo in case no enddate has been
         provided. in that case, enddate is computed from startdate and tenor. either
         enddate or tenor field are requested.
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from ..._enums import RepoCurveType
 from ..._object_definition import ObjectDefinition
 
 
 class PricingParameters(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
@@ -15,36 +16,36 @@
     ----------
     repo_curve_type : RepoCurveType or str, optional
         Curve used to compute the repo rate. it can be computed using following methods:
         - repocurve : rate is computed by interpolating a repo curve.     - depositcurve
         : rate is computed by interpolating a deposit curve.     - fixinglibor : rate is
         computed by interpolating libor rates.  if no curve can be found, the rate is
         computed using a deposit curve.
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The date at which the market data is retrieved. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). it
         should be less or equal tovaluationdate). optional. by
         default,marketdatadateisvaluationdateor today.
     report_ccy : str, optional
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date at which the instrument is valued. the value is expressed in iso 8601
         format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). by default,
         marketdatadate is used. if marketdatadate is not specified, the default value is
         today.
     """
 
     def __init__(
         self,
         repo_curve_type: Union[RepoCurveType, str] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         report_ccy: Optional[str] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.repo_curve_type = repo_curve_type
         self.market_data_date = market_data_date
         self.report_ccy = report_ccy
         self.valuation_date = valuation_date
 
@@ -73,15 +74,15 @@
         default,marketdatadateisvaluationdateor today.
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def report_ccy(self):
         """
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
@@ -102,8 +103,8 @@
         today.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf8
 
 from typing import Optional
 
+from ....._types import OptDateTime
 from ..._object_definition import ObjectDefinition
 
 from ._repo_parameters import RepoParameters
 from ..bond import PricingParameters as BondPricingParameters
 
 
 class UnderlyingPricingParameters(ObjectDefinition):
@@ -17,38 +18,38 @@
     ----------
     pricing_parameters_at_end : BondPricingParameters, optional
 
     pricing_parameters_at_start : BondPricingParameters, optional
 
     repo_parameters : RepoParameters, optional
 
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The date at which the market data is retrieved. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). it
         should be less or equal tovaluationdate). optional. by
         default,marketdatadateisvaluationdateor today.
     report_ccy : str, optional
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date at which the instrument is valued. the value is expressed in iso 8601
         format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). by default,
         marketdatadate is used. if marketdatadate is not specified, the default value is
         today.
     """
 
     def __init__(
         self,
         pricing_parameters_at_end: Optional[BondPricingParameters] = None,
         pricing_parameters_at_start: Optional[BondPricingParameters] = None,
         repo_parameters: Optional[RepoParameters] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         report_ccy: Optional[str] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.pricing_parameters_at_end = pricing_parameters_at_end
         self.pricing_parameters_at_start = pricing_parameters_at_start
         self.repo_parameters = repo_parameters
         self.market_data_date = market_data_date
         self.report_ccy = report_ccy
@@ -96,15 +97,15 @@
         default,marketdatadateisvaluationdateor today.
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def report_ccy(self):
         """
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
@@ -125,8 +126,8 @@
         today.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from typing import Optional, TYPE_CHECKING, List
 
 from ._swap_definition import SwapInstrumentDefinition
 from .._base_definition import BaseDefinition
 from ....._tools import try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
     from . import LegDefinition, PricingParameters
 
 
 class Definition(BaseDefinition):
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
         instrument_code: Optional[str] = None,
-        trade_date: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        trade_date: "OptDateTime" = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         legs: Optional[List["LegDefinition"]] = None,
         is_non_deliverable: Optional[bool] = None,
         settlement_ccy: Optional[str] = None,
         start_tenor: Optional[str] = None,
         template: Optional[str] = None,
         fields: "OptStrStrs" = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # coding: utf8
 from typing import Optional
 
+from ....._types import OptDateTime
 from ._swap_leg_definition import LegDefinition
 from .._instrument_definition import InstrumentDefinition
 
 
 class SwapInstrumentDefinition(InstrumentDefinition):
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
         instrument_code: Optional[str] = None,
-        trade_date: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        trade_date: "OptDateTime" = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         legs: Optional[LegDefinition] = None,
         is_non_deliverable: Optional[bool] = None,
         settlement_ccy: Optional[str] = None,
         start_tenor: Optional[str] = None,
         template: Optional[str] = None,
     ) -> None:
@@ -56,15 +57,15 @@
         Mandatory. Either the endDate or the tenor must be provided.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def instrument_code(self):
         """
         A swap RIC that is used to retrieve the description of the swap contract.
         Optional. Either instrumentCode, template, or legs must be provided.
         :return: str
@@ -108,15 +109,15 @@
         Optional. By default, it is derived from the TradeDate and the day to spot convention of the contract currency.
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def start_tenor(self):
         """
         The code indicating the period from a spot date to startdate of the instrument
         (e.g. '1m'). no default value applies.
         :return: str
@@ -160,8 +161,8 @@
         Optional. By default, the valuation date.
         :return: str
         """
         return self._get_parameter("tradeDate")
 
     @trade_date.setter
     def trade_date(self, value):
-        self._set_parameter("tradeDate", value)
+        self._set_datetime_parameter("tradeDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     NotionalExchange,
     StubRule,
     PriceSide,
 )
 from ..._models import AmortizationItem
 from ..._object_definition import ObjectDefinition
 from ....._tools import try_copy_to_list
+from ....._types import OptDateTime
 
 
 class LegDefinition(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
@@ -99,19 +100,19 @@
         index at the end of the interest period. the default value is 'inadvance'.
     index_fixing_lag : int, optional
         The number of working daysbetween the fixing date and the start of the coupon
         period ('inadvance') or the end of the coupon period ('inarrears'). the
         inadvance/inarrears mode is set in the indexresettype parameter. the default
         value is the fixing lag associated to the index defined/determined by default on
         the floating instrument.
-    first_regular_payment_date : str, optional
+    first_regular_payment_date : str or date or datetime or timedelta, optional
         The first regular interest payment date used for the odd first interest period.
         the value is expressed in iso 8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g.
         2021-01-01t00:00:00z). no default value applies.
-    last_regular_payment_date : str, optional
+    last_regular_payment_date : str or date or datetime or timedelta, optional
         The last regular interest payment date used for the odd last interest period.
         the value is expressed in iso 8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g.
         2021-01-01t00:00:00z). no default value applies.
     amortization_schedule : AmortizationItem, optional
         The amortization schedule of the instrument. it contains the following
         information:   startdate,   enddate,   remainingnotional,
         amortizationfrequency,   amount,   amortizationtype.  optional. no default value
@@ -205,16 +206,16 @@
         interest_calculation_method: Union[DayCountBasis, str] = None,
         accrued_calculation_method: Union[DayCountBasis, str] = None,
         payment_business_day_convention: Union[BusinessDayConvention, str] = None,
         payment_roll_convention: Union[DateRollingConvention, str] = None,
         index_reset_frequency: Union[Frequency, str] = None,
         index_reset_type: Union[IndexResetType, str] = None,
         index_fixing_lag: Optional[int] = None,
-        first_regular_payment_date: Optional[str] = None,
-        last_regular_payment_date: Optional[str] = None,
+        first_regular_payment_date: "OptDateTime" = None,
+        last_regular_payment_date: "OptDateTime" = None,
         amortization_schedule: Optional[List[AmortizationItem]] = None,
         payment_business_days: Optional[str] = None,
         notional_exchange: Union[NotionalExchange, str] = None,
         adjust_interest_to_payment_date: Union[AdjustInterestToPaymentDate, str] = None,
         index_compounding_method: Union[IndexCompoundingMethod, str] = None,
         interest_payment_delay: Optional[int] = None,
         stub_rule: Union[StubRule, str] = None,
@@ -555,15 +556,15 @@
         2021-01-01t00:00:00z). no default value applies.
         :return: str
         """
         return self._get_parameter("firstRegularPaymentDate")
 
     @first_regular_payment_date.setter
     def first_regular_payment_date(self, value):
-        self._set_parameter("firstRegularPaymentDate", value)
+        self._set_datetime_parameter("firstRegularPaymentDate", value)
 
     @property
     def fixed_rate_percent(self):
         """
         The interest rate of the instrument. the value is expressed in percentages.
         mandatory if no instrumentcode is defined. if instrumentcode is defined, the
         value comes from the instrument reference data.
@@ -678,15 +679,15 @@
         2021-01-01t00:00:00z). no default value applies.
         :return: str
         """
         return self._get_parameter("lastRegularPaymentDate")
 
     @last_regular_payment_date.setter
     def last_regular_payment_date(self, value):
-        self._set_parameter("lastRegularPaymentDate", value)
+        self._set_datetime_parameter("lastRegularPaymentDate", value)
 
     @property
     def leg_tag(self):
         """
         A user-defined string to identify the direction of the leg: 'paid' or
         'received'. optional. no default value applies.
         :return: str
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf8
 
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from ..._enums import (
     IndexConvexityAdjustmentIntegrationMethod,
     IndexConvexityAdjustmentMethod,
     PriceSide,
     TenorReferenceDate,
 )
 from ..._object_definition import ObjectDefinition
@@ -33,15 +34,15 @@
         swap start date is calculated from valuation date or from spot date
     discounting_ccy : str, optional
         The currency code, which defines the choice of the discounting curve. the value
         is expressed in iso 4217 alphabetical format (e.g. 'usd'). by default,
         settlementccy or the paid leg currency is used.
     discounting_tenor : str, optional
 
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The date at which the market data is retrieved. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). it
         should be less or equal tovaluationdate). optional. by
         default,marketdatadateisvaluationdateor today.
     market_value_in_deal_ccy : float, optional
         The dirty market value of the instrument computed as
         [cleanmarketvalueindealccy+accruedamountindealccy]. the value is expressed in
@@ -49,34 +50,34 @@
     report_ccy : str, optional
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
     use_legs_signing : bool, optional
         Enable the signing of "risk measures" and "valuation" outputs based on leg's
         direction the default value is false.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The date at which the instrument is valued. the value is expressed in iso 8601
         format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). by default,
         marketdatadate is used. if marketdatadate is not specified, the default value is
         today.
     """
 
     def __init__(
         self,
         index_convexity_adjustment_integration_method: Union[IndexConvexityAdjustmentIntegrationMethod, str] = None,
         index_convexity_adjustment_method: Union[IndexConvexityAdjustmentMethod, str] = None,
         price_side: Union[PriceSide, str] = None,
         tenor_reference_date: Union[TenorReferenceDate, str] = None,
         discounting_ccy: Optional[str] = None,
         discounting_tenor: Optional[str] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         market_value_in_deal_ccy: Optional[float] = None,
         report_ccy: Optional[str] = None,
         use_legs_signing: Optional[bool] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.index_convexity_adjustment_integration_method = index_convexity_adjustment_integration_method
         self.index_convexity_adjustment_method = index_convexity_adjustment_method
         self.price_side = price_side
         self.tenor_reference_date = tenor_reference_date
         self.discounting_ccy = discounting_ccy
@@ -180,15 +181,15 @@
         default,marketdatadateisvaluationdateor today.
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def market_value_in_deal_ccy(self):
         """
         The dirty market value of the instrument computed as
         [cleanmarketvalueindealccy+accruedamountindealccy]. the value is expressed in
         the deal currency. the default value is '0'.
@@ -236,8 +237,8 @@
         today.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,33 +14,33 @@
     PremiumSettlementType,
     SwaptionType,
 )
 from ..._models import InputFlow
 from ....._tools import create_repr, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
 
 
 class Definition(BaseDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
     Parameters
     ----------
     instrument_tag : str, optional
         A user defined string to identify the instrument. it can be used to link output
         results to the instrument definition.limited to 40 characters.only alphabetic,
         numeric and '- _.#=@' characters are supported. optional. no default value
         applies.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         The date the swaption starts. optional. by default it is derived from the
         tradedate and the day to spot convention of the contract currency.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity or expiry date of the instrument's leg. the value is expressed in
         iso 8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g. 2021-01-01t00:00:00z). either
         tenor or enddate must be provided. the default value is valuationdate shifted
         forward by tenor.
     tenor : str, optional
         The code indicating the period between startdate and enddate of the instrument
         (e.g. '6m', '1y'). mandatory, if enddate is not provided. the default value is
@@ -84,15 +84,15 @@
     pricing_parameters : PricingParameters, optional
         The pricing parameters to apply to this instrument. If pricing parameters
         are not provided at this level parameters defined globally at the request
         level are used. If no pricing parameters are provided globally default
         values apply.
     extended_params : dict, optional
         If necessary other parameters.
-    delivery_date : str, optional
+    delivery_date : str or date or datetime or timedelta, optional
         The date when the underlying asset is delivered.
         The value is expressed in ISO 8601 format: YYYY-MM-DDT[hh]:[mm]:[ss]Z (e.g. '2021-01-01T00:00:00Z').
 
     Methods
     -------
     get_data(session=session, on_response=on_response, async_mode=None)
         Returns a response to the data platform
@@ -117,16 +117,16 @@
     >>> stream = definition.get_stream()
     >>> stream.open()
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         notional_amount: Optional[float] = None,
         bermudan_swaption_definition: Optional[BermudanSwaptionDefinition] = None,
         buy_sell: Optional[BuySell] = None,
         exercise_style: Optional[ExerciseStyle] = None,
         payments: Optional[InputFlow] = None,
         premium_settlement_type: Union[PremiumSettlementType, str] = None,
@@ -134,15 +134,15 @@
         swaption_type: Union[SwaptionType, str] = None,
         underlying_definition: Optional[swap.Definition] = None,
         spread_vs_atm_in_bp: Optional[float] = None,
         strike_percent: Optional[float] = None,
         fields: "OptStrStrs" = None,
         pricing_parameters: Optional[PricingParameters] = None,
         extended_params: "ExtendedParams" = None,
-        delivery_date: Optional[str] = None,
+        delivery_date: "OptDateTime" = None,
     ):
         fields = try_copy_to_list(fields)
         self.underlying_definition = underlying_definition
         definition = SwaptionInstrumentDefinition(
             bermudan_swaption_definition=bermudan_swaption_definition,
             buy_sell=buy_sell,
             exercise_style=exercise_style,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf8
 
 
 from typing import Optional, List, Union
 
+from ....._types import OptDateTime
 from . import BermudanSwaptionDefinition
 from ..._enums import (
     BuySell,
     ExerciseStyle,
     PremiumSettlementType,
     SwaptionSettlementType,
     SwaptionType,
@@ -25,18 +26,18 @@
     Parameters
     ----------
     instrument_tag : str, optional
         A user defined string to identify the instrument. it can be used to link output
         results to the instrument definition.limited to 40 characters.only alphabetic,
         numeric and '- _.#=@' characters are supported. optional. no default value
         applies.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         The date the swaption starts. optional. by default it is derived from the
         tradedate and the day to spot convention of the contract currency.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity or expiry date of the instrument's leg. the value is expressed in
         iso 8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g. 2021-01-01t00:00:00z). either
         tenor or enddate must be provided. the default value is valuationdate shifted
         forward by tenor.
     tenor : str, optional
         The code indicating the period between startdate and enddate of the instrument
         (e.g. '6m', '1y'). mandatory, if enddate is not provided. the default value is
@@ -75,29 +76,29 @@
         owner of the swaption can enter the swap. the value is expressed in percentages.
         by default, fixedratepercent of the underlying swap is used.
     """
 
     def __init__(
         self,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         notional_amount: Optional[float] = None,
         bermudan_swaption_definition: Optional[BermudanSwaptionDefinition] = None,
         buy_sell: Union[BuySell, str] = None,
         exercise_style: Union[ExerciseStyle, str] = None,
         payments: Optional[List[InputFlow]] = None,
         premium_settlement_type: Union[PremiumSettlementType, str] = None,
         settlement_type: Union[SwaptionSettlementType, str] = None,
         swaption_type: Union[SwaptionType, str] = None,
         underlying_definition: Optional[swap.Definition] = None,
         spread_vs_atm_in_bp: Optional[float] = None,
         strike_percent: Optional[float] = None,
-        delivery_date: Optional[str] = None,
+        delivery_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.instrument_tag = instrument_tag
         self.start_date = start_date
         self.end_date = end_date
         self.tenor = tenor
         self.notional_amount = notional_amount
@@ -220,15 +221,15 @@
         forward by tenor.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def instrument_tag(self):
         """
         A user defined string to identify the instrument. it can be used to link output
         results to the instrument definition.limited to 40 characters.only alphabetic,
         numeric and '- _.#=@' characters are supported. optional. no default value
@@ -272,15 +273,15 @@
         tradedate and the day to spot convention of the contract currency.
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def strike_percent(self):
         """
         The set price at which the owner of the option can buy or sell the underlying
         asset. for a swaption, it is the fixed rate of the underlying swap at which the
         owner of the swaption can enter the swap. the value is expressed in percentages.
@@ -309,8 +310,8 @@
 
     @property
     def delivery_date(self):
         return self._get_parameter("deliveryDate")
 
     @delivery_date.setter
     def delivery_date(self, value):
-        self._set_parameter("deliveryDate", value)
+        self._set_datetime_parameter("deliveryDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding: utf8
 
 
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from ..._object_definition import ObjectDefinition
 from ..._enums import PriceSide
 
 
 class PricingParameters(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
     Parameters
     ----------
     price_side : PriceSide or str, optional
         The quoted price side of the instrument. optional. default value is 'mid'.
-    exercise_date : str, optional
+    exercise_date : str or date or datetime or timedelta, optional
 
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The date at which the market data is retrieved. the value is expressed in iso
         8601 format: yyyy-mm-ddt[hh]:[mm]:[ss]z (e.g., '2021-01-01t00:00:00z'). it
         should be less or equal tovaluationdate). optional. by
         default,marketdatadateisvaluationdateor today.
     market_value_in_deal_ccy : float, optional
         The market value of the instrument. the value is expressed in the deal currency.
         optional. no default value applies. note that premium takes priority over
@@ -33,36 +34,36 @@
     report_ccy : str, optional
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
     simulate_exercise : bool, optional
         Tells if in case of future cashflows should be considered as exercised or not.
         possible values:    true,    false.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The valuation date for pricing. If not set the valuation date is equal to
         market_data_date or Today. For assets that contains a settlementConvention,
         the default valuation date  is equal to the settlementdate of the Asset that is
         usually the TradeDate+SettlementConvention.
 
     Examples
     --------
     >>> import refinitiv.data.content.ipa.financial_contracts as rdf
     >>> rdf.swaption.PricingParameters(valuation_date="2020-04-24", nb_iterations=80)
     """
 
     def __init__(
         self,
         price_side: Union[PriceSide, str] = None,
-        exercise_date: Optional[str] = None,
-        market_data_date: Optional[str] = None,
+        exercise_date: "OptDateTime" = None,
+        market_data_date: "OptDateTime" = None,
         market_value_in_deal_ccy: Optional[float] = None,
         nb_iterations: Optional[int] = None,
         report_ccy: Optional[str] = None,
         simulate_exercise: Optional[bool] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
     ) -> None:
         super().__init__()
         self.price_side = price_side
         self.exercise_date = exercise_date
         self.market_data_date = market_data_date
         self.market_value_in_deal_ccy = market_value_in_deal_ccy
         self.nb_iterations = nb_iterations
@@ -87,28 +88,28 @@
         """
         :return: str
         """
         return self._get_parameter("exerciseDate")
 
     @exercise_date.setter
     def exercise_date(self, value):
-        self._set_parameter("exerciseDate", value)
+        self._set_datetime_parameter("exerciseDate", value)
 
     @property
     def market_data_date(self):
         """
         The market data date for pricing.
         By default, the marketDataDate date is the ValuationDate or Today.
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def market_value_in_deal_ccy(self):
         """
         MarketValueInDealCcy to override and that will be used as pricing analysis input to compute VolatilityPercent.
         No override is applied by default. Note that Premium takes priority over Volatility input.
         :return: float
@@ -167,8 +168,8 @@
         the settlementdate of the Asset that is usually the TradeDate+SettlementConvention.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     DateRollingConvention,
     DayCountBasis,
     Frequency,
 )
 from ....._tools import create_repr, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ....._types import ExtendedParams, OptStrStrs
+    from ....._types import ExtendedParams, OptStrStrs, OptDateTime
 
 
 class Definition(BaseDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
@@ -27,19 +27,19 @@
     instrument_code : str, optional
         Code to define the term deposit instrument. For the moment, only RICs for CDs
         and Wholesales deposits are supported, with deposit code (ex:"EUR1MD=").
     instrument_tag : str, optional
         User defined string to identify the instrument. It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported.
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         The date the term deposit starts accruing interest. Its effective date.
         By default it is derived from the ValuationDate and the day to spot convention
         of the contract currency.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity date of the term deposit contract. Either the endDate or the tenor
         must be provided.
     tenor : str, optional
         The period code that represents the time between the start date and end date of
         the contract.
         Mandatory if instrumentCode is null. Either the endDate or the tenor must be
         provided.
@@ -113,16 +113,16 @@
     >>> stream.open()
     """
 
     def __init__(
         self,
         instrument_code: Optional[str] = None,
         instrument_tag: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         fixed_rate_percent: Optional[float] = None,
         payment_business_day_convention: Union[BusinessDayConvention, str] = None,
         payment_roll_convention: Union[DateRollingConvention, str] = None,
         year_basis: Union[DayCountBasis, str] = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # coding: utf8
 from typing import Optional, Union
 
+from ....._types import OptDateTime
 from ..._enums import (
     BusinessDayConvention,
     DateRollingConvention,
     DayCountBasis,
     Frequency,
 )
 from .._instrument_definition import InstrumentDefinition
@@ -20,19 +21,19 @@
     instrument_tag : str, optional
         User defined string to identify the instrument. It can be used to link output
         results to the instrument definition. Only alphabetic, numeric and '- _.#=@'
         characters are supported.
     instrument_code : str, optional
         Code to define the term deposit instrument. For the moment, only RICs for CDs
         and Wholesales deposits are supported, with deposit code (ex:"EUR1MD=").
-    start_date : str, optional
+    start_date : str or date or datetime or timedelta, optional
         The date the term deposit starts accruing interest. Its effective date.
         By default it is derived from the ValuationDate and the day to spot convention
         of the contract currency.
-    end_date : str, optional
+    end_date : str or date or datetime or timedelta, optional
         The maturity date of the term deposit contract. Either the endDate or the tenor
         must be provided.
     tenor : str, optional
         The period code that represents the time between the start date and end date of
         the contract.
         Mandatory if instrumentCode is null. Either the endDate or the tenor must be
         provided.
@@ -65,16 +66,16 @@
     """
 
     def __init__(
         self,
         *,
         instrument_tag: Optional[str] = None,
         instrument_code: Optional[str] = None,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
+        start_date: "OptDateTime" = None,
+        end_date: "OptDateTime" = None,
         tenor: Optional[str] = None,
         notional_ccy: Optional[str] = None,
         notional_amount: Optional[float] = None,
         fixed_rate_percent: Optional[float] = None,
         payment_business_day_convention: Union[BusinessDayConvention, str] = None,
         payment_roll_convention: Union[DateRollingConvention, str] = None,
         year_basis: Union[DayCountBasis, str] = None,
@@ -181,15 +182,15 @@
         Either the endDate or the tenor must be provided.
         :return: str
         """
         return self._get_parameter("endDate")
 
     @end_date.setter
     def end_date(self, value):
-        self._set_parameter("endDate", value)
+        self._set_datetime_parameter("endDate", value)
 
     @property
     def fixed_rate_percent(self):
         """
         Fixed interest rate percent to be applied for notional by deal terms.
         E.g. "10" means 10%
         :return: float
@@ -263,15 +264,15 @@
         Optional. By default it is derived from the ValuationDate and the day to spot convention of the contract currency.
         :return: str
         """
         return self._get_parameter("startDate")
 
     @start_date.setter
     def start_date(self, value):
-        self._set_parameter("startDate", value)
+        self._set_datetime_parameter("startDate", value)
 
     @property
     def tenor(self):
         """
         The period code that represents the time between the start date and end date of the contract.
         Mandatory if instrumentCode is null.
         Either the endDate or the tenor must be provided.
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from typing import Optional, Union
 
 from ..._enums import PriceSide
 from ..._object_definition import ObjectDefinition
+from ....._types import OptDateTime
 
 
 class PricingParameters(ObjectDefinition):
     """
     API endpoint for Financial Contract analytics,
     that returns calculations relevant to each contract type.
 
     Parameters
     ----------
     price_side : PriceSide or str, optional
         Price Side to consider when retrieving Market Data.
-    market_data_date : str, optional
+    market_data_date : str or date or datetime or timedelta, optional
         The market data date for pricing.
         By default, the market_data_date date is the valuation_date or Today.
     report_ccy : str, optional
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). It is set for the fields ending with 'xxxinreportccy'. Optional. The
         default value is the notional currency.
-    valuation_date : str, optional
+    valuation_date : str or date or datetime or timedelta, optional
         The valuation date for pricing. If not set the valuation date is equal to
         market_data_date or Today. For assets that contains a settlementConvention, the
         default valuation date  is equal to the settlementdate of the Asset that is
         usually the TradeDate+SettlementConvention.
 
     Examples
     --------
@@ -34,17 +35,17 @@
 
     _income_tax_percent = None
 
     def __init__(
         self,
         price_side: Union[PriceSide, str] = None,
         income_tax_percent: Optional[float] = None,
-        market_data_date: Optional[str] = None,
+        market_data_date: "OptDateTime" = None,
         report_ccy: Optional[str] = None,
-        valuation_date: Optional[str] = None,
+        valuation_date: "OptDateTime" = None,
     ):
         super().__init__()
         self.price_side = price_side
         self.income_tax_percent = income_tax_percent
         self.market_data_date = market_data_date
         self.report_ccy = report_ccy
         self.valuation_date = valuation_date
@@ -76,15 +77,15 @@
         By default, the marketDataDate date is the ValuationDate or Today.
         :return: str
         """
         return self._get_parameter("marketDataDate")
 
     @market_data_date.setter
     def market_data_date(self, value):
-        self._set_parameter("marketDataDate", value)
+        self._set_datetime_parameter("marketDataDate", value)
 
     @property
     def report_ccy(self):
         """
         The reporting currency code, expressed in iso 4217 alphabetical format (e.g.,
         'usd'). it is set for the fields ending with 'xxxinreportccy'. optional. the
         default value is the notional currency.
@@ -105,8 +106,8 @@
         today.
         :return: str
         """
         return self._get_parameter("valuationDate")
 
     @valuation_date.setter
     def valuation_date(self, value):
-        self._set_parameter("valuationDate", value)
+        self._set_datetime_parameter("valuationDate", value)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/_news_data.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/_news_data_provider_layer.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/_news_data_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/_tools.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_data.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/headlines/_request_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/headlines/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/images/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/images/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/images/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/images/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/images/_image.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/images/_image.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_image_data.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_image_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/_report.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/_report.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/story/_data.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/story/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/story/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/story/_request_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/story/_response_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/story/_udf_html_parser.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/story/_udf_html_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/_top_news_headline.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/_top_news_headline.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py` & `refinitiv-data-1.3.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/_org_info_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
-from .._content_data import Data
-from .._content_provider_layer import ContentUsageLoggerMixin
-from ..._content_type import ContentType
-from ..._tools import validate_bool_value, try_copy_to_list
-from ...delivery._data._data_provider import DataProviderLayer, BaseResponse
+from ..._content_data import Data
+from ..._content_provider_layer import ContentUsageLoggerMixin
+from ...._content_type import ContentType
+from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ..._types import ExtendedParams, StrStrings
+    from ...._types import ExtendedParams, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the organization information for the requested instrument.
+    This class describe parameters to retrieve the latest consolidated shareholders report for the requested company.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
+    limit: int, optional
+        The limit parameter is used for paging. It allows users to select the number of records to be returned.
+
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
     >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.org_info.Definition("TRI.N")
+    >>> definition = ownership.consolidated.shareholders_report.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.OrgInfoDefinition"
+    _USAGE_CLS_NAME = "Ownership.Consolidated.ShareholdersReportDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
+        limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
+        validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_ORG_INFO,
+            ContentType.OWNERSHIP_CONSOLIDATED_SHAREHOLDERS_REPORT,
             universe=universe,
+            limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/_ownership_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/_ownership_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,60 @@
 from typing import Union, TYPE_CHECKING
 
-from .._enums import StatTypes
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
-from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ...._tools import validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
+    from .._enums import SortOrder
     from ...._types import ExtendedParams, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve holdings data breakdown by Investor Types,
-    Styles, Region, Countries, Rotations and Turnovers.
+    This class describe parameters to retrieve the latest 5 buy or sell activites for the requested company.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
-    stat_type: int, StatTypes
-        The statType parameter specifies which statistics type to be returned.
-        The types available are:
-            - Investor Type (1)
-            - Investment Style (2)
-            - Region (3)
-            - Rotation (4)
-            - Country (5)
-            - Metro Area (6)
-            - Investor Type Parent (7)
-            - Invest Style Parent (8)
+    sort_order: str, SortOrder
+        The sortOrder parameter specifies ascending (asc) or descending (desc) Sort Order.
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
-    extended_params: ExtendedParams, optional
+    extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
     >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.consolidated.breakdown.Definition("TRI.N", ownership.StatTypes.INVESTOR_TYPE)
-    >>> response = definition.get_data()
+    >>> definition = ownership.fund.recent_activity.Definition("TRI.N", ownership.SortOrder.ASCENDING)
+    >>> response = definition..get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Consolidated.BreakdownDefinition"
+    _USAGE_CLS_NAME = "Ownership.Fund.RecentActivityDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        stat_type: Union[int, StatTypes],
+        sort_order: Union[str, "SortOrder"],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(stat_type, [int, StatTypes], "stat_type")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_CONSOLIDATED_BREAKDOWN,
+            ContentType.OWNERSHIP_FUND_RECENT_ACTIVITY,
             universe=universe,
-            stat_type=stat_type,
+            sort_order=sort_order,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
-from ...._tools import validate_bool_value, try_copy_to_list
+from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
     from ...._types import ExtendedParams, StrStrings
 
 
 class Definition(
@@ -18,37 +18,44 @@
     This class describe parameters to retrieve the calculated concentration data by all consolidated investors.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
+    limit: int, optional
+        The limit parameter is used for paging. It allows users to select the number of records to be returned.
+        Default page size is 100 or 20 (depending on the operation).
+
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
     >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.consolidated.concentration.Definition("TRI.N")
+    >>> definition = ownership.consolidated.investors.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Consolidated.ConcentrationDefinition"
+    _USAGE_CLS_NAME = "Ownership.Consolidated.InvestorsDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
+        limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
+        validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_CONSOLIDATED_CONCENTRATION,
+            ContentType.OWNERSHIP_CONSOLIDATED_INVESTORS,
             universe=universe,
+            limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
@@ -11,51 +11,51 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the calculated concentration data by all consolidated investors.
+    This class describe parameters to retrieve the insider shareholders/declarable stakes investment
+    information in the requested company at the specified historical period.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
     limit: int, optional
         The limit parameter is used for paging. It allows users to select the number of records to be returned.
-        Default page size is 100 or 20 (depending on the operation).
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
     >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.consolidated.investors.Definition("TRI.N")
+    >>> definition = ownership.insider.shareholders_report.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Consolidated.InvestorsDefinition"
+    _USAGE_CLS_NAME = "Ownership.Insider.ShareholdersReportDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_CONSOLIDATED_INVESTORS,
+            ContentType.OWNERSHIP_INSIDER_SHAREHOLDERS_REPORT,
             universe=universe,
             limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_concentration_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,57 @@
-from typing import Union, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
 from ...._tools import validate_bool_value, try_copy_to_list
-from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
+from ....delivery._data._data_provider import (
+    DataProviderLayer,
+    BaseResponse,
+)
 
 if TYPE_CHECKING:
     from ...._types import ExtendedParams, StrStrings
-    from .._enums import SortOrder
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the latest 5 buy or sell activities for the requested company.
+    This class describe parameters to retrieve  the calculated concentration data for all fund investors.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
-    sort_order: str, SortOrder
-        The sortOrder parameter specifies ascending (asc) or descending (desc) Sort Order.
-
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
     >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.consolidated.recent_activity.Definition("TRI.N", "asc")
+    >>> definition = ownership.fund.concentration.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Consolidated.RecentActivityDefinition"
+    _USAGE_CLS_NAME = "Ownership.Fund.ConcentrationDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        sort_order: Union[str, "SortOrder"],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_CONSOLIDATED_RECENT_ACTIVITY,
+            ContentType.OWNERSHIP_FUND_CONCENTRATION,
             universe=universe,
-            sort_order=sort_order,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/investor/_holdings_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,50 +11,51 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the latest consolidated shareholders report for the requested company.
+    This class describe parameters to retrieve investor name, count and holdings data for any requested investor.
 
     Parameters
     ----------
     universe: str, list of str
         The Universe parameter allows the user to define the companies for which the content is returned.
 
     limit: int, optional
         The limit parameter is used for paging. It allows users to select the number of records to be returned.
+        Default page size is 100 or 20 (depending on the operation).
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
     >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.consolidated.shareholders_report.Definition("TRI.N")
+    >>> definition = ownership.investor.holdings.Definition("TRI.N")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Consolidated.ShareholdersReportDefinition"
+    _USAGE_CLS_NAME = "Ownership.Investor.HoldingsDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
         limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_CONSOLIDATED_SHAREHOLDERS_REPORT,
+            ContentType.OWNERSHIP_INVESTOR_HOLDINGS,
             universe=universe,
             limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 from typing import TYPE_CHECKING
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
-from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ...._tools import validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, StrStrings
+    from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the calculated concentration data
-    by top 10, 20, 50, 100 consolidated investors.
+    Describes the parameters used to retrieve the estimates summary values for KPI measures for interim periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
-    count: int
-        Number of records
-
+        Single instrument or list of instruments.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
+        Boolean that indicates whether or not to display field names in the headers.
+    extended_params: ExtendedParams, optional
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.consolidated.top_n_concentration.Definition("TRI.N", 30)
+    >>> from refinitiv.data.content import estimates
+    >>> definition = estimates.view_summary_kpi.interim.Definition(universe="BNPP.PA")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Consolidated.TopNConcentrationDefinition"
+    _USAGE_CLS_NAME = "Estimates.SummaryKPI.InterimDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        count: int,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(count, [int], "count")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_CONSOLIDATED_TOP_N_CONCENTRATION,
+            ContentType.ESTIMATES_VIEW_SUMMARY_KPI_INTERIM,
             universe=universe,
-            count=count,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_concentration_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-from typing import TYPE_CHECKING
+from typing import Union, TYPE_CHECKING
 
+from .._enums import Package
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
-from ...._tools import validate_bool_value, try_copy_to_list
-from ....delivery._data._data_provider import (
-    DataProviderLayer,
-    BaseResponse,
-)
+from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, StrStrings
+    from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve  the calculated concentration data for all fund investors.
+    Describes the parameters used to retrieve the estimates summary for all non-periodic estimates measures.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
+        Single instrument or list of instruments.
+    package: str, Package
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
+        Boolean that indicates whether or not to display field names in the headers.
+    extended_params: ExtendedParams, optional
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.fund.concentration.Definition("TRI.N")
+    >>> from refinitiv.data.content import estimates
+    >>> definition = estimates.view_summary.non_periodic_measures.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Fund.ConcentrationDefinition"
+    _USAGE_CLS_NAME = "Estimates.Summary.NonPeriodicMeasuresDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
+        package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
+        validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_FUND_CONCENTRATION,
+            ContentType.ESTIMATES_VIEW_SUMMARY_NON_PERIODIC_MEASURES,
             universe=universe,
+            package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_holdings_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_holdings_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_investors_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,80 @@
-from typing import TYPE_CHECKING, Optional
+from typing import Optional, TYPE_CHECKING
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, StrStrings
+    from ...._types import ExtendedParams, OptDateTime, StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve company ownership details. Also, information on
-    the top 20 fund shareholders invested in the requested company.
+    This class describe parameters to retrieve details on stakeholders and strategic entities
+    transactions that purchased the requested instruments. Further details of insider stakeholder
+    can be requested along with their holding details. The operation supports pagination, however,
+    it is dependent on user entitlements. Maximum 'count' value per page is 100. The default date
+    range is 20 transactions, unless the 'start date' and 'end date' define a smaller range. The
+    count value is checked by the service to determine if it does not exceed a specific number. If
+    it does, the service will overwrite the client value to service default value.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
+        The Universe parameter allows the user to define the single company for which the content is returned.
+
+    start: str, datetime, optional
+        The start parameter allows users to define the start date of a time series.
+        Dates are to be defined either by absolute or relative syntax.
+        Example, 20190529, -1Q, 1D, -3MA.
+
+    end: str, datetime, optional
+        The end parameter allows users to define the start date of a time series.
+        Dates are to be defined either by absolute or relative syntax.
+        Example, 20190529, -1Q, 1D, -3MA.
 
     limit: int, optional
         The limit parameter is used for paging. It allows users to select the number of records to be returned.
-        Default page size is 100 or 20 (depending on the operation).
 
     use_field_names_in_headers: bool, optional
         Return field name as column headers for data instead of title
 
     extended_params : ExtendedParams, optional
         If necessary other parameters.
 
     Examples
     --------
     >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.fund.investors.Definition("TRI.N")
+    >>> definition = ownership.insider.transaction_report.Definition("TRI.N", start="-1Q")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Fund.InvestorsDefinition"
+    _USAGE_CLS_NAME = "Ownership.Insider.TransactionReportDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
+        start: "OptDateTime" = None,
+        end: "OptDateTime" = None,
         limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
         validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_FUND_INVESTORS,
+            ContentType.OWNERSHIP_INSIDER_TRANSACTION_REPORT,
             universe=universe,
+            start=start,
+            end=end,
             limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/_basic_overview_definition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,57 @@
-from typing import Union, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
-from ..._content_data import Data
-from ..._content_provider_layer import ContentUsageLoggerMixin
-from ...._content_type import ContentType
-from ...._tools import validate_bool_value, try_copy_to_list
-from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
+from .._content_data import Data
+from .._content_provider_layer import ContentUsageLoggerMixin
+from ..._content_type import ContentType
+from ..._tools import create_repr, validate_bool_value, try_copy_to_list
+from ...delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from .._enums import SortOrder
-    from ...._types import ExtendedParams, StrStrings
+    from ..._types import StrStrings
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the latest 5 buy or sell activites for the requested company.
+    Defines the basic ESG data to retrieve.
 
     Parameters
     ----------
-    universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
-    sort_order: str, SortOrder
-        The sortOrder parameter specifies ascending (asc) or descending (desc) Sort Order.
-
+    universe : str, list of str
+        Single instrument or list of instruments.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
+        Boolean that indicates whether or not to display field names in the headers.
 
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.fund.recent_activity.Definition("TRI.N", ownership.SortOrder.ASCENDING)
-    >>> response = definition..get_data()
+    >>> from refinitiv.data.content import esg
+    >>> definition = esg.basic_overview.Definition("IBM.N")
+    >>> response = definition.get_data()
+
+    >>> response = await definition.get_data_async()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Fund.RecentActivityDefinition"
+    _USAGE_CLS_NAME = "ESG.BasicOverviewDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        sort_order: Union[str, "SortOrder"],
         use_field_names_in_headers: bool = False,
-        extended_params: "ExtendedParams" = None,
     ):
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_FUND_RECENT_ACTIVITY,
+            ContentType.ESG_BASIC_OVERVIEW,
             universe=universe,
-            sort_order=sort_order,
             use_field_names_in_headers=use_field_names_in_headers,
-            extended_params=extended_params,
+        )
+
+    def __repr__(self):
+        return create_repr(
+            self,
+            middle_path="basic_overview",
+            content=f"{{universe='{self._kwargs.get('universe')}'}}",
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
-from ...._tools import validate_types, validate_bool_value, try_copy_to_list
+from ...._tools import validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, StrStrings
+    from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
-
     """
-    This class describe parameters to retrieve the latest fund shareholders
-    investment information for the requested company.
+    Describes the parameters used to retrieve the estimated actuals values for KPI Measures for the reported annual
+    periods.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
-    limit: int, optional
-        The limit parameter is used for paging. It allows users to select the number of records to be returned.
-
+        Single instrument or list of instruments.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
+        Boolean that indicates whether or not to display field names in the headers.
+    extended_params: ExtendedParams, optional
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.fund.shareholders_report.Definition("TRI.N")
+    >>> from refinitiv.data.content import estimates
+    >>> definition = estimates.view_actuals_kpi.annual.Definition(universe="BNPP.PA")
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Fund.ShareholdersReportDefinition"
+    _USAGE_CLS_NAME = "Estimates.ActualsKPI.AnnualDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        limit: Optional[int] = None,
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(limit, [int, type(None)], "limit")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_FUND_SHAREHOLDERS_REPORT,
+            ContentType.ESTIMATES_VIEW_ACTUALS_KPI_ANNUAL,
             universe=universe,
-            limit=limit,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import TYPE_CHECKING
+from typing import Union, TYPE_CHECKING
 
+from .._enums import Package
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
@@ -11,51 +12,49 @@
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the calculated concentration data
-    by top 10, 20, 50, 100 fund investors.
+    Describes the parameters used to retrieve the estimates monthly historical snapshot value for the last 12 months
+    for all annual period estimates measures.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
-    count: int
-        Number of records
-
+        Single instrument or list of instruments.
+    package: str, Package
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history)
+        of the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
+        Boolean that indicates whether or not to display field names in the headers.
+    extended_params: ExtendedParams, optional
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.fund.top_n_concentration.Definition("TRI.N", 30)
+    >>> from refinitiv.data.content import estimates
+    >>> definition = estimates.view_summary.historical_snapshots_periodic_measures_annual.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Fund.TopNConcentrationDefinition"
+    _USAGE_CLS_NAME = "Estimates.Summary.HistoricalSnapshotsPeriodicMeasuresAnnualDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        count: int,
+        package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(count, [int], "count")
+        validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_FUND_TOP_N_CONCENTRATION,
+            ContentType.ESTIMATES_VIEW_SUMMARY_HISTORICAL_SNAPSHOTS_PERIODIC_MEASURES_ANNUAL,
             universe=universe,
-            count=count,
+            package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-from typing import TYPE_CHECKING, Optional
+from typing import Union, TYPE_CHECKING
 
 from ..._content_data import Data
 from ..._content_provider_layer import ContentUsageLoggerMixin
+from .._enums import Package
 from ...._content_type import ContentType
 from ...._tools import validate_types, validate_bool_value, try_copy_to_list
 from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, StrStrings
+    from ...._types import StrStrings, ExtendedParams
 
 
 class Definition(
     ContentUsageLoggerMixin[BaseResponse[Data]],
     DataProviderLayer[BaseResponse[Data]],
 ):
     """
-    This class describe parameters to retrieve the insider shareholders/declarable stakes investment
-    information in the requested company at the specified historical period.
+    Describes the parameters used to retrieve the estimates monthly historical snapshot value for non-periodic
+    estimate measures for the last 12 months.
 
     Parameters
     ----------
     universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
-    limit: int, optional
-        The limit parameter is used for paging. It allows users to select the number of records to be returned.
-
+        Single instrument or list of instruments.
+    package: str, Package
+        Packages of the content that are subsets in terms of breadth (number of fields) and depth (amount of history) of
+        the overall content set.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
+        Boolean that indicates whether or not to display field names in the headers.
+    extended_params: ExtendedParams, optional
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.insider.shareholders_report.Definition("TRI.N")
+    >>> from refinitiv.data.content import estimates
+    >>> definition = estimates.view_summary.historical_snapshots_non_periodic_measures.Definition(universe="IBM.N", package=estimates.Package.BASIC)
     >>> response = definition.get_data()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Insider.ShareholdersReportDefinition"
+    _USAGE_CLS_NAME = "Estimates.Summary.HistoricalSnapshotsNonPeriodicMeasuresDefinition"
 
     def __init__(
         self,
         universe: "StrStrings",
-        limit: Optional[int] = None,
+        package: Union[str, Package],
         use_field_names_in_headers: bool = False,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(limit, [int, type(None)], "limit")
+        validate_types(package, [str, Package], "package")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_INSIDER_SHAREHOLDERS_REPORT,
+            ContentType.ESTIMATES_VIEW_SUMMARY_HISTORICAL_SNAPSHOTS_NON_PERIODIC_MEASURES,
             universe=universe,
-            limit=limit,
+            package=package,
             use_field_names_in_headers=use_field_names_in_headers,
             extended_params=extended_params,
         )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_definition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,114 @@
-from typing import Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
-from ..._content_data import Data
-from ..._content_provider_layer import ContentUsageLoggerMixin
-from ...._content_type import ContentType
-from ...._tools import validate_types, validate_bool_value, try_copy_to_list
-from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
+from ._stream import (
+    Events,
+    FinalizedOrders,
+    UniverseTypes,
+    universe_type_arg_parser,
+    finalized_orders_arg_parser,
+    events_arg_parser,
+)
+from ._stream_facade import Stream
+from ..._tools import create_repr, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, OptDateTime, StrStrings
+    from ..._types import OptStr, ExtendedParams, OptStrStrs
+    from ..._core.session import Session
 
 
-class Definition(
-    ContentUsageLoggerMixin[BaseResponse[Data]],
-    DataProviderLayer[BaseResponse[Data]],
-):
+class Definition:
     """
-    This class describe parameters to retrieve details on stakeholders and strategic entities
-    transactions that purchased the requested instruments. Further details of insider stakeholder
-    can be requested along with their holding details. The operation supports pagination, however,
-    it is dependent on user entitlements. Maximum 'count' value per page is 100. The default date
-    range is 20 transactions, unless the 'start date' and 'end date' define a smaller range. The
-    count value is checked by the service to determine if it does not exceed a specific number. If
-    it does, the service will overwrite the client value to service default value.
+    This class describes Analytics Trade Data Service.
 
     Parameters
     ----------
-    universe: str, list of str
-        The Universe parameter allows the user to define the single company for which the content is returned.
-
-    start: str, datetime, optional
-        The start parameter allows users to define the start date of a time series.
-        Dates are to be defined either by absolute or relative syntax.
-        Example, 20190529, -1Q, 1D, -3MA.
-
-    end: str, datetime, optional
-        The end parameter allows users to define the start date of a time series.
-        Dates are to be defined either by absolute or relative syntax.
-        Example, 20190529, -1Q, 1D, -3MA.
-
-    limit: int, optional
-        The limit parameter is used for paging. It allows users to select the number of records to be returned.
-
-    use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
+    universe : list, optional
+        A list of RIC or symbol or user's id for retrieving trading analytics data.
+    fields : list, optional
+        A list of enumerate fields.
+    events : str or Events, optional
+        Enable/Disable the detail of order event in the streaming.
+        Default: False
+    finalized_orders : str or FinalizedOrders, optional
+        Enable/Disable the cached of finalized order of current day in the streaming.
+        Default: False
+    filters : list, optional
+        Set the condition of subset of trading streaming data.
+    universe_type : str or UniverseTypes, optional
+        A type of given universe can be RIC, Symbol or UserID.
+        Default: UniverseTypes.RIC
+    api: str, optional
+        Specifies the data source. It can be updated/added using config file
+    extended_params : dict, optional
+        If necessary other parameters
+
+    Methods
+    -------
+    get_stream(session=session)
+        Get stream object of this definition
 
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.insider.transaction_report.Definition("TRI.N", start="-1Q")
-    >>> response = definition.get_data()
+    >>> from refinitiv.data.content import trade_data_service
+    >>> definition = trade_data_service.Definition()
     """
 
-    _USAGE_CLS_NAME = "Ownership.Insider.TransactionReportDefinition"
-
     def __init__(
         self,
-        universe: "StrStrings",
-        start: "OptDateTime" = None,
-        end: "OptDateTime" = None,
-        limit: Optional[int] = None,
-        use_field_names_in_headers: bool = False,
+        universe: "OptStrStrs" = None,
+        universe_type: Union[str, UniverseTypes] = UniverseTypes.UserID,
+        fields: "OptStrStrs" = None,
+        events: Union[str, Events] = Events.No,
+        finalized_orders: Union[str, FinalizedOrders] = FinalizedOrders.No,
+        filters: "OptStrStrs" = None,
+        api: "OptStr" = None,
         extended_params: "ExtendedParams" = None,
     ):
-        validate_types(limit, [int, type(None)], "limit")
-        validate_bool_value(use_field_names_in_headers)
-        universe = try_copy_to_list(universe)
-
-        super().__init__(
-            ContentType.OWNERSHIP_INSIDER_TRANSACTION_REPORT,
-            universe=universe,
-            start=start,
-            end=end,
-            limit=limit,
-            use_field_names_in_headers=use_field_names_in_headers,
-            extended_params=extended_params,
+        self._universe = try_copy_to_list(universe)
+        self._universe_type = universe_type_arg_parser.get_str(universe_type)
+        self._fields = try_copy_to_list(fields)
+        self._events = events_arg_parser.get_str(events)
+        self._finalized_orders = finalized_orders_arg_parser.get_str(finalized_orders)
+        self._filters = try_copy_to_list(filters)
+        self._api = api
+        self._extended_params = extended_params
+
+    def __repr__(self):
+        return create_repr(
+            self,
+            middle_path="content.trade_data_service",
+            content={"universe": self._universe},
+        )
+
+    def get_stream(self, session: "Session" = None) -> Stream:
+        """
+        Returns a streaming trading analytics subscription.
+
+        Parameters
+        ----------
+        session : Session, optional
+            The Session used by the TradeDataService to retrieve data from the platform
+
+        Returns
+        -------
+        TradeDataStream
+
+        Examples
+        --------
+        >>> from refinitiv.data.content import trade_data_service
+        >>> definition = trade_data_service.Definition()
+        >>> stream = definition.get_stream()
+        >>> stream.open()
+        """
+        stream = Stream(
+            session=session,
+            universe=self._universe,
+            universe_type=self._universe_type,
+            fields=self._fields,
+            events=self._events,
+            finalized_orders=self._finalized_orders,
+            filters=self._filters,
+            api=self._api,
+            extended_params=self._extended_params,
         )
+        return stream
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/ownership/investor/_holdings_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/esg/_full_scores_definition.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,53 @@
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
-from ..._content_data import Data
-from ..._content_provider_layer import ContentUsageLoggerMixin
-from ...._content_type import ContentType
-from ...._tools import validate_types, validate_bool_value, try_copy_to_list
-from ....delivery._data._data_provider import DataProviderLayer, BaseResponse
+from ._base_definition import BaseDefinition
+from ..._content_type import ContentType
+from ..._tools import validate_types, validate_bool_value, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ...._types import ExtendedParams, StrStrings
+    from ..._types import StrStrings, OptInt
 
 
-class Definition(
-    ContentUsageLoggerMixin[BaseResponse[Data]],
-    DataProviderLayer[BaseResponse[Data]],
-):
+class Definition(BaseDefinition):
     """
-    This class describe parameters to retrieve investor name, count and holdings data for any requested investor.
+    Defines the ESG full scores data to retrieve.
 
     Parameters
     ----------
-    universe: str, list of str
-        The Universe parameter allows the user to define the companies for which the content is returned.
-
-    limit: int, optional
-        The limit parameter is used for paging. It allows users to select the number of records to be returned.
-        Default page size is 100 or 20 (depending on the operation).
-
+    universe : str, list of str
+        Single instrument or list of instruments.
+    start : int, optional
+        Initial value of financial years range to return.
+    end : int, optional
+        End range of financial years to return.
     use_field_names_in_headers: bool, optional
-        Return field name as column headers for data instead of title
-
-    extended_params : ExtendedParams, optional
-        If necessary other parameters.
-
+        Boolean that indicates whether or not to display field names in the headers.
     Examples
     --------
-    >>> from refinitiv.data.content import ownership
-    >>> definition = ownership.investor.holdings.Definition("TRI.N")
-    >>> response = definition.get_data()
+    >>> from refinitiv.data.content import esg
+    >>> definition = esg.full_scores.Definition(universe="4295904307", start=0, end=-5)
     """
 
-    _USAGE_CLS_NAME = "Ownership.Investor.HoldingsDefinition"
-
     def __init__(
         self,
         universe: "StrStrings",
-        limit: Optional[int] = None,
+        start: "OptInt" = None,
+        end: "OptInt" = None,
         use_field_names_in_headers: bool = False,
-        extended_params: "ExtendedParams" = None,
     ):
-        validate_types(limit, [int, type(None)], "limit")
+        validate_types(start, [int, type(None)], "start")
+        validate_types(end, [int, type(None)], "end")
         validate_bool_value(use_field_names_in_headers)
         universe = try_copy_to_list(universe)
 
         super().__init__(
-            ContentType.OWNERSHIP_INVESTOR_HOLDINGS,
+            ContentType.ESG_FULL_SCORES,
             universe=universe,
-            limit=limit,
+            start=start,
+            end=end,
             use_field_names_in_headers=use_field_names_in_headers,
-            extended_params=extended_params,
         )
+
+    def __repr__(self):
+        get_repr = super().__repr__()
+        return get_repr.replace("esg", "esg.full_scores")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_definition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,106 +1,90 @@
-from typing import TYPE_CHECKING
+# coding: utf8
 
-from ._pricing_content_provider import PricingData
-from ._stream_facade import Stream
-from .._content_provider_layer import ContentUsageLoggerMixin
-from ..._content_type import ContentType
-from ..._core.session import Session
-from ..._tools import create_repr, try_copy_to_list
-from ..._tools._common import universe_arg_parser, fields_arg_parser
-from ...delivery._data._data_provider import DataProviderLayer, BaseResponse
+
+from typing import TYPE_CHECKING, Optional
+
+from .omm_stream import OMMStream
+from ..._tools import create_repr, fields_arg_parser, try_copy_to_list
 
 if TYPE_CHECKING:
-    from ..._types import OptStr, ExtendedParams, StrStrings, OptStrStrs
+    from ..._types import ExtendedParams, OptStrStrs
+    from ..._core.session import Session
 
 
-class Definition(
-    ContentUsageLoggerMixin[BaseResponse[PricingData]],
-    DataProviderLayer[BaseResponse[PricingData]],
-):
+class Definition:
     """
-    This class defines parameters for requesting events from pricing
+    This class to subscribe to streaming items of any Domain Model
+    (e.g. MarkePrice, MarketByPrice, ...)
+    exposed by the underlying of the Refinitiv Data
 
     Parameters
     ----------
-    universe : str or list of str
-        The single/multiple instrument/s name (e.g. "EUR=" or ["EUR=", "CAD=", "UAH="]).
-    fields : str or list of str, optional
-        Specifies the specific fields to be delivered when messages arrive
-    service : str, optional
-        Name of the streaming service publishing the instruments
+    name : str, optional
+        Streaming instrument name.
     api: str, optional
-        Specifies the data source. It can be updated/added using config file
+        Streaming data source.
+    service : str, optional
+        Third-party service URL to manage the streaming data.
+    fields : str or list, optional
+        Single field or list of fields to return.
+    domain : str, optional
+        Specific streaming data domain.
     extended_params : dict, optional
-        Other parameters can be provided if necessary
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
-    >>> from refinitiv.data.content import pricing
-    >>> definition = pricing.Definition("EUR=")
-    >>> response = definition.get_data()
-
+    >>> from refinitiv.data.delivery import omm_stream
+    >>> definition = omm_stream.Definition("EUR")
     """
 
-    _USAGE_CLS_NAME = "Pricing.PricingDefinition"
-
     def __init__(
         self,
-        universe: "StrStrings",
+        name: str,
+        api: Optional[str] = None,
+        service: Optional[str] = None,
         fields: "OptStrStrs" = None,
-        service: "OptStr" = None,
-        api: "OptStr" = None,
+        domain: str = "MarketPrice",
         extended_params: "ExtendedParams" = None,
     ) -> None:
-        extended_params = extended_params or {}
-        universe = extended_params.pop("universe", universe)
-        universe = try_copy_to_list(universe)
-        universe = universe_arg_parser.get_list(universe)
-        fields = extended_params.pop("fields", fields)
-        fields = try_copy_to_list(fields)
-        fields = fields_arg_parser.get_unique(fields or [])
-        super().__init__(
-            data_type=ContentType.PRICING,
-            universe=universe,
-            fields=fields,
-            extended_params=extended_params,
-        )
-        self._universe = universe
-        self._fields = fields
-        self._service = service
+        self._name = name
         self._api = api
+        self._domain = domain
+        self._service = service
+        fields = try_copy_to_list(fields)
+        self._fields = fields and fields_arg_parser.get_list(fields)
         self._extended_params = extended_params
 
-    def __repr__(self) -> str:
-        return create_repr(
-            self,
-            content=f"{{name={self._universe}}}",
-        )
+    def __repr__(self):
+        content = f"{{name='{self._name}'}}"
+        return create_repr(self, middle_path="omm_stream", content=content)
 
-    def get_stream(self, session: Session = None) -> Stream:
+    def get_stream(self, session: "Session" = None) -> OMMStream:
         """
-        Summary line of this func create a pricing.Stream object for the defined data
+        Returns the previously defined data stream from the Refinitiv Data Platform.
 
         Parameters
         ----------
-        session : Session, optional
-            The Session defines the source where you want to retrieve your data
+        session: Session, optional
+            Session object. If it's not passed the default session will be used.
 
         Returns
         -------
-        pricing.Stream
+        OMMStream instance
 
         Examples
         --------
-        >>> from refinitiv.data.content import pricing
-        >>> definition = pricing.Definition("IBM")
+        >>> from refinitiv.data.delivery import omm_stream
+        >>> definition = omm_stream.Definition("EUR")
         >>> stream = definition.get_stream()
-        >>> stream.open()
         """
-        return Stream(
-            universe=self._universe,
+        stream = OMMStream(
             session=session,
-            fields=self._fields,
-            service=self._service,
+            name=self._name,
             api=self._api,
+            service=self._service,
+            fields=self._fields,
+            domain=self._domain,
             extended_params=self._extended_params,
         )
+        return stream
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/_pricing_content_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/_pricing_content_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/_stream_facade.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/_stream_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,32 +88,26 @@
             service=self._service,
             api=self._api,
             extended_params=self._extended_params,
         )
 
     def open(self, with_updates: bool = True) -> "OpenState":
         """
-        Summary line of this func open the Pricing connection by sending corresponding
-        requests for all requested instruments
+        Opens the streaming connection to the Pricing data, and sends corresponding requests for all requested
+        instruments.
 
-        Extended description of this class:
-             It will be opened once all the requested instruments are received
-             either on_refresh, on_status or other method.
-             Then the pricing.Stream can be used in order to retrieve data.
+         It will be opened once all the requested instruments are received
+         either on_refresh, on_status or other method.
+         Then the pricing.stream can be used in order to retrieve data.
 
         Parameters
         ----------
         with_updates : bool, optional
-            actions:
-                True - the streaming will work as usual and the data will be received
-                continuously.
-                False - only one data snapshot will be received
-                (single Refresh 'NonStreaming') and stream will be closed automatically.
-
-            Default: True
+            Boolean indicator of how to work with the stream. If True - all data will be received continuously. If
+            False - only the data snapshot will be received.
 
         Returns
         -------
         OpenState
 
         Examples
         --------
@@ -122,15 +116,15 @@
         >>> stream = definition.get_stream()
         >>> stream.open()
         """
         return super().open(with_updates=with_updates)
 
     def close(self) -> "OpenState":
         """
-        Summary line of this func closes the pricing connection, releases resources
+        Closes the streaming connection to the Pricing data.
 
         Returns
         -------
         OpenState
 
         Examples
         --------
@@ -173,28 +167,27 @@
     def get_snapshot(
         self,
         universe: Optional[Union[str, Strings]] = None,
         fields: Optional[Union[str, Strings]] = None,
         convert: OptBool = True,
     ) -> "pandas.DataFrame":
         """
-        Returns a Dataframe filled with snapshot values for a list of instrument names
-        and a list of fields.
+        Returns a snapshot of the instruments stored in the in-memory data cache of the stream. When the stream is
+        opened, this data cache is kept up-to-date with the latest updates received from the platform.
 
         Parameters
         ----------
         universe: str, list of str, optional
-            List of instruments to request snapshot data on.
+            Single instrument or list of instruments.
 
         fields: str, list of str, optional
-            List of fields to request.
+            Single field or list of fields to return.
 
         convert: bool, optional
-            If True, force numeric conversion for all values.
-            By default True.
+            If True - force numeric conversion to all values.
 
         Returns
         -------
             pandas.DataFrame
 
             pandas.DataFrame content:
                 - columns : instrument and fieled names
@@ -224,23 +217,20 @@
         """
         df = self._stream.get_snapshot(universe=universe, fields=fields, convert=convert)
         convert_df_columns_to_datetime_re(df, PRICING_DATETIME_PATTERN)
         return df
 
     def on_refresh(self, func: Callable[[Any, str, "Stream"], Any]) -> "Stream":
         """
-        Called when a stream on instrument_name was opened successfully or when the
-        stream is refreshed by the server
-        This callback is called with the reference to the steam object, the instrument
-        name and the instrument full image
+        Called every time the whole fields list of a requested instrument is received from the platform.
 
         Parameters
         ----------
         func : Callable
-            Callable object to process retrieved data
+            Callable object to process the retrieved data.
 
         Returns
         -------
         current instance
 
         Examples
         --------
@@ -255,22 +245,20 @@
         >>> stream.open()
         """
         self._stream.on_refresh(make_callback(func))
         return self
 
     def on_update(self, func: Callable[[Any, str, "Stream"], Any]) -> "Stream":
         """
-        Called when an update is received for a instrument_name
-        This callback is called with the reference to the stream object, the instrument
-        name and the instrument update
+        Called when some fields of one of the requested instruments are updated.
 
         Parameters
         ----------
         func : Callable
-            Callable object to process retrieved data
+            Callable object to process the retrieved data
 
         Returns
         -------
         current instance
 
         Examples
         --------
@@ -285,22 +273,20 @@
         >>> stream.open()
         """
         self._stream.on_update(make_callback(func))
         return self
 
     def on_status(self, func: Callable[[Any, str, "Stream"], Any]) -> "Stream":
         """
-        Called when a status is received for a instrument_name
-        This callback is called with the reference to the stream object, the instrument
-        name and the instrument status
+        Called when a status is received for one of the requested instruments.
 
         Parameters
         ----------
         func : Callable
-            Callable object to process retrieved data
+            Callable object to process the retrieved data.
 
         Returns
         -------
         current instance
 
         Examples
         --------
@@ -313,21 +299,21 @@
         >>> stream.open()
         """
         self._stream.on_status(make_callback(func))
         return self
 
     def on_complete(self, func: Callable[["Stream"], Any]) -> "Stream":
         """
-        Called when all subscriptions are completed
-        This callback is called with the reference to the stream object
+        Called after the requested instruments and fields are completely received. on_complete is only called once
+        per stream opening.
 
         Parameters
         ----------
         func : Callable
-            Callable object to process retrieved data
+            Callable object to process the retrieved data
 
         Returns
         -------
         current instance
 
         Examples
         --------
@@ -346,20 +332,20 @@
 
     def on_error(self, func: Callable) -> "Stream":
         self._stream.on_error(make_callback(func))
         return self
 
     def on_ack(self, func: Callable) -> "Stream":
         """
-        This function called when the stream received an ack message after sending a contribution.
+        Called when a data retrieval error happens.
 
         Parameters
         ----------
         func : Callable, optional
-             Callable object to process retrieved ack data
+             Callable object to process the retrieved data.
 
         Returns
         -------
         Stream
             current instance
 
         Examples
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_chain_record.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_record.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_chain_records.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chain_records.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 if TYPE_CHECKING:
     from ...._types import ExtendedParams
     from ...._core.session import Session
 
 
 class Definition(object):
     """
-    Class is designed to request streaming chains and decode it dynamically
+    Creates a definition of information about the specified chains to request and decode them dynamically.
 
     Parameters
     ----------
     name : str
-        Single instrument name
+        Single instrument chain name.
     service : str, optional
-        Name service
+        Streaming service name.
     skip_summary_links : bool, optional
-        Store skip summary links
+        If True - summary links will be skipped.
     skip_empty : bool, optional
-        Store skip empty
+        If True - empty data items will be skipped.
     override_summary_links : int, optional
-        Store the override number of summary links
+        Number of summary links that can be overridden.
     extended_params : dict, optional
-        If necessary other parameters
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.content.pricing import chain
     >>> definition_chain = chain.Definition("0#.FTSE")
     """
 
@@ -59,20 +59,21 @@
         )
 
     def get_stream(
         self,
         session: "Session" = None,
     ) -> Stream:
         """
-        Return a chain.Stream object for the defined data
+        Creates and returns the pricing chain object that allows you to get streaming data for previously defined
+        chains.
 
         Parameters
         ----------
         session : Session, optional
-            The Session defines the source where you want to retrieve your data
+            Session object. If it's not passed the default session will be used.
 
         Returns
         -------
         chain.Stream
 
         Examples
         -------
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_display_template.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_display_template.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/pricing/chain/_stream_facade.py` & `refinitiv-data-1.3.0/refinitiv/data/content/pricing/chain/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/search/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/content/search/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/search/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/search/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/search/_lookup_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/search/_lookup_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/search/_metadata_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/search/_metadata_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/search/_views.py` & `refinitiv-data-1.3.0/refinitiv/data/content/search/_views.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_asset_class.py` & `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_asset_state.py` & `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_asset_state.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_country_code.py` & `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_country_code.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
             ret_val = f"{ret_val} and ({search_all_category}{rcs_asset_category})"
 
     return ret_val
 
 
 class Definition(ContentProviderLayer):
     """
-    This class describe parameters to retrieve data for symbol conversion.
+    Creates a definition of information about the data that will be passed to the Search/Lookup API of the Refinitiv
+    Data Platform.
 
     Parameters
     ----------
     symbols: str or list of str
         Single instrument or list of instruments to convert.
 
     from_symbol_type: str or SymbolTypes, optional
@@ -64,15 +65,15 @@
 
     to_symbol_types: SymbolTypes, str or list of str or SymbolTypes, optional
         Instrument code to convert to.
         Possible values: 'CUSIP', 'ISIN', 'SEDOL', 'RIC', 'ticker', 'lipperID', 'IMO', 'OAPermID'
         Default: all symbol types are requested
 
     extended_params: dict, optional
-        Other parameters can be provided if necessary
+        Specifies the parameters that will be merged with the request.
 
     preferred_country_code: str or CountryCode, optional
         Unique ISO 3166 code for country
 
     asset_class: str or AssetClass, optional
         AssetClass value to build filter parameter.
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/symbol_conversion/_symbol_type.py` & `refinitiv-data-1.3.0/refinitiv/data/content/symbol_conversion/_symbol_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/trade_data_service/_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/content/trade_data_service/_stream_facade.py` & `refinitiv-data-1.3.0/refinitiv/data/content/trade_data_service/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_api_type.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_api_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_connection.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_provider_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,77 +20,45 @@
     custom_instruments_interday_summaries_data_provider,
     custom_instruments_intraday_summaries_data_provider,
 )
 from ...content.esg._esg_data_provider import esg_data_provider
 from ...content.estimates._data_provider import estimates_data_provider
 from ...content.filings._retrieval_data_provider import filings_retrieval_data_provider
 from ...content.filings._search_data_provider import filings_search_data_provider
-from ...content.fundamental_and_reference._data_provider import (
-    data_grid_rdp_data_provider,
-    data_grid_udf_data_provider,
-)
+from ...content.fundamental_and_reference._data_provider import data_grid_rdp_data_provider, data_grid_udf_data_provider
 from ...content.historical_pricing._historical_pricing_data_provider import (
     hp_events_data_provider,
     hp_summaries_data_provider,
 )
 from ...content.ipa._curves._curves_data_provider import (
     curves_data_provider,
     cross_currency_curves_definitions_data_provider,
     cross_currency_curves_definitions_delete_data_provider,
     cross_currency_curves_triangulate_definitions_data_provider,
     curve_data_provider,
+    forward_curves_data_provider,
 )
 from ...content.ipa._surfaces._surfaces_data_provider import surfaces_data_provider, swaption_surfaces_data_provider
-from ...content.ipa.dates_and_calendars.add_periods._add_periods_data_provider import (
-    add_period_data_provider,
-)
-from ...content.ipa.dates_and_calendars.holidays._holidays_data_provider import (
-    holidays_data_provider,
-)
-from ...content.ipa.dates_and_calendars.count_periods._count_periods_data_provider import (
-    count_periods_data_provider,
-)
-from ...content.ipa.dates_and_calendars.date_schedule._date_schedule_data_provider import (
-    date_schedule_data_provider,
-)
-from ...content.ipa.dates_and_calendars.is_working_day._is_working_day_data_provider import (
-    is_working_day_data_provider,
-)
-from ...content.ipa.financial_contracts._contracts_data_provider import (
-    contracts_data_provider,
-)
-from ...content.news.story._data_provider import (
-    news_story_data_provider_rdp,
-    news_story_data_provider_udf,
-)
-from ...content.news.headlines._data_provider import (
-    news_headlines_data_provider_udf,
-    news_headlines_data_provider_rdp,
-)
-from ...content.news.online_reports._data_provider import (
-    news_online_reports_data_provider,
-)
-from ...content.news.online_reports.hierarchy._data_provider import (
-    news_online_reports_hierarchy_data_provider,
-)
-from ...content.news.top_news._data_provider import (
-    news_top_news_data_provider,
-)
-from ...content.news.top_news.hierarchy._data_provider import (
-    news_top_news_hierarchy_data_provider,
-)
+from ...content.ipa.dates_and_calendars.add_periods._add_periods_data_provider import add_period_data_provider
+from ...content.ipa.dates_and_calendars.holidays._holidays_data_provider import holidays_data_provider
+from ...content.ipa.dates_and_calendars.count_periods._count_periods_data_provider import count_periods_data_provider
+from ...content.ipa.dates_and_calendars.date_schedule._date_schedule_data_provider import date_schedule_data_provider
+from ...content.ipa.dates_and_calendars.is_working_day._is_working_day_data_provider import is_working_day_data_provider
+from ...content.ipa.financial_contracts._contracts_data_provider import contracts_data_provider
+from ...content.news.story._data_provider import news_story_data_provider_rdp, news_story_data_provider_udf
+from ...content.news.headlines._data_provider import news_headlines_data_provider_udf, news_headlines_data_provider_rdp
+from ...content.news.online_reports._data_provider import news_online_reports_data_provider
+from ...content.news.online_reports.hierarchy._data_provider import news_online_reports_hierarchy_data_provider
+from ...content.news.top_news._data_provider import news_top_news_data_provider
+from ...content.news.top_news.hierarchy._data_provider import news_top_news_hierarchy_data_provider
 from ...content.news.images._data_provider import news_images_data_provider
 from ...content.ownership._ownership_data_provider import ownership_data_provider
 from ...content.pricing._pricing_content_provider import pricing_data_provider
 from ...content.pricing.chain._chains_data_provider import chains_data_provider
-from ...content.search._data_provider import (
-    search_data_provider,
-    lookup_data_provider,
-    metadata_data_provider,
-)
+from ...content.search._data_provider import search_data_provider, lookup_data_provider, metadata_data_provider
 
 if TYPE_CHECKING:
     from ._data_provider import DataProvider
     from ..._configure import _RDPConfig
 
 data_provider_by_data_type = {
     ContentType.CHAINS: chains_data_provider,
@@ -126,15 +94,15 @@
     ContentType.ESTIMATES_VIEW_SUMMARY_KPI_HISTORICAL_SNAPSHOTS_KPI: estimates_data_provider,
     ContentType.ESTIMATES_VIEW_SUMMARY_KPI_INTERIM: estimates_data_provider,
     ContentType.ESTIMATES_VIEW_SUMMARY_NON_PERIODIC_MEASURES: estimates_data_provider,
     ContentType.ESTIMATES_VIEW_SUMMARY_RECOMMENDATIONS: estimates_data_provider,
     ContentType.FILINGS_RETRIEVAL: filings_retrieval_data_provider,
     ContentType.FILINGS_SEARCH: filings_search_data_provider,
     ContentType.BOND_CURVE: curves_data_provider,
-    ContentType.FORWARD_CURVE: curves_data_provider,
+    ContentType.FORWARD_CURVE: forward_curves_data_provider,
     ContentType.CROSS_CURRENCY_CURVES_CURVES: curve_data_provider,
     ContentType.CROSS_CURRENCY_CURVES_DEFINITIONS_CREATE: cross_currency_curves_definitions_data_provider,
     ContentType.CROSS_CURRENCY_CURVES_DEFINITIONS_DELETE: cross_currency_curves_definitions_delete_data_provider,
     ContentType.CROSS_CURRENCY_CURVES_DEFINITIONS_GET: cross_currency_curves_definitions_data_provider,
     ContentType.CROSS_CURRENCY_CURVES_DEFINITIONS_UPDATE: cross_currency_curves_definitions_data_provider,
     ContentType.CROSS_CURRENCY_CURVES_DEFINITIONS_SEARCH: curve_data_provider,
     ContentType.CROSS_CURRENCY_CURVES_TRIANGULATE_DEFINITIONS_SEARCH: cross_currency_curves_triangulate_definitions_data_provider,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_data_provider_layer.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_data_provider_layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -125,26 +125,58 @@
         _check_response(response, config)
 
     def get_data(
         self,
         session: Optional["Session"] = None,
         on_response: Optional[Callable] = None,
     ) -> TypeData:
+        """
+        Sends a request to the client file store to retrieve the previously defined data.
+
+        Parameters
+        ----------
+        session : Session
+            Session object. If it's not passed the default session will be used.
+        on_response : Callable
+            User-defined callback function to process the retrieved data.
+
+        Returns
+        -------
+        TypeData instance.
+
+        """
         session = get_valid_session(session)
         response = get_data(self._data_type, self._provider, session, **self._kwargs)
         on_response and emit_event(on_response, response, self, session)
         self._check_response(response, session.config)
         return response
 
     async def get_data_async(
         self,
         session: Optional["Session"] = None,
         on_response: Optional[Callable] = None,
         closure: Optional[Any] = None,
     ) -> TypeData:
+        """
+        Sends an asynchronous request to the Refinitiv Data Platform to retrieve the previously defined data.
+
+        Parameters
+        ----------
+        session : Session
+            Session object. If it's not passed the default session will be used.
+        on_response : Callable
+            User-defined callback function to process the retrieved data.
+        closure : Any
+            Closure parameters that will be returned with the response
+
+        Returns
+        -------
+        TypeData instance
+
+        """
         if not self._kwargs.get("closure") and closure:
             self._kwargs["closure"] = closure
         session = get_valid_session(session)
         response = await get_data_async(self._data_type, self._provider, session, **self._kwargs)
         on_response and emit_event(on_response, response, self, session)
         return response
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_parsed_data.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_parsed_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_raw_data_parser.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_raw_data_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_request.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_request_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_response.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_response_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_data/_validators.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_data/_validators.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_omm_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_omm_stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 import asyncio
 import json
 import os
 from functools import partial
 from threading import Event
-from typing import Callable, Optional, TYPE_CHECKING, Any, Union
+from typing import Callable, Optional, TYPE_CHECKING, Any, Union, Tuple
 
 from ._protocol_type import ProtocolType
 from ._stream_listener import OMMStreamListener, StreamEvent
+from ._validator_exceptions import ValidationException, ValidationsException
 from .contrib import ContribResponse
 from .contrib import contrib_type_enum_arg_parser
-from .contrib._response import (
-    ErrorContribResponse,
-    AckContribResponse,
-    NullContribResponse,
-)
-from .stream import (
-    Stream,
-    update_message_with_extended_params,
-)
+from .contrib._response import RejectedContribResponse, ErrorContribResponse, AckContribResponse, NullContribResponse
+from .stream import Stream, update_message_with_extended_params
 from ..._tools import cached_property, OrEvent
 
 if TYPE_CHECKING:
     from .contrib import ContribType
     from ..._types import OptStr, ExtendedParams, Strings
     from ._stream_factory import StreamDetails
     from . import StreamConnection
@@ -69,32 +63,28 @@
         self._refresh_message = None
         self._status_message = None
         self._error_message = None
         self._ack_message = None
 
         self._error_event = Event()
         self._ack_event = Event()
-        self._update_event = Event()
 
         self._contrib_response = None
         self._is_contributing = False
         self._post_id = None
         self._post_user_info = None
 
     @cached_property
     def _contributed(self) -> OrEvent:
-        return OrEvent(self._error_event, self._update_event)
+        return OrEvent(self._error_event, self._ack_event)
 
     @property
     def post_id(self) -> int:
         return self._post_id
 
-    def get_next_post_id(self) -> int:
-        return next(self.session._contrib_post_id_counter)
-
     @property
     def post_user_info(self) -> dict:
         return self._post_user_info
 
     @property
     def name(self) -> str:
         return self._name
@@ -179,20 +169,14 @@
     def _do_on_stream_refresh(self, cxn: "StreamConnection", message: dict, *_) -> Any:
         self._refresh_message = message
         message_state = message.get("State", {})
         self._stream_state = message_state.get("Stream", "")
         self._message_state = message_state.get("Text", "")
         return message
 
-    def _on_stream_update(self, originator, *args) -> None:
-        self._propagate_event(StreamEvent.UPDATE, originator, *args)
-
-        if self.is_contributing:
-            self._update_event.set()
-
     def _on_stream_status(self, originator, *args) -> None:
         self._propagate_event(StreamEvent.STATUS, originator, *args)
 
         if self.is_open:
             self.dispatch_complete(originator, *args)
 
     def _do_on_stream_status(self, cxn: "StreamConnection", message: dict, *_) -> Any:
@@ -297,42 +281,93 @@
 
     def get_contrib_error_message(self) -> dict:
         return {
             "Type": "Error",
             "Message": "Contribute failed because of disconnection.",
         }
 
+    def _get_post_id(self):
+        return self.session._get_omm_stream_id()
+
+    def _validate_fields(self, fields: dict) -> Tuple[bool, dict]:
+        is_valid = True
+        config = self.session.config
+        is_field_validation = config.get(f"{self._cxn.api_cfg_key}.contrib.field-validation")
+
+        if is_field_validation:
+            endpoints_key, _ = self._cxn.api_cfg_key.rsplit(".", 1)
+            api = None
+            counter = 0
+            for endpoint in config.get(endpoints_key):
+                metadata_download = config.get(f"{endpoints_key}.{endpoint}.metadata.download")
+                if metadata_download:
+                    api = f"{endpoints_key}.{endpoint}"
+                    counter += 1
+
+            if api is None or counter == 0:
+                raise ValueError(f"Cannot find metadata download api in config")
+
+            if counter > 1:
+                raise ValueError(f"More than one metadata download api in config")
+
+            self.session._load_metadata(api=api)
+
+            error = None
+            try:
+                fields = self.session._validate_metadata(fields)
+            except ValidationException as e:
+                error = {"Text": e.value}
+            except ValidationsException as e:
+                error = e.invalid
+
+            if error:
+                is_valid = False
+                self._contrib_response = RejectedContribResponse(error)
+
+        return is_valid, fields
+
     def contribute(
         self,
         fields: dict,
         contrib_type: Union[str, "ContribType", None] = None,
         post_user_info: Optional[dict] = None,
     ) -> ContribResponse:
-        self._is_contributing = True
-        self._post_id = self.get_next_post_id()
-        self._post_user_info = post_user_info
-
-        self._error_event.clear()
-        self._ack_event.clear()
-        self._update_event.clear()
-
-        sent = self.send(self.get_contrib_message(fields, contrib_type))
-
-        if sent:
-            self._contributed.wait()
-            self._is_contributing = False
-
-            if self.is_close:
-                self._contrib_response = NullContribResponse()
-                self._on_stream_error(self, self.get_contrib_error_message())
+        if self.is_open:
+            self._is_contributing = True
+            self._post_id = self._get_post_id()
+            self._post_user_info = post_user_info
+
+            self._error_event.clear()
+            self._ack_event.clear()
 
-        else:
-            self._is_contributing = False
             self._contrib_response = NullContribResponse()
 
+            is_valid, fields = self._validate_fields(fields)
+
+            if is_valid:
+                sent = self.send(self.get_contrib_message(fields, contrib_type))
+
+                if sent:
+                    self._contributed.wait()
+                    self._is_contributing = False
+
+                    if self.is_close:
+                        self._on_stream_error(self, self.get_contrib_error_message())
+
+                else:
+                    self._is_contributing = False
+
+            else:
+                self._error(
+                    f"{self._classname} Contribute failure caused by fields validation, error={self._contrib_response}"
+                )
+
+        else:
+            raise ValueError(f"Cannot contribute to a {self.state} stream")
+
         return self._contrib_response
 
     async def contribute_async(
         self,
         fields: dict,
         contrib_type: Union[str, "ContribType", None] = None,
         post_user_info: Optional[dict] = None,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_rdp_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_rdp_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_factory.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,35 +65,36 @@
     ContentType.STREAMING_OFF_CONTRIB: APIType.STREAMING_PRICING,
     ContentType.STREAMING_OMM: APIType.STREAMING_PRICING,
     ContentType.STREAMING_RDP: APIType.STREAMING_CUSTOM,
 }
 
 connection_id_iterator = itertools.count(0)
 
-stream_class_by_protocol_type: Dict[ProtocolType, Type[Union[_OMMStream, _RDPStream]]] = {
-    ProtocolType.OMM: _OMMStream,
-    ProtocolType.RDP: _RDPStream,
-}
 
+def get_default_config_path(api_type) -> Union[str, None]:
+    default_config_path = None
+    api_key = api_config_key_by_api_type.get(api_type)
+    default_api = default_api_config_key_by_api_type.get(api_type)
+    if api_key and default_api:
+        default_config_path = f"{api_key}.{default_api}"
 
-def get_default_config_path(api_type):
-    return f"{api_config_key_by_api_type.get(api_type)}.{default_api_config_key_by_api_type.get(api_type)}"
+    return default_config_path
 
 
 @dataclass
 class StreamDetails:
     content_type: ContentType
     protocol_type: ProtocolType
     api_type: APIType
     _api_config_key: str = ""
 
     @property
     def api_config_key(self):
         if not self._api_config_key:
-            self._api_config_key = service_config_key_by_api_type.get(self.api_type)
+            self._api_config_key = get_default_config_path(self.api_type)
         return self._api_config_key
 
 
 def content_type_to_details(content_type: ContentType) -> StreamDetails:
     api_type = api_type_by_content_type.get(content_type, APIType.STREAMING_CUSTOM)
 
     if content_type is ContentType.NONE:
@@ -124,15 +125,15 @@
 
     api_type = APIType.STREAMING_CUSTOM if api else api_type_by_content_type.get(content_type, APIType.STREAMING_CUSTOM)
 
     if not service:
         service = session.config.get(service_config_key_by_api_type.get(api_type))
 
     stream = _OMMStream(
-        stream_id=next(session._omm_stream_counter),
+        stream_id=session._get_omm_stream_id(),
         session=session,
         name=name,
         domain=domain,
         service=service,
         fields=fields,
         key=key,
         extended_params=extended_params,
@@ -274,15 +275,15 @@
     if contrib_section and not api:
         api = CONTRIB_SECTION_KEY
 
     elif not contrib_section and not api:
         api_type = api_type_by_content_type.get(content_type, APIType.STREAMING_CUSTOM)
 
     stream = _OffStreamContrib(
-        post_id=next(session._contrib_post_id_counter),
+        post_id=session._get_omm_stream_id(),
         session=session,
         name=name,
         details=StreamDetails(content_type, ProtocolType.OMM_OFF_CONTRIB, api_type, api),
         service=service,
         domain=domain,
     )
     logger().debug(f" + Created offstream contrib={stream.classname}")
@@ -310,17 +311,16 @@
         content_type = ContentType.STREAMING_DICTIONARY
 
     api_type = api_type_by_content_type.get(content_type, APIType.STREAMING_CUSTOM)
     details = StreamDetails(content_type, ProtocolType.OMM, api_type, api)
     if not service:
         service = session.config.get(service_config_key_by_api_type.get(api_type))
 
-    stream_id = next(session._omm_stream_counter)
     stream = PrvDictionaryStream(
-        stream_id=stream_id,
+        stream_id=session._get_omm_stream_id(),
         session=session,
         name=name,
         details=details,
         domain=domain,
         service=service,
         key=key,
         extended_params=extended_params,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/_stream_listener.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/_stream_listener.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/base_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/base_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_funcs.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_funcs.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_offstream.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_offstream.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,21 @@
             domain=domain,
             service=service,
             on_error=on_error,
             on_ack=on_ack,
         )
         self._post_id = post_id
 
+    def _get_post_id(self):
+        return self._post_id
+
     @cached_property
     def _contributed(self) -> OrEvent:
         return OrEvent(self._error_event, self._ack_event)
 
-    def get_next_post_id(self) -> int:
-        return self.post_id
-
     def get_contrib_message(self, fields: dict, contrib_type: Union[str, "ContribType", None]) -> dict:
         return {
             "Ack": True,
             "ID": LOGIN_STREAM_ID,
             "Message": {
                 "Fields": fields,
                 "ID": 0,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/contrib/_response.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/contrib/_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,39 @@
     def error(self) -> str:
         pass
 
     @property
     def debug(self) -> dict:
         return self._message.get("Debug", {})
 
+    def __str__(self) -> str:
+        return str(self._message)
+
+
+class RejectedContribResponse(ContribResponse):
+    @property
+    def is_success(self) -> bool:
+        return False
+
+    @property
+    def type(self) -> str:
+        return "Error"
+
+    @property
+    def error(self) -> str:
+        return self._message.get("Text")
+
+    @property
+    def nak_message(self) -> str:
+        return ""
+
+    @property
+    def debug(self) -> dict:
+        return {}
+
 
 class AckContribResponse(ContribResponse):
     def __repr__(self) -> str:
         d = {"Type": self.type, "AckId": self.ack_id}
 
         if self.nak_code:
             d["NakCode"] = self.nak_code
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/event.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/event.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union, List, Dict, TYPE_CHECKING
 
 from ._dictionary_type import DictionaryType
 from ._enum_type_entry import EnumTypeEntry, create_enum_entry
 from ._field_description import FieldDescription, create_field_description
-from ._validator import validator, ValidateError
+from ._validator import validator
 from .._stream_factory import create_dictionary_stream
+from .._validator_exceptions import ValidationException
 from ...._content_type import ContentType
 from ...._core.log_reporter import PrvLogReporterMixin
 from ...._core.session import get_default
 from ...._tools import version_to_tuple
 
 if TYPE_CHECKING:
     from ._stream import PrvDictionaryStream
@@ -60,14 +61,22 @@
         self._fid_to_field_desc: Dict[int, FieldDescription] = {}
         self._acronym_to_field_desc: Dict[str, FieldDescription] = {}
         self._fid_to_enum_type: Dict[int, EnumTypeEntry] = {}
         self._dict_type_to_version: Dict[DictionaryType, tuple] = {}
         self._rippled_fields = set()
 
     @property
+    def is_field_dict_available(self) -> bool:
+        return bool(self._fid_to_field_desc)
+
+    @property
+    def is_enum_dict_available(self) -> bool:
+        return bool(self._fid_to_enum_type)
+
+    @property
     def versions(self) -> dict:
         """
         retrieve the field and enum type metadata version. e.g: {"RWFFld": (4,20,30), "RWFEnum": (17, 91)}
 
         Returns
         -------
         dict {"RWFFld": fld_version, "RWFEnum": enum_version}
@@ -213,15 +222,15 @@
         return value
 
     def is_valid_enum_field(self, key: Union[str, int], value: Union[str, int]) -> bool:
         is_valid = True
 
         try:
             validator.check_enum_field_value(key, value)
-        except ValidateError:
+        except ValidationException:
             is_valid = False
 
         return is_valid
 
     def validate(self, fields: dict, **kwargs) -> dict:
         """
         To check whether several fields' key and value are compliance with the dictionary definition.
@@ -249,31 +258,36 @@
         {
             'ASK': 'Field ASK cannot be found in metadata',
             'ASKSIZE': 'Field ASKSIZE cannot be found in metadata',
             'BID': 'Field BID cannot be found in metadata',
             'BIDSIZE': 110
         }
         """
+        if not self.is_field_dict_available:
+            raise ValidationException("Metadata not available")
+
         fields.update(kwargs)
         return validator.get_validated_fields_values(self, fields)
 
     def is_ripple_to_field(self, field_id: Union[int, str]) -> bool:
         if isinstance(field_id, str) and field_id in self._acronym_to_field_desc:
             field_id = self._acronym_to_field_desc[field_id]
 
         if isinstance(field_id, int) and field_id in self._fid_to_field_desc:
             return field_id in self._rippled_fields
 
         return False
 
-    def load(self, dictionary_type: Union[str, DictionaryType] = None):
+    def load(self, dictionary_type: Union[str, DictionaryType] = None, api: str = None) -> None:
         """
         Parameters
         ----------
         dictionary_type: DictionaryType, optional
+        api: str, optional
+            Specifies the data source. It can be updated/added using config file
 
         Returns
         -------
         None
 
         Examples
         ----------
@@ -292,32 +306,34 @@
 
         if dictionary_type == DictionaryType.RWF_FLD or not dictionary_type:
             load = True
             field_stream = create_dictionary_stream(
                 ContentType.STREAMING_DICTIONARY,
                 domain="Dictionary",
                 name=DictionaryType.RWF_FLD,
+                api=api,
                 session=self._session,
                 service=self._service,
                 on_refresh=self._on_refresh,
             )
-            field_stream.open()
+            field_stream.open(with_updates=False)
             field_stream.close()
 
         if dictionary_type == DictionaryType.RWF_ENUM or not dictionary_type:
             load = True
             enum_stream = create_dictionary_stream(
                 ContentType.STREAMING_DICTIONARY,
                 domain="Dictionary",
                 name=DictionaryType.RWF_ENUM,
+                api=api,
                 session=self._session,
                 service=self._service,
                 on_refresh=self._on_refresh,
             )
-            enum_stream.open()
+            enum_stream.open(with_updates=False)
             enum_stream.close()
 
         if not load:
             raise ValueError(f"Nothing to load for {dictionary_type}")
 
     def _on_refresh(self, stream: "PrvDictionaryStream", message: dict):
         domain = message.get("Domain")
@@ -330,41 +346,43 @@
 
         key = message.get("Key", {})
         if not key or key.get("Name") != stream.name:
             return
 
         self._fill_dictionary(stream.name, message.get("Series"))
 
-    def _fill_dictionary(self, dictionary_type: Union[str, DictionaryType], series: dict):
+    def _fill_dictionary(self, dictionary_type: Union[str, DictionaryType], series: dict) -> bool:
         if not series:
-            return
+            return False
 
         version = series.get("Summary", {}).get("Elements", {}).get("Version")
         if not version:
-            return
+            return False
 
         curr_version = self._dict_type_to_version.get(dictionary_type)
         if curr_version is None:
             self._dict_type_to_version[dictionary_type] = version_to_tuple(version)
 
         else:
             # check if version is newer
             if version_to_tuple(version) <= curr_version:
-                return
+                return False
 
         entries = series.get("Entries")
         if not entries:
-            return
+            return False
 
         if dictionary_type == DictionaryType.RWF_FLD:
             self._fill_field_dictionary(entries)
 
         elif dictionary_type == DictionaryType.RWF_ENUM:
             self._fill_enum_type_dictionary(entries)
 
+        return True
+
     def _fill_field_dictionary(self, entries: List[dict]):
         for elements in entries:
             if not elements:
                 continue
 
             try:
                 field_desc = create_field_description(elements["Elements"])
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_field_description.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_field_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_types.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/metadata/_validator.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/metadata/_validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import time
 import warnings
 from typing import Any, Union, TYPE_CHECKING, Dict, Callable
 
 from dateutil import parser
 
+from refinitiv.data.delivery._stream._validator_exceptions import ValidationException, ValidationsException
 from ._types import FieldType, RWFDataType
 
 if TYPE_CHECKING:
     from ._field_description import FieldDescription
     from ._dictionary import Dictionary
 
 INVALID_VALUE_ERROR_LOG_PATTERN = "Invalid value {0} for field {1}. Field type is {2}. {3}"
@@ -16,58 +17,63 @@
     "{0} value has been cut off to {1}, original value is {2}, the expected field's length is {3}"
 )
 INVALID_ENUM_ERROR_LOG_PATTERN = "Invalid enum value {0} for field {1}: {2}"
 
 ONE_DAY_SECS = 86400
 
 
-class ValidateError(Exception):
-    pass
-
-
 class Validator:
     @staticmethod
     def get_validated_fields_values(dic: "Dictionary", fields: dict) -> dict:
         validated_fields_values = {}
+        errors = {}
         for key, value in fields.items():
             field_desc = dic.get_field(key)
+            validated = value
 
             if field_desc is None:
-                validated = f"Field {key} cannot be found in metadata"
+                errors[key] = f"Field {key} cannot be found in metadata"
+                continue
+
+            field_desc_name = field_desc.name
+            if field_desc_name in validated_fields_values:
+                errors[key] = f"Field {key} already exists in the fields as {field_desc_name}"
+                continue
+
+            rwf_type = field_desc.rwf_type
+            rwf_len = field_desc.rwf_len
+            value_str = str(value)
 
-            elif field_desc.type == FieldType.ENUMERATED:
+            if field_desc.type == FieldType.ENUMERATED:
                 try:
                     validated = Validator.validate_enum_value(dic, field_desc, value)
-                except ValidateError as e:
-                    validated = str(e)
+                except ValidationException as e:
+                    errors[key] = e.value
+
+            elif rwf_type in {RWFDataType.RWF_RMTES_STRING, RWFDataType.RWF_BUFFER} and len(value_str) > rwf_len:
+                validated = value_str[:rwf_len]
 
             else:
-                rwf_type = field_desc.rwf_type
+                validate_value = mapping.get(rwf_type)
 
-                if (
-                    rwf_type in {RWFDataType.RWF_RMTES_STRING, RWFDataType.RWF_BUFFER}
-                    and len(str(value)) > field_desc.rwf_len
-                ):
-                    validated = str(value)[: field_desc.rwf_len]
+                if not validate_value:
+                    errors[key] = INVALID_VALUE_ERROR_LOG_PATTERN.format(
+                        value, field_desc_name, rwf_type, "This type is not supported"
+                    )
+                    continue
 
-                else:
-                    validate_value = mapping.get(field_desc.rwf_type)
+                try:
+                    validated = validate_value(field_desc, value)
+                except ValidationException as e:
+                    errors[key] = e.value
 
-                    if validate_value:
-                        try:
-                            validated = validate_value(field_desc, value)
-                        except ValidateError as e:
-                            validated = str(e)
-
-                    else:
-                        validated = INVALID_VALUE_ERROR_LOG_PATTERN.format(
-                            value, field_desc.name, rwf_type, "This type is not supported"
-                        )
+            validated_fields_values[field_desc_name] = validated
 
-            validated_fields_values[key] = validated
+        if errors:
+            raise ValidationsException(errors, validated_fields_values)
 
         return validated_fields_values
 
     @staticmethod
     def check_enum_field_value(dic: "Dictionary", field_desc: "FieldDescription", value: Union[str, int]):
         error = None
         key = field_desc.name
@@ -87,22 +93,24 @@
             if enum_value is None:
                 error = "invalid enumerated field display/value"
 
         else:
             error = "invalid enumerated field display/value"
 
         if error:
-            raise ValidateError(INVALID_ENUM_ERROR_LOG_PATTERN.format(value, field_desc.name, error))
+            raise ValidationException(INVALID_ENUM_ERROR_LOG_PATTERN.format(value, field_desc.name, error))
 
     @staticmethod
     def validate_enum_value(dic: "Dictionary", field_desc: "FieldDescription", value: Union[str, int]):
         Validator.check_enum_field_value(dic, field_desc, value)
-        validated_value = value
-        if isinstance(value, str):
+
+        if isinstance(value, str) and not value.isdigit():
             validated_value = dic.get_enum_value(field_desc.name, value)
+        else:
+            validated_value = int(value)
 
         return validated_value
 
     @staticmethod
     def validate_string_value(field_desc: "FieldDescription", value: Any) -> str:
         validated_value = value
         if not isinstance(value, str):
@@ -113,15 +121,15 @@
             if not validated_value.isascii():
                 non_ascii_str = ""
                 for c in validated_value:
                     if ord(c) >= 128:
                         non_ascii_str = non_ascii_str + c
 
                 if non_ascii_str:
-                    raise ValidateError(
+                    raise ValidationException(
                         INVALID_VALUE_ERROR_LOG_PATTERN.format(
                             validated_value,
                             field_desc.name,
                             "ASCII string",
                             f"It includes non ASCII characters '{non_ascii_str}'",
                         )
                     )
@@ -139,24 +147,24 @@
             except Exception as e:
                 error = str(e)
 
         elif not isinstance(value, int):
             error = "It must be integer."
 
         if error:
-            raise ValidateError(INVALID_VALUE_ERROR_LOG_PATTERN.format(value, field_desc.name, "INT64", error))
+            raise ValidationException(INVALID_VALUE_ERROR_LOG_PATTERN.format(value, field_desc.name, "INT64", error))
 
         return validated_value
 
     @staticmethod
     def validate_uint_value(field_desc: "FieldDescription", value: Union[int, str]) -> int:
         validated_value = Validator.validate_int_value(field_desc, value)
 
         if validated_value < 0:
-            raise ValidateError(
+            raise ValidationException(
                 INVALID_VALUE_ERROR_LOG_PATTERN.format(
                     validated_value, field_desc.name, "UINT64", "It must be positive integer or 0."
                 )
             )
 
         return validated_value
 
@@ -169,15 +177,15 @@
             for type_value in [int, float]:
                 try:
                     value = type_value(value)
                     return value
                 except ValueError:
                     pass
 
-            raise ValidateError(
+            raise ValidationException(
                 INVALID_VALUE_ERROR_LOG_PATTERN.format(
                     value, field_desc.name, "REAL64", f"field value {value} is not valid for REAL64"
                 )
             )
 
     @staticmethod
     def validate_time_seconds_value(field_desc: "FieldDescription", value: Union[int, datetime.time, str]) -> str:
@@ -214,15 +222,15 @@
                 valid = False
                 error = str(e)
 
         else:
             valid = False
 
         if not valid:
-            raise ValidateError(
+            raise ValidationException(
                 INVALID_VALUE_ERROR_LOG_PATTERN.format(
                     value, field_desc.name, f"TIME[{time_format[:field_desc.rwf_len]}]", error
                 )
             )
 
         return value
 
@@ -247,15 +255,15 @@
             _time = time.localtime(value)
             value = datetime.date(_time.tm_year, _time.tm_mon, _time.tm_mday)
 
         else:
             valid = False
 
         if not valid:
-            raise ValidateError(INVALID_VALUE_ERROR_LOG_PATTERN.format(value, field_desc.name, "DATE", error))
+            raise ValidationException(INVALID_VALUE_ERROR_LOG_PATTERN.format(value, field_desc.name, "DATE", error))
 
         return value
 
 
 mapping: Dict[RWFDataType, Callable[["FieldDescription", Any], Any]] = {
     RWFDataType.RWF_ASCII_STRING: Validator.validate_string_value,
     RWFDataType.RWF_INT64: Validator.validate_int_value,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/omm_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/omm_stream_connection.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/omm_stream_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         elif message_type == "Status":
             self._emitter.emit(event.status_by_id, self, message)
 
         elif message_type == "Error":
             # Detect if error is related to Post contrib request,
             # then forward event to post_id listener
             debug_message = message.get("Debug", {}).get("Message")
-            if debug_message:
+            if stream_id == LOGIN_STREAM_ID and debug_message:
                 try:
                     debug_dict = json.loads(debug_message)
                     post_id = debug_dict.get("PostID")
                     if post_id:
                         event = StreamEvent.get(post_id)
                 except json.decoder.JSONDecodeError:
                     self.error(f"Cannot decode Debug message as JSON: {debug_message}")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/omm_stream_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,95 @@
-# coding: utf8
+from typing import TYPE_CHECKING, Union
 
-
-from typing import TYPE_CHECKING, Optional
-
-from .omm_stream import OMMStream
-from ..._tools import create_repr, fields_arg_parser, try_copy_to_list
+from .. import content
+from .._types import OptStr, OptInt
+from ..content.search import Views
 
 if TYPE_CHECKING:
-    from ..._types import ExtendedParams, OptStrStrs
-    from ..._core.session import Session
+    import pandas as pd
 
 
-class Definition:
+def search(
+    query: OptStr = None,
+    view: Union[Views, str] = Views.SEARCH_ALL,
+    filter: OptStr = None,
+    order_by: OptStr = None,
+    boost: OptStr = None,
+    select: OptStr = None,
+    top: OptInt = 10,
+    skip: OptInt = 0,
+    group_by: OptStr = None,
+    group_count: OptInt = 3,
+    features: OptStr = None,
+    scope: OptStr = None,
+    terms: OptStr = None,
+) -> "pd.DataFrame":
     """
-    This class to subscribe to streaming items of any Domain Model
-    (e.g. MarkePrice, MarketByPrice, ...)
-    exposed by the underlying of the Refinitiv Data
+    This class describe parameters to retrieve data for search.
 
     Parameters
     ----------
-    name : str, optional
-        Name of the streaming instrument
-    api: str, optional
-        Specifies the data source. It can be updated/added using config file
-    service : str, optional
-        Offers the ability to use specific service to manage the
-        real-time streaming data
-    fields : str or list, optional
-        Specifies the specific fields delivered when messages arrive
-    domain : str, optional
-        Defines the domain for the specific data of interest
-        Default : "MarketPrice"
-    extended_params : dict, optional
-        Other parameters can be provided if necessary
+    query: str, optional
+        Keyword argument for view
+
+    view: Views or str, optional
+        The view for searching see at Views enum.
+        Default: Views.SEARCH_ALL
+
+    filter: str, optional
+        Where query is for unstructured end-user-oriented restriction, filter is for
+        structured programmatic restriction.
+
+    order_by: str, optional
+        Defines the order in which matching documents should be returned.
+
+    boost: str, optional
+        This argument supports exactly the same predicate expression syntax as filter,
+        but where filter restricts which documents are matched at all,
+        boost just applies a large scoring boost to documents it matches,
+        which will almost always guarantee that they appear at the top of the results.
+
+    select: str, optional
+        A comma-separated list of the properties of a document to be returned in the response.
+
+    top: int, optional
+        the maximum number of documents to retrieve. Must be non-negative.
+        default: 10
+
+    skip: int, optional
+        The number of documents to skip in the sorted result set before returning the
+        next top.
+
+    group_by: str, optional
+        If specified, this must name a single Groupable property.
+        returned documents are grouped into buckets based on their value for this
+        property.
+
+    group_count: str, optional
+        When supplied in combination with group_by, sets the maximum number of documents
+        to be returned per bucket.
+        default: 3
 
     Examples
     --------
-    >>> from refinitiv.data.delivery import omm_stream
-    >>> definition = omm_stream.Definition("EUR")
+    >>> from refinitiv.data as rd
+    >>> df = rd.discovery.search(query="cfo", view=rd.discovery.Views.PEOPLE)
     """
-
-    def __init__(
-        self,
-        name: str,
-        api: Optional[str] = None,
-        service: Optional[str] = None,
-        fields: "OptStrStrs" = None,
-        domain: str = "MarketPrice",
-        extended_params: "ExtendedParams" = None,
-    ) -> None:
-        self._name = name
-        self._api = api
-        self._domain = domain
-        self._service = service
-        fields = try_copy_to_list(fields)
-        self._fields = fields and fields_arg_parser.get_list(fields)
-        self._extended_params = extended_params
-
-    def __repr__(self):
-        content = f"{{name='{self._name}'}}"
-        return create_repr(self, middle_path="omm_stream", content=content)
-
-    def get_stream(self, session: "Session" = None) -> OMMStream:
-        """
-        Initialization subscribe to streaming items
-
-        Parameters
-        ----------
-        session: Session, optional
-            The Session defines the source where you want to retrieve your data
-
-        Returns
-        -------
-        current instance
-
-        Examples
-        --------
-        >>> from refinitiv.data.delivery import omm_stream
-        >>> definition = omm_stream.Definition("EUR")
-        >>> stream = definition.get_stream()
-        """
-        stream = OMMStream(
-            session=session,
-            name=self._name,
-            api=self._api,
-            service=self._service,
-            fields=self._fields,
-            domain=self._domain,
-            extended_params=self._extended_params,
+    return (
+        content.search.Definition(
+            query=query,
+            view=view,
+            filter=filter,
+            order_by=order_by,
+            boost=boost,
+            select=select,
+            top=top,
+            skip=skip,
+            group_by=group_by,
+            group_count=group_count,
+            features=features,
+            scope=scope,
+            terms=terms,
         )
-        return stream
+        .get_data()
+        .data.df
+    )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/proxy_info.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/proxy_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rdp_stream.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,33 +6,30 @@
 if TYPE_CHECKING:
     from ..._types import ExtendedParams, StrStrings
     from ..._core.session import Session
 
 
 class Definition:
     """
-    This class to subscribe to streaming items of RDP streaming protocol
-    that exposed by the underlying of the Refinitiv Data
+    Defines the data to retrieve using RDP the data stream from the Refinitiv Data Platform.
 
     Parameters
     ----------
     service: string, optional
-        name of RDP service
+        RDP service name.
     universe: list
-        RIC to retrieve item stream.
+        Single instrument or list of instruments.
     view: list
-        data fields to retrieve item stream
+        Data fields that should be retrieved from the data stream.
     parameters: dict
-        extra parameters to retrieve item stream.
+        Extra parameters to retrieve from the item stream.
     api: string
-        specific name of RDP streaming defined
-        in config file. i.e. 'streaming.trading-analytics.endpoints.redi'
+        RDP streaming data source.
     extended_params: dict, optional
-        Specify optional params
-        Default: None
+        Specifies the parameters that will be merged with the request.
 
     Examples
     --------
     >>> from refinitiv.data.delivery import rdp_stream
     >>> definition = rdp_stream.Definition(
     ...     service=None,
     ...     universe=[],
@@ -57,14 +54,27 @@
         self._universe = universe
         self._view = try_copy_to_list(view)
         self._parameters = parameters
         self._api = api
         self._extended_params = extended_params
 
     def get_stream(self, session: "Session" = None) -> RDPStream:
+        """
+        Returns the previously defined RDP data stream from the Refinitiv Data Platform.
+
+        Parameters
+        ----------
+        session : Session
+            Session object. If it's not passed the default session will be used.
+
+        Returns
+        -------
+        RDPStream instance.
+
+        """
         stream = RDPStream(
             session=session,
             service=self._service,
             universe=self._universe,
             view=self._view,
             parameters=self._parameters,
             api=self._api,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/conversion.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/conversion.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/ema.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/ema.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/rwf/socket.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/rwf/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import datetime
+import logging
 import socket
 import time
-import logging
 from collections import namedtuple
 from typing import Callable, Optional, Dict, Tuple
+from typing import TYPE_CHECKING
 
 from refinitiv.data._core.log_reporter import LogReporter
-from refinitiv.data._core.session import Session
 from refinitiv.data._errors import SessionError
 
+if TYPE_CHECKING:
+    from refinitiv.data._core.session import Session
+
 
 def _get_version(version: str):
     return tuple(map(int, version.split(".")[:3]))
 
 
 try:
     from ema import __version__ as _ema_version
@@ -47,15 +50,14 @@
     from .conversion import json_marketprice_msg_to_ema
     from .ema import (
         ema_login_message,
         create_programmatic_cfg,
         generate_login_msg,
     )
 
-
 if EMA_INSTALLED:
 
     class EmaPythonLogger(CustomLoggerClient):
         def __init__(self):
             super().__init__(EmaPythonLogger.log)
 
         severity_logging_map: dict = {
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_cache.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_cache.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_connection.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,18 @@
         return self._session
 
     @property
     def id(self) -> int:
         return self._id
 
     @property
+    def api_cfg_key(self) -> str:
+        return self._config.api_cfg_key
+
+    @property
     def subprotocol(self) -> str:
         return ""
 
     @property
     def state(self) -> StreamCxnState:
         return self._state
 
@@ -427,15 +431,15 @@
 
     def _on_ws_close(self, ws: websocket.WebSocketApp, close_status_code: str, close_msg: str) -> None:
         self.debug(
             f"{self._classname} on_ws_close: "
             f"close_status_code={close_status_code}, close_msg={close_msg}, "
             f"state={self.state}"
         )
-        self._emitter.emit(StreamCxnEvent.DISCONNECTED, self)
+        self._emitter and self._emitter.emit(StreamCxnEvent.DISCONNECTED, self)
         if not self.is_disposed:
             self._listener_created.clear()
 
     def _on_ws_error(self, ws: websocket.WebSocketApp, exc: Exception) -> None:
         self.debug(f"{self._classname} on_ws_error: Exception: {exc}")
         if DEBUG:
             self.debug(f"{traceback.format_exc()}")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/stream_state_manager.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/stream_state_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/_stream/ws/ws_client.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/_stream/ws/ws_client.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_buckets_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_buckets_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,42 +7,36 @@
 
 if TYPE_CHECKING:
     from ..._types import OptStrStrs
 
 
 class Definition(DataProviderLayer):
     """
-    Definition object.
+    Describes the parameters to retrieve the buckets from a client file store with all their attributes.
 
     Parameters
     __________
         name : str, optional
-            Filter results by Bucket name. (Partial match).
+            Bucket name for partial match searching.
         created_since : str, optional
-            Filter results by when the Bucket was created.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z).
+            Bucket creation date.
         modified_since : str, optional
-            Filter results by when the Bucket was last modified.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z).
+            Bucket modification date.
         available_from : str, optional
-            Filter results by when the Bucket was made available.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z).
+            Bucket availability start date.
         available_to : str, optional
-            Filter results by when the Bucket was made available.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z).
+            Bucket availability end date.
         attributes : list of str, optional
-            List of publisher-defined bucket attributes.
+            Publisher-defined bucket attributes.
         page_size : int, optional
             Number of buckets returned.
-            By default 25.
         skip_token : str, optional
-            Skip token is only used if a previous operation returned a partial result.
-            If a previous response contains a nextLink element, the value of the nextLink
-            element will include a skip token parameter that specifies a starting point to use
-            for subsequent calls.
+            Skip token is only used if a previous operation returned a partial result. If a previous response
+            contains a nextLink element, the value of the nextLink element will include a skip token parameter that
+            specifies a starting point to use for subsequent calls.
 
     Methods
     -------
     get_data(session=session)
         Returns a response to the data platform
     get_data_async(session=None)
         Returns a response asynchronously to the data platform
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_data_class.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_data_types.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_data_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,12 +43,18 @@
 
 
 class PackageData(BaseData):
     @property
     def packages(self):
         return self._iter_object
 
+    @property
+    def df(self):
+        if not self.raw.get("value"):
+            return DataFrame()
+        return super().df
+
 
 class FileData(BaseData):
     @property
     def files(self):
         return self._iter_object
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_file_downloader.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_file_sets_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_file_sets_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,54 +4,47 @@
 from .._data._data_provider_layer import DataProviderLayer
 from .._data._data_type import DataType
 from ..._tools import validate_types
 
 
 class Definition(DataProviderLayer):
     """
-    Definition object.
+    Describes the indivisible set of files inside a particular bucket with all their attributes.
 
     Parameters
     __________
         bucket : str
-            The name of the bucket for file-sets to be searched.
-            Only exactly matched results are returned.
+            The name of the bucket to retrieve file sets.
         name : str, optional
-            The name of the file-set. Only exactly matched results are returned.
+            Name of the file set.
         attributes : dict, optional
-            Dict of publisher-defined key-value attributes.
+            List of publisher-defined key-value attributes. Each key-pair value is split by a colon. (e.g.
+            attributes=key1:val1,key2:val2).
         package_id : str, optional
+            File set package ID.
         status : str, optional
              Filter file-set by status (Ready/Pending).
         available_from : str, optional
-            Filter results by when the file was made available.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z)
+            File set availability start date.
         available_to : str, optional
-            Filter results by when the file was made available.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z)
+            File set availability end date.
         content_from : str, optional
-            Filter results by the age of the content within the file.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z)
+            Age of the content within the file, start date.
         content_to : str, optional
-            Filter results by the age of the content within the file.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z)
+            Age of the content within the file, end date.
         created_since : str, optional
-            Filter results by the date/time the file was created.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ.(e.g. 2020-01-21T04:19:01Z)
+            File set creation date.
         modified_since : str, optional
-            Filter results by the date/time the file was updated.
-            The date/time format is YYYY-MM-DDTHH:mm:ssZ. (e.g. 2020-01-21T04:19:01Z)
+            File set modification date.
         skip_token : str, optional
-            Skip token is only used if a previous operation returned a partial result.
-            If a previous response contains a nextLink element, the value of the nextLink
-            element will include a skip token parameter that specifies a starting point to
-            use for subsequent calls.
+            Skip token is only used if a previous operation returned a partial result. If a previous response
+            contains a nextLink element, the value of the nextLink element will include a skip token parameter that
+            specifies a starting point to use for subsequent calls.
         page_size : int, optional
-            Number of fileset returned.
-            By default 25.
+            Returned filesets number.
 
     Methods
     -------
     get_data(session=session)
         Returns a response to the data platform
     get_data_async(session=None)
         Returns a response asynchronously to the data platform
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_files_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_files_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 from .._data._data_provider_layer import DataProviderLayer
 from .._data._data_type import DataType
 from ..._tools import validate_types
 
 
 class Definition(DataProviderLayer):
     """
-    Definition object.
+    Describes the files inside a particular file-set with all their attributes.
 
     Parameters
     __________
         fileset_id : str
-            The name of the file-set for files to be searched.
-            Only exactly matched results are returned.
+            File set ID for searching.
         file_name : str, optional
-            Filter results by file name.
+            File name for partial match searching.
         created_since : str or timedelta or datetime, optional
-            Filter results by when the Bucket was created.
+            File creation date.
         modified_since : str or timedelta or datetime, optional
-            Filter results by when the Bucket was last modified.
+            File last modification date.
         skip_token : str, optional
-            Used for server-side paging.
+            Skip token is only used if a previous operation returned a partial result. If a previous response
+            contains a nextLink element, the value of the nextLink element will include a skip token parameter that
+            specifies a starting point to use for subsequent calls.
         page_size : int, optional
-            Used for server-side paging.
-            By default 25.
+            Number of buckets returned.
 
     Methods
     -------
     get_data(session=session)
         Returns a response to the data platform
     get_data_async(session=None)
         Returns a response asynchronously to the data platform
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_iter_object.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_iter_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 class CFSPackage(BaseCFSObject):
     _child_type = DataType.CFS_FILE_SETS
     _params = ("package_id", "package_id")
 
     def __init__(self, data, provider, session=None):
         super().__init__(data, provider, session=session)
-        self._bucket_names = self._data["bucket_names"]
+        self._bucket_names = self._data.get("bucket_names", [])
 
     def __iter__(self):
         args = self._params
         kwargs = {args[0]: self._data[args[1]]}
         bucket_name = self._bucket_names[0] if self._bucket_names else []
         self._child_objects = get_data_by_data_type(
             data_type=self._child_type,
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_packages_definition.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_packages_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,44 +3,38 @@
 from .._data._data_provider_layer import DataProviderLayer
 from .._data._data_type import DataType
 from ..._tools import validate_types
 
 
 class Definition(DataProviderLayer):
     """
-    Definition object.
+    Describes the particular file packages inside the bucket.
 
     Parameters
     __________
         package_name : str, optional
-            Filter results by package name. (Partial match).
+            Package name for partial match searching.
          package_id: str, optional
-            CFS package with package id.
+            Package ID.
         package_type : str, optional
-            Filter results by package type.
-            Available values : core, bulk, private.
+            Package type.
         bucket_name : str, optional
-            List the package that associated with this bucket.
+            Package bucket name.
         page : int, optional
-            The offest number determine which set of result should be
-            returned from all results.
+            The offset number that determines how many pages should be returned.
         included_total_result : bool, optional
-            The flag to indicate if total record count should be returned.
-            By default False.
+            The flag to indicate if total record count should be returned or not.
         skip_token : str, optional
-            Skip token is only used if a previous operation returned a partial result.
-            If a previous response contains a nextLink element, the value of the nextLink
-            element will include a skip token parameter that specifies a starting point to use
-            for subsequent calls.
+            Skip token is only used if a previous operation returned a partial result. If a previous response
+            contains a nextLink element, the value of the nextLink element will include a skip token parameter that
+            specifies a starting point to use for subsequent calls.
         page_size : int, optional
             The number of package that will be returned into a single response.
-            By default 25.
         included_entitlement_result : bool, optional
-            The flag to indicate the entitlement checking on each package.
-            By default False.
+            The flag that enables the entitlement checking on each package.
 
     Methods
     -------
     get_data(session=session)
         Returns a response to the data platform
     get_data_async(session=None)
         Returns a response asynchronously to the data platform
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_tools.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/delivery/cfs/_unpacker.py` & `refinitiv-data-1.3.0/refinitiv/data/delivery/cfs/_unpacker.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,15 @@
     "Peers",
     "Chain",
     "Screener",
     "AssetClass",
     "AssetState",
     "CountryCode",
     "SymbolTypes",
-    "_Customers",
-    "_Suppliers",
 )
 
 from ._convert_symbols import convert_symbols
 from ._search import search
 from ._search_templates import templates as search_templates
-from ._stakeholders import Customers as _Customers, Suppliers as _Suppliers
 from ._universe_expanders import Peers, Chain, Screener
 from ..content.search import Views
 from ..content.symbol_conversion import AssetClass, AssetState, CountryCode, SymbolTypes
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_convert_symbols.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_convert_symbols.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_search_explorer/_dataclasses.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,361 +1,241 @@
 from dataclasses import dataclass
-from enum import IntEnum
-from typing import Union
-from refinitiv.data.content import search
-import pandas as pd
-
-
-def _convert_property_attribute(value):
-    return True if value == "True" else False if value == "False" else pd.NA
-
-
-def from_list(data: list, request_arguments: dict) -> "Property":
-    searchable = _convert_property_attribute(data[3])
-    sortable = _convert_property_attribute(data[4])
-    navigable = _convert_property_attribute(data[5])
-    groupable = _convert_property_attribute(data[6])
-    exact = _convert_property_attribute(data[7])
-    symbol = _convert_property_attribute(data[8])
-
-    return Property(
-        name=data[0],
-        value=data[1],
-        type=data[2],
-        searchable=searchable,
-        sortable=sortable,
-        navigable=navigable,
-        groupable=groupable,
-        exact=exact,
-        symbol=symbol,
-        request_arguments=request_arguments,
-    )
-
-
-class PropertyType(IntEnum):
-    Double = 1
-    String = 2
-    Date = 3
-    Boolean = 4
-    Integer = 5
+from typing import Union, TYPE_CHECKING, Dict
 
+from ._properties import Properties
+from ._property_type import PropertyType
 
-@dataclass
-class BucketsData:
-    """BucketsData has properties for requested navigator."""
-
-    name: str
-    value: list
-    count: list
-
-
-@dataclass
-class Navigator:
-    """Navigator object that has dataframe and BucketsData object for requested navigator."""
-
-    df: pd.DataFrame
-    navigator: BucketsData
-
-
-@dataclass
-class Properties:
-    """Properties objects that has dataframe and dict object that holds Property objects"""
-
-    df: pd.DataFrame
-    properties: dict
-
-
-@dataclass
-class Property:
-    """Property object that has data and metadata for specific property."""
-
-    name: str
-    value: str
-    type: str
-    searchable: Union[bool, str]
-    sortable: Union[bool, str]
-    navigable: Union[bool, str]
-    groupable: Union[bool, str]
-    exact: Union[bool, str]
-    symbol: Union[bool, str]
-    request_arguments: dict
-
-    def get_possible_values(self):
-        """
-        Retrieves the navigator data
-
-        Returns
-        -------
-            Navigator object
-
-        Examples
-        --------
-        >>> from refinitiv.data.discovery._search_explorer import SearchPropertyExplorer
-        >>> explorer = SearchPropertyExplorer()
-        >>> result = explorer.get_properties_for(
-        ...    view=search.Views.GOV_CORP_INSTRUMENTS,
-        ...    query = "santander bonds",
-        ...    filter = "IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
-        ...)
-        >>> prop = result.properties["RCSIssuerCountry"].get_possible_values()
-        """
-        response = search.Definition(
-            view=self.request_arguments["view"],
-            query=self.request_arguments["query"],
-            filter=self.request_arguments["filter"],
-            top=1,
-            select="_debugall",
-            order_by=self.request_arguments["order_by"],
-            navigators=self.name,
-        ).get_data()
-
-        data = {}
-        counts = []
-        labels = []
-        filters = []
-
-        navigator_data = list(response.data.raw["Navigators"].items())
-        navigator_name = navigator_data[0][0]
-        buckets = navigator_data[0][1]["Buckets"]
-
-        for value in buckets:
-            counts.append(value.get("Count", 0))
-            labels.append(value.get("Label", pd.NA))
-
-            if "Filter" in value:
-                filters.append(value["Filter"])
-
-        data[navigator_name] = labels
-        if len(filters) > 0:
-            data["Filter"] = filters
-
-        data["Count"] = counts
-        navigator_data = BucketsData(name=navigator_name, value=data[navigator_name], count=data["Count"])
-        df = pd.DataFrame(data)
-        return Navigator(df, navigator_data)
+if TYPE_CHECKING:
+    from ._property import Property
+    from pandas import DataFrame
 
 
 @dataclass
 class SearchPropertyExplorerResponse:
     """
     Response object that has stores requested properties data.
     """
 
     hits_count: int
-    properties: dict
-    df: pd.DataFrame
-    metadata: pd.DataFrame
-    navigators: pd.DataFrame
+    properties: Dict[str, "Property"]
+    df: "DataFrame"
+    navigators: "DataFrame"
 
-    def get_by_name(self, name: str) -> "Properties":
+    def get_by_name(self, name: str) -> Properties:
         """
-        Browse the properties that match the specified property name.
+        Browse the properties names that have relative match with specified query. Results are represented
+        as the dataframe and dict of objects.
 
         Parameters
         ----------
         name: str
-            argument for search in response df and find matched properties.
+            String to specify expected properties data.
 
         Returns
         -------
             Properties
 
         Examples
         --------
         >>> from refinitiv.data.discovery._search_explorer import SearchPropertyExplorer
+        >>> from refinitiv.data.content import search
         >>> explorer = SearchPropertyExplorer()
-        >>> properties = explorer.get_properties_for(
+        >>> santander_bonds = explorer.get_properties_for(
         ...    view=search.Views.GOV_CORP_INSTRUMENTS,
-        ...    query = "santander bonds",
-        ...    filter = "IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
-        ...)
-        >>> prop = properties.get_properties_object("active")
+        ...    query="santander bonds",
+        ...    filter="IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
+        ... )
+        >>> active = santander_bonds.get_properties_object("active")
         """
+        return Properties(df=self.get_properties_df(name), properties=self.get_properties_object(name))
 
-        df = self.get_properties_df(name)
-        props = self.get_properties_object(name)
-        return Properties(df, props)
-
-    def get_properties_object(self, name: Union[str, bool, int]) -> dict:
+    def get_properties_object(self, name: Union[str, bool, int]) -> Dict[str, "Property"]:
         """
-        Browse the properties that match the specified property name.
+        Browse the properties names that have relative match with specified query. Results are represented
+        as dict of objects.
 
         Parameters
         ----------
         name: Union[str, bool, int]
-            argument for search in response df and find matched properties.
+            Argument to specify expected properties data.
 
         Returns
         -------
             dict of Property objects
 
         Examples
         --------
         >>> from refinitiv.data.discovery._search_explorer import SearchPropertyExplorer
+        >>> from refinitiv.data.content import search
         >>> explorer = SearchPropertyExplorer()
-        >>> properties = explorer.get_properties_for(
+        >>> santander_bonds = explorer.get_properties_for(
         ...    view=search.Views.GOV_CORP_INSTRUMENTS,
-        ...    query = "santander bonds",
-        ...    filter = "IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
-        ...)
-        >>> prop = properties.get_properties_object("active")
+        ...    query="santander bonds",
+        ...    filter="IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
+        ... )
+        >>> active = santander_bonds.get_properties_object("active")
         """
-        if name is None:
-            return self.properties
+        name = str(name).lower()
+        return {
+            prop_name: prop_value for prop_name, prop_value in self.properties.items() if name in str(prop_name).lower()
+        }
 
-        return {item: value for item, value in self.properties.items() if str(name).lower() in str(item).lower()}
-
-    def get_properties_df(self, name: str) -> pd.DataFrame:
+    def get_properties_df(self, name: str) -> "DataFrame":
         """
-        Browse the properties that match the specified property name.
+        Browse the properties names that have relative match with specified query.
 
         Parameters
         ----------
         name: str
-            Item for searching and finding matched properties in response dataframe.
+            String to specify expected properties data.
 
         Returns
         -------
             pd.DataFrame
 
         Examples
         --------
         >>> from refinitiv.data.discovery._search_explorer import SearchPropertyExplorer
+        >>> from refinitiv.data.content import search
         >>> explorer = SearchPropertyExplorer()
-        >>> properties = explorer.get_properties_for(
+        >>> santander_bonds = explorer.get_properties_for(
         ...    view=search.Views.GOV_CORP_INSTRUMENTS,
-        ...    query = "santander bonds",
-        ...    filter = "IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
-        ...)
-        >>> prop = properties.get_properties_df("active")
-
+        ...    query="santander bonds",
+        ...    filter="IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
+        ... )
+        >>> active = santander_bonds.get_properties_df("active")
         """
         return self.df.loc[self.df.Property.str.contains(name.replace(" ", ""), na=False, case=False)]
 
-    def get_by_value(self, value: Union[str, bool, int]) -> Properties:
+    def get_by_type(self, property_type: Union[str, PropertyType]) -> Properties:
         """
-        Browse the properties that match the specified property value.
+        Browse the types that match the specified query. Results are represented as the dataframe and dict of objects.
 
         Parameters
         ----------
-        value: str, bool, int
-            String for searching and finding matched properties in response dataframe.
+        property_type: str, PropertyType
+            Argument to specify expected properties data.
 
         Returns
         -------
             Properties
 
         Examples
         --------
         >>> from refinitiv.data.discovery._search_explorer import SearchPropertyExplorer
+        >>> from refinitiv.data.content import search
         >>> explorer = SearchPropertyExplorer()
-        >>> properties = explorer.get_properties_for(
+        >>> santander_bonds = explorer.get_properties_for(
         ...    view=search.Views.GOV_CORP_INSTRUMENTS,
-        ...    query = "santander bonds",
-        ...    filter = "IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
-        ...)
-        >>> prop = properties.get_by_value("active")
-        """
-        if isinstance(value, bool):
-            result = self.get_by_type(PropertyType.Boolean)
-            df = result.df
-            properties = result.properties
-            df = df[df["Example Value"] == str(value)]
-
-            response_properties = {}
+        ...    query="santander bonds",
+        ...    filter="IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
+        ... )
+        >>> str_properties = santander_bonds.get_by_type(PropertyType.String)
+        """
+        return Properties(
+            df=self.df.loc[self.df.Type.str.contains(property_type, na=False, case=False)],
+            properties={
+                prop_name: prop_value
+                for prop_name, prop_value in self.properties.items()
+                if str(prop_value.type) == property_type
+            },
+        )
 
-            for _property, attributes in properties.items():
-                if attributes.value == str(value):
-                    response_properties[_property] = attributes
-            result = Properties(df, response_properties)
-
-        elif isinstance(value, str) or isinstance(value, int):
-            value = str(value)
-            props = {
-                name: self.properties[name]
-                for name, values in self.properties.items()
-                if value.lower() in values.value.lower()
-            }
-            df = self.df.loc[self.df["Example Value"].str.contains(value, na=False, case=False)]
-
-            result = Properties(df, props)
-        else:
-            raise ValueError("Invalid data type. Please provide number, boolean or string.")
-        return result
-
-    def get_navigable(self, prop: str = None) -> "Properties":
+    def get_by_value(self, value: Union[str, bool, int]) -> Properties:
         """
-
-        Browse and returns navigable properties.
+        Browse the properties example values that match the specified query. Results are represented
+        as the dataframe and dict of objects.
 
         Parameters
         ----------
-        prop: str
-            String to fing the matching types.
+        value: str, bool, int
+            Argument to specify expected properties data.
 
         Returns
         -------
             Properties
 
         Examples
         --------
         >>> from refinitiv.data.discovery._search_explorer import SearchPropertyExplorer
+        >>> from refinitiv.data.content import search
         >>> explorer = SearchPropertyExplorer()
-        >>> properties = explorer.get_properties_for(
+        >>> santander_bonds = explorer.get_properties_for(
         ...    view=search.Views.GOV_CORP_INSTRUMENTS,
-        ...    query = "santander bonds",
-        ...    filter = "IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
-        ...)
-        >>> result = properties.get_navigable()
-        """
-        properties = self.get_properties_object(prop)
-
-        props = {}
-        for _property, attributes in properties.items():
-            if attributes.navigable is True:
-                props[_property] = attributes
+        ...    query="santander bonds",
+        ...    filter="IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
+        ... )
+        >>> active = santander_bonds.get_by_value("active")
+        """
+        if isinstance(value, bool):
+            value = str(value)
+            result = self.get_by_type(PropertyType.Boolean)
+            df = result.df
+            properties = Properties(
+                df=df[df["Example Value"] == value],
+                properties={
+                    prop_name: prop_value
+                    for prop_name, prop_value in result.properties.items()
+                    if prop_value.value == value
+                },
+            )
 
-        df = self.df.loc[self.df["Navigable"] == "True"]
-        if prop:
-            df = self._filter_df(df, prop)
-        return Properties(df, props)
+        elif isinstance(value, str) or isinstance(value, int):
+            value = str(value)
+            lower = str.lower
+            value_lower = value.lower()
+            properties = Properties(
+                df=self.df.loc[self.df["Example Value"].str.contains(value, na=False, case=False)],
+                properties={
+                    prop_name: prop_value
+                    for prop_name, prop_value in self.properties.items()
+                    if value_lower in lower(prop_value.value)
+                },
+            )
 
-    def get_by_type(self, property_type: Union[str, PropertyType]) -> Properties:
+        else:
+            raise ValueError("Invalid data type. Please provide number, boolean or string.")
+
+        return properties
+
+    def get_navigable(self, prop: str = None) -> "Properties":
         """
-        Browse the types that match the specified property type
+        Browse all navigable properties, narrow down results by specifying name of navigable property. Results are
+        represented as the dataframe and dict of objects.
 
         Parameters
         ----------
-        property_type: str, PropertyType
-            String to fing the matching types.
+        prop: str
+            String to specify expected properties data.
 
         Returns
         -------
-            pd.DataFrame
+            Properties
 
         Examples
         --------
         >>> from refinitiv.data.discovery._search_explorer import SearchPropertyExplorer
+        >>> from refinitiv.data.content import search
         >>> explorer = SearchPropertyExplorer()
-        >>> properties = explorer.get_properties_for(
+        >>> santander_bonds = explorer.get_properties_for(
         ...    view=search.Views.GOV_CORP_INSTRUMENTS,
-        ...    query = "santander bonds",
-        ...    filter = "IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
-        ...)
-        >>> result = properties.get_by_type(PropertyType.String)
-
+        ...    query="santander bonds",
+        ...    filter="IsPerpetualSecurity ne true and IsActive eq true and not(AssetStatus in ('MAT' 'DC'))",
+        ... )
+        >>> navigable = santander_bonds.get_navigable()
         """
-        if not isinstance(property_type, PropertyType):
-            raise ValueError(f"Invalid property type specified. Type must be: {PropertyType}")
+        if prop is None:
+            properties = self.properties
 
-        props = {}
-        for prop, value in self.properties.items():
-            if str(value.type) == property_type.name:
-                props[prop] = value
-
-        df = self.df.loc[self.df.Type.str.contains(property_type.name, na=False, case=False)]
+        else:
+            properties = self.get_properties_object(prop)
 
-        return Properties(df, props)
+        df = self.df.loc[self.df["Navigable"] == "True"]
+        if prop:
+            df = df.loc[df.Property.str.contains(prop, na=False, case=False)]
 
-    @staticmethod
-    def _filter_df(df, prop):
-        return df.loc[df.Property.str.contains(prop, na=False, case=False)]
+        return Properties(
+            df=df,
+            properties={
+                prop_name: prop_value for prop_name, prop_value in properties.items() if prop_value.navigable is True
+            },
+        )
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/base.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/base.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/embedded.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/embedded.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/manage.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         if key not in config:
             raise KeyError(f"Template or Namespace '{name}' is not found in the config")
 
         data = config[key] or {}
         if "request_body" not in data:
             return UserNamespace(key)
 
-        data = config[key].as_attrdict() if data else {}
+        data = config[key].as_attrdict()
         return template_from_config_data(name, data, self._CONFIG_PREFIX)
 
     def keys(self) -> List[str]:
         """Get list of available search template names"""
         return list(self)
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/namespaces.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/namespaces.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/search.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_search_templates/utils.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_search_templates/utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass
 class StakeholderData:
     instrument: str
+    is_public: bool
     relationship_type: str
+    company_common_name: str
     related_organization_id: str
     value_chains_relationship_confidence_score: str
     value_chain_relationship_freshness_score: str
     value_chains_relationship_update_date: str
+    country_of_headquarters: str
+    trbc_industry_name: str
+    credit_smartratios_implied_rating: str
+    private_company_smartratios_implied_rating: str
     document_title: Optional[str] = None
     ric: Optional[str] = None
     issue_isin: Optional[str] = None
     sedol: Optional[str] = None
 
     @classmethod
     def from_list(cls, datum: list) -> "StakeholderData":
         return cls(
             instrument=datum[0],
-            relationship_type=datum[1],
-            related_organization_id=datum[2],
-            value_chains_relationship_confidence_score=datum[4],
-            value_chain_relationship_freshness_score=datum[5],
-            value_chains_relationship_update_date=datum[6],
+            is_public=datum[1],
+            relationship_type=datum[2],
+            related_organization_id=datum[3],
+            company_common_name=datum[4],
+            value_chains_relationship_confidence_score=datum[5],
+            value_chain_relationship_freshness_score=datum[6],
+            value_chains_relationship_update_date=datum[7],
+            country_of_headquarters=datum[8],
+            trbc_industry_name=datum[9],
+            credit_smartratios_implied_rating=datum[10],
+            private_company_smartratios_implied_rating=datum[11],
         )
 
     def update(self, datum: dict):
         self.document_title = datum.get("DocumentTitle")
         self.ric = datum.get("RIC")
         self.issue_isin = datum.get("IssueISIN")
         self.sedol = datum.get("SEDOL")
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, instrument: str):
         self._instrument = instrument
 
     @property
     def df(self) -> pd.DataFrame:
         return self._df
 
-    def fetch(self):
+    def get_data(self):
         """
         Gets data from the server.
         """
         self._stakeholders, self._df = fetch_data(self._instrument, self._relationship_type)
         self.rics = [item.ric for item in self._stakeholders if item.ric is not None]
 
     def __iter__(self):
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_chain.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_chain.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/discovery/_universe_expanders/_screener.py` & `refinitiv-data-1.3.0/refinitiv/data/discovery/_universe_expanders/_screener.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/early_access/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/early_access/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/eikon/_data_grid.py` & `refinitiv-data-1.3.0/refinitiv/data/eikon/_data_grid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/eikon/_json_requests.py` & `refinitiv-data-1.3.0/refinitiv/data/eikon/_json_requests.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/eikon/_news_request.py` & `refinitiv-data-1.3.0/refinitiv/data/eikon/_news_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/eikon/_streaming_prices.py` & `refinitiv-data-1.3.0/refinitiv/data/eikon/_streaming_prices.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/eikon/_symbology.py` & `refinitiv-data-1.3.0/refinitiv/data/eikon/_symbology.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/eikon/_time_series.py` & `refinitiv-data-1.3.0/refinitiv/data/eikon/_time_series.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/eikon/_tools.py` & `refinitiv-data-1.3.0/refinitiv/data/eikon/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/errors.py` & `refinitiv-data-1.3.0/refinitiv/data/errors.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/session/__init__.py` & `refinitiv-data-1.3.0/refinitiv/data/session/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/session/desktop.py` & `refinitiv-data-1.3.0/refinitiv/data/session/desktop.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/session/platform.py` & `refinitiv-data-1.3.0/refinitiv/data/session/platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 This type of session is used to connect directly to the Refinitiv Data Platform or through a Real-Time Distribution
 System. If you would like to connect directly to RDP, you require a Refinitiv Data account (either a user account or
 a machine account). In both instances, you need to provide Refinitiv data credentials to create the session. If you
 would like to work through a Real-Time Distribution System, you need the IP of the local platform and a username (in
-other words, a DACS user name).
+other words, a DACS username).
 """
 
 __all__ = ("Definition", "GrantPassword")
 
+from typing import Union as _Union
+
 from .._core.session.grant_password import GrantPassword
 
 
 class Definition(object):
     """
     Platform session.
     Can be defined indirectly using the name of a session defined
@@ -33,22 +35,26 @@
         application. When this parameter is set to True, opening this session
         automatically disconnects the other application. When this parameter is set to
         False, the opening of this session fails preserving the other application.
     deployed_platform_host: str, optional
         Host name (or IP) and port to be used to connect to Real-Time Distribution
         System.
     deployed_platform_username: str, optional
-        DACS user name identifying the user when to connecting
+        DACS username identifying the user when to connect
         to a Real-Time Distribution System
     dacs_position: str, optional
         DACS position identifying the terminal when connecting to a Real-Time
         Distribution System.
     dacs_application_id: str, optional
         Must contain the user's Data Access Control System application ID.
         For more information, refer to the DACS documentation on my.refinitiv.com
+    proxies: str or dict, optional
+        Proxies configuration. If string, should be the URL of the proxy
+        (e.g. 'https://proxy.com:8080'). If a dict, the keys are the protocol
+        name (e.g. 'http', 'https') and the values are the proxy URLs.
 
     Raises
     ----------
     Exception
         If app-key is not found in the config file and in arguments.
 
     Examples
@@ -58,37 +64,37 @@
     >>> platform_session = definition.get_session()
     """
 
     def __init__(
         self,
         name: str = "default",
         app_key: str = None,
-        grant=None,
+        grant: GrantPassword = None,
         signon_control: bool = True,
         deployed_platform_host: str = None,
         deployed_platform_username: str = None,
         dacs_position: str = None,
         dacs_application_id: str = None,
+        proxies: _Union[str, dict] = None,
     ) -> None:
-        from .._core.session._session_provider import (
-            _make_platform_session_provider_by_arguments,
-        )
+        from .._core.session._session_provider import _make_platform_session_provider_by_arguments
 
         if not isinstance(name, str):
             raise ValueError("Invalid session name type, please provide string.")
 
         self._create_session = _make_platform_session_provider_by_arguments(
             session_name=name,
             app_key=app_key,
             signon_control=signon_control,
             deployed_platform_host=deployed_platform_host,
             deployed_platform_username=deployed_platform_username,
             dacs_position=dacs_position,
             dacs_application_id=dacs_application_id,
             grant=grant,
+            proxies=proxies,
         )
 
     def get_session(self):
         """
         Creates and returns the session.
 
         Returns
```

### Comparing `refinitiv-data-1.2.0/refinitiv/data/usage_collection/_logger.py` & `refinitiv-data-1.3.0/refinitiv/data/usage_collection/_logger.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv/data/usage_collection/_utils.py` & `refinitiv-data-1.3.0/refinitiv/data/usage_collection/_utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.2.0/refinitiv_data.egg-info/PKG-INFO` & `refinitiv-data-1.3.0/refinitiv_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refinitiv-data
-Version: 1.2.0
+Version: 1.3.0
 Summary: Client for Refinitiv Data Platform API's
 Author: REFINITIV
 License: Apache 2.0
 Project-URL: Homepage, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python
 Project-URL: Documentation, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python/documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `refinitiv-data-1.2.0/refinitiv_data.egg-info/SOURCES.txt` & `refinitiv-data-1.3.0/refinitiv_data.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
-python
 changes/template.jinja
 refinitiv/__init__.py
 refinitiv/data/__init__.py
 refinitiv/data/_base_enum.py
 refinitiv/data/_config_defaults.py
 refinitiv/data/_config_functions.py
 refinitiv/data/_configure.py
@@ -28,14 +27,15 @@
 refinitiv/data/_core/session/_retry_transport.py
 refinitiv/data/_core/session/_session.py
 refinitiv/data/_core/session/_session_cxn_factory.py
 refinitiv/data/_core/session/_session_cxn_type.py
 refinitiv/data/_core/session/_session_definition.py
 refinitiv/data/_core/session/_session_provider.py
 refinitiv/data/_core/session/_session_type.py
+refinitiv/data/_core/session/_user_uuid.py
 refinitiv/data/_core/session/access_token_updater.py
 refinitiv/data/_core/session/auth_manager.py
 refinitiv/data/_core/session/connection.py
 refinitiv/data/_core/session/event.py
 refinitiv/data/_core/session/event_code.py
 refinitiv/data/_core/session/global_settings.py
 refinitiv/data/_core/session/grant_password.py
@@ -798,14 +798,15 @@
 refinitiv/data/delivery/_stream/_rdp_stream.py
 refinitiv/data/delivery/_stream/_stream_cxn_cache.py
 refinitiv/data/delivery/_stream/_stream_cxn_config_data.py
 refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py
 refinitiv/data/delivery/_stream/_stream_factory.py
 refinitiv/data/delivery/_stream/_stream_listener.py
 refinitiv/data/delivery/_stream/_stream_type.py
+refinitiv/data/delivery/_stream/_validator_exceptions.py
 refinitiv/data/delivery/_stream/base_stream.py
 refinitiv/data/delivery/_stream/event.py
 refinitiv/data/delivery/_stream/omm_stream.py
 refinitiv/data/delivery/_stream/omm_stream_connection.py
 refinitiv/data/delivery/_stream/omm_stream_definition.py
 refinitiv/data/delivery/_stream/proxy_info.py
 refinitiv/data/delivery/_stream/rdp_stream.py
@@ -857,16 +858,22 @@
 refinitiv/data/delivery/cfs/file_sets.py
 refinitiv/data/delivery/cfs/files.py
 refinitiv/data/delivery/cfs/packages.py
 refinitiv/data/discovery/__init__.py
 refinitiv/data/discovery/_convert_symbols.py
 refinitiv/data/discovery/_search.py
 refinitiv/data/discovery/_search_explorer/__init__.py
-refinitiv/data/discovery/_search_explorer/_dataclasses.py
+refinitiv/data/discovery/_search_explorer/_buckets_data.py
+refinitiv/data/discovery/_search_explorer/_df_builder.py
+refinitiv/data/discovery/_search_explorer/_navigator.py
+refinitiv/data/discovery/_search_explorer/_properties.py
+refinitiv/data/discovery/_search_explorer/_property.py
+refinitiv/data/discovery/_search_explorer/_property_type.py
 refinitiv/data/discovery/_search_explorer/_search_explorer.py
+refinitiv/data/discovery/_search_explorer/_search_explorer_response.py
 refinitiv/data/discovery/_search_templates/__init__.py
 refinitiv/data/discovery/_search_templates/base.py
 refinitiv/data/discovery/_search_templates/embedded.py
 refinitiv/data/discovery/_search_templates/manage.py
 refinitiv/data/discovery/_search_templates/namespaces.py
 refinitiv/data/discovery/_search_templates/search.py
 refinitiv/data/discovery/_search_templates/utils.py
```

