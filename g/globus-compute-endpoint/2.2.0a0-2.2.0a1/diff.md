# Comparing `tmp/globus-compute-endpoint-2.2.0a0.tar.gz` & `tmp/globus-compute-endpoint-2.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.2.0a0.tar", last modified: Tue Jun 20 18:07:15 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.2.0a1.tar", last modified: Wed Jun 21 18:53:29 2023, max compression
```

## Comparing `globus-compute-endpoint-2.2.0a0.tar` & `globus-compute-endpoint-2.2.0a1.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.087910 globus-compute-endpoint-2.2.0a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.0a0/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-20 18:07:15.087990 globus-compute-endpoint-2.2.0a0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.0a0/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.075462 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    16673 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.077930 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.078953 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/
--rw-r--r--   0 lei        (501) staff       (20)       41 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6129 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/config.py
--rw-r--r--   0 lei        (501) staff       (20)      766 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)     3448 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/model.py
--rw-r--r--   0 lei        (501) staff       (20)     7326 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/utils.py
--rw-r--r--   0 lei        (501) staff       (20)    26645 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    20355 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    24826 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.079869 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.080215 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.081621 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/
--rw-r--r--   0 lei        (501) staff       (20)      318 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     5954 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/base.py
--rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/globus_compute.py
--rw-r--r--   0 lei        (501) staff       (20)     4336 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/helper.py
--rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/process_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     3715 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/thread_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.081785 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.085518 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    50314 2023-06-06 16:42:30.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    36129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.085755 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.086326 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.087150 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-06-20 17:58:38.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.076163 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     3092 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      344 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-20 18:07:15.088238 globus-compute-endpoint-2.2.0a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3685 2023-06-20 17:58:29.000000 globus-compute-endpoint-2.2.0a0/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.087677 globus-compute-endpoint-2.2.0a0/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.0a0/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.026301 globus-compute-endpoint-2.2.0a1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       83 2023-06-21 18:50:46.000000 globus-compute-endpoint-2.2.0a1/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-21 18:53:29.026365 globus-compute-endpoint-2.2.0a1/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.0a1/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.013800 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    16673 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.016674 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.017964 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/
+-rw-r--r--   0 lei        (501) staff       (20)       41 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6129 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      766 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)      117 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/default_config.yaml
+-rw-r--r--   0 lei        (501) staff       (20)     3448 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/model.py
+-rw-r--r--   0 lei        (501) staff       (20)     7326 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)    26645 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    20355 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    24826 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.018912 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.019230 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      110 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.020508 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/
+-rw-r--r--   0 lei        (501) staff       (20)      318 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     5954 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/globus_compute.py
+-rw-r--r--   0 lei        (501) staff       (20)     4336 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/helper.py
+-rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/process_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     3715 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/thread_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.020639 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.024293 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    50314 2023-06-06 16:42:30.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    36129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8499 2023-06-21 18:50:27.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.024472 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.024964 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.025667 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-06-21 18:52:01.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.014518 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     3152 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      344 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-06-21 18:53:29.000000 globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-21 18:53:29.026607 globus-compute-endpoint-2.2.0a1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3685 2023-06-21 18:51:52.000000 globus-compute-endpoint-2.2.0a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:29.026116 globus-compute-endpoint-2.2.0a1/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a1/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.0a1/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a1/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.2.0a0/LICENSE` & `globus-compute-endpoint-2.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/PKG-INFO` & `globus-compute-endpoint-2.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.0a0
+Version: 2.2.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.0a0/PyPI.md` & `globus-compute-endpoint-2.2.0a1/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/config.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/default_config.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/model.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/model.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/utils.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/config/utils.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/globus_compute.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/globus_compute.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/helper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/process_pool.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/process_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/thread_pool.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/engines/thread_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/logging_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 import logging.config
 import logging.handlers
 import os
 import pathlib
 import re
 import sys
 import uuid
+from datetime import datetime
 
 log = logging.getLogger(__name__)
 
 DEFAULT_FORMAT = (
-    "%(created)f %(asctime)s %(levelname)s %(processName)s-%(process)d "
+    "%(asctime)s %(levelname)s %(processName)s-%(process)d "
     "%(threadName)s-%(thread)d %(name)s:%(lineno)d %(funcName)s "
     "%(message)s"
 )
 
 _ital = "\033[3m"
 _redb = "\033[41m"
 _teal = "\033[32m"
@@ -29,28 +30,36 @@
 _yelb = "\033[43m"
 _purp = "\033[35m"
 _cyan = "\033[36m"
 _gray = "\033[37m"
 _grayonb = "\033[37;40m"
 _r = "\033[m"
 _C_BASE = (
-    f"{_teal}%(created)f{_r} {_yel}%(asctime)s{_r} {_ital}%(levelname)s{_r}"
+    f"{_yel}%(asctime)s{_r} {_ital}%(levelname)s{_r}"
     " %(processName)s-%(process)d %(threadName)s-%(thread)d"
     f" %(name)s:{_cyan}%(lineno)d{_r} {_purp}%(funcName)s{_r}"
 )
 COLOR_ERROR = _redb
 COLOR_WARNING = _yelb
 COLOR_INFO = _gray
 COLOR_DEBUG = _grayonb
 C_ERROR_FMT = _C_BASE + f" {COLOR_ERROR}%(message)s{_r}"
 C_WARNING_FMT = _C_BASE + f" {COLOR_WARNING}%(message)s{_r}"
 C_INFO_FMT = _C_BASE + f" {COLOR_INFO}%(message)s{_r}"
 C_DEBUG_FMT = _C_BASE + f" {COLOR_DEBUG}%(message)s{_r}"
 
 
+class DatetimeFormatter(logging.Formatter):
+    def formatTime(self, record, datefmt=None):
+        ct = datetime.fromtimestamp(record.created)
+        if not datefmt:
+            datefmt = self.default_time_format
+        return ct.strftime(datefmt)
+
+
 class ComputeConsoleFormatter(logging.Formatter):
     """
     For internal use only.
     This formatter handles output to standard streams in the following way:
 
     if 'debug' is False (default):
         info messages and below are treated as "user output" and are minimally decorated
@@ -62,22 +71,20 @@
 
     _u = "[0-9A-Fa-f]"  # convenience
     _uuid_re = f"{_u}{{8}}-{_u}{{4}}-{_u}{{4}}-{_u}{{4}}-{_u}{{12}}"
     # match uuids for colorization that have not otherwise already been colorized
     uuid_re = re.compile(rf"(?<!\dm)({_uuid_re})")
 
     def __init__(
-        self,
-        debug: bool = False,
-        no_color: bool = False,
-        fmt: str = "",
-        datefmt: str = "%Y-%m-%d %H:%M:%S",
+        self, debug: bool = False, no_color: bool = False, fmt: str = "", **kwargs
     ) -> None:
         super().__init__()
 
+        kwargs.setdefault("datefmt", "%Y-%m-%d %H:%M:%S,%f")
+
         self.use_color = debug and not no_color and sys.stderr.isatty()
 
         if fmt:
             d_fmt, i_fmt, w_fmt, e_fmt = fmt, fmt, fmt, fmt
         else:
             d_fmt, i_fmt, w_fmt, e_fmt = (
                 C_DEBUG_FMT,
@@ -90,21 +97,21 @@
             ansi_re = re.compile("\033.*?m")
             d_fmt = ansi_re.sub("", d_fmt)
             i_fmt = ansi_re.sub("", i_fmt)
             w_fmt = ansi_re.sub("", w_fmt)
             e_fmt = ansi_re.sub("", e_fmt)
 
         if debug:
-            self._error_formatter = logging.Formatter(fmt=e_fmt, datefmt=datefmt)
-            self._warning_formatter = logging.Formatter(fmt=w_fmt, datefmt=datefmt)
-            self._debug_formatter = logging.Formatter(fmt=d_fmt, datefmt=datefmt)
-            self._info_formatter = logging.Formatter(fmt=i_fmt, datefmt=datefmt)
+            self._error_formatter = DatetimeFormatter(fmt=e_fmt, **kwargs)
+            self._warning_formatter = DatetimeFormatter(fmt=w_fmt, **kwargs)
+            self._debug_formatter = DatetimeFormatter(fmt=d_fmt, **kwargs)
+            self._info_formatter = DatetimeFormatter(fmt=i_fmt, **kwargs)
         else:
-            self._info_formatter = logging.Formatter(fmt="> %(message)s")
-            self._warning_formatter = logging.Formatter(fmt=w_fmt, datefmt=datefmt)
+            self._info_formatter = DatetimeFormatter(fmt="> %(message)s")
+            self._warning_formatter = DatetimeFormatter(fmt=w_fmt, **kwargs)
             self._error_formatter = self._warning_formatter
             self._debug_formatter = self._warning_formatter
 
     def format(self, record: logging.LogRecord):
         if self.use_color:
             # Highlight all UUIDs
             if record.levelno > logging.WARNING:
@@ -154,21 +161,23 @@
     if console_enabled:
         log_handlers.append("console")
 
     return {
         "version": 1,
         "formatters": {
             "streamfmt": {
-                "()": "globus_compute_endpoint.logging_config.ComputeConsoleFormatter",
+                "()": ComputeConsoleFormatter,
                 "debug": debug,
                 "no_color": no_color,
+                "datefmt": "%Y-%m-%d %H:%M:%S,%f",
             },
             "filefmt": {
+                "()": DatetimeFormatter,
                 "format": DEFAULT_FORMAT,
-                "datefmt": "%Y-%m-%d %H:%M:%S",
+                "datefmt": "%Y-%m-%d %H:%M:%S,%f",
             },
         },
         "handlers": {
             "console": {
                 "class": "logging.StreamHandler",
                 "level": "DEBUG",
                 "formatter": "streamfmt",
@@ -197,17 +206,18 @@
 
 
 def _get_stream_dict_config(debug: bool, no_color: bool) -> dict:
     return {
         "version": 1,
         "formatters": {
             "streamfmt": {
-                "()": "globus_compute_endpoint.logging_config.ComputeConsoleFormatter",
+                "()": ComputeConsoleFormatter,
                 "debug": debug,
                 "no_color": no_color,
+                "datefmt": "%Y-%m-%d %H:%M:%S,%f",
             },
         },
         "handlers": {
             "console": {
                 "class": "logging.StreamHandler",
                 "level": "DEBUG" if debug else "INFO",
                 "formatter": "streamfmt",
```

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.0a0"
+__version__ = "2.2.0a1"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.0a0
+Version: 2.2.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.2.0a1/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 globus_compute_endpoint/endpoint/interchange.py
 globus_compute_endpoint/endpoint/messages_compat.py
 globus_compute_endpoint/endpoint/result_store.py
 globus_compute_endpoint/endpoint/taskqueue.py
 globus_compute_endpoint/endpoint/config/__init__.py
 globus_compute_endpoint/endpoint/config/config.py
 globus_compute_endpoint/endpoint/config/default_config.py
+globus_compute_endpoint/endpoint/config/default_config.yaml
 globus_compute_endpoint/endpoint/config/model.py
 globus_compute_endpoint/endpoint/config/utils.py
 globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
 globus_compute_endpoint/endpoint/rabbit_mq/base.py
 globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
 globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
 globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
```

### Comparing `globus-compute-endpoint-2.2.0a0/setup.py` & `globus-compute-endpoint-2.2.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.2.0a0",
+    "globus-compute-sdk==2.2.0a1",
     "globus-compute-common==0.2.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.2.0a0/tests/conftest.py` & `globus-compute-endpoint-2.2.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.0a0/tests/utils.py` & `globus-compute-endpoint-2.2.0a1/tests/utils.py`

 * *Files identical despite different names*

