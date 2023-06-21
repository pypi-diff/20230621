# Comparing `tmp/regula.documentreader.webclient-6.8.1.tar.gz` & `tmp/regula.documentreader.webclient-6.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regula.documentreader.webclient-6.8.1.tar", last modified: Wed May 24 12:09:57 2023, max compression
+gzip compressed data, was "regula.documentreader.webclient-6.8.3.tar", last modified: Wed Jun 21 14:18:58 2023, max compression
```

## Comparing `regula.documentreader.webclient-6.8.1.tar` & `regula.documentreader.webclient-6.8.3.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.971589 regula.documentreader.webclient-6.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-24 12:09:57.971589 regula.documentreader.webclient-6.8.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula/documentreader/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/
--rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/api/document_reader_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/fiber.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/ident.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/image_ident.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/ocr_security_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/security_feature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/images.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/raw_result_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/recognition_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2987 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/recognition_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/text_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.955588 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12356 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.955588 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5872 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api/process_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26739 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16380 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4944 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.971589 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11546 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/area_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/area_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_check_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/bc_pdf417_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/bc_roidetect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/check_diagnose.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/chosen_document_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7627 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/chosen_document_type_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3719 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/container_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/critical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5477 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/data_module.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/details_optical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7940 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/details_rfid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_bar_code_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10823 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7661 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_image_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4049 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_image_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_position_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_position_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18666 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2847 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_type_recognition_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7743 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3691 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/fdsid_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/fiber_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/fiber_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9575 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphic_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphic_field_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3670 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphic_fields_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphics_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3582 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphics_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ident_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ident_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3451 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_check_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4648 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_available_source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5524 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10847 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_field_value.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9548 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/lcid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7915 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/lexical_analysis_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/license_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/license_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/light.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3484 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/list_verified_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/measure_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/mrz_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ocr_security_text_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11554 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/one_candidate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5388 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/original_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/p_array_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/parsing_notification_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/per_document_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/photo_ident_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/point_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/points_container.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55259 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_params_rfid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7804 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4983 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_request_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10150 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4385 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_system_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/processing_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/raw_image_container_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5908 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/rectangle_coordinates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7501 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/result_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2965 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/rfid_location.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5960 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/rfid_origin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/security_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/security_feature_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2816 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/source_validity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8033 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/status_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/status_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3987 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/string_recognition_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5455 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/symbol_candidate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5176 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/symbol_recognition_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7450 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5543 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_available_source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_data_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3740 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_data_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12342 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37483 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_field_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10245 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_post_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7066 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3394 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10687 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/tfdsid_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/transaction_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2905 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/verification_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10406 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/verified_field_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/visibility.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12496 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:09:57.951588 regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-24 12:09:57.000000 regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-24 12:09:57.000000 regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:09:57.000000 regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 12:09:57.000000 regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 12:09:57.000000 regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:09:57.971589 regula.documentreader.webclient-6.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 12:09:25.000000 regula.documentreader.webclient-6.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.409600 regula.documentreader.webclient-6.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-21 14:18:58.409600 regula.documentreader.webclient-6.8.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.389600 regula.documentreader.webclient-6.8.3/regula/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.389600 regula.documentreader.webclient-6.8.3/regula/documentreader/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.389600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.393600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.393600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/api/document_reader_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.393600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.393600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/fiber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/ident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/image_ident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/ocr_security_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/security_feature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/raw_result_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3132 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/recognition_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3114 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/recognition_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/text_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.393600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12356 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.393600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5872 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api/process_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26739 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16380 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4944 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.409600 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11546 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/area_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/area_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_check_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/bc_pdf417_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/bc_roidetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/check_diagnose.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/chosen_document_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7627 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/chosen_document_type_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3719 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/container_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/critical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5477 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/data_module.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/details_optical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7940 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/details_rfid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_bar_code_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10823 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7661 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_image_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4049 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_image_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_position_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_position_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18666 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2847 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_type_recognition_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7743 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3691 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/fdsid_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/fiber_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/fiber_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9575 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphic_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphic_field_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3670 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphic_fields_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphics_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3582 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphics_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ident_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ident_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3451 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_check_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4648 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_available_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5524 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10847 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_field_value.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9548 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/lcid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7915 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/lexical_analysis_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/license_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/license_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/light.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3484 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/list_verified_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/measure_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/mrz_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ocr_security_text_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11554 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/one_candidate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5388 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/original_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/p_array_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/parsing_notification_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/per_document_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/photo_ident_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/point_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/points_container.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55259 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_params_rfid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7804 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4983 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_request_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10150 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4385 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_system_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/processing_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/raw_image_container_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5908 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/rectangle_coordinates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7501 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/result_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2965 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/rfid_location.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5960 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/rfid_origin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3525 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/security_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/security_feature_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2816 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/source_validity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8033 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/status_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/status_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3987 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/string_recognition_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5455 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/symbol_candidate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5176 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/symbol_recognition_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7450 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5543 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_available_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_data_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3740 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_data_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12342 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37483 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_field_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10245 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_post_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7066 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3394 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10687 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/tfdsid_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/transaction_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2905 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/verification_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10406 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/verified_field_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/visibility.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12496 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:58.389600 regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-21 14:18:58.000000 regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-06-21 14:18:58.000000 regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:18:58.000000 regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:18:58.000000 regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 14:18:58.000000 regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:18:58.409600 regula.documentreader.webclient-6.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-21 14:18:25.000000 regula.documentreader.webclient-6.8.3/setup.py
```

### Comparing `regula.documentreader.webclient-6.8.1/PKG-INFO` & `regula.documentreader.webclient-6.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.documentreader.webclient
-Version: 6.8.1
+Version: 6.8.3
 Summary: Regula's Document Reader python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: document-reader-client,document reader,document recognition,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.documentreader.webclient-6.8.1/README.md` & `regula.documentreader.webclient-6.8.3/README.md`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/__init__.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/api/document_reader_api.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/api/document_reader_api.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/__init__.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/__init__.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/images.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/images.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/raw_result_item.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/raw_result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/recognition_request.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/recognition_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import base64
 from typing import List, Union
 
 from regula.documentreader.webclient import LicenseResult, EncryptedRCLResult, ContainerList, Result
 from regula.documentreader.webclient.gen.models import ImageData, ProcessParams
 from regula.documentreader.webclient.gen.models.process_request import ProcessRequest
 from regula.documentreader.webclient.gen.models.process_request_image import ProcessRequestImage
@@ -76,7 +77,11 @@
                 system_info=ProcessSystemInfo(), tag=tag
             )
         if container_list:
             super().__init__(
                 process_param=process_params, container_list=container_list,
                 system_info=ProcessSystemInfo(), tag=tag
             )
+
+    @property
+    def json(self) -> str:
+        return json.dumps(self.to_dict())
```

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/recognition_response.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/recognition_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import base64
+import json
 from typing import Optional, List
 from regula.documentreader.webclient import ImageQualityCheckList, OneCandidate
 from regula.documentreader.webclient.ext.models.authenticity.authenticity_check_list import AuthenticityCheckList
 from regula.documentreader.webclient.ext.models.images import Images
 from regula.documentreader.webclient.ext.models.text import Text
 from regula.documentreader.webclient.gen import ResultItem
 from regula.documentreader.webclient.gen.models.process_response import ProcessResponse
@@ -18,14 +20,18 @@
     def text(self) -> Optional[Text]:
         result = self.result_by_type(Result.TEXT)
         if result:
             return result.text
         return None
 
     @property
+    def json(self) -> str:
+        return json.dumps(self.low_lvl_response.to_dict())
+
+    @property
     def status(self) -> Optional[Status]:
         result = self.result_by_type(Result.STATUS)
         if result:
             return result.status
         return None
 
     @property
```

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/text.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/text.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/ext/models/text_field.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/ext/models/text_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/__init__.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api/default_api.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api/default_api.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api/process_api.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api/process_api.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/api_client.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/api_client.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/configuration.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/configuration.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/exceptions.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/exceptions.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/__init__.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/area_array.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/area_array.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/area_container.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/area_container.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_check_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_check_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_check_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_check_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/authenticity_result_type.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/authenticity_result_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/bc_pdf417_info.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/bc_pdf417_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/bc_roidetect.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/bc_roidetect.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/check_diagnose.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/check_diagnose.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/check_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/check_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/chosen_document_type.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/chosen_document_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/chosen_document_type_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/chosen_document_type_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/container_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/container_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/critical.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/critical.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/data_module.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/data_module.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/details_optical.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/details_optical.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/details_rfid.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/details_rfid.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/device_info.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/device_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_bar_code_info.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_bar_code_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_format.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_format.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_image.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_image.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_image_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_image_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_image_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_image_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_position.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_position.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_position_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_position_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_position_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_position_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_type.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_type_recognition_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_type_recognition_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/fdsid_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/fdsid_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/fiber_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/fiber_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/fiber_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/fiber_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphic_field.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphic_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphic_field_type.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphic_field_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphic_fields_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphic_fields_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphics_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphics_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/graphics_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/graphics_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ident_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ident_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ident_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ident_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_data.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_data.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_qa.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_qa.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_check.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_check.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_check_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_check_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_check_type.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_check_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_available_source.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_available_source.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_field.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_field_value.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_field_value.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/images_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/images_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/lcid.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/lcid.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/lexical_analysis_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/lexical_analysis_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/license_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/license_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/license_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/license_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/light.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/light.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/list_verified_fields.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/list_verified_fields.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/log_level.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/log_level.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/measure_system.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/measure_system.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/mrz_format.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/mrz_format.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ocr_security_text_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ocr_security_text_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/one_candidate.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/one_candidate.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/original_symbol.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/original_symbol.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/p_array_field.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/p_array_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/parsing_notification_codes.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/parsing_notification_codes.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/per_document_config.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/per_document_config.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/photo_ident_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/photo_ident_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/point.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/point.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/point_array.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/point_array.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/points_container.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/points_container.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_params.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_params.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_params_rfid.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_params_rfid.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_request.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_request.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_request_image.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_request_image.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_response.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_response.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/process_system_info.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/process_system_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/processing_status.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/processing_status.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/raw_image_container_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/raw_image_container_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/rectangle_coordinates.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/rectangle_coordinates.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/result_item.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/rfid_location.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/rfid_location.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/rfid_origin.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/rfid_origin.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/scenario.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
     MRZ_OR_BARCODE = "MrzOrBarcode"
 
     MRZ_OR_LOCATE = "MrzOrLocate"
 
     MRZ_AND_LOCATE = "MrzAndLocate"
 
+    BARCODE_AND_LOCATE = "BarcodeAndLocate"
+
     MRZ_OR_OCR = "MrzOrOcr"
 
     MRZ_OR_BARCODE_OR_OCR = "MrzOrBarcodeOrOcr"
 
     LOCATE_VISUAL_AND_MRZ_OR_OCR = "LocateVisual_And_MrzOrOcr"
 
     FULL_PROCESS = "FullProcess"
@@ -56,15 +58,15 @@
 
     OCR_FREE = "OcrFree"
 
     CREDIT_CARD = "CreditCard"
 
     CAPTURE = "Capture"
 
-    allowable_values = [MRZ, BARCODE, LOCATE, OCR, DOCTYPE, MRZ_OR_BARCODE, MRZ_OR_LOCATE, MRZ_AND_LOCATE, MRZ_OR_OCR, MRZ_OR_BARCODE_OR_OCR, LOCATE_VISUAL_AND_MRZ_OR_OCR, FULL_PROCESS, FULL_AUTH, ID3RUS, RUS_STAMP, OCR_FREE, CREDIT_CARD, CAPTURE]  # noqa: E501
+    allowable_values = [MRZ, BARCODE, LOCATE, OCR, DOCTYPE, MRZ_OR_BARCODE, MRZ_OR_LOCATE, MRZ_AND_LOCATE, BARCODE_AND_LOCATE, MRZ_OR_OCR, MRZ_OR_BARCODE_OR_OCR, LOCATE_VISUAL_AND_MRZ_OR_OCR, FULL_PROCESS, FULL_AUTH, ID3RUS, RUS_STAMP, OCR_FREE, CREDIT_CARD, CAPTURE]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/security_feature_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/security_feature_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/security_feature_type.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/security_feature_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/source.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/source.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/source_validity.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/source_validity.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/status.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/status.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/status_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/status_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/status_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/status_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/string_recognition_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/string_recognition_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/symbol_candidate.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/symbol_candidate.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/symbol_recognition_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/symbol_recognition_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_available_source.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_available_source.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_data_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_data_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_data_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_data_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_field.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_field_type.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_field_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_field_value.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_field_value.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_post_processing.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_post_processing.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/text_result_all_of.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/text_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/tfdsid_list.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/tfdsid_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/transaction_info.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/transaction_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/verification_result.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/verification_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/verified_field_map.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/verified_field_map.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/models/visibility.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/models/visibility.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula/documentreader/webclient/gen/rest.py` & `regula.documentreader.webclient-6.8.3/regula/documentreader/webclient/gen/rest.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/PKG-INFO` & `regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.documentreader.webclient
-Version: 6.8.1
+Version: 6.8.3
 Summary: Regula's Document Reader python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: document-reader-client,document reader,document recognition,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.documentreader.webclient-6.8.1/regula.documentreader.webclient.egg-info/SOURCES.txt` & `regula.documentreader.webclient-6.8.3/regula.documentreader.webclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.8.1/setup.py` & `regula.documentreader.webclient-6.8.3/setup.py`

 * *Files identical despite different names*

