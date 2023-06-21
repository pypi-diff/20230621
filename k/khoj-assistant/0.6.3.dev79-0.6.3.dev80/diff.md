# Comparing `tmp/khoj_assistant-0.6.3.dev79.tar.gz` & `tmp/khoj_assistant-0.6.3.dev80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jun 21 07:13:21 2023, max compression
+gzip compressed data, last modified: Wed Jun 21 08:13:50 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev79.tar` & `khoj_assistant-0.6.3.dev80.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/__init__.py
--rw-r--r--   0        0        0    10848 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17819 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     1362 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      647 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_data_integration.html
--rw-r--r--   0        0        0      657 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0     9826 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     2151 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     3671 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     5756 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    12543 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     2872 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0   275822 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0   205167 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0     4031 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    13101 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     3866 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3070 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4158 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/LICENSE
--rw-r--r--   0        0        0    22852 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/README.md
--rw-r--r--   0        0        0     2781 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/pyproject.toml
--rw-r--r--   0        0        0    25188 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10848 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17819 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     1362 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      647 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/base_data_integration.html
+-rw-r--r--   0        0        0      657 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0     9826 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     2151 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     3671 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     5756 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    12543 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     2872 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0   275822 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0   205167 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0  1300505 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13101 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     3866 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3070 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4158 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/LICENSE
+-rw-r--r--   0        0        0    22943 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/README.md
+-rw-r--r--   0        0        0     2781 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/pyproject.toml
+-rw-r--r--   0        0        0    25279 2023-06-21 08:13:50.000000 khoj_assistant-0.6.3.dev80/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev80/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/main.py` & `khoj_assistant-0.6.3.dev80/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/404.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_data_integration.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/base_data_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.6.3.dev80/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev80/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev80/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev80/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev80/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev80/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev80/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev80/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev80/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev80/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/.gitignore` & `khoj_assistant-0.6.3.dev80/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/LICENSE` & `khoj_assistant-0.6.3.dev80/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/README.md` & `khoj_assistant-0.6.3.dev80/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Khoj 🦅
+<h1><img src="src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg" width="200" alt="Khoj Logo"></h1>
 [![test](https://github.com/khoj-ai/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/khoj-ai/khoj/actions/workflows/test.yml)
 [![dockerize](https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/khoj-ai/khoj/pkgs/container/khoj)
 [![pypi](https://github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 
 *An AI personal assistant for your digital brain*
 
 **Supported Plugins**
@@ -304,15 +304,15 @@
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
  - Open the Khoj desktop GUI, add your [OpenAI API key](https://beta.openai.com/account/api-keys) and click *Configure*
-   Ensure khoj is started **without** the `--no-gui` flag. Check your system tray to see if Khoj 🦅 is minimized there.
+   Ensure khoj is started **without** the `--no-gui` flag. Check your system tray to see if Khoj is minimized there.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
     processor:
       conversation:
     -    openai-api-key: # "YOUR_OPENAI_API_KEY"
     +    openai-api-key: sk-aaaaaaaaaaaaaaaaaaaaaaaahhhhhhhhhhhhhhhhhhhhhhhh
         model: "text-davinci-003"
```

### Comparing `khoj_assistant-0.6.3.dev79/pyproject.toml` & `khoj_assistant-0.6.3.dev80/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev79/PKG-INFO` & `khoj_assistant-0.6.3.dev80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev79
+Version: 0.6.3.dev80
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -50,15 +50,15 @@
 Requires-Dist: khoj-assistant[test]; extra == 'dev'
 Requires-Dist: mypy>=1.0.1; extra == 'dev'
 Requires-Dist: pre-commit>=3.0.4; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest>=7.1.2; extra == 'test'
 Description-Content-Type: text/markdown
 
-# Khoj 🦅
+<h1><img src="src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg" width="200" alt="Khoj Logo"></h1>
 [![test](https://github.com/khoj-ai/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/khoj-ai/khoj/actions/workflows/test.yml)
 [![dockerize](https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/khoj-ai/khoj/pkgs/container/khoj)
 [![pypi](https://github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 
 *An AI personal assistant for your digital brain*
 
 **Supported Plugins**
@@ -360,15 +360,15 @@
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
  - Open the Khoj desktop GUI, add your [OpenAI API key](https://beta.openai.com/account/api-keys) and click *Configure*
-   Ensure khoj is started **without** the `--no-gui` flag. Check your system tray to see if Khoj 🦅 is minimized there.
+   Ensure khoj is started **without** the `--no-gui` flag. Check your system tray to see if Khoj is minimized there.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
     processor:
       conversation:
     -    openai-api-key: # "YOUR_OPENAI_API_KEY"
     +    openai-api-key: sk-aaaaaaaaaaaaaaaaaaaaaaaahhhhhhhhhhhhhhhhhhhhhhhh
         model: "text-davinci-003"
```

