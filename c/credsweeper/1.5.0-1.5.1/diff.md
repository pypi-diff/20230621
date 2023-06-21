# Comparing `tmp/credsweeper-1.5.0.tar.gz` & `tmp/credsweeper-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.5.0.tar", last modified: Tue Jun 13 10:20:00 2023, max compression
+gzip compressed data, was "credsweeper-1.5.1.tar", last modified: Wed Jun 21 11:06:13 2023, max compression
```

## Comparing `credsweeper-1.5.0.tar` & `credsweeper-1.5.1.tar`

### file list

```diff
@@ -1,154 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-13 10:19:49.000000 credsweeper-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-13 10:20:00.773329 credsweeper-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-13 10:19:49.000000 credsweeper-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.757329 credsweeper-1.5.0/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/morpheme_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/deep_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/zip_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.765329 credsweeper-1.5.0/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/patch_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/text_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/cred_card_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/structured_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_entropy_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_pem_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_structured_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.757329 credsweeper-1.5.0/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 10:20:00.773329 credsweeper-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 10:19:49.000000 credsweeper-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-06-13 10:19:49.000000 credsweeper-1.5.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    43683 2023-06-13 10:19:49.000000 credsweeper-1.5.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 11:05:58.000000 credsweeper-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-21 11:06:13.265659 credsweeper-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-21 11:05:58.000000 credsweeper-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.221659 credsweeper-1.5.1/credsweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.225659 credsweeper-1.5.1/credsweeper/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/morpheme_checklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.229659 credsweeper-1.5.1/credsweeper/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.229659 credsweeper-1.5.1/credsweeper/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/line_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.237659 credsweeper-1.5.1/credsweeper/deep_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/zip_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.241659 credsweeper-1.5.1/credsweeper/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/patch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/text_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.257659 credsweeper-1.5.1/credsweeper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/cred_card_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.257659 credsweeper-1.5.1/credsweeper/filters/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/structured_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_method_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_pem_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_structured_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/variable_not_allowed_pattern_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/ml_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/rules/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/scanner/scan_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/credsweeper/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/secret/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/secret/log.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/credsweeper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22458 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/credsweeper/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/apply_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.225659 credsweeper-1.5.1/credsweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 11:06:13.265659 credsweeper-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-21 11:05:58.000000 credsweeper-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-06-21 11:05:59.000000 credsweeper-1.5.1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43633 2023-06-21 11:05:59.000000 credsweeper-1.5.1/tests/test_main.py
```

### Comparing `credsweeper-1.5.0/LICENSE` & `credsweeper-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/PKG-INFO` & `credsweeper-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.0
+Version: 1.5.1
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.0/README.md` & `credsweeper-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/__init__.py` & `credsweeper-1.5.1/credsweeper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

### Comparing `credsweeper-1.5.0/credsweeper/__main__.py` & `credsweeper-1.5.1/credsweeper/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,15 @@
                         metavar="PATH")
     parser.add_argument("--save-xlsx",
                         nargs="?",
                         help="save result to xlsx file (default: output.xlsx)",
                         const="output.xlsx",
                         dest="xlsx_filename",
                         metavar="PATH")
+    parser.add_argument("--sort", help="enable output sorting", dest="sort_output", action="store_true")
     parser.add_argument("--log",
                         "-l",
                         help=f"provide logging level of {list(Logger.LEVELS.keys())}"
                         f"(default: 'warning', case insensitive)",
                         default="warning",
                         dest="log",
                         metavar="LOG_LEVEL",
@@ -267,14 +268,15 @@
             denylist = []
 
         credsweeper = CredSweeper(rule_path=args.rule_path,
                                   config_path=args.config_path,
                                   api_validation=args.api_validation,
                                   json_filename=json_filename,
                                   xlsx_filename=xlsx_filename,
+                                  sort_output=args.sort_output,
                                   pool_count=args.jobs,
                                   ml_batch_size=args.ml_batch_size,
                                   ml_threshold=args.ml_threshold,
                                   find_by_ext=args.find_by_ext,
                                   depth=args.depth,
                                   doc=args.doc,
                                   severity=args.severity,
```

### Comparing `credsweeper-1.5.0/credsweeper/app.py` & `credsweeper-1.5.1/credsweeper/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     def __init__(self,
                  rule_path: Optional[str] = None,
                  config_path: Optional[str] = None,
                  api_validation: bool = False,
                  json_filename: Union[None, str, Path] = None,
                  xlsx_filename: Union[None, str, Path] = None,
+                 sort_output: bool = False,
                  use_filters: bool = True,
                  pool_count: int = 1,
                  ml_batch_size: Optional[int] = 16,
                  ml_threshold: Union[float, ThresholdPreset] = ThresholdPreset.medium,
                  find_by_ext: bool = False,
                  depth: int = 0,
                  doc: bool = False,
@@ -98,14 +99,15 @@
         self.scanner = Scanner(self.config, rule_path)
         self.doc_scanner = Scanner(self.config, rule_path, ["doc"])
         self.deep_scanner = DeepScanner(self.config, self.scanner)
         self.deep_doc_scanner = DeepScanner(self.config, self.doc_scanner)
         self.credential_manager = CredentialManager()
         self.json_filename: Union[None, str, Path] = json_filename
         self.xlsx_filename: Union[None, str, Path] = xlsx_filename
+        self.sort_output = sort_output
         self.ml_batch_size = ml_batch_size
         self.ml_threshold = ml_threshold
         self.ml_validator = None
         self.__log_level = log_level
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
@@ -146,15 +148,15 @@
             config_dict["exclude"]["values"] = config_dict["exclude"].get("values", []) + exclude_values
 
         return config_dict  # type: ignore
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def _use_ml_validation(self) -> bool:
-        if isinstance(self.ml_threshold, float) and self.ml_threshold <= 0:
+        if isinstance(self.ml_threshold, (float, int)) and 0 >= self.ml_threshold:
             return False
         return True
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     # the import cannot be done on top due
     # TypeError: cannot pickle 'onnxruntime.capi.onnxruntime_pybind11_state.InferenceSession' object
@@ -352,23 +354,33 @@
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def export_results(self) -> None:
         """Save credential candidates to json file or print them to a console."""
         is_exported = False
 
+        credentials = self.credential_manager.get_credentials()
+
+        if self.sort_output:
+            credentials.sort(key=lambda x: (  #
+                x.line_data_list[0].path,  #
+                x.line_data_list[0].line_num,  #
+                x.severity,  #
+                x.rule_name,  #
+                x.line_data_list[0].value  #
+            ))
+
         if self.json_filename:
             is_exported = True
-            Util.json_dump([credential.to_json() for credential in self.credential_manager.get_credentials()],
-                           file_path=self.json_filename)
+            Util.json_dump([credential.to_json() for credential in credentials], file_path=self.json_filename)
 
         if self.xlsx_filename:
             is_exported = True
             data_list = []
-            for credential in self.credential_manager.get_credentials():
+            for credential in credentials:
                 data_list.extend(credential.to_dict_list())
             df = pd.DataFrame(data=data_list)
             df.to_excel(self.xlsx_filename, index=False)
 
         if is_exported is False:
-            for credential in self.credential_manager.get_credentials():
+            for credential in credentials:
                 print(credential)
```

### Comparing `credsweeper-1.5.0/credsweeper/common/constants.py` & `credsweeper-1.5.1/credsweeper/common/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,25 +57,28 @@
     base36 = "base36"
     base64 = "base64"
     hex = "hex"
 
 
 class Chars(Enum):
     """Stores three types characters sets.
-
-    Parameters:
-        HEX_CHARS: set of characters, hexadecimal numeral system (Base16)
-        BASE36_CHARS: set of 36 characters, used in Base36 encoding
-        BASE64_CHARS: set of 64 characters, used in Base64 encoding
-
     """
-    HEX_CHARS = "1234567890abcdefABCDEF"
+
+    # set of characters, hexadecimal numeral system (Base16). Upper- and lowercase
+    HEX_CHARS = "0123456789ABCDEFabcdef"
+    # set of 32 characters, used in Base32 encoding
     BASE32_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZ234567"
+    # set of 36 characters, used in Base36 encoding
     BASE36_CHARS = "abcdefghijklmnopqrstuvwxyz1234567890"
+    # standard base64 with padding sign
     BASE64_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/="
+    # URL- and filename-safe standard
+    BASE64URL_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_"
+    # standard base64
+    BASE64STD_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"
 
 
 class KeyValidationOption(Enum):
     """API validation state"""
     INVALID_KEY = 0
     VALIDATED_KEY = 1
     UNDECIDED = 2
```

### Comparing `credsweeper-1.5.0/credsweeper/common/keyword_checklist.py` & `credsweeper-1.5.1/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.5.1/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.5.1/credsweeper/common/morpheme_checklist.txt`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 _ret
 _rev
 _rgb
 _rsa_
 _rw_
 _rx_
 _sdr_
-_sha
 _src
 _to
 _tx_
 _un
 _up
 _val
 _vol
@@ -145,15 +144,17 @@
 arian
 arker
 arpa
 array
 arro
 art
 ascii
+ash
 asia
+asic
 ask
 assembl
 assert
 assoc
 asure
 asyn
 ately
@@ -184,17 +185,15 @@
 azure
 back
 badge
 balanc
 bank
 bann
 bar
-base
-bash
-basic
+bas
 batch
 batt
 beac
 beans
 beat
 begin
 behav
@@ -286,15 +285,14 @@
 chacha
 chain
 change
 channel
 chant
 chapter
 char
-chase
 check
 chevron
 child
 chin
 chip
 choices
 chomp
@@ -395,15 +393,15 @@
 cut
 cyan
 cycle
 daily
 danger
 darken
 darwin
-dash
+das
 data
 date
 davinci
 day
 dead
 debug
 decimal
@@ -580,15 +578,15 @@
 final
 find
 fine
 fire
 firm
 first
 fix
-flash
+flas
 flat
 fleet
 flick
 float
 floor
 fluent
 fluid
@@ -620,14 +618,15 @@
 gauss
 gen
 geo
 gest
 get
 ghbor
 ghz_
+gian
 ging
 git
 given
 global
 gobble
 google
 grab
@@ -644,18 +643,25 @@
 gress
 grid
 gro
 grpc
 guard
 guest
 guish
+ha1-
+ha1_
+ha2-
+ha256
+ha2_
+ha394
+ha512
 hack
 half
 hard
-hash
+has
 have
 having
 havior
 hdmi
 head
 health
 hear
@@ -718,18 +724,21 @@
 ini
 injec
 inn
 insert
 insig
 instead
 int
+inval
 invent
 inver
 invoke
 ion
+ipv4
+ipv6
 iron
 irq_
 is_
 ished
 iso_
 isolat
 issue
@@ -919,14 +928,15 @@
 never
 new
 next
 nexus
 nielsen
 ning
 nipp
+nish
 nism
 node
 non
 norm
 not
 nsive
 ntal
@@ -952,14 +962,15 @@
 on_
 oncat
 one
 onfig
 only
 open
 opted
+opti
 oracle
 orbi
 order
 ordinar
 ores
 organ
 ories
@@ -1054,15 +1065,15 @@
 provi
 prox
 pseudo
 pster
 psycho
 pub
 pull
-purchas
+purcha
 purple
 push
 put
 pwr_
 python
 qos
 quantum
@@ -1109,14 +1120,15 @@
 refer
 reflect
 refresh
 reg_
 regexp
 regio
 regist
+regs
 regul
 rejec
 relat
 release
 reli
 remar
 remo
@@ -1186,16 +1198,16 @@
 sams
 saves
 savi
 scala
 scale
 scali
 scen
-schedu
-scheme
+sched
+schem
 scope
 scram
 screen
 scri
 scro
 seal
 searc
@@ -1218,17 +1230,18 @@
 seria
 series
 serv
 sessio
 set
 sever
 sex
-sha256
-sha384
-sha512
+sha1
+sha2
+sha3
+sha5
 shadow
 shape
 shift
 ship
 shoot
 short
 shot
@@ -1248,28 +1261,29 @@
 sing
 sip
 sites
 size
 sizi
 skip
 slack
-slash
+slas
 slave
 sleep
 slice
 slick
 slide
 slot
 smar
 smooth
 snap
 sness
 sniff
 snip
 social
+sock
 soft
 solid
 solve
 sony
 sort
 sound
 source
@@ -1286,15 +1300,15 @@
 spray
 sql
 src_
 ssl
 stack
 stan
 star
-stash
+stas
 stat
 stdin
 steer
 stem
 sten
 step
 stic
@@ -1320,16 +1334,15 @@
 succes
 such
 suffi
 suite
 sum
 sun
 supe
-suppl
-suppo
+supp
 surro
 suspe
 swap
 swift
 swing
 switch
 swizz
```

### Comparing `credsweeper-1.5.0/credsweeper/config/config.py` & `credsweeper-1.5.1/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.5.1/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/credentials/candidate.py` & `credsweeper-1.5.1/credsweeper/credentials/candidate.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.5.1/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/credentials/candidate_key.py` & `credsweeper-1.5.1/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/credentials/credential_manager.py` & `credsweeper-1.5.1/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/credentials/line_data.py` & `credsweeper-1.5.1/credsweeper/credentials/line_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from functools import cached_property
 from typing import Any, Dict, Optional, Tuple
 
 from credsweeper.config import Config
 from credsweeper.utils import Util
 
 
 class LineData:
@@ -67,14 +68,20 @@
         """line getter"""
         return self.__line
 
     @line.setter
     def line(self, line: str) -> None:
         """line setter"""
         self.__line = line
+        self.__dict__.pop("line_len", None)
+
+    @cached_property
+    def line_len(self) -> int:
+        """line_len getter"""
+        return len(self.__line)
 
     @property
     def line_num(self) -> int:
         """line_num getter"""
         return self.__line_num
 
     @line_num.setter
```

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/byte_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/deep_scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,16 +171,20 @@
             # break recursion if maximal depth is reached
             logger.debug("bottom reached %s recursive_limit_size:%d", struct_provider.file_path, recursive_limit_size)
             return candidates
 
         depth -= 1
 
         items: List[Tuple[Union[int, str], Any]] = []
+        struct_key: Optional[str] = None
+        struct_value: Optional[str] = None
         if isinstance(struct_provider.struct, dict):
             items = list(struct_provider.struct.items())
+            struct_key = struct_provider.struct.get("key")
+            struct_value = struct_provider.struct.get("value")
         elif isinstance(struct_provider.struct, list) or isinstance(struct_provider.struct, tuple):
             items = list(enumerate(struct_provider.struct))
         else:
             logger.error("Not supported type:%s val:%s", str(type(struct_provider.struct)), str(struct_provider.struct))
 
         for key, value in items:
             if isinstance(value, dict) or isinstance(value, list) or isinstance(value, tuple):
@@ -205,22 +209,33 @@
                                                           file_path=struct_provider.file_path,
                                                           file_type=struct_provider.file_type,
                                                           info=f"{struct_provider.info}|STRING:{key}")
                 new_limit = recursive_limit_size - len(str_struct_provider.data)
                 new_candidates = self.recursive_scan(str_struct_provider, depth, new_limit)
                 candidates.extend(new_candidates)
 
-                # use key = "value" scan for common cases like in Python code
+                # use key = "value" scan for common cases like in TOML
                 if isinstance(struct_provider.struct, dict):
-                    str_provider = StringContentProvider([f"{key} = \"{value}\""],
+                    line = f"{key} = \"{value}\""
+                    str_provider = StringContentProvider([line],
                                                          file_path=struct_provider.file_path,
-                                                         file_type=".py",
-                                                         info=f"{struct_provider.info}|STRING:`{key} = \"{value}\"`")
+                                                         file_type=".toml",
+                                                         info=f"{struct_provider.info}|STRING:`{line}`")
                     str_analysis_targets = str_provider.get_analysis_target()
                     new_candidates = self.scanner.scan(str_analysis_targets)
                     augment_candidates(candidates, new_candidates)
             elif isinstance(value, int) or isinstance(value, float):
                 pass
             else:
                 logger.debug("Not supported type:%s value(%s)", str(type(value)), str(value))
 
+        # last check when dictionary is {"key": "api_key", "value": "XXXXXXX"} -> {"api_key": "XXXXXXX"}
+        if isinstance(struct_key, str) and isinstance(struct_value, str):
+            line = f"{struct_key} = \"{struct_value}\""
+            key_value_provider = StringContentProvider([line],
+                                                       file_path=struct_provider.file_path,
+                                                       file_type=".toml",
+                                                       info=f"{struct_provider.info}|STRING:`{line}`")
+            key_value_analysis_targets = key_value_provider.get_analysis_target()
+            new_candidates = self.scanner.scan(key_value_analysis_targets)
+            augment_candidates(candidates, new_candidates)
         return candidates
```

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/html_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.5.1/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/__init__.py` & `credsweeper-1.5.1/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/content_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/data_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.5.1/credsweeper/file_handler/file_path_extractor.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/files_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/patch_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/patch_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/file_handler/text_provider.py` & `credsweeper-1.5.1/credsweeper/file_handler/text_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/filters/__init__.py` & `credsweeper-1.5.1/credsweeper/filters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 
 from credsweeper.filters.cred_card_number_check import CreditCardNumberCheck
 from credsweeper.filters.line_specific_key_check import LineSpecificKeyCheck
 from credsweeper.filters.separator_unusual_check import SeparatorUnusualCheck
 from credsweeper.filters.value_allowlist_check import ValueAllowlistCheck
 from credsweeper.filters.value_array_dictionary_check import ValueArrayDictionaryCheck
 from credsweeper.filters.value_base32_data_check import ValueBase32DataCheck
+from credsweeper.filters.value_base64_data_check import ValueBase64DataCheck
 from credsweeper.filters.value_blocklist_check import ValueBlocklistCheck
 from credsweeper.filters.value_camel_case_check import ValueCamelCaseCheck
 from credsweeper.filters.value_couple_keyword_check import ValueCoupleKeywordCheck
 from credsweeper.filters.value_dictionary_keyword_check import ValueDictionaryKeywordCheck
 from credsweeper.filters.value_dictionary_value_length_check import ValueDictionaryValueLengthCheck
 from credsweeper.filters.value_entropy_base32_check import ValueEntropyBase32Check
 from credsweeper.filters.value_entropy_base36_check import ValueEntropyBase36Check
+from credsweeper.filters.value_entropy_base64_check import ValueEntropyBase64Check
 from credsweeper.filters.value_entropy_check import ValueEntropyCheck
 from credsweeper.filters.value_file_path_check import ValueFilePathCheck
 from credsweeper.filters.value_first_word_check import ValueFirstWordCheck
 from credsweeper.filters.value_grafana_check import ValueGrafanaCheck
 from credsweeper.filters.value_json_web_token_check import ValueJsonWebTokenCheck
 from credsweeper.filters.value_last_word_check import ValueLastWordCheck
 from credsweeper.filters.value_length_check import ValueLengthCheck
 from credsweeper.filters.value_method_check import ValueMethodCheck
 from credsweeper.filters.value_not_allowed_pattern_check import ValueNotAllowedPatternCheck
+from credsweeper.filters.value_not_part_encoded_check import ValueNotPartEncodedCheck
 from credsweeper.filters.value_number_check import ValueNumberCheck
 from credsweeper.filters.value_pattern_check import ValuePatternCheck
 from credsweeper.filters.value_pattern_length_check import ValuePatternLengthCheck
 from credsweeper.filters.value_pem_pattern_check import ValuePemPatternCheck
 from credsweeper.filters.value_similarity_check import ValueSimilarityCheck
 from credsweeper.filters.value_split_keyword_check import ValueSplitKeywordCheck
 from credsweeper.filters.value_string_type_check import ValueStringTypeCheck
 from credsweeper.filters.value_structured_token_check import ValueStructuredTokenCheck
 from credsweeper.filters.value_token_base32_check import ValueTokenBase32Check
 from credsweeper.filters.value_token_base36_check import ValueTokenBase36Check
+from credsweeper.filters.value_token_base64_check import ValueTokenBase64Check
 from credsweeper.filters.value_token_check import ValueTokenCheck
 from credsweeper.filters.value_useless_word_check import ValueUselessWordCheck
 from credsweeper.filters.variable_not_allowed_pattern_check import VariableNotAllowedPatternCheck
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/cred_card_number_check.py` & `credsweeper-1.5.1/credsweeper/filters/cred_card_number_check.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class CreditCardNumberCheck(Filter):
     """Check that value is a credit card number."""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             False, if the sequence is not card number. True if it is
 
         """
         if line_data.value is None \
                 or 16 != len(line_data.value) \
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/filter.py` & `credsweeper-1.5.1/credsweeper/filters/filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from abc import abstractmethod
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 
 
 class Filter:
     """Base class for all filters that operates on 'line_data' objects."""
 
     @abstractmethod
     def __init__(self, config: Config):
         raise NotImplementedError()
 
     @abstractmethod
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         raise NotImplementedError()
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/group/__init__.py` & `credsweeper-1.5.1/credsweeper/filters/group/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,7 +3,8 @@
 from credsweeper.filters.group.general_keyword import GeneralKeyword
 from credsweeper.filters.group.general_pattern import GeneralPattern
 from credsweeper.filters.group.password_keyword import PasswordKeyword
 from credsweeper.filters.group.structured_token import StructuredToken
 from credsweeper.filters.group.token_pattern import TokenPattern
 from credsweeper.filters.group.url_credentials_group import UrlCredentialsGroup
 from credsweeper.filters.group.weird_base36_token import WeirdBase36Token
+from credsweeper.filters.group.weird_base64_token import WeirdBase64Token
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/group/group.py` & `credsweeper-1.5.1/credsweeper/filters/group/group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.5.1/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.5.1/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.5.1/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.5.1/credsweeper/filters/line_specific_key_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class LineSpecificKeyCheck(Filter):
     """Check that values from list below is not in candidate line."""
 
@@ -13,19 +14,20 @@
     NOT_ALLOWED_PATTERN = re.compile(  #
         Util.get_regex_combine_or(NOT_ALLOWED),  #
         flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if line_data.line is None:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.5.1/credsweeper/filters/separator_unusual_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class SeparatorUnusualCheck(Filter):
     """Check that candidate have no double symbol ops (like ++, --, <<) or comparison ops (like != or ==) as separator.
 
     Example:
@@ -12,19 +13,20 @@
         `pwd << value`
 
     """
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if line_data.separator is None:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_allowlist_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueAllowlistCheck(Filter):
     """Check that patterns from the list is not present in the candidate value."""
 
@@ -16,19 +17,20 @@
     ALLOWED_PATTERN = re.compile(  #
         Util.get_regex_combine_or(ALLOWED),  #
         flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_array_dictionary_check.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueArrayDictionaryCheck(Filter):
     """Match call to dictionary or array element.
 
     This filter checks only calls, not declarations:
@@ -14,19 +15,20 @@
     """
 
     PATTERN = re.compile("\\[('|\")?.+('|\")?\\]")
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_base32_data_check.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import base64
 import contextlib
 import string
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueBase32DataCheck(Filter):
     """
     Check that candidate is NOT an ascii encoded string with entropy check
     """
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received weird base32 token which must be a random string
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, when need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_blocklist_check.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueBlocklistCheck(Filter):
     """Check that words from block list is lest that 70% of candidate value length."""
 
     NOT_ALLOWED = [
@@ -13,19 +14,20 @@
         "bearer",
         "string",
     ]
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_first_word_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
-class ValueCamelCaseCheck(Filter):
-    """Check that candidate is not written in camel case."""
+class ValueFirstWordCheck(Filter):
+    """Check that secret doesn't starts with special character."""
 
-    CAMEL_CASE = ["^([a-z]+([A-Z][a-z]+)+)$", "^([A-Z][a-z]+([A-Z][a-z]+)+)$"]
-    CAMEL_CASE_PATTERN = re.compile(Util.get_regex_combine_or(CAMEL_CASE))
+    NOT_ALLOWED = [
+        "\\=", "\\{", "\\)", "\\<", "\\>", "\\#", "\\:", "\\\\", "\\/\\/", "\\_", "\\\\[u]", "\\/\\*", "\\%[deflspuvxz]"
+    ]
+    NOT_ALLOWED_PATTERN = re.compile(  #
+        f"^{Util.get_regex_combine_or(NOT_ALLOWED)}",  #
+        flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-
-        if self.CAMEL_CASE_PATTERN.match(line_data.value):
+        if self.NOT_ALLOWED_PATTERN.match(line_data.value):
             return True
-
         return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_last_word_check.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from credsweeper.common import static_keyword_checklist
+import re
+
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueCoupleKeywordCheck(Filter):
-    """Check value if TWO words from morphemes checklist exists in value"""
+class ValueLastWordCheck(Filter):
+    """Check that secret is not short value that ends with `:`."""
+
+    NOT_ALLOWED_COLON_PATTERN = re.compile(".*:$", flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        value = line_data.value.lower()
-        matches = 0
-        for keyword in static_keyword_checklist.morpheme_set:
-            if keyword in value:
-                matches += 1
-                if 1 < matches:
-                    return True
+        if len(line_data.value) < 16 and self.NOT_ALLOWED_COLON_PATTERN.search(line_data.value):
+            return True
         return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from credsweeper.common import static_keyword_checklist
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueDictionaryKeywordCheck(Filter):
     """Check that no word from dictionary present in the candidate value."""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_similarity_check.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueDictionaryValueLengthCheck(Filter):
-    """Check that candidate length is between 5 and 30."""
+class ValueSimilarityCheck(Filter):
+    """Check if candidate value is at least 70% same as candidate keyword. Like: `secret = "mysecret"`."""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if not line_data.value:
+        # Cannot evaluate if key is None
+        if line_data.key is None:
+            return False
+        if line_data.key.lower() in line_data.value.lower() and \
+                len(line_data.key) / len(line_data.value) >= 0.7:
             return True
-        if len(line_data.value) < 4 or len(line_data.value) > 30:
+        if line_data.variable is not None and line_data.value in line_data.variable:
             return True
         return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_entropy_base32_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import math
 
 from credsweeper.common.constants import Chars
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueEntropyBase32Check(Filter):
     """Check that candidate have Shanon Entropy (for [a-z0-9])"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_entropy_base36_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import math
 
 from credsweeper.common.constants import Chars
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueEntropyBase36Check(Filter):
     """Check that candidate have Shanon Entropy (for [a-z0-9])"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_entropy_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_entropy_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueEntropyCheck(Filter):
     """Check that candidate have Shanon Entropy > 3 (for HEX_CHARS or BASE36_CHARS) or > 4.5 (for BASE64_CHARS)."""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_file_path_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueFilePathCheck(Filter):
     r"""Check that candidate value is a path or not.
 
     Check if a value contains either '/' or ':\' separators (but not both)
     and do not have any special characters ( !$`&*()+)
     """
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
-class ValueFirstWordCheck(Filter):
-    """Check that secret doesn't starts with special character."""
+class ValueNotAllowedPatternCheck(Filter):
+    """Check that secret doesn't open or closes brackets or a new line."""
 
-    NOT_ALLOWED = [
-        "\\=", "\\{", "\\)", "\\<", "\\>", "\\#", "\\:", "\\\\", "\\/\\/", "\\_", "\\\\[u]", "\\/\\*", "\\%[deflspuvxz]"
-    ]
+    NOT_ALLOWED = ["[,<>{};\\]\\[](\\s)*", "(\\s)+[\\\\]", "(\\\\n)(\\s)*"]
     NOT_ALLOWED_PATTERN = re.compile(  #
-        f"^{Util.get_regex_combine_or(NOT_ALLOWED)}",  #
+        f"{Util.get_regex_combine_or(NOT_ALLOWED)}$",  #
         flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        if self.NOT_ALLOWED_PATTERN.match(line_data.value):
+        if self.NOT_ALLOWED_PATTERN.search(line_data.value):
             return True
         return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_grafana_check.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import base64
 import contextlib
 import json
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueGrafanaCheck(Filter):
     """Grafana Provisioned API Key and Access Policy Token"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received token which might be structured.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, when need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_json_web_token_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import base64
 import contextlib
 import json
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueJsonWebTokenCheck(Filter):
     """
     Check that candidate is JWT which starts usually from 'eyJ'
     only header is parsed with "typ" or "alg" member from example of RFC7519
     https://datatracker.ietf.org/doc/html/rfc7519
     """
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received token which might be structured.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, when need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_couple_keyword_check.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-import re
-
+from credsweeper.common import static_keyword_checklist
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueLastWordCheck(Filter):
-    """Check that secret is not short value that ends with `:`."""
-
-    NOT_ALLOWED_COLON_PATTERN = re.compile(".*:$", flags=re.IGNORECASE)
+class ValueCoupleKeywordCheck(Filter):
+    """Check value if TWO words from morphemes checklist exists in value"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        if len(line_data.value) < 16 and self.NOT_ALLOWED_COLON_PATTERN.search(line_data.value):
-            return True
+        value = line_data.value.lower()
+        matches = 0
+        for keyword in static_keyword_checklist.morpheme_set:
+            if keyword in value:
+                matches += 1
+                if 1 < matches:
+                    return True
         return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_method_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_method_check.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueMethodCheck(Filter):
     """Check if potential candidate value is a function.
 
     Check if potential candidate value is a function by looking for '(', ')' or 'function' sub-strings in it
     """
 
     PATTERN = re.compile(".*\\(.*\\).*")
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_length_check.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-import re
-
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
-from credsweeper.utils import Util
-
 
-class ValueNotAllowedPatternCheck(Filter):
-    """Check that secret doesn't open or closes brackets or a new line."""
 
-    NOT_ALLOWED = ["[,<>{};\\]\\[](\\s)*", "(\\s)+[\\\\]", "(\\\\n)(\\s)*"]
-    NOT_ALLOWED_PATTERN = re.compile(  #
-        f"{Util.get_regex_combine_or(NOT_ALLOWED)}$",  #
-        flags=re.IGNORECASE)
+class ValueLengthCheck(Filter):
+    """Check if potential candidate value is not too short (longer or equal to `min_len`)."""
 
-    def __init__(self, config: Config = None) -> None:
-        pass
+    def __init__(self, config: Config) -> None:
+        self.min_len = config.min_keyword_value_length
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        if self.NOT_ALLOWED_PATTERN.search(line_data.value):
+        if len(line_data.value) < self.min_len:
             return True
         return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_pattern_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValuePatternCheck(Filter):
     """Check if candidate value contain specific pattern.
 
     Similar to linguistic sequences of characters, random strings shouldn't contain math sequences of
@@ -88,19 +89,20 @@
             else:
                 count = 1
                 continue
             if count == self.pattern_len:
                 return True
         return False
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Arg:
             line_data: LineData object, credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             boolean variable. True, if need to filter candidate and False if left
 
         """
         if not line_data.value or len(line_data.value) < self.pattern_len:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_pem_pattern_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_pem_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_camel_case_check.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+import re
+
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
+from credsweeper.utils import Util
+
 
+class ValueCamelCaseCheck(Filter):
+    """Check that candidate is not written in camel case."""
 
-class ValueSimilarityCheck(Filter):
-    """Check if candidate value is at least 70% same as candidate keyword. Like: `secret = "mysecret"`."""
+    CAMEL_CASE = ["^([a-z]+([A-Z][a-z]+)+)$", "^([A-Z][a-z]+([A-Z][a-z]+)+)$"]
+    CAMEL_CASE_PATTERN = re.compile(Util.get_regex_combine_or(CAMEL_CASE))
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        # Cannot evaluate if key is None
-        if line_data.key is None:
-            return False
-        if line_data.key.lower() in line_data.value.lower() and \
-                len(line_data.key) / len(line_data.value) >= 0.7:
+        if not line_data.value:
             return True
-        if line_data.variable is not None and line_data.value in line_data.variable:
+
+        if self.CAMEL_CASE_PATTERN.match(line_data.value):
             return True
+
         return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_split_keyword_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from typing import Union
 
 from credsweeper.common import static_keyword_checklist
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueSplitKeywordCheck(Filter):
     """Check value by splitting with standard whitespace separators and any word is not matched in checklist."""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_string_type_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueStringTypeCheck(Filter):
     r"""Check if line_data is in source code file that require quotes for string declaration.
 
     If it is, then checks if line_data really have string literal declaration.
@@ -18,19 +19,20 @@
 
     False otherwise
     """
 
     def __init__(self, config: Config) -> None:
         self.check_for_literals = config.check_for_literals
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not self.check_for_literals:
             return False
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_structured_token_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_structured_token_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import base64
 import binascii
 import contextlib
 
 from credsweeper.common.constants import LATIN_1
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueStructuredTokenCheck(Filter):
     """Check that candidate have a known structure"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received token which might be structured.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_token_base32_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from password_strength import PasswordStats
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueTokenBase32Check(Filter):
     """Check that candidate have good randomization"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_token_base64_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from password_strength import PasswordStats
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueTokenBase36Check(Filter):
+class ValueTokenBase64Check(Filter):
     """Check that candidate have good randomization"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
 
         strength = float(PasswordStats(line_data.value).strength())
-        min_strength = ValueTokenBase36Check.get_min_strength(len(line_data.value))
+        min_strength = ValueTokenBase64Check.get_min_strength(len(line_data.value))
         return min_strength > strength
 
     @staticmethod
     def get_min_strength(x: int) -> float:
-        """Returns minimal strength. Precalculated data is applied for speedup"""
-        if 15 == x:
-            y = 0.66
+        """Returns minimal strength. Precalculated rounded data is applied for speedup"""
+        if 18 == x:
+            y = 0.7
+        elif 20 == x:
+            y = 0.8
         elif 24 == x:
             y = 0.9
-        elif 25 == x:
+        elif 32 == x:
             y = 0.9
-        elif 8 <= x <= 32:
-            # approximation not exceed standard deviation
-            y = ((0.000067 * x - 0.00571) * x + 0.1718) * x - 0.86
+        elif x < 40:
+            y = ((0.0000405 * x - 0.004117) * x + 0.141) * x - 0.65
         else:
             y = 1
         return y
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_token_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_token_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
 class ValueTokenCheck(Filter):
     """Check if first substring of token is shorter than 5.
 
     Split candidate value into substrings using ` ;`{})(<>[]` separators. Check if first substring is shorter than 5
@@ -17,19 +18,20 @@
     """
 
     SPLIT_PATTERN = " |;|\\)|\\(|{|}|<|>|\\[|\\]|`"
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.5.1/credsweeper/filters/value_useless_word_check.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueUselessWordCheck(Filter):
     """Check is candidate value contains sub-rows with operators (like ->)."""
 
@@ -18,19 +19,20 @@
     NOT_ALLOWED_PATTERN = re.compile(  #
         Util.get_regex_combine_or(NOT_ALLOWED),  #
         flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.5.1/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
+from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class VariableNotAllowedPatternCheck(Filter):
     """Check if candidate variable is a regex placeholder or ends with match character (like + or >)."""
 
@@ -13,19 +14,20 @@
     NOT_ALLOWED_PATTERN = re.compile(  #
         Util.get_regex_combine_or(NOT_ALLOWED),  #
         flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
 
-    def run(self, line_data: LineData) -> bool:
+    def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
+            target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if line_data.variable is None:
             return True
```

### Comparing `credsweeper-1.5.0/credsweeper/logger/logger.py` & `credsweeper-1.5.1/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/ml_model/features.py` & `credsweeper-1.5.1/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.5.1/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.5.1/credsweeper/ml_model/ml_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/ml_model/model_config.json` & `credsweeper-1.5.1/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/rules/config.yaml` & `credsweeper-1.5.1/credsweeper/rules/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -22,29 +22,29 @@
   usage_list:
     - src
 
 - name: AWS Client ID
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>(ABIA|ACCA|AGPA|AIDA|AIPA|AKIA|ANPA|ANVA|AROA|APKA|ASCA|ASIA)[0-9A-Z]{16,17})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>(ABIA|ACCA|AGPA|AIDA|AIPA|AKIA|ANPA|ANVA|AROA|APKA|ASCA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - A
   min_line_len: 20
   usage_list:
     - src
     - doc
 
 - name: AWS Multi
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>(AKIA|ASIA)[0-9A-Z]{16,17})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>(AKIA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
     - (?P<value>[0-9a-zA-Z/+]{40})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - AKIA
     - ASIA
   min_line_len: 20
@@ -52,15 +52,15 @@
     - src
     - doc
 
 - name: AWS MWS Key
   severity: high
   type: pattern
   values:
-    - (?P<value>amzn\.mws\.[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12})
+    - (^|[^0-9A-Za-z])(?P<value>amzn\.mws\.[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - amzn
   min_line_len: 30
   usage_list:
     - src
@@ -79,34 +79,34 @@
   usage_list:
     - src
 
 - name: Dynatrace API Token
   severity: high
   type: pattern
   values:
-    - (?P<value>dt0[a-zA-Z]{1}[0-9]{2}\.[A-Z0-9]{24}\.[A-Z0-9]{64})
+    - (^|[^0-9A-Za-z])(?P<value>dt0[a-zA-Z]{1}[0-9]{2}\.[A-Z0-9]{24}\.[A-Z0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - dt0
   min_line_len: 90
   usage_list:
     - src
     - doc
 
 - name: Facebook Access Token
   severity: high
   type: pattern
   values:
-    - (?P<value>EAACEdEose0cBA[0-9A-Za-z]+)
+    - (^|[^0-9A-Za-z])(?P<value>EAAC[0-9A-Za-z]{27,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
-    - EAACEdEose0cBA
-  min_line_len: 15
+    - EAAC
+  min_line_len: 31
   usage_list:
     - src
     - doc
 
 - name: Github Old Token
   severity: high
   type: pattern
@@ -123,15 +123,15 @@
     - src
     - doc
 
 - name: Google API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>AIza[0-9A-Za-z\-_]{35})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>AIza[0-9A-Za-z_-]{35})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - GoogleApiKeyValidation
   required_substrings:
     - AIza
   min_line_len: 39
@@ -140,15 +140,15 @@
     - doc
 
 - name: Google Multi
   severity: high
   type: pattern
   values:
     - (?P<value>[0-9]+\-[0-9A-Za-z_]{32}\.apps\.googleusercontent\.com)
-    - (?<![0-9a-zA-Z_-])(?P<value>[0-9a-zA-Z_-]{24})([^0-9A-Za-z]|$)
+    - (?<![0-9a-zA-Z_-])(?P<value>[0-9a-zA-Z_-]{24})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - GoogleMultiValidation
   required_substrings:
     - .apps.googleusercontent.com
   min_line_len: 40
@@ -156,29 +156,29 @@
     - src
     - doc
 
 - name: Google OAuth Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ya29\.[0-9A-Za-z\-_]+)
+    - (^|[^0-9A-Za-z])(?P<value>ya29\.[0-9A-Za-z_-]{22,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - ya29.
-  min_line_len: 6
+  min_line_len: 27
   usage_list:
     - src
     - doc
 
 - name: Heroku API Key
   severity: high
   type: pattern
   values:
-    - (?P<value>(?i)heroku(.{0,20})?[0-9a-f]{8}(-[0-9a-f]{4})+-[0-9a-f]{12})
+    - (?P<value>(?i)heroku(.{0,20})?[0-9a-f]{8}(-[0-9a-f]{4})+-[0-9a-f]{12})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - heroku
   min_line_len: 24
   usage_list:
     - src
@@ -198,29 +198,29 @@
     - src
     - doc
 
 - name: JSON Web Token
   severity: medium
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>eyJ[A-Za-z0-9-_=]+(\.[A-Za-z0-9-_.+\/=]+)?)
+    - (^|[^0-9A-Za-z])(?P<value>eyJ[A-Za-z0-9=_-]{13,}(\.[A-Za-z0-9-_.+\/=]+)?)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - eyJ
-  min_line_len: 9
+  min_line_len: 16
   usage_list:
     - src
     - doc
 
 - name: MailChimp API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>[0-9a-zA-Z]{32}-us[0-9]{1,2})
+    - (^|[^0-9A-Za-z])(?P<value>[0-9a-zA-Z]{32}-us[0-9]{1,2})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - MailChimpKeyValidation
   required_substrings:
     - -us
   min_line_len: 35
@@ -228,15 +228,15 @@
     - src
     - doc
 
 - name: MailGun API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>key-[0-9a-zA-Z]{32})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>key-[0-9a-zA-Z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - key-
   min_line_len: 36
   usage_list:
     - src
@@ -256,15 +256,15 @@
   usage_list:
     - src
 
 - name: PayPal Braintree Access Token
   severity: high
   type: pattern
   values:
-    - (?P<value>access_token\$production\$[0-9a-z]{16}\$[0-9a-z]{32})
+    - (?P<value>access_token\$production\$[0-9a-z]{16}\$[0-9a-z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   required_substrings:
     - access_token$production$
   min_line_len: 72
   usage_list:
     - src
@@ -281,15 +281,15 @@
   usage_list:
     - src
 
 - name: Picatic API Key
   severity: high
   type: pattern
   values:
-    - (?P<value>sk_live_[0-9a-z]{32})
+    - (?P<value>sk_live_[0-9a-z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   required_substrings:
     - sk_live_
   min_line_len: 40
   usage_list:
     - src
@@ -322,15 +322,15 @@
     - src
     - doc
 
 - name: Shopify Token
   severity: high
   type: pattern
   values:
-    - (?P<value>shp(at|ca|pa|ss)_[a-fA-F0-9]{32})
+    - (?P<value>shp(at|ca|pa|ss)_[a-fA-F0-9]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   required_substrings:
     - shp
   min_line_len: 38
   usage_list:
     - src
     - doc
@@ -365,15 +365,15 @@
     - src
     - doc
 
 - name: Stripe Standard API Key
   severity: high
   type: pattern
   values:
-    - (?P<value>sk_live_[0-9a-zA-Z]{24})
+    - (?P<value>sk_live_[0-9a-zA-Z]{24})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - StripeApiKeyValidation
   required_substrings:
     - sk_live_
   min_line_len: 32
@@ -381,29 +381,29 @@
     - src
     - doc
 
 - name: Stripe Restricted API Key
   severity: high
   type: pattern
   values:
-    - (?P<value>rk_live_[0-9a-zA-Z]{24})
+    - (?P<value>rk_live_[0-9a-zA-Z]{24})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - rk_live_
   min_line_len: 32
   usage_list:
     - src
     - doc
 
 - name: Square Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>EAAA[0-9A-Za-z\-_]{60})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>EAAA[0-9A-Za-z_-]{60})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SquareAccessTokenValidation
   required_substrings:
     - EAAA
   min_line_len: 64
@@ -411,15 +411,15 @@
     - src
     - doc
 
 - name: Square Client ID
   severity: medium
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>sq0[a-z]{3}-[0-9A-Za-z\-_]{22})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>sq0[a-z]{3}-[0-9A-Za-z_-]{22})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SquareClientIdValidation
   required_substrings:
     - sq0
   min_line_len: 29
@@ -427,15 +427,15 @@
     - src
     - doc
 
 - name: Square OAuth Secret
   severity: high
   type: pattern
   values:
-    - (?P<value>sq0csp-[0-9A-Za-z\-_]{43})
+    - (?P<value>sq0csp-[0-9A-Za-z_-]{43})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   required_substrings:
     - sq0csp
   min_line_len: 50
   usage_list:
     - src
@@ -454,15 +454,15 @@
   usage_list:
     - src
 
 - name: Twilio API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>SK[0-9a-fA-F]{32})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>SK[0-9a-fA-F]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - SK
   min_line_len: 34
   usage_list:
     - src
@@ -508,15 +508,15 @@
   usage_list:
     - src
 
 - name: Telegram Bot API Token
   severity: high
   type: pattern
   values:
-    - (?P<value>[0-9]{8,10}:[0-9A-Za-z_-]{35})
+    - (?P<value>[0-9]{8,10}:[0-9A-Za-z_-]{35})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   required_substrings:
     - :AA
   min_line_len: 45
   usage_list:
     - src
     - doc
@@ -657,257 +657,301 @@
     - src
     - doc
 
 - name: Azure Secret Value
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_~.-]{3}8Q~[a-zA-Z0-9_~.-]{34})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_~.-]{3}8Q~[a-zA-Z0-9_~.-]{34})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 40
   required_substrings:
     - 8Q~
   usage_list:
     - src
     - doc
 
 - name: Bitbucket App Password
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ATBB[A-Za-z0-9]{24}[A-F0-9]{8})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>ATBB[A-Za-z0-9]{24}[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 28
   required_substrings:
     - ATBB
   usage_list:
     - src
     - doc
 
 - name: Bitbucket Repository Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ATCTT3xFfGN0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>ATCTT3xFfGN0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 183
   required_substrings:
     - ATCTT3xFfGN0
   usage_list:
     - src
     - doc
 
 - name: Bitbucket HTTP Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>BBDC-[NMO][ADgjQTwz][A-Za-z0-9+/]{42})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>BBDC-[NMO][ADgjQTwz][A-Za-z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 49
   required_substrings:
     - BBDC-
   usage_list:
     - src
     - doc
 
+- name: Bitbucket Client ID
+  severity: info
+  type: pattern
+  values:
+    - (^|[^0-9A-Za-z.$_/+-])(?P<value>[a-zA-Z0-9]{18}([a-zA-Z0-9]{14})?)([^0-9A-Za-z.$_/+-]|$)
+  filter_type: WeirdBase64Token
+  min_line_len: 18
+  usage_list:
+    - src
+    - doc
+
+- name: Bitbucket Client Secret
+  severity: info
+  type: pattern
+  values:
+    - (^|[^0-9A-Za-z.$_/+-])(?P<value>([a-zA-Z0-9_-]{32}){1,2})([^0-9A-Za-z.$_/+-]|$)
+  filter_type: WeirdBase64Token
+  min_line_len: 32
+  usage_list:
+    - src
+    - doc
+
 - name: Jira / Confluence PAT token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z+/-])(?P<value>[NMO][ADgjQTwz][a-zA-Z0-9+/]{42})([^0-9A-Za-z+/-]|$)
+    - (^|[^0-9A-Za-z+/-])(?P<value>[NMO][ADgjQTwz][a-zA-Z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 44
   required_substrings:
     - M
     - N
     - O
   usage_list:
     - src
     - doc
 
+- name: Atlassian Old PAT token
+  severity: info
+  type: pattern
+  values:
+    - (^|[^0-9A-Za-z.$_/+-])(?P<value>[a-zA-Z0-9]{24})([^=0-9A-Za-z.$_/+-]|$)
+  filter_type: WeirdBase64Token
+  min_line_len: 24
+  usage_list:
+    - src
+    - doc
+
 - name: Atlassian PAT token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ATATT3xFfGF0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>ATATT3xFfGF0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 191
   required_substrings:
     - ATATT3xFfGF0
   usage_list:
     - src
     - doc
 
 - name: Digital Ocean PAT
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>dop_v1_[a-f0-9]{64})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>dop_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 71
   required_substrings:
     - dop_v1_
   usage_list:
     - src
     - doc
 
 - name: Digital Ocean OAuth Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>doo_v1_[a-f0-9]{64})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>doo_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 71
   required_substrings:
     - doo_v1_
   usage_list:
     - src
     - doc
 
 - name: Dropbox OAuth2 API Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>sl.[A-Za-z0-9_-]{135})([^0-9A-Za-z]|$)
+    - (^|[^0-9A-Za-z])(?P<value>sl.[A-Za-z0-9_-]{135})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 138
   required_substrings:
     - sl.
   usage_list:
     - src
     - doc
 
 - name: NuGet API key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>oy2[a-z0-9]{43})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>oy2[a-z0-9]{43})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 46
   required_substrings:
     - oy2
   usage_list:
     - src
     - doc
 
 - name: Gitlab PAT
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glpat-[a-zA-Z0-9_-]{20})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>glpat-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 26
   required_substrings:
     - glpat-
   usage_list:
     - src
     - doc
 
 - name: Gitlab Pipeline Trigger Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glptt-[a-f0-9]{40})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>glptt-[a-f0-9]{40})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 46
   required_substrings:
     - glptt-
   usage_list:
     - src
     - doc
 
 - name: Gitlab Registration Runner Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>GR1348941[a-zA-Z0-9_-]{20})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>GR1348941[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 29
   required_substrings:
     - GR1348941
   usage_list:
     - src
     - doc
 
 - name: Gitlab Registration Runner Token 2023
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glrt-[a-zA-Z0-9_-]{20})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>glrt-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 25
   required_substrings:
     - glrt-
   usage_list:
     - src
     - doc
 
 - name: Grafana Provisioned API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>eyJ[a-zA-Z0-9=/-]{64,360})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>eyJ[a-zA-Z0-9=/-]{64,360})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueGrafanaCheck
   min_line_len: 67
   required_substrings:
     - eyJ
   usage_list:
     - src
     - doc
 
 - name: Grafana Access Policy Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glc_eyJ[a-zA-Z0-9=/-]{80,360})([^0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>glc_eyJ[a-zA-Z0-9=/-]{80,360})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueGrafanaCheck
   min_line_len: 87
   required_substrings:
     - glc_eyJ
   usage_list:
     - src
     - doc
 
 - name: Dropbox API secret (long term)
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?=[A-Za-z0-9]{64})(?P<value>[A-Za-z0-9]{10,12}[B-Za-z0-9]A{10,12}[B-Za-z0-9][A-Za-z0-9]{40,44})([^0-9A-Za-z_/-]|$)
+    - (^|[^0-9A-Za-z])(?=[A-Za-z0-9]{64})(?P<value>[A-Za-z0-9]{10,12}[B-Za-z0-9]A{10,12}[B-Za-z0-9][A-Za-z0-9]{40,44})([^=0-9A-Za-z_/+-]|$)
   filter_type: []
   min_line_len: 43
   required_substrings:
     - AAAAAAAAAA
   usage_list:
     - src
     - doc
 
 - name: Dropbox App secret
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>[a-z0-9]{15})([^=0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z_/+-])(?P<value>[a-z0-9]{15})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 15
   usage_list:
     - src
     - doc
 
 - name: Gitlab Incoming Email Token
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z._/+-])(?P<value>[a-z0-9]{24,25})([^=0-9A-Za-z+/_-]|$)
+    - (^|[^0-9A-Za-z._/+-])(?P<value>[a-z0-9]{24,25})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 24
   usage_list:
     - src
     - doc
 
+- name: Gitlab Feed Token
+  severity: info
+  type: pattern
+  values:
+    - (^|[^0-9A-Za-z._/+-])(?P<value>[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
+  filter_type: WeirdBase64Token
+  min_line_len: 20
+  usage_list:
+    - src
+    - doc
+
 - name: Jira 2FA
   severity: info
   type: pattern
   values:
     - (^|[^0-9A-Za-z_/+-])(?P<value>[A-Z2-7]{16})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueCoupleKeywordCheck
```

### Comparing `credsweeper-1.5.0/credsweeper/rules/rule.py` & `credsweeper-1.5.1/credsweeper/rules/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,20 +44,20 @@
     # mandatory fields
     NAME = "name"
     SEVERITY = "severity"
     TYPE = "type"
     USAGE_LIST = "usage_list"
     VALUES = "values"
     FILTER_TYPE = "filter_type"
+    MIN_LINE_LEN = "min_line_len"
 
     # auxiliary fields
     USE_ML = "use_ml"
     REQUIRED_SUBSTRINGS = "required_substrings"
     VALIDATIONS = "validations"
-    MIN_LINE_LEN = "min_line_len"
 
     def __init__(self, config: Config, rule_dict: Dict) -> None:
         self.config = config
         self._assert_rule_mandatory_fields(rule_dict)
         # mandatory fields
         self.__rule_name = str(rule_dict[Rule.NAME])
         if severity := Severity.get(rule_dict[Rule.SEVERITY]):
@@ -238,15 +238,17 @@
         Args:
             rule_template: dictionary loaded from the config file
 
         Raises:
             ValueError if missing fields is present
 
         """
-        mandatory_fields = [Rule.NAME, Rule.SEVERITY, Rule.TYPE, Rule.USAGE_LIST, Rule.VALUES, Rule.FILTER_TYPE]
+        mandatory_fields = [
+            Rule.NAME, Rule.SEVERITY, Rule.TYPE, Rule.USAGE_LIST, Rule.VALUES, Rule.FILTER_TYPE, Rule.MIN_LINE_LEN
+        ]
         missing_fields = [field for field in mandatory_fields if field not in rule_template]
         if len(missing_fields) > 0:
             raise ValueError(f"Malformed rule config file. Contain rule with missing fields: {missing_fields}.")
 
     @cached_property
     def required_substrings(self) -> List[str]:
         """required_substrings getter"""
```

### Comparing `credsweeper-1.5.0/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.5.1/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.5.1/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.5.1/credsweeper/scanner/scan_type/scan_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,33 +33,34 @@
             Candidate object if pattern defined in a rule is present in a line and filters defined in rule do not
             remove current line. None otherwise
 
         """
         raise NotImplementedError()
 
     @classmethod
-    def filtering(cls, config: Config, line_data: LineData, filters: List[Filter]) -> bool:
+    def filtering(cls, config: Config, target: AnalysisTarget, line_data: LineData, filters: List[Filter]) -> bool:
         """Check if line data should be removed based on filters.
 
         If `use_filters` option is false, always return False
 
         Args:
             config: dict of credsweeper configuration
-            line_data: Line data to check with filters
+            target: AnalysisTarget from which `line_data` was obtained
+            line_data: Line data to check with `filters`
             filters: Filters to use
 
         Return:
             boolean: True if line_data should be removed. False otherwise.
             If `use_filters` option is false, always return False
 
         """
         if not config.use_filters:
             return False
         for filter_ in filters:
-            if filter_.run(line_data):
+            if filter_.run(line_data, target):
                 logger.debug("Filtered line with filter: %s in file: %s:%d  in line: %s", filter_.__class__.__name__,
                              line_data.path, line_data.line_num, line_data.line)
                 return True
         return False
 
     @classmethod
     def get_line_data(
@@ -83,15 +84,15 @@
         if not cls.is_pattern_detected_line(target.line, pattern):
             return None
         logger.debug("Valid line for pattern: %s in file: %s:%d in line: %s", pattern, target.file_path,
                      target.line_num, target.line)
         line_data = LineData(config, target.line, target.line_num, target.file_path, target.file_type, target.info,
                              pattern)
 
-        if cls.filtering(config, line_data, filters):
+        if cls.filtering(config, target, line_data, filters):
             return None
         return line_data
 
     @classmethod
     def is_pattern_detected_line(cls, line: str, pattern: re.Pattern) -> bool:
         """Check if pattern present in the line.
```

### Comparing `credsweeper-1.5.0/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.5.1/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/scanner/scanner.py` & `credsweeper-1.5.1/credsweeper/scanner/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,16 @@
         """
         keyword_targets = []
         pattern_targets = []
         pem_targets = []
 
         for target in targets:
             # Ignore target if it's too long
-            line_len = len(target.line)
-            if line_len > MAX_LINE_LENGTH:
-                logger.warning(f"Skipped oversize({line_len}) line in {target.file_path}:{target.line_num}", )
+            if target.line_len > MAX_LINE_LENGTH:
+                logger.warning(f"Skipped oversize({target.line_len}) line in {target.file_path}:{target.line_num}", )
                 continue
             # Trim string from outer spaces to make future `a in str` checks faster
             target_line_trimmed = target.line.strip()
             target_line_trimmed_len = len(target_line_trimmed)
             # Ignore target if trimmed part is too short
             if target_line_trimmed_len < self.min_len:
                 continue
```

### Comparing `credsweeper-1.5.0/credsweeper/secret/config.json` & `credsweeper-1.5.1/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/secret/log.yaml` & `credsweeper-1.5.1/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/utils/util.py` & `credsweeper-1.5.1/credsweeper/utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "old": Optional[int],  #
         "new": Optional[int],  #
         "line": Union[str, bytes],  # bytes are possibly since whatthepatch v1.0.4
         "hunk": Any  # not used
     })
 
 
-@dataclass
+@dataclass(frozen=True)
 class DiffRowData:
     """Class for keeping data of diff row."""
 
     line_type: DiffRowType
     line_numb: int
     line: str
```

### Comparing `credsweeper-1.5.0/credsweeper/validations/__init__.py` & `credsweeper-1.5.1/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/apply_validation.py` & `credsweeper-1.5.1/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/github_token_validation.py` & `credsweeper-1.5.1/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.5.1/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.5.1/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.5.1/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.5.1/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.5.1/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.5.1/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.5.1/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper/validations/validation.py` & `credsweeper-1.5.1/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/credsweeper.egg-info/PKG-INFO` & `credsweeper-1.5.1/credsweeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.0
+Version: 1.5.1
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.0/credsweeper.egg-info/SOURCES.txt` & `credsweeper-1.5.1/credsweeper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,52 +56,57 @@
 credsweeper/filters/cred_card_number_check.py
 credsweeper/filters/filter.py
 credsweeper/filters/line_specific_key_check.py
 credsweeper/filters/separator_unusual_check.py
 credsweeper/filters/value_allowlist_check.py
 credsweeper/filters/value_array_dictionary_check.py
 credsweeper/filters/value_base32_data_check.py
+credsweeper/filters/value_base64_data_check.py
 credsweeper/filters/value_blocklist_check.py
 credsweeper/filters/value_camel_case_check.py
 credsweeper/filters/value_couple_keyword_check.py
 credsweeper/filters/value_dictionary_keyword_check.py
 credsweeper/filters/value_dictionary_value_length_check.py
 credsweeper/filters/value_entropy_base32_check.py
 credsweeper/filters/value_entropy_base36_check.py
+credsweeper/filters/value_entropy_base64_check.py
 credsweeper/filters/value_entropy_check.py
 credsweeper/filters/value_file_path_check.py
 credsweeper/filters/value_first_word_check.py
 credsweeper/filters/value_grafana_check.py
 credsweeper/filters/value_json_web_token_check.py
 credsweeper/filters/value_last_word_check.py
 credsweeper/filters/value_length_check.py
 credsweeper/filters/value_method_check.py
 credsweeper/filters/value_not_allowed_pattern_check.py
+credsweeper/filters/value_not_part_encoded_check.py
 credsweeper/filters/value_number_check.py
 credsweeper/filters/value_pattern_check.py
 credsweeper/filters/value_pattern_length_check.py
 credsweeper/filters/value_pem_pattern_check.py
 credsweeper/filters/value_similarity_check.py
 credsweeper/filters/value_split_keyword_check.py
 credsweeper/filters/value_string_type_check.py
 credsweeper/filters/value_structured_token_check.py
 credsweeper/filters/value_token_base32_check.py
 credsweeper/filters/value_token_base36_check.py
+credsweeper/filters/value_token_base64_check.py
 credsweeper/filters/value_token_check.py
 credsweeper/filters/value_useless_word_check.py
 credsweeper/filters/variable_not_allowed_pattern_check.py
 credsweeper/filters/group/__init__.py
 credsweeper/filters/group/general_keyword.py
 credsweeper/filters/group/general_pattern.py
 credsweeper/filters/group/group.py
 credsweeper/filters/group/password_keyword.py
 credsweeper/filters/group/structured_token.py
 credsweeper/filters/group/token_pattern.py
 credsweeper/filters/group/url_credentials_group.py
 credsweeper/filters/group/weird_base36_token.py
+credsweeper/filters/group/weird_base64_token.py
 credsweeper/logger/__init__.py
 credsweeper/logger/logger.py
 credsweeper/ml_model/__init__.py
 credsweeper/ml_model/features.py
 credsweeper/ml_model/ml_model.onnx
 credsweeper/ml_model/ml_validator.py
 credsweeper/ml_model/model_config.json
```

### Comparing `credsweeper-1.5.0/setup.py` & `credsweeper-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.0/tests/test_app.py` & `credsweeper-1.5.1/tests/test_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import subprocess
 import sys
 import tempfile
 import time
 from typing import AnyStr, Tuple
 from unittest import TestCase
 
+import deepdiff
 import pytest
 
 from credsweeper.app import APP_PATH
 from credsweeper.utils import Util
-from tests import AZ_STRING, SAMPLES_FILTERED_BY_POST_COUNT, SAMPLES_POST_CRED_COUNT, SAMPLES_IN_DEEP_3, SAMPLES_PATH, \
+from tests import AZ_STRING, SAMPLES_POST_CRED_COUNT, SAMPLES_IN_DEEP_3, SAMPLES_PATH, \
     TESTS_PATH, SAMPLES_CRED_COUNT
 
 
 class TestApp(TestCase):
 
     @staticmethod
     def _m_credsweeper(args) -> Tuple[str, str]:
@@ -170,18 +171,18 @@
             ["--path", target_path, "--ml_threshold", "0", "--api_validation", "--log", "silence"], )
         output = " ".join(_stdout.split()[:-1])
 
         expected = f"""
                     rule: Google API Key
                     / severity: high
                     / line_data_list:
-                    [line: 'AIzaGiReoGiCrackleCrackle12315618112315'
+                    [line: 'AIzaGiReoG-CrackleCrackle12315618_12315'
                         / line_num: 1
                         / path: {target_path}
-                        / value: 'AIzaGiReoGiCrackleCrackle12315618112315'
+                        / value: 'AIzaGiReoG-CrackleCrackle12315618_12315'
                         / entropy_validation: True]
                     / api_validation: INVALID_KEY
                     / ml_validation: NOT_AVAILABLE\n
                     Detected Credentials: 1\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
@@ -212,14 +213,15 @@
                    " [--ml_threshold FLOAT_OR_STR]" \
                    " [--ml_batch_size POSITIVE_INT]" \
                    " [--api_validation]" \
                    " [--jobs POSITIVE_INT]" \
                    " [--skip_ignored]" \
                    " [--save-json [PATH]]" \
                    " [--save-xlsx [PATH]]" \
+                   " [--sort]" \
                    " [--log LOG_LEVEL]" \
                    " [--size_limit SIZE_LIMIT]" \
                    " [--banner] " \
                    " [--version] " \
                    "python -m credsweeper: error: one of the arguments" \
                    " --path" \
                    " --diff_path" \
@@ -467,25 +469,44 @@
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
                 self.assertEqual(0, len(report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_p(self) -> None:
+        normal_report = []
+        sorted_report = []
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             # depth = 3
             _stdout, _stderr = self._m_credsweeper(
                 ["--log", "silence", "--path",
                  str(SAMPLES_PATH), "--save-json", json_filename, "--depth", "3"])
             self.assertTrue(os.path.exists(json_filename))
             with open(json_filename, "r") as json_file:
-                report = json.load(json_file)
-                self.assertEqual(SAMPLES_POST_CRED_COUNT + SAMPLES_IN_DEEP_3 - SAMPLES_FILTERED_BY_POST_COUNT,
-                                 len(report))
+                normal_report.extend(json.load(json_file))
+                self.assertEqual(SAMPLES_IN_DEEP_3, len(normal_report))
+            sorted_json_filename = os.path.join(tmp_dir, f"{__name__}.json")
+            _stdout, _stderr = self._m_credsweeper([
+                "--log", "silence", "--path",
+                str(SAMPLES_PATH), "--sort", "--save-json", sorted_json_filename, "--depth", "3"
+            ])
+            self.assertTrue(os.path.exists(sorted_json_filename))
+            with open(sorted_json_filename, "r") as json_file:
+                sorted_report.extend(json.load(json_file))
+                self.assertEqual(SAMPLES_IN_DEEP_3, len(sorted_report))
+        self.assertTrue(deepdiff.DeepDiff(sorted_report, normal_report))
+        # exclude equal items of dict instead custom __lt__ realization
+        for n in range(len(normal_report) - 1, -1, -1):
+            for i in sorted_report:
+                if i == normal_report[n]:
+                    del normal_report[n]
+                    break
+        # 0 - means all items were matched
+        self.assertEqual(0, len(normal_report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_n(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             # depth is not set
```

### Comparing `credsweeper-1.5.0/tests/test_main.py` & `credsweeper-1.5.1/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 from credsweeper.common.constants import ThresholdPreset, Severity
 from credsweeper.credentials import Candidate
 from credsweeper.file_handler.files_provider import FilesProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
 from credsweeper.file_handler.text_provider import TextProvider
 from credsweeper.utils import Util
 from tests import SAMPLES_CRED_COUNT, SAMPLES_CRED_LINE_COUNT, SAMPLES_POST_CRED_COUNT, SAMPLES_PATH, AZ_STRING, \
-    TESTS_PATH, SAMPLES_IN_DEEP_1, SAMPLES_FILTERED_BY_POST_COUNT, SAMPLES_IN_DEEP_3, SAMPLES_IN_DEEP_2, \
+    TESTS_PATH, SAMPLES_IN_DEEP_1, SAMPLES_IN_DEEP_3, SAMPLES_IN_DEEP_2, \
     SAMPLES_FILES_COUNT
+from tests.data import DATA_TEST_CFG
 
 
 class TestMain(unittest.TestCase):
 
     def test_ml_validation_p(self) -> None:
         cred_sweeper = CredSweeper()
         self.assertEqual(ThresholdPreset.medium, cred_sweeper.ml_threshold)
@@ -184,14 +185,15 @@
         with tempfile.TemporaryDirectory() as tmp_dir:
             args_mock = Mock(log='warning',
                              path=None,
                              config_path=None,
                              diff_path=[str(target_path)],
                              json_filename=os.path.join(tmp_dir, f"{__name__}.json"),
                              xlsx_filename=None,
+                             sort_output=False,
                              rule_path=None,
                              jobs=1,
                              ml_threshold=0.0,
                              depth=9,
                              doc=False,
                              size_limit="1G",
                              api_validation=False,
@@ -231,14 +233,15 @@
             xlsx_filename = os.path.join(tmp_dir, "report.xlsx")
             args_mock = Mock(log='warning',
                              config_path=None,
                              path=[str(SAMPLES_PATH)],
                              diff_path=None,
                              json_filename=json_filename,
                              xlsx_filename=xlsx_filename,
+                             sort_output=True,
                              rule_path=None,
                              jobs=1,
                              ml_threshold=0.0,
                              depth=0,
                              doc=False,
                              size_limit="1G",
                              find_by_ext=False,
@@ -435,25 +438,22 @@
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_p(self) -> None:
         # test for finding files with --depth
         content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
         cred_sweeper = CredSweeper(depth=1)
         cred_sweeper.run(content_provider=content_provider)
-        self.assertEqual(SAMPLES_POST_CRED_COUNT + SAMPLES_IN_DEEP_1 - SAMPLES_FILTERED_BY_POST_COUNT,
-                         len(cred_sweeper.credential_manager.get_credentials()))
+        self.assertEqual(SAMPLES_IN_DEEP_1, len(cred_sweeper.credential_manager.get_credentials()))
         cred_sweeper.config.depth = 3
         cred_sweeper.run(content_provider=content_provider)
-        self.assertEqual(SAMPLES_POST_CRED_COUNT + SAMPLES_IN_DEEP_3 - SAMPLES_FILTERED_BY_POST_COUNT,
-                         len(cred_sweeper.credential_manager.get_credentials()))
+        self.assertEqual(SAMPLES_IN_DEEP_3, len(cred_sweeper.credential_manager.get_credentials()))
 
         cred_sweeper.config.depth = 2
         cred_sweeper.run(content_provider=content_provider)
-        self.assertEqual(SAMPLES_POST_CRED_COUNT + SAMPLES_IN_DEEP_2 - SAMPLES_FILTERED_BY_POST_COUNT,
-                         len(cred_sweeper.credential_manager.get_credentials()))
+        self.assertEqual(SAMPLES_IN_DEEP_2, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_n(self) -> None:
         content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
         cred_sweeper = CredSweeper(depth=0)
         cred_sweeper.run(content_provider=content_provider)
@@ -613,15 +613,15 @@
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         expected_credential_lines = [
             "508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0",
             'secret = "Ndjbwu88s22ygavsdhgt5454v3h1x"',
             'password = "Cr3DeHTbIal"',
             'password = "0dm1nk0"',
             '"password" = "p@$$w0Rd42"',
-            'secret = "BNbNbws73bdhss329ssakKhds1203843"',
+            'secret = "BNbNbws73bdhss329ssakKhds120384"',
             '"token" = "H72gsdv2dswPneHduwhfd"',
         ]
         self.assertEqual(len(expected_credential_lines), len(found_credentials))
         for cred in found_credentials:
             self.assertEqual(1, len(cred.line_data_list))
             self.assertIn(cred.line_data_list[0].line, expected_credential_lines)
             expected_credential_lines.remove(cred.line_data_list[0].line)
@@ -748,21 +748,20 @@
                 k["severity"],
                 k["ml_probability"],
             ))
 
         # do not use parametrised tests with unittests
         self.maxDiff = 65536
         # instead the config file is used
-        with open(TESTS_PATH / "data" / ".cfg.json", "r") as f:
-            config = json.load(f)
         with tempfile.TemporaryDirectory() as tmp_dir:
-            for cfg in config:
-                # important key in .cfg.json is "json_filename"
+            for cfg in DATA_TEST_CFG:
                 with open(TESTS_PATH / "data" / cfg["json_filename"], "r") as f:
                     expected_result = json.load(f)
+                # informative parameter, relative with other tests counters. CredSweeper does not know it and fails
+                cred_count = cfg.pop("__cred_count")
                 prepare(expected_result)
                 tmp_file = Path(tmp_dir) / cfg["json_filename"]
                 # apply the current path to keep equivalence in path
                 os.chdir(TESTS_PATH.parent)
                 content_provider: FilesProvider = TextProvider(["tests/samples"])
                 # replace output report file to place in tmp_dir
                 cfg["json_filename"] = str(tmp_file)
@@ -773,14 +772,15 @@
                 prepare(test_result)
 
                 diff = deepdiff.DeepDiff(test_result, expected_result)
                 if diff:
                     # prints produced report to compare with present data in tests/data
                     print(f"\nThe produced report for {cfg['json_filename']}:\n{json.dumps(test_result)}", flush=True)
                 self.assertDictEqual({}, diff, cfg)
+                self.assertEqual(cred_count, len(expected_result), cfg["json_filename"])
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     @pytest.mark.skipif(not os.getenv("BRUTEFORCEMAXEXTENSION4ML"),
                         reason="run the test only for renaming samples with maximal ml_probability")
     def test_samples_ml_p(self) -> None:
         extensions = [
```

