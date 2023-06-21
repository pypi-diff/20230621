# Comparing `tmp/pdfservices-sdk-2.2.0.tar.gz` & `tmp/pdfservices-sdk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfservices-sdk-2.2.0.tar", last modified: Mon May 15 16:56:39 2023, max compression
+gzip compressed data, was "pdfservices-sdk-2.3.0.tar", last modified: Wed Jun 21 10:04:59 2023, max compression
```

## Comparing `pdfservices-sdk-2.2.0.tar` & `pdfservices-sdk-2.3.0.tar`

### file list

```diff
@@ -1,113 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.627454 pdfservices-sdk-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.627454 pdfservices-sdk-2.2.0/src/adobe/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.627454 pdfservices-sdk-2.2.0/src/adobe/pdfservices/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/service_account_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/client_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.631455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/platform_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/storage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/auth_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/session_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/request_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/service_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/request_header_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/response_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/path_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/validation_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/file_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.635455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-15 16:56:18.000000 pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:56:39.639455 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:56:39.000000 pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.262143 pdfservices-sdk-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-21 10:04:59.262143 pdfservices-sdk-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:04:59.262143 pdfservices-sdk-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.250143 pdfservices-sdk-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.250143 pdfservices-sdk-2.3.0/src/adobe/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.250143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.250143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.250143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/auth/service_account_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/auth/service_principal_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/client_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.250143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/exception/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.250143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.254143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.254143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.254143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.254143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.254143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.254143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.254143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/platform_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/storage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/auth_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/service_principal_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/session_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/constants/request_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/constants/service_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/request_header_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/response_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/internal_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/internal_execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/path_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/validation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/io/file_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.258143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.262143 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-21 10:04:41.000000 pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:04:59.262143 pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-21 10:04:59.000000 pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-21 10:04:59.000000 pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:04:59.000000 pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:04:59.000000 pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 10:04:59.000000 pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 10:04:59.000000 pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/top_level.txt
```

### Comparing `pdfservices-sdk-2.2.0/LICENSE.md` & `pdfservices-sdk-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/PKG-INFO` & `pdfservices-sdk-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfservices-sdk
-Version: 2.2.0
+Version: 2.3.0
 Summary: Adobe PDFServices Client Library
 Home-page: https://www.adobe.com/go/pdftoolsapi_doc
 Author: Adobe Document Services
 Author-email: extractapi@adobe.com
 License: Apache2
 Description: PDFServices Python SDK
         =======================
```

### Comparing `pdfservices-sdk-2.2.0/README.md` & `pdfservices-sdk-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/setup.py` & `pdfservices-sdk-2.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdfservices-sdk",
-    version="2.2.0",
+    version="2.3.0",
     author='Adobe Document Services',
     author_email='extractapi@adobe.com',
     license='Apache2',
     description="Adobe PDFServices Client Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.adobe.com/go/pdftoolsapi_doc",
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/auth/service_account_credentials.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/auth/service_account_credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,38 +9,32 @@
 # governing permissions and limitations under the License.
 import json
 import os
 from abc import ABC
 
 from adobe.pdfservices.operation.internal.constants.service_constants import ServiceConstants
 from adobe.pdfservices.operation.internal.util import path_util, file_utils
-from .credentials import Credentials
-from ..internal.util.validation_util import is_empty
-
-
-def _is_valid(value, name):
-    if is_empty(value):
-        raise ValueError(name + " must not be blank")
-    return value
+from .credentials import Credentials, _is_valid
 
 
 class ServiceAccountCredentials(Credentials, ABC):
     """
-    Service Account credentials allow your application to call PDF Tools Extract API on behalf of the application itself,
-    or on behalf of an enterprise organization. For getting the credentials,
-    `Click Here <https://www.adobe.com/go/pdfextractapi_requestform>`_.
-    """
+     Service Account credentials allow your application to call PDF Services API on behalf of the application itself,
+     or on behalf of an enterprise organization.
+
+     .. deprecated:: 2.3.0
+         Notice: JWT based service account credentials has been deprecated. Please use OAuth Server-to-Server based :class:`ServicePrincipalCredentials`.
+     """
 
-    # TODO Can this constructor be excluded from documentation
     def __init__(self, client_id, client_secret, private_key, organization_id, account_id):
-        self._client_id = _is_valid(client_id, "client_id")
-        self._client_secret = _is_valid(client_secret, "client_secret")
-        self._private_key = _is_valid(private_key, "private_key")
-        self._organization_id = _is_valid(organization_id, "organization_id")
-        self._account_id = _is_valid(account_id, "account_id")
+        self._client_id = _is_valid(client_id, 'client_id')
+        self._client_secret = _is_valid(client_secret, 'client_secret')
+        self._private_key = _is_valid(private_key, 'private_key')
+        self._organization_id = _is_valid(organization_id, 'organization_id')
+        self._account_id = _is_valid(account_id, 'account_id')
 
     @property
     def client_id(self):
         """ Client Id (API Key) """
         return self._client_id
 
     @property
@@ -51,15 +45,15 @@
     @property
     def private_key(self):
         """  Content of the Private Key (PEM format) """
         return self._private_key
 
     @property
     def organization_id(self):
-        """Identifies the organization(format: org_ident@AdobeOrg) that has been configured for access to PDF Tools API."""
+        """ Identifies the organization (format: org_ident@AdobeOrg) that has been configured for access to PDF Services API. """
         return self._organization_id
 
     @property
     def account_id(self):
         """Account ID(format: id@techacct.adobe.com)"""
         return self._account_id
 
@@ -120,15 +114,15 @@
             :return: This Builder instance to add any additional parameters.
             :rtype: ServiceAccountCredentials.Builder
             """
             self._private_key = private_key
             return self
 
         def with_organization_id(self, organization_id: str):
-            """ Set Organization Id (format: org_ident@AdobeOrg) that has been configured for access to PDF Tools API
+            """ Set Organization Id (format: org_ident@AdobeOrg) that has been configured for access to PDF Services API
 
             :param organization_id: Organization ID (format: org_ident@AdobeOrg)
             :type organization_id: str
             :return: This Builder instance to add any additional parameters.
             :rtype: ServiceAccountCredentials.Builder
             """
             self._organization_id = organization_id
@@ -194,12 +188,15 @@
             return self
 
         def build(self):
             """ Returns a new :class:`ServiceAccountCredentials` instance built from the current state of this builder.
 
             :return: A ServiceAccountCredentials instance.
             :rtype: ServiceAccountCredentials
+
+            .. deprecated:: 2.3.0
+                 Notice: JWT based service account credentials has been deprecated. Please use OAuth Server-to-Server based :class:`ServicePrincipalCredentials`.
             """
 
             from adobe.pdfservices.operation.internal.auth.service_account_credentials_with_uri import ServiceAccountCredentialsWithUri
             return ServiceAccountCredentialsWithUri(self._client_id, self._client_secret, self._private_key, self._organization_id, self._account_id,
                                              self._pdf_services_uri, self._ims_base_uri, self._claim)
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/client_config.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/client_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,8 @@
             """
             Returns a new :class:`ClientConfig` instance built from the current state of this builder.
 
             :return: A ClientConfig instance.
             :rtype: ClientConfig
             """
             from adobe.pdfservices.operation.internal.internal_client_config import InternalClientConfig
-            return InternalClientConfig(self._connect_timeout, self._read_timeout, self._pdf_services_uri)
+            return InternalClientConfig(self._connect_timeout, self._read_timeout, self._pdf_services_uri)
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/exception/exceptions.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/execution_context.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/execution_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     Sample Usage:
 
     .. code-block:: python
 
         try:
             base_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
-            credentials = Credentials.service_account_credentials_builder() \\
-                .from_file(base_path + "/pdfservices-api-credentials.json") \\
-                .build()
+            credentials = Credentials.service_principal_credentials_builder(). \
+                with_client_id(os.getenv('PDF_SERVICES_CLIENT_ID')). \
+                with_client_secret(os.getenv('PDF_SERVICES_CLIENT_SECRET')). \
+                build()
 
             execution_context = ExecutionContext.create(credentials)
             extract_pdf_operation = ExtractPDFOperation.create_new()
 
             source = FileRef.create_from_local_file(base_path + "/resources/extractPdfInput.pdf")
             extract_pdf_operation.set_input(source)
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/document.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/document.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/asset_upload_uri_request.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_output.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/autotagpdf/autotag_pdf_request.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/extract_pdf_request.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/engine.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/request/platform/platform_api_request.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/job_status.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/platform_api.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/platform_api.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/api/storage_api.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/auth_factory.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/auth_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,23 @@
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 from adobe.pdfservices.operation.auth.credentials import Credentials
 from adobe.pdfservices.operation.auth.service_account_credentials import ServiceAccountCredentials
+from adobe.pdfservices.operation.auth.service_principal_credentials import ServicePrincipalCredentials
 from adobe.pdfservices.operation.internal.auth.jwt_authenticator import JwtAuthenticator
+from adobe.pdfservices.operation.internal.auth.service_principal_authenticator import ServicePrincipalAuthenticator
+from adobe.pdfservices.operation.internal.internal_client_config import InternalClientConfig
 
 
 class AuthenticatorFactory:
 
     @staticmethod
-    def get_authenticator(credential: Credentials):
+    def get_authenticator(credential: Credentials, client_config: InternalClientConfig):
         if isinstance(credential, ServiceAccountCredentials):
             return JwtAuthenticator(credential)
+        elif isinstance(credential, ServicePrincipalCredentials):
+            return ServicePrincipalAuthenticator(credential, client_config)
         else:
             raise ValueError("Invalid Credentials provided as argument")
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/authenticator.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,33 +27,40 @@
 from adobe.pdfservices.operation.internal.constants.service_constants import ServiceConstants, custom_error_messages
 from adobe.pdfservices.operation.internal.http import http_client
 from adobe.pdfservices.operation.internal.http.http_method import HttpMethod
 from adobe.pdfservices.operation.internal.http.http_request import HttpRequest
 
 
 class JwtAuthenticator(Authenticator):
+    """
+        Authenticator for JWT based Service Account credentials
+    """
     token: SessionToken = None
     service_account_configuration: ServiceAccountCredentialsWithUri
     jwt_endpoint = ''
 
     def __init__(self, service_account_configuration):
         self.service_account_configuration = service_account_configuration
         self._logger = logging.getLogger(__name__)
         pass
 
     def session_token(self):
+        """ Access token for the PDF Services API """
         if self.token:
             if self.older_in_minute() <= 2:
                 return self.token
         return self.refresh_token()
 
     def older_in_minute(self):
+        """ Time remaining in minutes till token expiry """
         return int((datetime.now() - self.token.expired_at).seconds / 60)
 
     def refresh_token(self):
+        """ Refreshes the access token sent to PDF Services API """
+
         jwt_token = self._prepare_jwt()
         url = "{jwt_endpoint}/{jwt_uri_suffix}".format(
             jwt_endpoint=self.service_account_configuration.ims_base_uri,
             jwt_uri_suffix=ServiceConstants.JWT_URI_SUFFIX
         )
         access_token_request_payload = {"jwt_token": jwt_token,
                                         "client_id": self.service_account_configuration.client_id,
@@ -66,17 +73,20 @@
             content = json.loads(response.content)
             self.token = SessionToken(content['access_token'], content['expires_in'])
         except Exception:
             raise SdkException("Exception in fetching access token", sys.exc_info())
         return self.token
 
     def get_api_key(self):
+        """ API key for Service Account credentials """
         return self.service_account_configuration.client_id
 
     def handle_ims_failure(self, response):
+        """ Handling of IMS failure during call to PDF Services API """
+
         self._logger.error(
             "IMS call failed with status code {error_code}".format(error_code=response.status_code))
         content = json.loads(response.content)
         # When error is returned with no description
         if not content.get("error_description", None) or content["error_description"].isspace():
             content["error_description"] = content.get("error", None)
         # Special handling for invalid token and certificate expiry cases
@@ -88,14 +98,16 @@
         raise OperationException(message="Error response received for IMS request",
                                  status_code=response.status_code,
                                  error_code=content.get("error", None),
                                  error_message=content.get("error_description", None),
                                  request_tracking_id=ResponseUtil.get_request_tracking_id_from_response(response, True))
 
     def _prepare_jwt(self):
+        """ Prepares the JWT token for the request to PDF Services API """
+
         audience = "{base_uri}/{audience_suffix}{client_id}".format(
             base_uri=self.service_account_configuration.ims_base_uri,
             audience_suffix=ServiceConstants.JWT_AUDIENCE_SUFFIX,
             client_id=self.service_account_configuration.client_id
         )
         payload = {
             'sub': self.service_account_configuration.account_id,
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/auth/session_token.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/auth/session_token.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/request_key.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/constants/request_key.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/constants/service_constants.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/constants/service_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 custom_error_messages = {
 
     # Custom IMS error messages
-    "imsInvalidTokenGenericErrorMessage": 'Either your certificate for PDF Tools API credentials has expired or an ' +
+    "imsInvalidTokenGenericErrorMessage": 'Either your certificate for PDF Services API credentials has expired or an ' +
                                           'invalid Organization_ID/Account_ID has been used in credentials. Please visit Adobe IO ' +
                                           'Console(http://console.adobe.io/) to update your public certificate to use the same credentials or to check ' +
                                           'the value of Organization Id or Account ID.',
-    "imsCertificateExpiredErrorMessage": 'Your certificate for PDF Tools API credentials might have expired. ' +
+    "imsCertificateExpiredErrorMessage": 'Your certificate for PDF Services API credentials might have expired. ' +
                                          'Please visit Adobe IO Console(http://console.adobe.io/) to update your public certificate to use the same ' +
                                          'credentials.',
 
     # Service usage exception error messages
     "serviceUsageLimitReachedErrorMessage": 'Service usage limit has been reached. Please retry after sometime.',
     "integrationServiceUsageLimitReachedErrorMessage": 'Service usage limit has been reached for the integration. ' +
                                                        'Please retry after sometime.',
 
     # Quota specific exception error messages
     "quotaExhaustedErrorMessage": 'Free trial quota exhausted. Please visit (www.adobe.com/go/pdftoolsapi_err_quota) to ' +
-                                  'upgrade to paid credentials.',
+                                   'upgrade to paid credentials.',
     "quotaUnavailableErrorMessage": 'Quota for this operation is not available. Please visit ' +
-                                    '(www.adobe.com/go/pdftoolsapi_home) to start using free trial quota.'
+                                     '(www.adobe.com/go/pdftoolsapi_home) to start using free trial quota.'
 }
 
 
 class ServiceConstants:
     HTTP_CONNECT_TIMEOUT = 4000
     HTTP_READ_TIMEOUT = 10000
     HTTP_MAX_RETRIES = 1
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/exceptions.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_client.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             return response
 
 
 def _append_default_headers(headers: dict):
     # Set SDK Info header
     headers[DefaultHeaders.DC_APP_INFO_HEADER_KEY] = "{lang}-{name}-{version}".format(lang="python",
                                                                                       name='pdfservices-sdk',
-                                                                                      version='2.2.0')
+                                                                                      version='2.3.0')
     headers[DefaultHeaders.ACCEPT_HEADER_NAME] = DefaultHeaders.JSON_TXT_CONTENT_TYPE
 
 
 def _execute_request(http_request: HttpRequest):
     response = None
     timeout = (http_request.connect_timeout, http_request.read_timeout)
     try:
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_method.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/http_method.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/http_request.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/http_request.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/request_header_const.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/request_header_const.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/http/response_util.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/http/response_util.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_client_config.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/internal_client_config.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/internal_execution_context.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/internal_execution_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 # 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 from adobe.pdfservices.operation.auth.service_account_credentials import ServiceAccountCredentials
+from adobe.pdfservices.operation.auth.service_principal_credentials import ServicePrincipalCredentials
 from adobe.pdfservices.operation.execution_context import ExecutionContext
 
 from adobe.pdfservices.operation.internal.auth.auth_factory import AuthenticatorFactory
 from adobe.pdfservices.operation.internal.internal_client_config import InternalClientConfig
 
 
 class InternalExecutionContext(ExecutionContext):
     _credentials = None
     authenticator = None
     _client_config: InternalClientConfig = None
 
     def __init__(self, credentials, client_config):
-        if isinstance(credentials, ServiceAccountCredentials):
+        if isinstance(credentials, ServiceAccountCredentials) or isinstance(credentials, ServicePrincipalCredentials):
             self._credentials = credentials
             if isinstance(client_config, InternalClientConfig):
                 self._client_config = client_config
             else:
                 self._client_config = InternalClientConfig()
             self._client_config.validate()
-            self.authenticator = AuthenticatorFactory.get_authenticator(self._credentials)
+            self.authenticator = AuthenticatorFactory.get_authenticator(self._credentials, self._client_config)
         else:
             raise ValueError("Invalid Credentials provided as argument")
 
     @property
     def client_config(self):
         return self._client_config
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/io/file_ref_impl.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/service/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/service/autotag_pdf_service.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/service/extract_pdf_service.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/file_utils.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/json_hint_encoder.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/path_util.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/path_util.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/internal/util/validation_util.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/internal/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/io/file_ref.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/io/file_ref.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/operation.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/operation.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/autotag_pdf_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
     Sample usage.
 
     .. code-block:: python
 
         try:
             base_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-            credentials = Credentials.service_account_credentials_builder() \\
-                .from_file(base_path + "/pdfservices-api-credentials.json") \\
-                .build()
+            credentials = Credentials.service_principal_credentials_builder(). \\
+                with_client_id(os.getenv('PDF_SERVICES_CLIENT_ID')). \\
+                with_client_secret(os.getenv('PDF_SERVICES_CLIENT_SECRET')). \\
+                build()
 
             execution_context = ExecutionContext.create(credentials)
             autotag_pdf_operation = AutotagPDFOperation.create_new()
 
             input_file_path = 'autotagPdfInput.pdf'
             source = FileRef.create_from_local_file(base_path + "/resources/" + input_file_path)
             autotag_pdf_operation.set_input(source)
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/extract_pdf_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,18 @@
     Sample usage.
 
     .. code-block:: python
 
         try:
             base_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
-            credentials = Credentials.service_account_credentials_builder() \\
-                .from_file(base_path + "/pdfservices-api-credentials.json") \\
-                .build()
+            credentials = Credentials.service_principal_credentials_builder(). \\
+                with_client_id(os.getenv('PDF_SERVICES_CLIENT_ID')). \\
+                with_client_secret(os.getenv('PDF_SERVICES_CLIENT_SECRET')). \\
+                build()
 
             execution_context = ExecutionContext.create(credentials)
             extract_pdf_operation = ExtractPDFOperation.create_new()
 
             source = FileRef.create_from_local_file(base_path + "/resources/extractPdfInput.pdf")
             extract_pdf_operation.set_input(source)
```

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/autotagpdf/autotag_pdf_options.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_element_type.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_pdf_options.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/extract_renditions_element_type.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/pdfops/options/extractpdf/table_structure_type.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/adobe/pdfservices/operation/region.py` & `pdfservices-sdk-2.3.0/src/adobe/pdfservices/operation/region.py`

 * *Files identical despite different names*

### Comparing `pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/PKG-INFO` & `pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfservices-sdk
-Version: 2.2.0
+Version: 2.3.0
 Summary: Adobe PDFServices Client Library
 Home-page: https://www.adobe.com/go/pdftoolsapi_doc
 Author: Adobe Document Services
 Author-email: extractapi@adobe.com
 License: Apache2
 Description: PDFServices Python SDK
         =======================
```

### Comparing `pdfservices-sdk-2.2.0/src/pdfservices_sdk.egg-info/SOURCES.txt` & `pdfservices-sdk-2.3.0/src/pdfservices_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/adobe/pdfservices/operation/client_config.py
 src/adobe/pdfservices/operation/execution_context.py
 src/adobe/pdfservices/operation/operation.py
 src/adobe/pdfservices/operation/region.py
 src/adobe/pdfservices/operation/auth/__init__.py
 src/adobe/pdfservices/operation/auth/credentials.py
 src/adobe/pdfservices/operation/auth/service_account_credentials.py
+src/adobe/pdfservices/operation/auth/service_principal_credentials.py
 src/adobe/pdfservices/operation/exception/__init__.py
 src/adobe/pdfservices/operation/exception/exceptions.py
 src/adobe/pdfservices/operation/internal/__init__.py
 src/adobe/pdfservices/operation/internal/exceptions.py
 src/adobe/pdfservices/operation/internal/extension_media_type_mapping.py
 src/adobe/pdfservices/operation/internal/internal_client_config.py
 src/adobe/pdfservices/operation/internal/internal_execution_context.py
@@ -40,14 +41,15 @@
 src/adobe/pdfservices/operation/internal/api/dto/response/platform/job_error_response.py
 src/adobe/pdfservices/operation/internal/api/dto/response/platform/platform_api_response.py
 src/adobe/pdfservices/operation/internal/auth/__init__.py
 src/adobe/pdfservices/operation/internal/auth/auth_factory.py
 src/adobe/pdfservices/operation/internal/auth/authenticator.py
 src/adobe/pdfservices/operation/internal/auth/jwt_authenticator.py
 src/adobe/pdfservices/operation/internal/auth/service_account_credentials_with_uri.py
+src/adobe/pdfservices/operation/internal/auth/service_principal_authenticator.py
 src/adobe/pdfservices/operation/internal/auth/session_token.py
 src/adobe/pdfservices/operation/internal/constants/__init__.py
 src/adobe/pdfservices/operation/internal/constants/request_key.py
 src/adobe/pdfservices/operation/internal/constants/service_constants.py
 src/adobe/pdfservices/operation/internal/http/__init__.py
 src/adobe/pdfservices/operation/internal/http/http_client.py
 src/adobe/pdfservices/operation/internal/http/http_method.py
```

