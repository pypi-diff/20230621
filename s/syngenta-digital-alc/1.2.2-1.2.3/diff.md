# Comparing `tmp/syngenta_digital_alc-1.2.2.tar.gz` & `tmp/syngenta_digital_alc-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngenta_digital_alc-1.2.2.tar", last modified: Wed Jun  2 06:13:41 2021, max compression
+gzip compressed data, was "syngenta_digital_alc-1.2.3.tar", last modified: Tue Nov 16 00:13:34 2021, max compression
```

## Comparing `syngenta_digital_alc-1.2.2.tar` & `syngenta_digital_alc-1.2.3.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13148 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12244 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-06-02 06:13:41.344048 syngenta_digital_alc-1.2.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      729 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2146 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/request_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3540 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/request_validator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3056 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/response_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3029 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/router.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      339 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/common/json_helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2194 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/common/logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/common/troubleshoot_decorator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/dynamodb/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/dynamodb/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2161 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/dynamodb/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/generic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/generic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/generic/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      293 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/generic/handler_requirements.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/s3/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/s3/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1797 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/s3/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sns/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sns/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sns/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sns/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sns/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sqs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sqs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sqs/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sqs/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2395 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc/sqs/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.336048 syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13148 2021-06-02 06:13:41.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3061 2021-06-02 06:13:41.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-06-02 06:13:41.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2021-06-02 06:13:41.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2021-06-02 06:13:41.000000 syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5161 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/mock_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2631 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3478 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_request_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3923 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_request_validator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      983 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_router.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1913 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/common/test_logger.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5188 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/dynamodb/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1371 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/dynamodb/test_event_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/generic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/generic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/generic/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/generic/test_event_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1591 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2942 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/test_event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/test_record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/test_event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1970 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/test_record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:41.340048 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3279 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      570 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/test_event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2021-06-02 06:13:31.000000 syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/test_record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14565 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13661 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/custom_exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      729 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2146 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3540 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_validator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3056 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/response_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3455 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/router.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      339 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/json_helper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2194 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/logger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/troubleshoot_decorator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2161 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      293 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/handler_requirements.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1797 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/handler_requirements.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2395 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14565 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3181 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_before_all.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5161 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2631 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3478 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3923 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_validator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1956 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_router.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1913 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/test_logger.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5188 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1371 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/test_event_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/test_event_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1591 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2942 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1970 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_record_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3279 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      570 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_event_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_record_client.py
```

### Comparing `syngenta_digital_alc-1.2.2/LICENSE` & `syngenta_digital_alc-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/PKG-INFO` & `syngenta_digital_alc-1.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta_digital_alc
-Version: 1.2.2
+Version: 1.2.3
 Summary: DRY approach to working with AWS Lambdas
 Home-page: https://github.com/syngenta-digital/alc-python.git
 Author: Paul Cruse III, Technical Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -171,14 +171,57 @@
 `code`              | status code of response (will default to 204 if no content && will default 400 if errors found in response)
 `authorizer`        | authorizer of apigateway event (will default to use headers if using with [serverless offline](https://www.npmjs.com/package/serverless-offline))
 `base64_encoded`    | whether your body is base64Encoded [see docs](https://docs.aws.amazon.com/apigateway/latest/developerguide/set-up-lambda-proxy-integrations.html#api-gateway-simple-proxy-for-lambda-output-format)
 `compress`          | if set to true, will automatically compress, json and b64 encode as well as compress the body of your response and add appropriate headers
 `has_errors()`      | function will tell you if errors in the response
 `set_error()`       | function will set error key and message
 
+***(OPTIONAL) RUN LOGIC BEFORE EVERY REQUEST***
+
+This is a feature which allows you to interrogate all requests before they hit your endpoint. Here are some things to remember:
+
+* your function will run only after a valid route and method have been determined
+* runs before any validation
+* requires you use the `BeforeAllException` class to stop processing or route will continue
+* must be a pure function that is passed in context
+
+#### Example configuration
+```python
+import os
+
+from syngenta_digital_alc.apigateway.router import Router
+
+from example.function.to.import import example_before_all
+
+
+def route(event, context):
+    router = Router(
+        base_path='{}/{}'.format(os.environ['service'], 'v1'),
+        handler_path='application.v1.controller.apigateway',
+        schema_path='application/openapi.yml',
+        event=event,
+        context=context,
+        before_all=example_before_all.run # this is the important part
+    )
+    return router.route()   
+```
+
+#### Example before all function
+
+```python
+from syngenta_digital_alc.apigateway.custom_exceptions import BeforeAllException
+from syngenta_digital_alc.apigateway.handler_requirements import handler_requirements
+
+
+@handler_requirements()
+def run(request, response):
+    if not request.headers.get('x-api-key') == 'some-secret-key':
+        raise BeforeAllException(code=401, key_path='headers:x-api-key', message='you need an api key')
+
+```
 
 ### sqs events
 
 0. Setting Up your lambda to listen to the Queue
 
 ```yml
 functions:
```

### Comparing `syngenta_digital_alc-1.2.2/README.md` & `syngenta_digital_alc-1.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -148,14 +148,57 @@
 `code`              | status code of response (will default to 204 if no content && will default 400 if errors found in response)
 `authorizer`        | authorizer of apigateway event (will default to use headers if using with [serverless offline](https://www.npmjs.com/package/serverless-offline))
 `base64_encoded`    | whether your body is base64Encoded [see docs](https://docs.aws.amazon.com/apigateway/latest/developerguide/set-up-lambda-proxy-integrations.html#api-gateway-simple-proxy-for-lambda-output-format)
 `compress`          | if set to true, will automatically compress, json and b64 encode as well as compress the body of your response and add appropriate headers
 `has_errors()`      | function will tell you if errors in the response
 `set_error()`       | function will set error key and message
 
+***(OPTIONAL) RUN LOGIC BEFORE EVERY REQUEST***
+
+This is a feature which allows you to interrogate all requests before they hit your endpoint. Here are some things to remember:
+
+* your function will run only after a valid route and method have been determined
+* runs before any validation
+* requires you use the `BeforeAllException` class to stop processing or route will continue
+* must be a pure function that is passed in context
+
+#### Example configuration
+```python
+import os
+
+from syngenta_digital_alc.apigateway.router import Router
+
+from example.function.to.import import example_before_all
+
+
+def route(event, context):
+    router = Router(
+        base_path='{}/{}'.format(os.environ['service'], 'v1'),
+        handler_path='application.v1.controller.apigateway',
+        schema_path='application/openapi.yml',
+        event=event,
+        context=context,
+        before_all=example_before_all.run # this is the important part
+    )
+    return router.route()   
+```
+
+#### Example before all function
+
+```python
+from syngenta_digital_alc.apigateway.custom_exceptions import BeforeAllException
+from syngenta_digital_alc.apigateway.handler_requirements import handler_requirements
+
+
+@handler_requirements()
+def run(request, response):
+    if not request.headers.get('x-api-key') == 'some-secret-key':
+        raise BeforeAllException(code=401, key_path='headers:x-api-key', message='you need an api key')
+
+```
 
 ### sqs events
 
 0. Setting Up your lambda to listen to the Queue
 
 ```yml
 functions:
```

### Comparing `syngenta_digital_alc-1.2.2/setup.py` & `syngenta_digital_alc-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/handler_requirements.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/handler_requirements.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/request_client.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/request_validator.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_validator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/response_client.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/response_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/apigateway/router.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 import importlib.util
 import os
 
+from syngenta_digital_alc.apigateway.custom_exceptions import BeforeAllException
 from syngenta_digital_alc.apigateway.response_client import ResponseClient
 from syngenta_digital_alc.common import logger
 
 
 class Router:
 
     def __init__(self, **kwargs):
         self.event = kwargs['event']
         self.context = kwargs['context']
         self.handler_path = kwargs['handler_path']
         self.base_path = kwargs['base_path']
         self.schema_path = kwargs.get('schema_path')
+        self.before_all = kwargs.get('before_all')
         self.router_response = ResponseClient()
 
     def route(self):
-        route_results = self._route_request()
-        if self.router_response.has_errors:
+        try:
+            return self._route_request()
+        except BeforeAllException as b_error:
+            self.router_response.code = b_error.code
+            self.router_response.set_error(b_error.key_path, b_error.message)
+            return self.router_response.response
+        except:
             return self.router_response.response
-        return route_results
 
     def _route_request(self):
-        handler_module = self._run_route()
-        if handler_module:
-            return self._run_method(handler_module)
-        return None
+        handler_module = self._get_route()
+        handler_function = self._get_method(handler_module)
+        if self.before_all and callable(self.before_all):
+            self.before_all(self.event, self.context, self.schema_path)
+        return self._run_endpoint(handler_module, handler_function)
 
-    def _run_route(self):
+    def _get_route(self):
         import_path = self._get_import_path()
         file_path = self._get_file_path()
         if os.path.exists(file_path):
             spec = importlib.util.spec_from_file_location(import_path, file_path)
             handler_module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(handler_module)
             return handler_module
-        self._set_error(404, 'url', 'path not found')
-        return None
+        return self._set_error(404, 'url', 'path not found')
 
-    def _run_method(self, handler_module):
+    def _get_method(self, handler_module):
         method = self.event['httpMethod'].lower()
         if hasattr(handler_module, method):
-            return self._run_endpoint(handler_module, method)
-        self._set_error(403, 'method', 'method not allowed')
-        return None
+            return method
+        return self._set_error(403, 'method', 'method not allowed')
 
     def _run_endpoint(self, handler_module, method):
         try:
-            method_results = getattr(handler_module, method)(self.event, self.context, self.schema_path)
-            return method_results
+            return getattr(handler_module, method)(self.event, self.context, self.schema_path)
         except Exception as error:
-            self._set_error(500, 'server', 'internal server error', error)
+            return self._set_error(500, 'server', 'internal server error', error)
 
     def _clean_path(self, path):
         if path[0] == '/':
             path = path[1:]
         if path[-1] == '/':
             path = path[:-1]
         return path
 
     def _get_import_path(self):
         event_path = self._clean_path(self.event['path'])
         base_path = self._clean_path(self.base_path)
-        endpoint_import = event_path.replace('{}'.format(base_path), '').replace('-', '_')
+        endpoint_import = event_path.replace(
+            '{}'.format(base_path), '').replace('-', '_')
         return '{}.{}'.format(self.handler_path, endpoint_import)
 
     def _get_file_path(self):
         event_path = self._clean_path(self.event['path'])
         base_path = self._clean_path(self.base_path)
-        endpoint_file = event_path.replace('{}'.format(base_path), '').replace('-', '_')
+        endpoint_file = event_path.replace(
+            '{}'.format(base_path), '').replace('-', '_')
         if not endpoint_file:
             endpoint_file = '__init__'
         return '{}/{}.py'.format(self.handler_path.replace('.', '/'), endpoint_file)
 
-    def _set_error(self, code, key_path, message, error = None):
+    def _set_error(self, code, key_path, message, error=None):
         self.router_response.code = code
         self.router_response.set_error(key_path, message)
         if error and not os.getenv('UNITTEST'):
             logger.log(level='ERROR', log=error, trace=True)
+        raise Exception(message)
```

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/common/logger.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/logger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/common/troubleshoot_decorator.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/troubleshoot_decorator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/dynamodb/record_client.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/s3/record_client.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/sns/record_client.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc/sqs/record_client.py` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/PKG-INFO` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta-digital-alc
-Version: 1.2.2
+Version: 1.2.3
 Summary: DRY approach to working with AWS Lambdas
 Home-page: https://github.com/syngenta-digital/alc-python.git
 Author: Paul Cruse III, Technical Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -171,14 +171,57 @@
 `code`              | status code of response (will default to 204 if no content && will default 400 if errors found in response)
 `authorizer`        | authorizer of apigateway event (will default to use headers if using with [serverless offline](https://www.npmjs.com/package/serverless-offline))
 `base64_encoded`    | whether your body is base64Encoded [see docs](https://docs.aws.amazon.com/apigateway/latest/developerguide/set-up-lambda-proxy-integrations.html#api-gateway-simple-proxy-for-lambda-output-format)
 `compress`          | if set to true, will automatically compress, json and b64 encode as well as compress the body of your response and add appropriate headers
 `has_errors()`      | function will tell you if errors in the response
 `set_error()`       | function will set error key and message
 
+***(OPTIONAL) RUN LOGIC BEFORE EVERY REQUEST***
+
+This is a feature which allows you to interrogate all requests before they hit your endpoint. Here are some things to remember:
+
+* your function will run only after a valid route and method have been determined
+* runs before any validation
+* requires you use the `BeforeAllException` class to stop processing or route will continue
+* must be a pure function that is passed in context
+
+#### Example configuration
+```python
+import os
+
+from syngenta_digital_alc.apigateway.router import Router
+
+from example.function.to.import import example_before_all
+
+
+def route(event, context):
+    router = Router(
+        base_path='{}/{}'.format(os.environ['service'], 'v1'),
+        handler_path='application.v1.controller.apigateway',
+        schema_path='application/openapi.yml',
+        event=event,
+        context=context,
+        before_all=example_before_all.run # this is the important part
+    )
+    return router.route()   
+```
+
+#### Example before all function
+
+```python
+from syngenta_digital_alc.apigateway.custom_exceptions import BeforeAllException
+from syngenta_digital_alc.apigateway.handler_requirements import handler_requirements
+
+
+@handler_requirements()
+def run(request, response):
+    if not request.headers.get('x-api-key') == 'some-secret-key':
+        raise BeforeAllException(code=401, key_path='headers:x-api-key', message='you need an api key')
+
+```
 
 ### sqs events
 
 0. Setting Up your lambda to listen to the Queue
 
 ```yml
 functions:
```

### Comparing `syngenta_digital_alc-1.2.2/syngenta_digital_alc.egg-info/SOURCES.txt` & `syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 syngenta_digital_alc/__init__.py
 syngenta_digital_alc.egg-info/PKG-INFO
 syngenta_digital_alc.egg-info/SOURCES.txt
 syngenta_digital_alc.egg-info/dependency_links.txt
 syngenta_digital_alc.egg-info/requires.txt
 syngenta_digital_alc.egg-info/top_level.txt
 syngenta_digital_alc/apigateway/__init__.py
+syngenta_digital_alc/apigateway/custom_exceptions.py
 syngenta_digital_alc/apigateway/handler_requirements.py
 syngenta_digital_alc/apigateway/request_client.py
 syngenta_digital_alc/apigateway/request_validator.py
 syngenta_digital_alc/apigateway/response_client.py
 syngenta_digital_alc/apigateway/router.py
 syngenta_digital_alc/common/__init__.py
 syngenta_digital_alc/common/json_helper.py
@@ -35,14 +37,15 @@
 syngenta_digital_alc/sqs/__init__.py
 syngenta_digital_alc/sqs/event_client.py
 syngenta_digital_alc/sqs/handler_requirements.py
 syngenta_digital_alc/sqs/record_client.py
 tests/__init__.py
 tests/syngenta_digital_alc/__init__.py
 tests/syngenta_digital_alc/apigateway/__init__.py
+tests/syngenta_digital_alc/apigateway/mock_before_all.py
 tests/syngenta_digital_alc/apigateway/mock_data.py
 tests/syngenta_digital_alc/apigateway/mock_handler.py
 tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
 tests/syngenta_digital_alc/apigateway/test_request_client.py
 tests/syngenta_digital_alc/apigateway/test_request_validator.py
 tests/syngenta_digital_alc/apigateway/test_response.py
 tests/syngenta_digital_alc/apigateway/test_router.py
```

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/mock_data.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_request_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_request_validator.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_validator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/apigateway/test_response.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_response.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/common/test_logger.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/test_logger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/dynamodb/mock_data.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/dynamodb/test_event_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/generic/test_event_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/mock_data.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/test_event_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/s3/test_record_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/mock_data.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/test_event_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sns/test_record_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/mock_data.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/test_event_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.2/tests/syngenta_digital_alc/sqs/test_record_client.py` & `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_record_client.py`

 * *Files identical despite different names*

