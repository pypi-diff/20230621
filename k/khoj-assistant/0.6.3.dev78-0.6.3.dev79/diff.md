# Comparing `tmp/khoj_assistant-0.6.3.dev78.tar.gz` & `tmp/khoj_assistant-0.6.3.dev79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jun 20 08:39:33 2023, max compression
+gzip compressed data, last modified: Wed Jun 21 07:13:21 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev78.tar` & `khoj_assistant-0.6.3.dev79.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/__init__.py
--rw-r--r--   0        0        0    10848 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17819 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     1363 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      647 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/base_data_integration.html
--rw-r--r--   0        0        0      657 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0     9826 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     2151 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     3671 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     5756 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    12543 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     2872 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0   275822 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0   205167 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0     4031 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    13101 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     3866 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3070 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4158 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/LICENSE
--rw-r--r--   0        0        0    22877 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/README.md
--rw-r--r--   0        0        0     2785 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/pyproject.toml
--rw-r--r--   0        0        0    25217 2023-06-20 08:39:33.000000 khoj_assistant-0.6.3.dev78/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10848 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17819 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     1362 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      647 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_data_integration.html
+-rw-r--r--   0        0        0      657 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0     9826 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     2151 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     3671 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     5756 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    12543 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     2872 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0   275822 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0   205167 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0     4031 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13101 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     3866 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3070 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4158 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/LICENSE
+-rw-r--r--   0        0        0    22852 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/README.md
+-rw-r--r--   0        0        0     2781 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/pyproject.toml
+-rw-r--r--   0        0        0    25188 2023-06-21 07:13:21.000000 khoj_assistant-0.6.3.dev79/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev79/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/main.py` & `khoj_assistant-0.6.3.dev79/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/404.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_config.html`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         <title>Khoj - Settings</title>
     	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
     </head>
     <body class="khoj-configure">
         <header>
             <div>
                 <h1>Khoj Settings</h1>
-                <p>Check out our <a href="https://github.com/debanjum/khoj">source code on Github</a></p>
+                <p>Check out our <a href="https://github.com/khoj-ai/khoj">source code on Github</a></p>
             </div>
             <div>
                 <h2>Ready?</h2>
                 <div id="actions">
                     <button onclick="window.location.href='/';" >
                         Search
                     </button>
```

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/base_data_integration.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_data_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.6.3.dev79/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev79/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev79/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev79/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev79/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev79/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev79/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev79/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev79/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev79/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/.gitignore` & `khoj_assistant-0.6.3.dev79/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/LICENSE` & `khoj_assistant-0.6.3.dev79/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev78/README.md` & `khoj_assistant-0.6.3.dev79/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Khoj 🦅
-[![test](https://github.com/debanjum/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/debanjum/khoj/actions/workflows/test.yml)
-[![dockerize](https://github.com/debanjum/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/debanjum/khoj/pkgs/container/khoj)
-[![pypi](https://github.com/debanjum/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
+[![test](https://github.com/khoj-ai/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/khoj-ai/khoj/actions/workflows/test.yml)
+[![dockerize](https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/khoj-ai/khoj/pkgs/container/khoj)
+[![pypi](https://github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 
 *An AI personal assistant for your digital brain*
 
 **Supported Plugins**
 
-[![Khoj on Obsidian](https://img.shields.io/badge/Obsidian-%23483699.svg?style=for-the-badge&logo=obsidian&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#readme)
-[![Khoj on Emacs](https://img.shields.io/badge/Emacs-%237F5AB6.svg?&style=for-the-badge&logo=gnu-emacs&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#readme)
+[![Khoj on Obsidian](https://img.shields.io/badge/Obsidian-%23483699.svg?style=for-the-badge&logo=obsidian&logoColor=white)](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#readme)
+[![Khoj on Emacs](https://img.shields.io/badge/Emacs-%237F5AB6.svg?&style=for-the-badge&logo=gnu-emacs&logoColor=white)](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#readme)
 
 ## Table of Contents
 
 - [Features](#Features)
 - [Demos](#Demos)
   - [Khoj in Obsidian](#khoj-in-obsidian)
   - [Khoj in Emacs, Browser](#khoj-in-emacs-browser)
@@ -64,15 +64,15 @@
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
   - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files, Github repositories, and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
-https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
+https://github.com/khoj-ai/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
 - Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
@@ -84,42 +84,42 @@
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
 
 <details><summary>Description</summary>
 
 - Install Khoj via pip
 - Start Khoj app
-- Add this readme and [khoj.el readme](https://github.com/debanjum/khoj/tree/master/src/interface/emacs) as org-mode for Khoj to index
+- Add this readme and [khoj.el readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs) as org-mode for Khoj to index
 - Search \"*Setup editor*\" on the Web and Emacs. Re-rank the results for better accuracy
-- Top result is what we are looking for, the [section to Install Khoj.el on Emacs](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#2-Install-Khojel)
+- Top result is what we are looking for, the [section to Install Khoj.el on Emacs](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#2-Install-Khojel)
 </details>
 
 <details><summary>Analysis</summary>
 
 - The results do not have any words used in the query
   - *Based on the top result it seems the re-ranking model understands that Emacs is an editor?*
 - The results incrementally update as the query is entered
 - The results are re-ranked, for better accuracy, once user hits enter
 </details>
 
 ### Interfaces
 
-![](https://github.com/debanjum/khoj/blob/master/docs/interfaces.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/interfaces.png?)
 
 ## Architecture
 
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_architecture.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_architecture.png?)
 
 ## Setup
 These are the general setup instructions for Khoj.
 
 - Make sure [python](https://realpython.com/installing-python/) (version 3.10 or lower) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
-- Check the [Khoj.el Readme](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
+- Check the [Khoj.el Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
   Its simpler as it can skip the server *install*, *run* and *configure* step below.
-- Check the [Khoj Obsidian Readme](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
+- Check the [Khoj Obsidian Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
   Its simpler as it can skip the *configure* step below.
 
 ### 1. Install
 - On Linux/MacOS
   ```shell
   python -m pip install khoj-assistant
   ```
@@ -143,18 +143,18 @@
 2. Click `Configure` and wait. The app will download ML models and index the content for search
 
 ### 4. Install Interface Plugins
 Khoj exposes a web interface by default.<br />
 The optional steps below allow using Khoj from within an existing application like Obsidian or Emacs.
 
 - **Khoj Obsidian**:<br />
-[Install](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) the Khoj Obsidian plugin
+[Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) the Khoj Obsidian plugin
 
 - **Khoj Emacs**:<br />
-[Install](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#2-Install-Khojel) khoj.el
+[Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#2-Install-Khojel) khoj.el
 
 ## Use
 ### Khoj Search
 - **Khoj via Obsidian**
   - Click the *Khoj search* icon 🔎 on the [Ribbon](https://help.obsidian.md/User+interface/Workspace/Ribbon) or Search for *Khoj: Search* in the [Command Palette](https://help.obsidian.md/Plugins/Command+palette)
 - **Khoj via Emacs**
   - Run `M-x khoj <user-query>`
@@ -197,15 +197,15 @@
 - [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
 
 #### Use
 1. Open [/chat](http://localhost:8000/chat)[^2]
 2. Type your queries and see response by Khoj from your notes
 
 #### Demo
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_chat_web_interface.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_chat_web_interface.png?)
 
 ### Details
 1. Your query is used to retrieve the most relevant notes, if any, using Khoj search
 2. These notes, the last few messages and associated metadata is passed to ChatGPT along with your query for a response
 
 ## Upgrade
 ### Upgrade Khoj Server
@@ -217,19 +217,19 @@
 ```shell
 # Maps to the latest commit on the master branch
 pip install --upgrade --pre khoj-assistant
 ```
 
 ### Upgrade Khoj on Emacs
 - Use your Emacs Package Manager to Upgrade
-- See [khoj.el readme](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#Upgrade) for details
+- See [khoj.el readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Upgrade) for details
 
 ### Upgrade Khoj on Obsidian
 - Upgrade via the Community plugins tab on the settings pane in the Obsidian app
-- See the [khoj plugin readme](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) for details
+- See the [khoj plugin readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) for details
 
 ## Uninstall
 1. (Optional) Hit `Ctrl-C` in the terminal running the khoj server to stop it
 2. Delete the khoj directory in your home folder (i.e `~/.khoj` on Linux, Mac or `C:\Users\<your-username>\.khoj` on Windows)
 3. Uninstall the khoj server with `pip uninstall khoj-assistant`
 4. (Optional) Uninstall khoj.el or the khoj obsidian plugin in the standard way on Emacs, Obsidian
 
@@ -239,15 +239,15 @@
 - **Details**: `pip install khoj-assistant` fails while building the `tokenizers` dependency. Complains about Rust.
 - **Fix**: Install Rust to build the tokenizers package. For example on Mac run:
     ```shell
     brew install rustup
     rustup-init
     source ~/.cargo/env
     ```
-- **Refer**: [Issue with Fix](https://github.com/debanjum/khoj/issues/82#issuecomment-1241890946) for more details
+- **Refer**: [Issue with Fix](https://github.com/khoj-ai/khoj/issues/82#issuecomment-1241890946) for more details
 
 #### Search starts giving wonky results
 - **Fix**: Open [/api/update?force=true](http://localhost:8000/api/update?force=true)[^2] in browser to regenerate index from scratch
 - **Note**: *This is a fix for when you percieve the search results have degraded. Not if you think they've always given wonky results*
 
 #### Khoj in Docker errors out with \"Killed\" in error message
 - **Fix**: Increase RAM available to Docker Containers in Docker Settings
@@ -260,15 +260,15 @@
 ### Access Khoj on Mobile
 1. [Setup Khoj](#Setup) on your personal server. This can be any always-on machine, i.e an old computer, RaspberryPi(?) etc
 2. [Install](https://tailscale.com/kb/installation/) [Tailscale](tailscale.com/) on your personal server and phone
 3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:8000` or `http://name-of-server:8000` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
 4. Click the [Add to Homescreen](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen) button
 5. Enjoy exploring your notes, transactions and images from your phone!
 
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_pwa_android.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_pwa_android.png?)
 
 ### Use OpenAI Models for Search
 #### Setup
 1. Set `encoder-type`, `encoder` and `model-directory` under `asymmetric` and/or `symmetric` `search-type` in your `khoj.yml`[^1]:
    ```diff
       asymmetric:
    -    encoder: "sentence-transformers/multi-qa-MiniLM-L6-cos-v1"
@@ -355,23 +355,23 @@
 - Search, indexing on a GPU has not been tested yet
 
 ## Development
 ### Visualize Codebase
 
 *[Interactive Visualization](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=debanjum%2Fkhoj)*
 
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_codebase_visualization_0.2.1.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_codebase_visualization_0.2.1.png?)
 
 ### Setup
 #### Using Pip
 ##### 1. Install
 
 ```shell
 # Get Khoj Code
-git clone https://github.com/debanjum/khoj && cd khoj
+git clone https://github.com/khoj-ai/khoj && cd khoj
 
 # Create, Activate Virtual Environment
 python3 -m venv .venv && source .venv/bin/activate
 
 # Install Khoj for Development
 pip install -e .[dev]
 ```
@@ -392,15 +392,15 @@
 
   Note: Wait after configuration for khoj to Load ML model, generate embeddings and expose API to query notes, images, transactions etc specified in config YAML
 
 #### Using Docker
 ##### 1. Clone
 
 ```shell
-git clone https://github.com/debanjum/khoj && cd khoj
+git clone https://github.com/khoj-ai/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
 - **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf, Github repositories, and beancount directories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
@@ -420,15 +420,15 @@
 
 #### Using Conda
 ##### 1. Install Dependencies
 - [Install Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
 
 ##### 2. Install Khoj
 ```shell
-git clone https://github.com/debanjum/khoj && cd khoj
+git clone https://github.com/khoj-ai/khoj && cd khoj
 conda env create -f config/environment.yml
 conda activate khoj
 python3 -m pip install pyqt6  # As conda does not support pyqt6 yet
 ```
 
 ##### 3. Configure
 - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
```

### Comparing `khoj_assistant-0.6.3.dev78/pyproject.toml` & `khoj_assistant-0.6.3.dev79/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     "langchain >= 0.0.187",
     "pypdf >= 3.9.0",
     "requests >= 2.26.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://github.com/debanjum/khoj#readme"
-Issues = "https://github.com/debanjum/khoj/issues"
-Discussions = "https://github.com/debanjum/khoj/discussions"
-Releases = "https://github.com/debanjum/khoj/releases"
+Homepage = "https://github.com/khoj-ai/khoj#readme"
+Issues = "https://github.com/khoj-ai/khoj/issues"
+Discussions = "https://github.com/khoj-ai/khoj/discussions"
+Releases = "https://github.com/khoj-ai/khoj/releases"
 
 [project.scripts]
 khoj = "khoj.main:run"
 
 [project.optional-dependencies]
 test = [
     "pytest >= 7.1.2",
```

### Comparing `khoj_assistant-0.6.3.dev78/PKG-INFO` & `khoj_assistant-0.6.3.dev79/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev78
+Version: 0.6.3.dev79
 Summary: A natural language search engine for your personal notes, transactions and images
-Project-URL: Homepage, https://github.com/debanjum/khoj#readme
-Project-URL: Issues, https://github.com/debanjum/khoj/issues
-Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
-Project-URL: Releases, https://github.com/debanjum/khoj/releases
+Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
+Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
+Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
+Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: AI,NLP,beancount,images,markdown,org-mode,pdf,productivity,search,semantic-search
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,24 +51,24 @@
 Requires-Dist: mypy>=1.0.1; extra == 'dev'
 Requires-Dist: pre-commit>=3.0.4; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest>=7.1.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Khoj 🦅
-[![test](https://github.com/debanjum/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/debanjum/khoj/actions/workflows/test.yml)
-[![dockerize](https://github.com/debanjum/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/debanjum/khoj/pkgs/container/khoj)
-[![pypi](https://github.com/debanjum/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
+[![test](https://github.com/khoj-ai/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/khoj-ai/khoj/actions/workflows/test.yml)
+[![dockerize](https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/khoj-ai/khoj/pkgs/container/khoj)
+[![pypi](https://github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 
 *An AI personal assistant for your digital brain*
 
 **Supported Plugins**
 
-[![Khoj on Obsidian](https://img.shields.io/badge/Obsidian-%23483699.svg?style=for-the-badge&logo=obsidian&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#readme)
-[![Khoj on Emacs](https://img.shields.io/badge/Emacs-%237F5AB6.svg?&style=for-the-badge&logo=gnu-emacs&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#readme)
+[![Khoj on Obsidian](https://img.shields.io/badge/Obsidian-%23483699.svg?style=for-the-badge&logo=obsidian&logoColor=white)](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#readme)
+[![Khoj on Emacs](https://img.shields.io/badge/Emacs-%237F5AB6.svg?&style=for-the-badge&logo=gnu-emacs&logoColor=white)](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#readme)
 
 ## Table of Contents
 
 - [Features](#Features)
 - [Demos](#Demos)
   - [Khoj in Obsidian](#khoj-in-obsidian)
   - [Khoj in Emacs, Browser](#khoj-in-emacs-browser)
@@ -120,15 +120,15 @@
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
   - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files, Github repositories, and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
-https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
+https://github.com/khoj-ai/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
 - Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
@@ -140,42 +140,42 @@
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
 
 <details><summary>Description</summary>
 
 - Install Khoj via pip
 - Start Khoj app
-- Add this readme and [khoj.el readme](https://github.com/debanjum/khoj/tree/master/src/interface/emacs) as org-mode for Khoj to index
+- Add this readme and [khoj.el readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs) as org-mode for Khoj to index
 - Search \"*Setup editor*\" on the Web and Emacs. Re-rank the results for better accuracy
-- Top result is what we are looking for, the [section to Install Khoj.el on Emacs](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#2-Install-Khojel)
+- Top result is what we are looking for, the [section to Install Khoj.el on Emacs](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#2-Install-Khojel)
 </details>
 
 <details><summary>Analysis</summary>
 
 - The results do not have any words used in the query
   - *Based on the top result it seems the re-ranking model understands that Emacs is an editor?*
 - The results incrementally update as the query is entered
 - The results are re-ranked, for better accuracy, once user hits enter
 </details>
 
 ### Interfaces
 
-![](https://github.com/debanjum/khoj/blob/master/docs/interfaces.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/interfaces.png?)
 
 ## Architecture
 
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_architecture.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_architecture.png?)
 
 ## Setup
 These are the general setup instructions for Khoj.
 
 - Make sure [python](https://realpython.com/installing-python/) (version 3.10 or lower) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
-- Check the [Khoj.el Readme](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
+- Check the [Khoj.el Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
   Its simpler as it can skip the server *install*, *run* and *configure* step below.
-- Check the [Khoj Obsidian Readme](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
+- Check the [Khoj Obsidian Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
   Its simpler as it can skip the *configure* step below.
 
 ### 1. Install
 - On Linux/MacOS
   ```shell
   python -m pip install khoj-assistant
   ```
@@ -199,18 +199,18 @@
 2. Click `Configure` and wait. The app will download ML models and index the content for search
 
 ### 4. Install Interface Plugins
 Khoj exposes a web interface by default.<br />
 The optional steps below allow using Khoj from within an existing application like Obsidian or Emacs.
 
 - **Khoj Obsidian**:<br />
-[Install](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) the Khoj Obsidian plugin
+[Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) the Khoj Obsidian plugin
 
 - **Khoj Emacs**:<br />
-[Install](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#2-Install-Khojel) khoj.el
+[Install](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#2-Install-Khojel) khoj.el
 
 ## Use
 ### Khoj Search
 - **Khoj via Obsidian**
   - Click the *Khoj search* icon 🔎 on the [Ribbon](https://help.obsidian.md/User+interface/Workspace/Ribbon) or Search for *Khoj: Search* in the [Command Palette](https://help.obsidian.md/Plugins/Command+palette)
 - **Khoj via Emacs**
   - Run `M-x khoj <user-query>`
@@ -253,15 +253,15 @@
 - [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
 
 #### Use
 1. Open [/chat](http://localhost:8000/chat)[^2]
 2. Type your queries and see response by Khoj from your notes
 
 #### Demo
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_chat_web_interface.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_chat_web_interface.png?)
 
 ### Details
 1. Your query is used to retrieve the most relevant notes, if any, using Khoj search
 2. These notes, the last few messages and associated metadata is passed to ChatGPT along with your query for a response
 
 ## Upgrade
 ### Upgrade Khoj Server
@@ -273,19 +273,19 @@
 ```shell
 # Maps to the latest commit on the master branch
 pip install --upgrade --pre khoj-assistant
 ```
 
 ### Upgrade Khoj on Emacs
 - Use your Emacs Package Manager to Upgrade
-- See [khoj.el readme](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#Upgrade) for details
+- See [khoj.el readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Upgrade) for details
 
 ### Upgrade Khoj on Obsidian
 - Upgrade via the Community plugins tab on the settings pane in the Obsidian app
-- See the [khoj plugin readme](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) for details
+- See the [khoj plugin readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#2-Setup-Plugin) for details
 
 ## Uninstall
 1. (Optional) Hit `Ctrl-C` in the terminal running the khoj server to stop it
 2. Delete the khoj directory in your home folder (i.e `~/.khoj` on Linux, Mac or `C:\Users\<your-username>\.khoj` on Windows)
 3. Uninstall the khoj server with `pip uninstall khoj-assistant`
 4. (Optional) Uninstall khoj.el or the khoj obsidian plugin in the standard way on Emacs, Obsidian
 
@@ -295,15 +295,15 @@
 - **Details**: `pip install khoj-assistant` fails while building the `tokenizers` dependency. Complains about Rust.
 - **Fix**: Install Rust to build the tokenizers package. For example on Mac run:
     ```shell
     brew install rustup
     rustup-init
     source ~/.cargo/env
     ```
-- **Refer**: [Issue with Fix](https://github.com/debanjum/khoj/issues/82#issuecomment-1241890946) for more details
+- **Refer**: [Issue with Fix](https://github.com/khoj-ai/khoj/issues/82#issuecomment-1241890946) for more details
 
 #### Search starts giving wonky results
 - **Fix**: Open [/api/update?force=true](http://localhost:8000/api/update?force=true)[^2] in browser to regenerate index from scratch
 - **Note**: *This is a fix for when you percieve the search results have degraded. Not if you think they've always given wonky results*
 
 #### Khoj in Docker errors out with \"Killed\" in error message
 - **Fix**: Increase RAM available to Docker Containers in Docker Settings
@@ -316,15 +316,15 @@
 ### Access Khoj on Mobile
 1. [Setup Khoj](#Setup) on your personal server. This can be any always-on machine, i.e an old computer, RaspberryPi(?) etc
 2. [Install](https://tailscale.com/kb/installation/) [Tailscale](tailscale.com/) on your personal server and phone
 3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:8000` or `http://name-of-server:8000` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
 4. Click the [Add to Homescreen](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen) button
 5. Enjoy exploring your notes, transactions and images from your phone!
 
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_pwa_android.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_pwa_android.png?)
 
 ### Use OpenAI Models for Search
 #### Setup
 1. Set `encoder-type`, `encoder` and `model-directory` under `asymmetric` and/or `symmetric` `search-type` in your `khoj.yml`[^1]:
    ```diff
       asymmetric:
    -    encoder: "sentence-transformers/multi-qa-MiniLM-L6-cos-v1"
@@ -411,23 +411,23 @@
 - Search, indexing on a GPU has not been tested yet
 
 ## Development
 ### Visualize Codebase
 
 *[Interactive Visualization](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=debanjum%2Fkhoj)*
 
-![](https://github.com/debanjum/khoj/blob/master/docs/khoj_codebase_visualization_0.2.1.png?)
+![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_codebase_visualization_0.2.1.png?)
 
 ### Setup
 #### Using Pip
 ##### 1. Install
 
 ```shell
 # Get Khoj Code
-git clone https://github.com/debanjum/khoj && cd khoj
+git clone https://github.com/khoj-ai/khoj && cd khoj
 
 # Create, Activate Virtual Environment
 python3 -m venv .venv && source .venv/bin/activate
 
 # Install Khoj for Development
 pip install -e .[dev]
 ```
@@ -448,15 +448,15 @@
 
   Note: Wait after configuration for khoj to Load ML model, generate embeddings and expose API to query notes, images, transactions etc specified in config YAML
 
 #### Using Docker
 ##### 1. Clone
 
 ```shell
-git clone https://github.com/debanjum/khoj && cd khoj
+git clone https://github.com/khoj-ai/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
 - **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf, Github repositories, and beancount directories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
@@ -476,15 +476,15 @@
 
 #### Using Conda
 ##### 1. Install Dependencies
 - [Install Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
 
 ##### 2. Install Khoj
 ```shell
-git clone https://github.com/debanjum/khoj && cd khoj
+git clone https://github.com/khoj-ai/khoj && cd khoj
 conda env create -f config/environment.yml
 conda activate khoj
 python3 -m pip install pyqt6  # As conda does not support pyqt6 yet
 ```
 
 ##### 3. Configure
 - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
```

