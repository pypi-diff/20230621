# Comparing `tmp/syngenta_digital_alc-1.2.3.tar.gz` & `tmp/syngenta_digital_alc-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngenta_digital_alc-1.2.3.tar", last modified: Tue Nov 16 00:13:34 2021, max compression
+gzip compressed data, was "syngenta_digital_alc-1.2.5.tar", last modified: Wed Jun 21 17:45:33 2023, max compression
```

## Comparing `syngenta_digital_alc-1.2.3.tar` & `syngenta_digital_alc-1.2.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14565 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13661 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/custom_exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      729 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2146 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3540 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_validator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3056 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/response_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3455 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/router.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      339 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/json_helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2194 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      724 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/troubleshoot_decorator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2161 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      293 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/generic/handler_requirements.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1797 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/handler_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2395 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.252763 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14565 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3181 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2021-11-16 00:13:34.000000 syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_before_all.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5161 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2631 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3478 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3923 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_validator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1956 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_router.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1913 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/test_logger.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5188 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1371 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/test_event_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/test_event_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.256763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1591 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2942 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1773 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1970 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_record_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:34.260763 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3279 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      570 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_event_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2021-11-16 00:13:20.000000 syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_record_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.298652 syngenta_digital_alc-1.2.5/
+-rw-r--r--   0 dbankhead   (501) staff       (20)    11357 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/LICENSE
+-rw-r--r--   0 dbankhead   (501) staff       (20)    14528 2023-06-21 17:45:33.298760 syngenta_digital_alc-1.2.5/PKG-INFO
+-rw-r--r--   0 dbankhead   (501) staff       (20)    13661 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/README.md
+-rw-r--r--   0 dbankhead   (501) staff       (20)       68 2023-06-21 17:45:33.299204 syngenta_digital_alc-1.2.5/setup.cfg
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1239 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/setup.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.289495 syngenta_digital_alc-1.2.5/syngenta_digital_alc/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/__init__.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.291239 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      283 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/custom_exceptions.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      729 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/handler_requirements.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2146 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     3716 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_validator.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     3056 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/response_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     3509 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/router.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.291766 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      339 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/json_helper.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2194 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/logger.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      724 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/troubleshoot_decorator.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.292300 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/
+-rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      480 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      294 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/handler_requirements.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2161 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/record_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.292697 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/
+-rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      329 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      293 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/generic/handler_requirements.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.293303 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/
+-rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      478 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      288 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/handler_requirements.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1797 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/record_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.293818 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/
+-rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      479 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      288 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/handler_requirements.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2026 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/record_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.294398 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/
+-rw-r--r--   0 dbankhead   (501) staff       (20)       24 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      479 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      289 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/handler_requirements.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2395 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/record_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.290037 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/
+-rw-r--r--   0 dbankhead   (501) staff       (20)    14528 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/PKG-INFO
+-rw-r--r--   0 dbankhead   (501) staff       (20)     3181 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/SOURCES.txt
+-rw-r--r--   0 dbankhead   (501) staff       (20)        1 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/dependency_links.txt
+-rw-r--r--   0 dbankhead   (501) staff       (20)       51 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/requires.txt
+-rw-r--r--   0 dbankhead   (501) staff       (20)       27 2023-06-21 17:45:33.000000 syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/top_level.txt
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.294528 syngenta_digital_alc-1.2.5/tests/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/__init__.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.294605 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/__init__.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.295812 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      464 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_before_all.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     5161 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_data.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      192 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_handler.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2665 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     3478 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     3923 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_validator.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1682 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_response.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1956 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_router.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.296047 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1913 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/test_logger.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.296391 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     5188 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/mock_data.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1371 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/test_event_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.296739 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)       82 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/mock_data.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      551 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/test_event_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.297224 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1591 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/mock_data.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2942 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1993 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_record_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.297819 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1175 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/mock_data.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1773 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     1970 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_record_client.py
+drwxr-xr-x   0 dbankhead   (501) staff       (20)        0 2023-06-21 17:45:33.298518 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/
+-rw-r--r--   0 dbankhead   (501) staff       (20)        0 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/__init__.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     3279 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/mock_data.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)      570 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_event_client.py
+-rw-r--r--   0 dbankhead   (501) staff       (20)     2430 2023-06-21 16:53:52.000000 syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_record_client.py
```

### Comparing `syngenta_digital_alc-1.2.3/LICENSE` & `syngenta_digital_alc-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/PKG-INFO` & `syngenta_digital_alc-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: syngenta_digital_alc
-Version: 1.2.3
+Version: 1.2.5
 Summary: DRY approach to working with AWS Lambdas
 Home-page: https://github.com/syngenta-digital/alc-python.git
 Author: Paul Cruse III, Technical Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -408,9 +406,7 @@
 
 ### Unit Testing
 
 To run unit test, enter command:
 ```bash
 pipenv run test
 ```
-
-
```

### Comparing `syngenta_digital_alc-1.2.3/README.md` & `syngenta_digital_alc-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/setup.py` & `syngenta_digital_alc-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/handler_requirements.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/handler_requirements.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_client.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/request_validator.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/request_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import jsonref
 from jsonschema import Draft7Validator
 import yaml
-
+import functools
 
 class RequestValidator:
 
     def __init__(self, request_client, response_client, schema_path = ''):
         self.request_client = request_client
         self.response_client = response_client
         self.schema_path = schema_path
@@ -55,23 +55,26 @@
         json_schema = self._get_combined_schema(schema)
         schema_validator = Draft7Validator(json_schema)
         for schema_error in sorted(schema_validator.iter_errors(request), key=str):
             self.response_client.set_error(self._get_error_path(schema_error), schema_error.message)
 
     def _get_combined_schema(self, schema):
         combined_schema = {}
-        swagger = self._get_api_doc()
-        definitions = jsonref.loads(json.dumps(swagger))['components']['schemas']
-        definition_schema = definitions[schema]
+        schema_definitions = self.openapi_to_resolved_json(path_openapi=self.schema_path)
+        definition_schema = schema_definitions[schema]
         json_schemas = definition_schema['allOf'] if definition_schema.get('allOf') else [definition_schema]
         for json_schema in json_schemas:
             combined_schema.update(json_schema)
         combined_schema['additionalProperties'] = False
         return combined_schema
 
     def _get_error_path(self, error):
         path = '.'.join(str(path) for path in error.path)
         return path if path else 'root'
 
-    def _get_api_doc(self):
-        with open(self.schema_path) as api_doc:
-            return yaml.load(api_doc, Loader=yaml.FullLoader)
+    @staticmethod
+    @functools.lru_cache
+    def openapi_to_resolved_json(path_openapi: str):
+        with open(path_openapi) as api_doc:
+            as_yaml = yaml.load(api_doc, Loader=yaml.FullLoader)
+            definitions = jsonref.loads(json.dumps(as_yaml))['components']['schemas']
+            return definitions
```

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/response_client.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/response_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/apigateway/router.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/apigateway/router.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     def route(self):
         try:
             return self._route_request()
         except BeforeAllException as b_error:
             self.router_response.code = b_error.code
             self.router_response.set_error(b_error.key_path, b_error.message)
             return self.router_response.response
-        except:
+        except Exception as error:
+            logger.log(level='ERROR', log=error, trace=True)
             return self.router_response.response
 
     def _route_request(self):
         handler_module = self._get_route()
         handler_function = self._get_method(handler_module)
         if self.before_all and callable(self.before_all):
             self.before_all(self.event, self.context, self.schema_path)
@@ -62,23 +63,21 @@
         if path[-1] == '/':
             path = path[:-1]
         return path
 
     def _get_import_path(self):
         event_path = self._clean_path(self.event['path'])
         base_path = self._clean_path(self.base_path)
-        endpoint_import = event_path.replace(
-            '{}'.format(base_path), '').replace('-', '_')
+        endpoint_import = event_path.replace('{}'.format(base_path), '').replace('-', '_')
         return '{}.{}'.format(self.handler_path, endpoint_import)
 
     def _get_file_path(self):
         event_path = self._clean_path(self.event['path'])
         base_path = self._clean_path(self.base_path)
-        endpoint_file = event_path.replace(
-            '{}'.format(base_path), '').replace('-', '_')
+        endpoint_file = event_path.replace('{}'.format(base_path), '').replace('-', '_')
         if not endpoint_file:
             endpoint_file = '__init__'
         return '{}/{}.py'.format(self.handler_path.replace('.', '/'), endpoint_file)
 
     def _set_error(self, code, key_path, message, error=None):
         self.router_response.code = code
         self.router_response.set_error(key_path, message)
```

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/logger.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/logger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/common/troubleshoot_decorator.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/common/troubleshoot_decorator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/dynamodb/record_client.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/dynamodb/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/s3/record_client.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/s3/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/sns/record_client.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/sns/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc/sqs/record_client.py` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc/sqs/record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/PKG-INFO` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: syngenta-digital-alc
-Version: 1.2.3
+Version: 1.2.5
 Summary: DRY approach to working with AWS Lambdas
 Home-page: https://github.com/syngenta-digital/alc-python.git
 Author: Paul Cruse III, Technical Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -408,9 +406,7 @@
 
 ### Unit Testing
 
 To run unit test, enter command:
 ```bash
 pipenv run test
 ```
-
-
```

### Comparing `syngenta_digital_alc-1.2.3/syngenta_digital_alc.egg-info/SOURCES.txt` & `syngenta_digital_alc-1.2.5/syngenta_digital_alc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/mock_data.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_handler_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import unittest
 
 from syngenta_digital_alc.apigateway.handler_requirements import handler_requirements
 from tests.syngenta_digital_alc.apigateway import mock_data
 
+
 @handler_requirements()
 def handle_no_validation(request, response):
     response.body = "Hello"
 
+
 @handler_requirements(required_path_parameters=['proxy'])
 def handle_validation_required_path(request, response):
     response.body = "Hello"
 
+
 @handler_requirements(required_path_parameters=['proxy_fail'])
 def handle_validation_required_path_fail(request, response):
     response.body = "Hello"
 
+
 @handler_requirements(required_headers=['x-api-key'])
 def handle_validation_required_headers(request, response):
     response.body = "Hello"
 
+
 @handler_requirements(required_headers=['x-api-key-fail'])
 def handle_validation_required_headers_fail(request, response):
     response.body = "Hello"
 
+
 @handler_requirements(required_body='v1-test-request')
 def handle_validation_required_body(request, response):
     response.body = "Hello"
 
+
 @handler_requirements(required_body='v1-test-request-fail')
 def handle_validation_required_body_fail(request, response):
     response.body = "Hello"
 
+
 class ApiGatewayHandlerDecoratorTest(unittest.TestCase):
 
     def test_no_authorization(self):
         response = handle_no_validation(mock_data.apigateway_event(), None)
         self.assertEqual(response['statusCode'], 200)
         self.assertEqual(response['body'], "Hello")
 
@@ -49,14 +57,16 @@
         self.assertEqual(response['body'], "Hello")
 
     def test_with_validation_require_headers_fail(self):
         response = handle_validation_required_headers_fail(mock_data.apigateway_event(), None)
         self.assertEqual(response['statusCode'], 400)
 
     def test_with_validation_require_body(self):
-        response = handle_validation_required_body(mock_data.apigateway_event_with_body('pass'), None, 'tests/openapi.yml')
+        response = handle_validation_required_body(
+            mock_data.apigateway_event_with_body('pass'), None, 'tests/openapi.yml')
         self.assertEqual(response['statusCode'], 200)
         self.assertEqual(response['body'], "Hello")
 
     def test_with_validation_require_body_fail(self):
-        response = handle_validation_required_body(mock_data.apigateway_event_with_body('fail'), None, 'tests/openapi.yml')
+        response = handle_validation_required_body(
+            mock_data.apigateway_event_with_body('fail'), None, 'tests/openapi.yml')
         self.assertEqual(response['statusCode'], 400)
```

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_request_validator.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_request_validator.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_response.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_response.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/apigateway/test_router.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/apigateway/test_router.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/common/test_logger.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/common/test_logger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/mock_data.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/dynamodb/test_event_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/dynamodb/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/generic/test_event_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/generic/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/mock_data.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_event_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/s3/test_record_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/s3/test_record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/mock_data.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_event_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sns/test_record_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sns/test_record_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/mock_data.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_event_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_event_client.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_alc-1.2.3/tests/syngenta_digital_alc/sqs/test_record_client.py` & `syngenta_digital_alc-1.2.5/tests/syngenta_digital_alc/sqs/test_record_client.py`

 * *Files identical despite different names*

