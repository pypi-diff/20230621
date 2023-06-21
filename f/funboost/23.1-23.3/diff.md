# Comparing `tmp/funboost-23.1-py3-none-any.whl.zip` & `tmp/funboost-23.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1910762 bytes, number of entries: 242
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-13 01:20 funboost/__init__.py
+Zip file size: 1915034 bytes, number of entries: 246
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-19 02:37 funboost/__init__.py
 -rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-13 01:20 funboost/__init__old.py
--rw-rw-rw-  2.0 fat     6223 b- defN 23-Jun-09 01:42 funboost/constant.py
+-rw-rw-rw-  2.0 fat     6261 b- defN 23-Jun-20 05:54 funboost/constant.py
 -rw-rw-rw-  2.0 fat     7358 b- defN 23-Jun-05 04:48 funboost/funboost_config_deafult.py
 -rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-13 09:47 funboost/set_frame_config.py
 -rw-rw-rw-  2.0 fat     4186 b- defN 23-Jun-19 02:19 funboost/assist/celery_helper.py
 -rw-rw-rw-  2.0 fat     2089 b- defN 23-May-22 01:31 funboost/assist/dramatiq_helper.py
 -rw-rw-rw-  2.0 fat     1760 b- defN 23-May-24 11:10 funboost/assist/huey_helper.py
 -rw-rw-rw-  2.0 fat     1509 b- defN 23-Jun-09 03:23 funboost/assist/rq_helper.py
 -rw-rw-rw-  2.0 fat     4831 b- defN 23-Jun-09 01:42 funboost/assist/rq_windows_worker.py
@@ -26,15 +26,15 @@
 -rw-rw-rw-  2.0 fat     9548 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor0223.py
 -rw-rw-rw-  2.0 fat     9568 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_back.py
 -rw-rw-rw-  2.0 fat     5728 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_janus.py
 -rw-rw-rw-  2.0 fat      126 b- defN 22-Sep-17 06:12 funboost/consumers/__init__.py
 -rw-rw-rw-  2.0 fat    82870 b- defN 23-Jun-19 02:19 funboost/consumers/base_consumer.py
 -rw-rw-rw-  2.0 fat     7574 b- defN 23-Jun-06 01:47 funboost/consumers/celery_consumer.py
 -rw-rw-rw-  2.0 fat     4574 b- defN 23-May-04 06:09 funboost/consumers/celery_consumer000.py
--rw-rw-rw-  2.0 fat     5877 b- defN 23-Mar-29 02:19 funboost/consumers/confirm_mixin.py
+-rw-rw-rw-  2.0 fat     6033 b- defN 23-Jun-20 04:59 funboost/consumers/confirm_mixin.py
 -rw-rw-rw-  2.0 fat     2144 b- defN 23-May-23 07:08 funboost/consumers/dramatiq_consumer.py
 -rw-rw-rw-  2.0 fat     2025 b- defN 23-May-15 01:33 funboost/consumers/http_consumer.py
 -rw-rw-rw-  2.0 fat     4463 b- defN 22-Sep-17 06:12 funboost/consumers/http_consumer000.py
 -rw-rw-rw-  2.0 fat     1080 b- defN 23-May-04 12:12 funboost/consumers/httpsqs_consumer.py
 -rw-rw-rw-  2.0 fat     1856 b- defN 23-May-24 11:08 funboost/consumers/huey_consumer.py
 -rw-rw-rw-  2.0 fat     4217 b- defN 23-May-04 12:12 funboost/consumers/kafka_consumer.py
 -rw-rw-rw-  2.0 fat     6947 b- defN 23-Jun-09 09:53 funboost/consumers/kafka_consumer_manually_commit.py
@@ -44,21 +44,22 @@
 -rw-rw-rw-  2.0 fat     2228 b- defN 23-May-04 12:12 funboost/consumers/mqtt_consumer.py
 -rw-rw-rw-  2.0 fat     2183 b- defN 23-May-04 12:12 funboost/consumers/nameko_consumer.py
 -rw-rw-rw-  2.0 fat     1076 b- defN 23-May-04 12:12 funboost/consumers/nats_consumer.py
 -rw-rw-rw-  2.0 fat     1461 b- defN 23-May-18 03:26 funboost/consumers/nsq_consumer.py
 -rw-rw-rw-  2.0 fat     1238 b- defN 23-May-04 12:12 funboost/consumers/peewee_conusmer.py
 -rw-rw-rw-  2.0 fat     1005 b- defN 23-May-04 12:12 funboost/consumers/persist_queue_consumer.py
 -rw-rw-rw-  2.0 fat     2414 b- defN 23-May-04 12:12 funboost/consumers/pulsar_consumer.py
--rw-rw-rw-  2.0 fat     1721 b- defN 23-May-12 09:09 funboost/consumers/rabbitmq_amqpstorm_consumer.py
+-rw-rw-rw-  2.0 fat     2048 b- defN 23-Jun-20 01:27 funboost/consumers/rabbitmq_amqpstorm_consumer.py
 -rw-rw-rw-  2.0 fat     5433 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_pika_consumer.py
 -rw-rw-rw-  2.0 fat     4674 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_pika_consumerv0.py
 -rw-rw-rw-  2.0 fat     1260 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_rabbitpy_consumer.py
 -rw-rw-rw-  2.0 fat     3031 b- defN 23-May-04 12:12 funboost/consumers/redis_brpoplpush_consumer.py
 -rw-rw-rw-  2.0 fat     2829 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer.py
 -rw-rw-rw-  2.0 fat     7545 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_ack_able.py
+-rw-rw-rw-  2.0 fat     4282 b- defN 23-Jun-21 02:07 funboost/consumers/redis_consumer_priority.py
 -rw-rw-rw-  2.0 fat      922 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_simple.py
 -rw-rw-rw-  2.0 fat     7135 b- defN 22-Sep-17 06:12 funboost/consumers/redis_filter.py
 -rw-rw-rw-  2.0 fat     1206 b- defN 23-May-04 12:12 funboost/consumers/redis_pubsub_consumer.py
 -rw-rw-rw-  2.0 fat     6497 b- defN 23-May-25 02:22 funboost/consumers/redis_stream_consumer.py
 -rw-rw-rw-  2.0 fat     1653 b- defN 23-May-04 12:12 funboost/consumers/rocketmq_consumer.py
 -rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-08 11:07 funboost/consumers/rq_consumer.py
 -rw-rw-rw-  2.0 fat     1309 b- defN 23-May-04 12:12 funboost/consumers/sqlachemy_consumer.py
@@ -78,15 +79,15 @@
 -rw-rw-rw-  2.0 fat     8819 b- defN 23-Jun-05 04:48 funboost/core/function_result_status_saver.py
 -rw-rw-rw-  2.0 fat     1169 b- defN 23-Jun-08 03:26 funboost/core/get_booster.py
 -rw-rw-rw-  2.0 fat      340 b- defN 23-Jun-08 02:52 funboost/core/global_boosters.py
 -rw-rw-rw-  2.0 fat     1193 b- defN 23-Jun-12 01:35 funboost/core/helper_funs.py
 -rw-rw-rw-  2.0 fat     7782 b- defN 23-Jun-05 04:48 funboost/core/msg_result_getter.py
 -rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-08 03:05 funboost/core/muliti_process_enhance.py
 -rw-rw-rw-  2.0 fat      178 b- defN 22-Sep-17 06:12 funboost/factories/__init__.py
--rw-rw-rw-  2.0 fat     8738 b- defN 23-Jun-09 03:28 funboost/factories/broker_kind__publsiher_consumer_type_map.py
+-rw-rw-rw-  2.0 fat     8976 b- defN 23-Jun-20 05:54 funboost/factories/broker_kind__publsiher_consumer_type_map.py
 -rw-rw-rw-  2.0 fat      946 b- defN 23-May-29 03:09 funboost/factories/consumer_factory.py
 -rw-rw-rw-  2.0 fat     2281 b- defN 23-May-29 03:09 funboost/factories/publisher_factotry.py
 -rw-rw-rw-  2.0 fat     4841 b- defN 22-Sep-17 06:12 funboost/function_result_web/app.py
 -rw-rw-rw-  2.0 fat     7345 b- defN 23-Mar-08 10:19 funboost/function_result_web/functions.py
 -rw-rw-rw-  2.0 fat     4045 b- defN 22-Feb-21 07:34 funboost/function_result_web/__pycache__/app.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     3921 b- defN 22-Mar-30 13:56 funboost/function_result_web/__pycache__/functions.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     7674 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/css/custom.css
@@ -99,38 +100,39 @@
 -rw-rw-rw-  2.0 fat      546 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/password.png
 -rw-rw-rw-  2.0 fat     2912 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/tick.png
 -rw-rw-rw-  2.0 fat      622 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/user.png
 -rw-rw-rw-  2.0 fat    96383 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/js/jquery-1.11.0.min.js
 -rw-rw-rw-  2.0 fat    19501 b- defN 22-Feb-21 12:32 funboost/function_result_web/templates/index.html
 -rw-rw-rw-  2.0 fat     2007 b- defN 21-Dec-27 01:40 funboost/function_result_web/templates/login.html
 -rw-rw-rw-  2.0 fat      131 b- defN 22-Sep-17 06:12 funboost/publishers/__init__.py
--rw-rw-rw-  2.0 fat    15148 b- defN 23-Jun-08 03:14 funboost/publishers/base_publisher.py
--rw-rw-rw-  2.0 fat     3755 b- defN 23-Jun-16 11:28 funboost/publishers/celery_publisher.py
+-rw-rw-rw-  2.0 fat    15844 b- defN 23-Jun-20 05:06 funboost/publishers/base_publisher.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-Jun-20 04:23 funboost/publishers/celery_publisher.py
 -rw-rw-rw-  2.0 fat     3897 b- defN 23-May-04 06:09 funboost/publishers/celery_publisher000.py
 -rw-rw-rw-  2.0 fat     3541 b- defN 23-Mar-23 05:32 funboost/publishers/confluent_kafka_publisher.py
 -rw-rw-rw-  2.0 fat     1410 b- defN 23-May-22 01:23 funboost/publishers/dramatiq_publisher.py
 -rw-rw-rw-  2.0 fat      753 b- defN 23-May-04 11:53 funboost/publishers/http_publisher.py
 -rw-rw-rw-  2.0 fat     2783 b- defN 22-Sep-17 06:12 funboost/publishers/httpsqs_publisher.py
 -rw-rw-rw-  2.0 fat     1101 b- defN 23-May-24 11:08 funboost/publishers/huey_publisher.py
 -rw-rw-rw-  2.0 fat     2160 b- defN 23-Apr-03 10:55 funboost/publishers/kafka_publisher.py
 -rw-rw-rw-  2.0 fat     5321 b- defN 23-May-15 01:33 funboost/publishers/kombu_publisher.py
 -rw-rw-rw-  2.0 fat     1365 b- defN 22-Sep-17 06:12 funboost/publishers/local_python_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1874 b- defN 23-Mar-14 02:56 funboost/publishers/mongomq_publisher.py
 -rw-rw-rw-  2.0 fat     3050 b- defN 22-Sep-17 06:12 funboost/publishers/mqtt_publisher.py
--rw-rw-rw-  2.0 fat     2147 b- defN 23-Apr-28 06:21 funboost/publishers/nameko_publisher.py
+-rw-rw-rw-  2.0 fat     1662 b- defN 23-Jun-19 06:54 funboost/publishers/nameko_publisher.py
 -rw-rw-rw-  2.0 fat      776 b- defN 21-Dec-27 01:40 funboost/publishers/nats_publisher.py
 -rw-rw-rw-  2.0 fat     1302 b- defN 22-Sep-17 06:12 funboost/publishers/nsq_publisher.py
 -rw-rw-rw-  2.0 fat     1095 b- defN 22-Sep-17 06:12 funboost/publishers/peewee_publisher.py
 -rw-rw-rw-  2.0 fat     2540 b- defN 22-Sep-17 06:12 funboost/publishers/persist_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-13 03:56 funboost/publishers/pulsar_publisher.py
--rw-rw-rw-  2.0 fat     2725 b- defN 23-Apr-17 07:35 funboost/publishers/rabbitmq_amqpstorm_publisher.py
+-rw-rw-rw-  2.0 fat     3137 b- defN 23-Jun-20 02:17 funboost/publishers/rabbitmq_amqpstorm_publisher.py
 -rw-rw-rw-  2.0 fat     2343 b- defN 22-Sep-17 06:12 funboost/publishers/rabbitmq_pika_publisher.py
 -rw-rw-rw-  2.0 fat     1953 b- defN 22-Sep-17 06:12 funboost/publishers/rabbitmq_rabbitpy_publisher.py
 -rw-rw-rw-  2.0 fat     3982 b- defN 23-May-10 03:22 funboost/publishers/redis_publisher.py
 -rw-rw-rw-  2.0 fat      278 b- defN 22-Sep-17 06:12 funboost/publishers/redis_publisher_lpush.py
+-rw-rw-rw-  2.0 fat     2104 b- defN 23-Jun-20 05:54 funboost/publishers/redis_publisher_priority.py
 -rw-rw-rw-  2.0 fat      872 b- defN 23-Apr-28 03:12 funboost/publishers/redis_publisher_simple.py
 -rw-rw-rw-  2.0 fat      721 b- defN 22-Sep-17 06:12 funboost/publishers/redis_pubsub_publisher.py
 -rw-rw-rw-  2.0 fat     2037 b- defN 21-Dec-27 01:40 funboost/publishers/redis_stream_publisher.py
 -rw-rw-rw-  2.0 fat     2343 b- defN 23-Mar-23 05:32 funboost/publishers/rocketmq_publisher.py
 -rw-rw-rw-  2.0 fat      893 b- defN 23-Jun-13 01:20 funboost/publishers/rq_publisher.py
 -rw-rw-rw-  2.0 fat     1215 b- defN 22-Sep-17 06:12 funboost/publishers/sqla_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1335 b- defN 23-May-10 08:53 funboost/publishers/tcp_publisher.py
@@ -167,16 +169,18 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/__init__.py
 -rw-rw-rw-  2.0 fat      131 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/mongomq/__init__.py
 -rw-rw-rw-  2.0 fat     2486 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/lock.py
 -rw-rw-rw-  2.0 fat     7902 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/mongomq.py
 -rw-rw-rw-  2.0 fat     7867 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/mongomq0000.py
 -rw-rw-rw-  2.0 fat     4811 b- defN 22-Apr-01 02:17 funboost/utils/dependency_packages/mongomq/test.py
 -rw-rw-rw-  2.0 fat      377 b- defN 21-Dec-27 01:40 funboost/utils/dependency_packages/mongomq/utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-19 06:09 funboost/utils/dependency_packages_in_pythonpath/__init__.py
 -rw-rw-rw-  2.0 fat      341 b- defN 23-Mar-09 12:29 funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
--rw-rw-rw-  2.0 fat      545 b- defN 23-Mar-09 11:52 funboost/utils/dependency_packages_in_pythonpath/readme.md
+-rw-rw-rw-  2.0 fat      814 b- defN 23-Jun-19 02:58 funboost/utils/dependency_packages_in_pythonpath/readme.md
+-rw-rw-rw-  2.0 fat      165 b- defN 23-Jun-19 10:52 funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-37.pyc
 -rw-rw-rw-  2.0 fat      475 b- defN 23-Mar-09 11:46 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc
 -rw-rw-rw-  2.0 fat      312 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-37.pyc
 -rw-rw-rw-  2.0 fat      316 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc
 -rw-rw-rw-  2.0 fat     1223 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
 -rw-rw-rw-  2.0 fat   182652 b- defN 23-Mar-23 05:34 funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py
 -rw-rw-rw-  2.0 fat      183 b- defN 23-Feb-27 10:21 funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py
 -rw-rw-rw-  2.0 fat    62239 b- defN 23-Mar-23 05:34 funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py
@@ -232,13 +236,13 @@
 -rw-rw-rw-  2.0 fat      909 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/__init__.py
 -rw-rw-rw-  2.0 fat     2243 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/pycompat.py
 -rw-rw-rw-  2.0 fat    19131 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/tracer.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/utils.py
 -rw-rw-rw-  2.0 fat     3693 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/variables.py
 -rw-rw-rw-  2.0 fat     2417 b- defN 23-Jun-09 01:42 funboost/utils/times/__init__.py
 -rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-09 01:42 funboost/utils/times/version.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    26616 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    26209 b- defN 23-Jun-19 02:22 funboost-23.1.dist-info/RECORD
-242 files, 3294282 bytes uncompressed, 1867342 bytes compressed:  43.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26616 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    26669 b- defN 23-Jun-21 02:07 funboost-23.3.dist-info/RECORD
+246 files, 3302262 bytes uncompressed, 1870838 bytes compressed:  43.4%
```

## zipnote {}

```diff
@@ -162,14 +162,17 @@
 
 Filename: funboost/consumers/redis_consumer.py
 Comment: 
 
 Filename: funboost/consumers/redis_consumer_ack_able.py
 Comment: 
 
+Filename: funboost/consumers/redis_consumer_priority.py
+Comment: 
+
 Filename: funboost/consumers/redis_consumer_simple.py
 Comment: 
 
 Filename: funboost/consumers/redis_filter.py
 Comment: 
 
 Filename: funboost/consumers/redis_pubsub_consumer.py
@@ -378,14 +381,17 @@
 
 Filename: funboost/publishers/redis_publisher.py
 Comment: 
 
 Filename: funboost/publishers/redis_publisher_lpush.py
 Comment: 
 
+Filename: funboost/publishers/redis_publisher_priority.py
+Comment: 
+
 Filename: funboost/publishers/redis_publisher_simple.py
 Comment: 
 
 Filename: funboost/publishers/redis_pubsub_publisher.py
 Comment: 
 
 Filename: funboost/publishers/redis_stream_publisher.py
@@ -510,20 +516,26 @@
 
 Filename: funboost/utils/dependency_packages/mongomq/test.py
 Comment: 
 
 Filename: funboost/utils/dependency_packages/mongomq/utils.py
 Comment: 
 
+Filename: funboost/utils/dependency_packages_in_pythonpath/__init__.py
+Comment: 
+
 Filename: funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/readme.md
 Comment: 
 
+Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-37.pyc
+Comment: 
+
 Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-37.pyc
 Comment: 
 
 Filename: funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc
@@ -705,23 +717,23 @@
 
 Filename: funboost/utils/times/__init__.py
 Comment: 
 
 Filename: funboost/utils/times/version.py
 Comment: 
 
-Filename: funboost-23.1.dist-info/LICENSE
+Filename: funboost-23.3.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-23.1.dist-info/METADATA
+Filename: funboost-23.3.dist-info/METADATA
 Comment: 
 
-Filename: funboost-23.1.dist-info/WHEEL
+Filename: funboost-23.3.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-23.1.dist-info/top_level.txt
+Filename: funboost-23.3.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-23.1.dist-info/RECORD
+Filename: funboost-23.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funboost/__init__.py

```diff
@@ -31,11 +31,12 @@
 
 from funboost.core.booster import boost, Booster
 from funboost.core.get_booster import get_booster
 
 from funboost.core.exit_signal import set_interrupt_signal_handler
 from funboost.core.helper_funs import run_forever
 
-# 有的包默认没加handlers，原始的日志不漂亮且不可跳转不知道哪里发生的。这里把warnning级别以上的日志默认加上handlers。
-# nb_log.get_logger(name='', log_level_int=30, log_filename='pywarning.log')
 
 set_interrupt_signal_handler()
+
+# 有的包默认没加handlers，原始的日志不漂亮且不可跳转不知道哪里发生的。这里把warnning级别以上的日志默认加上handlers。
+# nb_log.get_logger(name='', log_level_int=30, log_filename='pywarning.log')
```

## funboost/constant.py

```diff
@@ -21,15 +21,16 @@
     KAFKA = 8  # 基于kafka作为分布式消息队列，如果随意重启会丢失消息，建议使用BrokerEnum.CONFLUENT_KAFKA。
 
     """基于confluent-kafka包，包的性能比kafka-python提升10倍。同时应对反复随意重启部署消费代码的场景，此消费者实现至少消费一次，第8种BrokerEnum.KAFKA是最多消费一次。"""
     CONFLUENT_KAFKA = 16
     KAFKA_CONFLUENT = CONFLUENT_KAFKA
 
     REDIS_ACK_ABLE = 9  # 基于redis的 list + 临时unack的set队列，采用了 lua脚本操持了取任务和加到pengding为原子性，随意重启和掉线不会丢失任务。
-    # 集群里面的所有电脑或服务器时间一定要设置成自动获取，不然会发生消费重复问题，单台没事。
+
+    REDIS_PRIORITY = 109 #  # 基于redis的多 list + 临时unack的set队列，blpop监听多个key，和rabbitmq的x-max-priority属性一样，支持任务优先级。
 
     SQLACHEMY = 10  # 基于SQLACHEMY 的连接作为分布式消息队列中间件支持持久化和消费确认。支持mysql oracle sqlserver等5种数据库。
 
     ROCKETMQ = 11  # 基于 rocketmq 作为分布式消息队列，这个中间件必须在linux下运行，win不支持。
 
     REDIS_STREAM = 12  # 基于redis 5.0 版本以后，使用 stream 数据结构作为分布式消息队列，支持消费确认和持久化和分组消费，是redis官方推荐的消息队列形式，比list结构更适合。
```

## funboost/consumers/confirm_mixin.py

```diff
@@ -82,12 +82,13 @@
                     if current_queue_unacked_msg_queue_name.split(f'{self._queue_name}__unack_id_')[1] not in current_queue_hearbeat_ids:
                         self.logger.warning(f'{current_queue_unacked_msg_queue_name} 是掉线或关闭消费者的')
                         while 1:
                             if self.redis_db_frame.exists(current_queue_unacked_msg_queue_name):
                                 for unacked_task_str in self.redis_db_frame.zrevrange(current_queue_unacked_msg_queue_name, 0, 1000):
                                     self.logger.warning(f'从 {current_queue_unacked_msg_queue_name} 向 {self._queue_name} 重新放入掉线消费者未消费确认的任务'
                                                         f' {unacked_task_str.decode()}')
-                                    self.redis_db_frame.lpush(self._queue_name, unacked_task_str)
+                                    # self.redis_db_frame.lpush(self._queue_name, unacked_task_str)
+                                    self.publisher_of_same_queue.publish(unacked_task_str) # redis优先级队列的入队不一样，不使用上面。
                                     self.redis_db_frame.zrem(current_queue_unacked_msg_queue_name, unacked_task_str)
                     else:
                         pass
                         # print('是活跃消费者')
```

## funboost/consumers/rabbitmq_amqpstorm_consumer.py

```diff
@@ -7,28 +7,30 @@
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.publishers.rabbitmq_amqpstorm_publisher import RabbitmqPublisherUsingAmqpStorm
 
 
 class RabbitmqConsumerAmqpStorm(AbstractConsumer):
     """
     使用AmqpStorm实现的，多线程安全的，不用加锁。
+    funboost 强烈推荐使用这个做消息对内中间件。
     """
+    BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'x-max-priority':None}   # x-max-priority 是 rabbitmq的优先级队列配置，必须为整数，强烈建议要小于5。为None就代表队列不支持优先级。
 
 
     def _shedual_task(self):
         # noinspection PyTypeChecker
         def callback(amqpstorm_message: amqpstorm.Message):
             body = amqpstorm_message.body
             # self.logger.debug(f'从rabbitmq的 [{self._queue_name}] 队列中 取出的消息是：  {body}')
             self._print_message_get_from_broker('rabbitmq', body)
             body = json.loads(body)
             kw = {'amqpstorm_message': amqpstorm_message, 'body': body}
             self._submit_task(kw)
 
-        rp = RabbitmqPublisherUsingAmqpStorm(self.queue_name)
+        rp = RabbitmqPublisherUsingAmqpStorm(self.queue_name,broker_exclusive_config=self.broker_exclusive_config)
         rp.init_broker()
         rp.channel_wrapper_by_ampqstormbaic.qos(self._concurrent_num)
         rp.channel_wrapper_by_ampqstormbaic.consume(callback=callback, queue=self.queue_name, no_ack=False)
         rp.channel.start_consuming(auto_decode=True)
 
     def _confirm_consume(self, kw):
         # noinspection PyBroadException
```

## funboost/factories/broker_kind__publsiher_consumer_type_map.py

```diff
@@ -1,18 +1,20 @@
 import typing
 
+from funboost.consumers.redis_consumer_priority import RedisPriorityConsumer
 from funboost.publishers.base_publisher import AbstractPublisher
 from funboost.consumers.base_consumer import AbstractConsumer
 
 from funboost.constant import BrokerEnum
 
 from funboost.publishers.http_publisher import HTTPPublisher
 from funboost.publishers.nats_publisher import NatsPublisher
 from funboost.publishers.peewee_publisher import PeeweePublisher
 from funboost.publishers.redis_publisher_lpush import RedisPublisherLpush
+from funboost.publishers.redis_publisher_priority import RedisPriorityPublisher
 from funboost.publishers.redis_pubsub_publisher import RedisPubSubPublisher
 from funboost.publishers.tcp_publisher import TCPPublisher
 from funboost.publishers.txt_file_publisher import TxtFilePublisher
 from funboost.publishers.udp_publisher import UDPPublisher
 from funboost.publishers.zeromq_publisher import ZeroMqPublisher
 from funboost.publishers.kafka_publisher import KafkaPublisher
 from funboost.publishers.local_python_queue_publisher import LocalPythonQueuePublisher
@@ -59,14 +61,15 @@
     BrokerEnum.MEMORY_QUEUE: (LocalPythonQueuePublisher, LocalPythonQueueConsumer),
     BrokerEnum.RABBITMQ_PIKA: (RabbitmqPublisher, RabbitmqConsumer),
     BrokerEnum.MONGOMQ: (MongoMqPublisher, MongoMqConsumer),
     BrokerEnum.PERSISTQUEUE: (PersistQueuePublisher, PersistQueueConsumer),
     BrokerEnum.NSQ: (NsqPublisher, NsqConsumer),
     BrokerEnum.KAFKA: (KafkaPublisher, KafkaConsumer),
     BrokerEnum.REDIS_ACK_ABLE: (RedisPublisher, RedisConsumerAckAble),
+    BrokerEnum.REDIS_PRIORITY:(RedisPriorityPublisher,RedisPriorityConsumer),
     BrokerEnum.ROCKETMQ: (RocketmqPublisher, RocketmqConsumer),
     BrokerEnum.REDIS_STREAM: (RedisStreamPublisher, RedisStreamConsumer),
     BrokerEnum.ZEROMQ: (ZeroMqPublisher, ZeroMqConsumer),
     BrokerEnum.RedisBrpopLpush: (RedisPublisherLpush, RedisBrpopLpushConsumer),
     BrokerEnum.MQTT: (MqttPublisher, MqttConsumer),
     BrokerEnum.HTTPSQS: (HttpsqsPublisher, HttpsqsConsumer),
     BrokerEnum.UDP: (UDPPublisher, UDPConsumer),
```

## funboost/publishers/base_publisher.py

```diff
@@ -38,14 +38,17 @@
                  is_print_detail_exception: bool = None,
                  msg_expire_senconds: int = None,
                  is_using_rpc_mode: bool = None,
 
                  countdown: typing.Union[float, int] = None,
                  eta: datetime.datetime = None,
                  misfire_grace_time: typing.Union[int, None] = None,
+
+                 other_extra_params: dict = None,
+
                  ):
         """
 
         :param function_timeout: 超时杀死
         :param max_retry_times:
         :param is_print_detail_exception:
         :param msg_expire_senconds:
@@ -77,14 +80,16 @@
             raise ValueError('不能同时设置eta和countdown')
         self.eta = eta
         self.countdown = countdown
         self.misfire_grace_time = misfire_grace_time
         if misfire_grace_time is not None and misfire_grace_time < 1:
             raise ValueError(f'misfire_grace_time 的值要么是大于1的整数， 要么等于None')
 
+        self.other_extra_params = other_extra_params
+
     def to_dict(self):
         if isinstance(self.countdown, datetime.datetime):
             self.countdown = time_util.DatetimeConverter(self.countdown).datetime_str
         priority_consuming_control_config_dict = {k: v for k, v in self.__dict__.items() if v is not None}  # 使中间件消息不要太长，框架默认的值不发到中间件。
         return priority_consuming_control_config_dict
 
 
@@ -183,24 +188,22 @@
     def _init_count(self):
         self._current_time = time.time()
         self.count_per_minute = 0
 
     def custom_init(self):
         pass
 
-    def publish(self, msg: typing.Union[str, dict], task_id=None,
-                priority_control_config: PriorityConsumingControlConfig = None):
-        """
-
-        :param msg:函数的入参字典或者字典转json。,例如消费函数是 def add(x,y)，你就发布 {"x":1,"y":2}
-        :param task_id:可以指定task_id,也可以不指定就随机生产uuid
-        :param priority_control_config:优先级配置，消息可以携带优先级配置，覆盖boost的配置。
-        :return:
-        """
-        if isinstance(msg, str):
+    @staticmethod
+    def _get_from_other_extra_params(k: str, msg):
+        msg_dict = json.loads(msg) if isinstance(msg, str) else msg
+        return msg_dict['extra'].get('other_extra_params', {}).get(k, None)
+
+    def _convert_msg(self, msg: typing.Union[str, dict], task_id=None,
+                     priority_control_config: PriorityConsumingControlConfig = None) -> (typing.Dict, typing.Dict, typing.Dict):
+        if isinstance(msg, (str,bytes)):
             msg = json.loads(msg)
         msg_function_kw = copy.deepcopy(msg)
         raw_extra = {}
         if 'extra' in msg:
             msg_function_kw.pop('extra')
             raw_extra = msg['extra']
         if self.publish_params_checker:
@@ -208,14 +211,26 @@
         task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
         extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
                         'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
         if priority_control_config:
             extra_params.update(priority_control_config.to_dict())
         extra_params.update(raw_extra)
         msg['extra'] = extra_params
+        return msg, msg_function_kw, extra_params
+
+    def publish(self, msg: typing.Union[str, dict], task_id=None,
+                priority_control_config: PriorityConsumingControlConfig = None):
+        """
+
+        :param msg:函数的入参字典或者字典转json。,例如消费函数是 def add(x,y)，你就发布 {"x":1,"y":2}
+        :param task_id:可以指定task_id,也可以不指定就随机生产uuid
+        :param priority_control_config:优先级配置，消息可以携带优先级配置，覆盖boost的配置。
+        :return:
+        """
+        msg, msg_function_kw, extra_params = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         decorators.handle_exception(retry_times=10, is_throw_error=True, time_sleep=0.1)(
             self.concrete_realization_of_publish)(json.dumps(msg, ensure_ascii=False))
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
```

## funboost/publishers/celery_publisher.py

```diff
@@ -37,31 +37,15 @@
         # self._celery_app = celery_app
         # self._celery_fun = f
 
         celery_app.conf.task_routes.update({self.queue_name: {"queue": self.queue_name}})
 
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None) -> celery.result.AsyncResult:
-        if isinstance(msg, str):
-            msg = json.loads(msg)
-        msg_function_kw = copy.deepcopy(msg)
-        raw_extra = {}
-        if 'extra' in msg:
-            msg_function_kw.pop('extra')
-            raw_extra = msg['extra']
-        if self.publish_params_checker:
-            self.publish_params_checker.check_params(msg_function_kw)
-        task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
-        extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
-                        'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
-        if priority_control_config:
-            extra_params.update(priority_control_config.to_dict())
-        extra_params.update(raw_extra)
-        msg['extra'] = extra_params
-
+        msg, msg_function_kw, extra_params = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         celery_result = celery_app.send_task(name=self.queue_name, kwargs=msg_function_kw, task_id=extra_params['task_id'])  # type: celery.result.AsyncResult
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
             if time.time() - self._current_time > 10:
```

## funboost/publishers/nameko_publisher.py

```diff
@@ -21,24 +21,15 @@
     """
 
     def custom_init(self):
         self._rpc = ClusterRpcProxy(NAMEKO_CONFIG)
 
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None):
-        if isinstance(msg, str):
-            msg = json.loads(msg)
-        msg_function_kw = copy.copy(msg)
-        if self.publish_params_checker:
-            self.publish_params_checker.check_params(msg)
-        task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
-        msg['extra'] = extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
-                                       'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
-        if priority_control_config:
-            extra_params.update(priority_control_config.to_dict())
+        msg, msg_function_kw, extra_params = self._convert_msg(msg, task_id, priority_control_config)
         t_start = time.time()
         with self._rpc as rpc:
             res = getattr(rpc, self.queue_name).call(**msg_function_kw)
         self.logger.debug(f'调用nameko的 {self.queue_name} service 的 call方法 耗时{round(time.time() - t_start, 4)}秒，入参  {msg_function_kw}')  # 显示msg太长了。
         return res
 
     def concrete_realization_of_publish(self, msg):
```

## funboost/publishers/rabbitmq_amqpstorm_publisher.py

```diff
@@ -2,55 +2,62 @@
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 12:06
 import amqpstorm
 from amqpstorm.basic import Basic as AmqpStormBasic
 from amqpstorm.queue import Queue as AmqpStormQueue
 from funboost import funboost_config_deafult
 from funboost.publishers.base_publisher import AbstractPublisher, deco_mq_conn_error
+from funboost.utils import decorators
 
 
 class RabbitmqPublisherUsingAmqpStorm(AbstractPublisher):
     # 使用amqpstorm包实现的mq操作。
     # 实例属性没在__init__里面写，造成代码补全很麻烦，写在这里做类属性，方便pycharm补全
     connection = amqpstorm.UriConnection
     channel = amqpstorm.Channel
     channel_wrapper_by_ampqstormbaic = AmqpStormBasic
     queue = AmqpStormQueue
     DURABLE = True
 
+    def custom_init(self):
+        arguments = {}
+        if self.broker_exclusive_config['x-max-priority']:
+            arguments['x-max-priority'] = self.broker_exclusive_config['x-max-priority']
+        self.queue_declare_params = dict(queue=self._queue_name, durable=self.DURABLE, arguments=arguments,auto_delete=False)
+
     # noinspection PyAttributeOutsideInit
     # @decorators.synchronized
     def init_broker(self):
         # username=app_config.RABBITMQ_USER, password=app_config.RABBITMQ_PASS, host=app_config.RABBITMQ_HOST, port=app_config.RABBITMQ_PORT, virtual_host=app_config.RABBITMQ_VIRTUAL_HOST, heartbeat=60 * 10
         self.logger.warning(f'使用AmqpStorm包 链接mq')
         self.connection = amqpstorm.UriConnection(
             f'amqp://{funboost_config_deafult.RABBITMQ_USER}:{funboost_config_deafult.RABBITMQ_PASS}@{funboost_config_deafult.RABBITMQ_HOST}:{funboost_config_deafult.RABBITMQ_PORT}/{funboost_config_deafult.RABBITMQ_VIRTUAL_HOST}?heartbeat={60 * 10}&timeout=20000'
         )
         self.channel = self.connection.channel()  # type:amqpstorm.Channel
         self.channel_wrapper_by_ampqstormbaic = AmqpStormBasic(self.channel)
         self.queue = AmqpStormQueue(self.channel)
-        self.queue.declare(queue=self._queue_name, durable=self.DURABLE)
+        self.queue.declare(**self.queue_declare_params)
 
     # @decorators.tomorrow_threads(10)
     @deco_mq_conn_error
-    def concrete_realization_of_publish(self, msg):
+    def concrete_realization_of_publish(self, msg: str):
         self.channel_wrapper_by_ampqstormbaic.publish(exchange='',
                                                       routing_key=self._queue_name,
                                                       body=msg,
-                                                      properties={'delivery_mode': 2}, )
+                                                      properties={'delivery_mode': 2, 'priority': self._get_from_other_extra_params('priroty', msg)}, )
         # nb_print(msg)
 
     @deco_mq_conn_error
     def clear(self):
         self.queue.purge(self._queue_name)
         self.logger.warning(f'清除 {self._queue_name} 队列中的消息成功')
 
     @deco_mq_conn_error
     def get_message_count(self):
         # noinspection PyUnresolvedReferences
-        return self.queue.declare(queue=self._queue_name, durable=True)['message_count']
+        return self.queue.declare(**self.queue_declare_params)['message_count']
 
     # @deco_mq_conn_error
     def close(self):
         self.channel.close()
         self.connection.close()
         self.logger.warning('关闭amqpstorm包 链接mq')
```

## funboost/utils/dependency_packages_in_pythonpath/readme.md

```diff
@@ -1,9 +1,13 @@
 ## 这个文件夹被添加到 sys.path中去了。
 
+funboost __init__.py 第一行就把这个添加到 sys.path了,相当于 export PYTHONPATH 了。
+```python
+from funboost.utils.dependency_packages_in_pythonpath import add_to_pythonpath # 这是把 dependency_packages_in_pythonpath 添加到 PYTHONPATH了。
+```
 
 这个文件夹存放的是三方包或三方包的修改版。
 
 当 import funboost时候会自动 把这个文件夹添加到 sys.path (PYTHONPATH)
 
 
 ## 如果是开发者为了方便pycharm不显示波浪线提示没安装的错误和更好的自动补全提示
```

## Comparing `funboost-23.1.dist-info/LICENSE` & `funboost-23.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-23.1.dist-info/METADATA` & `funboost-23.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 23.1
+Version: 23.3
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

## Comparing `funboost-23.1.dist-info/RECORD` & `funboost-23.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-funboost/__init__.py,sha256=zw3heGt7VlM6lhZCHl5oSGEU0_maNM7HQHwr1vOatvY,2341
+funboost/__init__.py,sha256=b0QCToD6xthLiftBpMU5u_ISXKA4oDe0k_yJAtteD7E,2341
 funboost/__init__old.py,sha256=cSzw-ZQqtAAp5_-7eONXQT5fwz_JbZlRjDQPASDLUHk,20378
-funboost/constant.py,sha256=WXfZxM5uG5Cbjz6tSVRiImaBIGZz_V7b2iBiBbUmIlk,6223
+funboost/constant.py,sha256=X_foUR_tggz8VO_-9z3egC191fBPiq2XxSe1p1ftSkc,6261
 funboost/funboost_config_deafult.py,sha256=CSawbw5Yzkk73wMNOxhxkrkncS-OOSEYismtbK547xA,7358
 funboost/set_frame_config.py,sha256=hz_38C-IXEulYpHQdr1fhsMcdEDCHIsF2la8MkHiIjA,9149
 funboost/assist/celery_helper.py,sha256=YvKP21xUzgazZHeFGq4FTgtd0A1g3BGNWzKLQ3gNygc,4186
 funboost/assist/dramatiq_helper.py,sha256=lRNouO8MyCB_Qj2ppYG4FbMpf-2Aok8QhtGZLH1zWkg,2089
 funboost/assist/huey_helper.py,sha256=VEzMdQDVJJ-ujcOXKw7chrTgvieLz4si3hrjt8gIK38,1760
 funboost/assist/rq_helper.py,sha256=-tUZ00FzkczwBAkbbISPHF-8J0K7HLSZsue39WiF-cM,1509
 funboost/assist/rq_windows_worker.py,sha256=jQlGmU0FWPVoKVP8cyuwTuAca9VfSd75F5Qw_hR04y0,4831
@@ -25,15 +25,15 @@
 funboost/concurrent_pool/backup/async_pool_executor0223.py,sha256=iTxxJFk2lu1P9ZAIkBip3euq3oEQ4_qTODy3xUaOecY,9548
 funboost/concurrent_pool/backup/async_pool_executor_back.py,sha256=vIgUUyF4Zb0jIRPWgNPqyO09YEkQP32kkpGBldqm4qA,9568
 funboost/concurrent_pool/backup/async_pool_executor_janus.py,sha256=OHMWJ9l3EYTpPpcrPrGGKd4K0tmQ2PN8HiX0Dta0EOo,5728
 funboost/consumers/__init__.py,sha256=ZXY_6Kut1VYNQiF5aWEgIWobsW1ht9YUP0TdRZRWFqI,126
 funboost/consumers/base_consumer.py,sha256=G-hmhk6H0F7tbKrwkXSUv1n37J1LXJ_yTffaPMfrJ50,82870
 funboost/consumers/celery_consumer.py,sha256=6CqorZH5pbxIjVwn5gNzcxSbos5YWT8eYqxYyYjgUcY,7574
 funboost/consumers/celery_consumer000.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
-funboost/consumers/confirm_mixin.py,sha256=H0w07PceU2gGf6X1EXvAB5oD7IavzGv96bQTxm-58sE,5877
+funboost/consumers/confirm_mixin.py,sha256=oVBQ1RayIBFOzGNTJ69HdBR_kLd46xd0VfCOKfqDpLA,6033
 funboost/consumers/dramatiq_consumer.py,sha256=kiHM1wpSZykYDomtSGZ2PlMInCDn_8GOGEHqHUD9m0o,2144
 funboost/consumers/http_consumer.py,sha256=3HF8tsH90fUPX3iOmVid_nqW_7hZCFaL7feOkuAM36U,2025
 funboost/consumers/http_consumer000.py,sha256=NXOSiN1qpLAJfJkuF6SjFpWQ28YxMDULzWCBTNMwYe8,4463
 funboost/consumers/httpsqs_consumer.py,sha256=LICZzovaMVrZsJY4GgLrk3EaHz8f9ZZBLKZtWl3frMc,1080
 funboost/consumers/huey_consumer.py,sha256=_Z2lpfAzvs1HqkSouncN7eH1VfyQJPYNZNgv1FbZj-U,1856
 funboost/consumers/kafka_consumer.py,sha256=2BZT5UQIGqjS1emsX--V1J8gWFOhMjCMMiSnWy_Hto0,4217
 funboost/consumers/kafka_consumer_manually_commit.py,sha256=L-GYQrZ91TWCeI-GIDMXYg3LXFcq0mQ1ACu0gp4bkTI,6947
@@ -43,21 +43,22 @@
 funboost/consumers/mqtt_consumer.py,sha256=StlfPUeQ6o0HiZBpt7TlC_r2DjzPHBZBF2xLSxQW13A,2228
 funboost/consumers/nameko_consumer.py,sha256=IVwUxBixUx2m3F_q8Xn-UsnJWXayMpnOIZjICCd6mcU,2183
 funboost/consumers/nats_consumer.py,sha256=lIYLKvMHNReHnNqGtBA4wot4Ncaobtk60zVHFgm-9Zc,1076
 funboost/consumers/nsq_consumer.py,sha256=PaMRsP8oeRg0H_tq4FL7YhNUdOWAqJkjrwZWoYPNkqU,1461
 funboost/consumers/peewee_conusmer.py,sha256=fbspeWbv6F3EsIIBAjkM_FNh2vMyrDsydju23WAVHvE,1238
 funboost/consumers/persist_queue_consumer.py,sha256=8HzRcMFE6OKiF_CL3atC42Ien_yf5daG3LU38YBKWi0,1005
 funboost/consumers/pulsar_consumer.py,sha256=2DuklBV5dSY-_gW2EpRWz8QSy-VjZclj0gJUvLTyJHA,2414
-funboost/consumers/rabbitmq_amqpstorm_consumer.py,sha256=1YtnhlpVK1Nk4FnfFZOog1P9FU916TLnWJuezUGkED8,1721
+funboost/consumers/rabbitmq_amqpstorm_consumer.py,sha256=Qg1Uv4Tk6Tbu9szys6P4U_5BpsOgZuO_kdiR6lb1MlQ,2048
 funboost/consumers/rabbitmq_pika_consumer.py,sha256=9L7CA2wYT-RNpaVfLKrFk6UJtONEIlfuDZYCjxHDOtc,5433
 funboost/consumers/rabbitmq_pika_consumerv0.py,sha256=Yr-GJlgtkYB4qx8hKZZRx8PyCGwKAlSvRFKEf-SBXnM,4674
 funboost/consumers/rabbitmq_rabbitpy_consumer.py,sha256=q-DXy2MHgsFfBssVIlqgziFw2jPkxAT4TyeDnlE0zwI,1260
 funboost/consumers/redis_brpoplpush_consumer.py,sha256=rVdlmODLEQ8_k-gXFnaMFK8LaiKu3EiZMG2q5jmG8qk,3031
 funboost/consumers/redis_consumer.py,sha256=f9nASEQUR3VHk5JH5Plf3RqKXmxogfrshu63RaFnfDM,2829
 funboost/consumers/redis_consumer_ack_able.py,sha256=DlZd76FTPo-AUiTreQd7cSiT5QAM5K9rFItAwLt2n5Y,7545
+funboost/consumers/redis_consumer_priority.py,sha256=avxU89EZuGk-wQeWEpASBU7ustxAHp3KzQcq34wb2Fg,4282
 funboost/consumers/redis_consumer_simple.py,sha256=9D3uvLw_9WOmLmwys1K39DK3gj1ex_q6NXadXwyGwrs,922
 funboost/consumers/redis_filter.py,sha256=TVyT2i9JhmhsJFyQZDx98phTiwBccNTl9fcErEDGXTM,7135
 funboost/consumers/redis_pubsub_consumer.py,sha256=eSy5QBMPaouiQbeGQ3ZaLVpU1BF8g3B_4CAJHFqhmmI,1206
 funboost/consumers/redis_stream_consumer.py,sha256=hPUMBoixd7F0Y9U4A8xC6QyOdM4EJAbXsgocHkRCarQ,6497
 funboost/consumers/rocketmq_consumer.py,sha256=sqJwxNFOz7c-4Dbk5Rgj_iJqDVwRVCGsw_tMTArGc2o,1653
 funboost/consumers/rq_consumer.py,sha256=JX84k6Jiv4pBiQMmnhdJ7s7Qz4ub5TWS4T7qTF-WdlM,876
 funboost/consumers/sqlachemy_consumer.py,sha256=-pY9pvAVUCw_T-1bRKRT37vNGjvv6BK9h-I5kfelpVk,1309
@@ -77,15 +78,15 @@
 funboost/core/function_result_status_saver.py,sha256=6dMLpa74t3zsHF20lqfgAdCeRD1yc1oJcw--Usk-A3c,8819
 funboost/core/get_booster.py,sha256=YlImXa5yjvuON_9JOa2yAlPw0tHj7RET5jBjmbj1gcM,1169
 funboost/core/global_boosters.py,sha256=CDrnKhxEEb-GxTL7JhrDTD1tyhLj7ciAtO1Cy2iyi1Q,340
 funboost/core/helper_funs.py,sha256=JDIawL6BWViC37rOJ9gFS8f4vCaispiA8Y7Zch-VM_o,1193
 funboost/core/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
 funboost/core/muliti_process_enhance.py,sha256=zNodv3Ww5yCmwO6xCh7k8HntFHjIYYJ9EPaGinvPV9Q,3814
 funboost/factories/__init__.py,sha256=s7kKKjR1HU5eMjPD6r5b-SXTVMo1zBp2JjOAtkyt5Yo,178
-funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=HlicHXVG_Pe3ZWoiZl84LSnhiU6fjJnB87gyo5MnKYM,8738
+funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=00VqI85iEh566n_Zb6hs4QFtPzR3ZAejT-gXJFiYbbI,8976
 funboost/factories/consumer_factory.py,sha256=KFvYkx1a7egtSiTLuVsoRMKLUAotx-QJX1jAI8Xzo3s,946
 funboost/factories/publisher_factotry.py,sha256=Vz66GrCxMt7GV5iqyIXSzZcC_eHF8fj-2kYduzbTTpg,2281
 funboost/function_result_web/app.py,sha256=xUSDBwwDA5wQVWFdFBXj9Y1s7BOh2itUw5pCZl0URMw,4841
 funboost/function_result_web/functions.py,sha256=OIPMxc4jv51qnhBxFGfTZnpMx5p4lQflPoTviDTbJUc,7345
 funboost/function_result_web/__pycache__/app.cpython-37.pyc,sha256=p-jwU7xf31KOJhmhNXqj6J79PTxjMbiTU16gAotpSEw,4045
 funboost/function_result_web/__pycache__/functions.cpython-37.pyc,sha256=KuU8DnYhFpYN0p9rdDXE9mqFuE7eKkcXHCNze3aAdOw,3921
 funboost/function_result_web/static/assets/css/custom.css,sha256=3brvjy2aBOTIXcTUK4NV6dX5wFRqx6K2aLu_jQn63jM,7674
@@ -98,38 +99,39 @@
 funboost/function_result_web/static/images/password.png,sha256=0jRivuQAhWKtkS73p8f_KiLy3D39_flqVTrpFKJPNqk,546
 funboost/function_result_web/static/images/tick.png,sha256=S9dZYN4HQzw7JsWPw3ut1dQp4OTJ_Uh2Qp2KUDF1Jv8,2912
 funboost/function_result_web/static/images/user.png,sha256=HxLjNc83WZzZEscZRdmVhGKlPXNdp_EKmmYxafuyb3g,622
 funboost/function_result_web/static/js/jquery-1.11.0.min.js,sha256=ryQZ3RXgnqkTz-lNEw-YcEhnMuV3ZODwLqOEbyBBRu4,96383
 funboost/function_result_web/templates/index.html,sha256=dWe-JFQhsDpoNjSsBF4P6SJWp_KvHX8EP_yECS5r7_o,19501
 funboost/function_result_web/templates/login.html,sha256=q37dj7O0LeyiV38Zd5P1Qn_qmhjdFomuYTRY1Yk48Bo,2007
 funboost/publishers/__init__.py,sha256=xqBHlvsJQVPfbdvP84G0LHmVB7-pFBS7vDnX1Uo9pVY,131
-funboost/publishers/base_publisher.py,sha256=QmK7g-U7vLl06-PbBxkblqDgEOeeRPMHIBMY5POZWqM,15148
-funboost/publishers/celery_publisher.py,sha256=exRiObJcRTpY_PgTc3rvGiu4kRMQ7OA8a4A4yKyzAyE,3755
+funboost/publishers/base_publisher.py,sha256=2eLwOgi6TnuGTRzQmaB7dXg5q52Cl1_10xd_CeXGujk,15844
+funboost/publishers/celery_publisher.py,sha256=ePnHIlO-XevW6zRvAgdnpQixiC5ogZsT0cNYeptcmCE,3073
 funboost/publishers/celery_publisher000.py,sha256=ag2s7MzPPrnNdza3u8vcbDJqtiqbQw4lJJzAVuJ6GF0,3897
 funboost/publishers/confluent_kafka_publisher.py,sha256=cpbyWvZ0T_kM62LWeBKRUuEuMkJAKOof97UUMSz6-Dk,3541
 funboost/publishers/dramatiq_publisher.py,sha256=RoZzfvkS5H-XXcmHGBomuvkQRQBlVyiaCdWpgy0LL9o,1410
 funboost/publishers/http_publisher.py,sha256=pS3z_AVqH6h4PAgqB7usihvzLJP5ZzfPKQRMQfHrJHQ,753
 funboost/publishers/httpsqs_publisher.py,sha256=7cf5ijwrbp4smq6ofndrKisruAqG0Wzfo_d_7bnLUk4,2783
 funboost/publishers/huey_publisher.py,sha256=z1CF18YZkQY6lqeoc6tiJkaYsRjRicbhYYeoHSvdD-w,1101
 funboost/publishers/kafka_publisher.py,sha256=cmlJ0mvwq0Ajlth4VQqwnoe6v_bZ4eIz49GgkiJr-ZU,2160
 funboost/publishers/kombu_publisher.py,sha256=TJt24M_Y4x8wjXHFl2hp6z3Dat6rjuA_xGiqA8RbRLg,5321
 funboost/publishers/local_python_queue_publisher.py,sha256=veskMS5tjeneYU9HmrJLXZSK9_UT48NzHzcljjOoy3g,1365
 funboost/publishers/mongomq_publisher.py,sha256=xQr3KMQEKksX4OEvzPlCl8v1VeBHaoZtYw2QujOUyGo,1874
 funboost/publishers/mqtt_publisher.py,sha256=NKVDE5R12QL99IXgRjJtF4phyW8QaXKxHkqW5p_kXr4,3050
-funboost/publishers/nameko_publisher.py,sha256=HtR8I_NemyJCO2KL-w8geNMhZcoj06_95QZ8qq1-gog,2147
+funboost/publishers/nameko_publisher.py,sha256=k1XHZQgtRz0b9A22rLYrnGB5ghtDsq5MfMuqdk1Lqw0,1662
 funboost/publishers/nats_publisher.py,sha256=hFfaQovij9dm8w-iRN0SgiHHoS_TlrTAjw42dPwCLSA,776
 funboost/publishers/nsq_publisher.py,sha256=Go4UjLd_Vt4JuVtfkmCuuXrmxUXv1y6NaBQJX6s1XUo,1302
 funboost/publishers/peewee_publisher.py,sha256=RsYAqBKf_ZLxkGJeZPWExzG4cpUac7weCeNhcSQ9hZc,1095
 funboost/publishers/persist_queue_publisher.py,sha256=x6qRiR3Ln-jX9KPC5GvBzUzAlmZ0HDjU1KTnILXVJrw,2540
 funboost/publishers/pulsar_publisher.py,sha256=3BqDtywExvTIw1KZWG4kT1uz029uw2YkntLggZ-Ao6A,1238
-funboost/publishers/rabbitmq_amqpstorm_publisher.py,sha256=0o6D7xD8wDalj-FEWfqkZBr_HjyUKRf_CsGOq6_8ygA,2725
+funboost/publishers/rabbitmq_amqpstorm_publisher.py,sha256=C32sQZpjv1iJtFDD6g_q0wI7Arw9i0RDsRVVOBRKzi4,3137
 funboost/publishers/rabbitmq_pika_publisher.py,sha256=jZZw3DUiZ4VqJ6FqZGdv7qo3F_ltzHuKsy_5-j4jkCs,2343
 funboost/publishers/rabbitmq_rabbitpy_publisher.py,sha256=GGXPKxE6-mAjqMIKqwvR9d7L-zuJQcQoU9uRsQLNGas,1953
 funboost/publishers/redis_publisher.py,sha256=mUHxfdHYrUn_Dw59NifN-mFsnj53hOhZDoEFlWs-W5M,3982
 funboost/publishers/redis_publisher_lpush.py,sha256=xEWuCTtbDcKFLTxGrECrbIVapFfUwqX2-GHenMClu-Q,278
+funboost/publishers/redis_publisher_priority.py,sha256=zGhSAvpFVBXfAmfGQdWL9cixdpLhLQ6yR3XvBLnbdF4,2104
 funboost/publishers/redis_publisher_simple.py,sha256=hLVWiDjy9ObGTmv7Vtrz21d18Fxkb52IfO5ZzaXjzMQ,872
 funboost/publishers/redis_pubsub_publisher.py,sha256=_6s7sbcGOSXxN2ZkBSDk9ILskmbj9cZTQyYHLQTYOuI,721
 funboost/publishers/redis_stream_publisher.py,sha256=DLxFcTlze0IdYFoaRmTcY8GCOaRwbj4aBNbylkt9gRA,2037
 funboost/publishers/rocketmq_publisher.py,sha256=vY82WgutDPsS9px6rukU1d3AexmsT_tqSS2dmX-Pw-c,2343
 funboost/publishers/rq_publisher.py,sha256=ANHrYnPTEj7KF_D_ov2L7PAT9swl82kjDazFqN1ULBY,893
 funboost/publishers/sqla_queue_publisher.py,sha256=yUbge08K311-jWlFyOUw6g7-Z-flbxEeWCeCTGnJcic,1215
 funboost/publishers/tcp_publisher.py,sha256=qMecOpgVqwTy-VYyevv4mCR6H5bQhCirRbJmcJIaFCE,1335
@@ -166,16 +168,18 @@
 funboost/utils/dependency_packages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/utils/dependency_packages/mongomq/__init__.py,sha256=yP7LHPsZ5ResiexksmtyJc9HGbMJWwZ0gOvHk2vNcz0,131
 funboost/utils/dependency_packages/mongomq/lock.py,sha256=anmWK7yoFnjW0ovPFuUiEKgIzw_1gymi2-mnyd3ViYY,2486
 funboost/utils/dependency_packages/mongomq/mongomq.py,sha256=A-_Y0OXmCqGHiCdOFWW4V0ciMyp6gIaPPVK95uaqd_k,7902
 funboost/utils/dependency_packages/mongomq/mongomq0000.py,sha256=DEZ_41VvmQD5eao5KOjF_s5_t-kso6zIsipFREm6ckY,7867
 funboost/utils/dependency_packages/mongomq/test.py,sha256=Tcmme3U3KXFSkdknO71bge4aLcWbZkTcyL5ufNZkco4,4811
 funboost/utils/dependency_packages/mongomq/utils.py,sha256=ljhcLhNf3yOc7IgnuRdFqLtwTGynRNd2uXZNRvStAL0,377
+funboost/utils/dependency_packages_in_pythonpath/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py,sha256=eOaK0Cr1yAmLcHhOM5-nV9XxXhQFZQkiaBECY65sFuc,341
-funboost/utils/dependency_packages_in_pythonpath/readme.md,sha256=ZXVbfoLHWKFMaEhY3UF3O1Ac5hIryDlWvV8iEWep7BM,545
+funboost/utils/dependency_packages_in_pythonpath/readme.md,sha256=fazVs-DBVTKan8X-2Jjqo5jxV4Abdaywj4SLzb_BLcA,814
+funboost/utils/dependency_packages_in_pythonpath/__pycache__/__init__.cpython-37.pyc,sha256=Oy1-_q-VLcFLQ7RRp8B-fbBkNOb2SepePLYW4L5DQ6U,165
 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc,sha256=sWX6OxFSOtD3N3H4ndWNS5xusjqwp54NNzddJ8dxMc0,475
 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-37.pyc,sha256=Y9-hpQ_g0oRz3GWiUhB4GUW8rpxoQlQ4rQV17pPscLo,312
 funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-39.pyc,sha256=KoT6tPC8DlM-7KwaYL3tNlnnd9PCjzYJK61JYuRTcKc,316
 funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py,sha256=DPdTb309wR_E5zR3RVoUYuR1jotheJL3PXdqNBHi2yg,1223
 funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py,sha256=o0SVW1qgNTAmKDAO6GoznN9EnibdgBB7XvLU49RXfeg,182652
 funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py,sha256=yplKtDh6CsO-sWqowLgyF5D3kwzcw7npEjlOGA3465k,183
 funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py,sha256=n_Z9ggf3AxW5fXvLEumEUA6gTtovytoXhMD1CWFk6tw,62239
@@ -231,12 +235,12 @@
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
 funboost/utils/times/__init__.py,sha256=Y4bQD3SIA_E7W2YvHq2Qdi0dGM4H2DxyFNdDOuFOq1w,2417
 funboost/utils/times/version.py,sha256=11XfnZVVzOgIhXXdeN_mYfdXThfrsbQHpA0wCjz-hpg,17
-funboost-23.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-23.1.dist-info/METADATA,sha256=NgbajoPP2oHHYl2V01BoEFyhGT2mzK0IVGGoZVv5OtY,26616
-funboost-23.1.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-funboost-23.1.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-23.1.dist-info/RECORD,,
+funboost-23.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-23.3.dist-info/METADATA,sha256=_tShdyF1bWkC8_jhJQyBBkloVBs1g9iLqLY3cXAd8j0,26616
+funboost-23.3.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+funboost-23.3.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-23.3.dist-info/RECORD,,
```

