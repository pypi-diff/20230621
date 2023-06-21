# Comparing `tmp/bullmq-0.5.5.tar.gz` & `tmp/bullmq-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.5.5.tar", last modified: Fri Jun 16 16:50:45 2023, max compression
+gzip compressed data, was "bullmq-0.5.6.tar", last modified: Wed Jun 21 21:37:51 2023, max compression
```

## Comparing `bullmq-0.5.5.tar` & `bullmq-0.5.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.505620 bullmq-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-16 16:50:45.505620 bullmq-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-16 16:48:49.000000 bullmq-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.497620 bullmq-0.5.5/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 16:50:43.000000 bullmq-0.5.5/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.505620 bullmq-0.5.5/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/addJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/changePriority-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getState-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/pause-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/promote-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.505620 bullmq-0.5.5/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.497620 bullmq-0.5.5/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-16 16:50:45.509620 bullmq-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-16 16:48:49.000000 bullmq-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:37:51.807532 bullmq-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-21 21:37:51.807532 bullmq-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-21 21:36:44.000000 bullmq-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:37:51.803532 bullmq-0.5.6/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-21 21:37:49.000000 bullmq-0.5.6/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:37:51.807532 bullmq-0.5.6/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/changePriority-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/getState-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/pause-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/promote-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-21 21:37:24.000000 bullmq-0.5.6/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:37:51.807532 bullmq-0.5.6/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-21 21:36:44.000000 bullmq-0.5.6/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:37:51.803532 bullmq-0.5.6/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-21 21:37:51.000000 bullmq-0.5.6/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-21 21:37:51.000000 bullmq-0.5.6/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:37:51.000000 bullmq-0.5.6/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 21:37:51.000000 bullmq-0.5.6/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 21:37:51.000000 bullmq-0.5.6/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-21 21:37:51.807532 bullmq-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-21 21:36:44.000000 bullmq-0.5.6/setup.py
```

### Comparing `bullmq-0.5.5/PKG-INFO` & `bullmq-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.5
+Version: 0.5.6
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.5/README.md` & `bullmq-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/backoffs.py` & `bullmq-0.5.6/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/addJob-8.lua` & `bullmq-0.5.6/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/changeDelay-3.lua` & `bullmq-0.5.6/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/changePriority-4.lua` & `bullmq-0.5.6/bullmq/commands/changePriority-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.5.6/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/drain-4.lua` & `bullmq-0.5.6/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/getCounts-1.lua` & `bullmq-0.5.6/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/getRanges-1.lua` & `bullmq-0.5.6/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/getState-7.lua` & `bullmq-0.5.6/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/getStateV2-7.lua` & `bullmq-0.5.6/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/isFinished-3.lua` & `bullmq-0.5.6/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-0.5.6/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.5.6/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,16 @@
       eventStreamKey 'event stream' (STREAM)
       maxStalledJobCount  Max stalled job count
       queueKeyPrefix  queue.toKey('')
       timestamp  timestamp
       maxCheckTime  max check time
     Events:
       'stalled' with stalled job id.
-]] local rcall = redis.call
+]]
+local rcall = redis.call
 -- Includes
 --[[
   Function to loop in batches.
   Just a bit of warning, some commands as ZREM
   could receive a maximum of 7000 parameters per call.
 ]]
 local function batches(n, batchSize)
```

### Comparing `bullmq-0.5.5/bullmq/commands/moveToActive-9.lua` & `bullmq-0.5.6/bullmq/commands/moveToActive-9.lua`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     end
     return nextTimestamp
   end
 end
 local function getRateLimitTTL(maxJobs, rateLimiterKey)
   if maxJobs then
     local pttl = rcall("PTTL", rateLimiterKey)
-    if pttl <= 0 then
+    if pttl == 0 then
       rcall("DEL", rateLimiterKey)
     end
     local jobCounter = tonumber(rcall("GET", rateLimiterKey) or 0)
     if jobCounter >= maxJobs then
       if pttl > 0 then
         return pttl
       end
@@ -216,10 +216,10 @@
     -- this script is not really moving, it is preparing the job for processing
     return moveJobFromWaitToActive(KEYS, ARGV[1], target, jobId, ARGV[2], maxJobs, expireTime, opts)
   end
 end
 -- Return the timestamp for the next delayed job if any.
 local nextTimestamp = getNextDelayedTimestamp(KEYS[7])
 if (nextTimestamp ~= nil) then
-  return { 0, 0, 0, nextTimestamp}
+  return { 0, 0, 0, nextTimestamp }
 end
 return { 0, 0, 0, 0}
```

### Comparing `bullmq-0.5.5/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.5.6/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.5.6/bullmq/commands/moveToFinished-12.lua`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
     end
     rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
   end
 end
 local function getRateLimitTTL(maxJobs, rateLimiterKey)
   if maxJobs then
     local pttl = rcall("PTTL", rateLimiterKey)
-    if pttl <= 0 then
+    if pttl == 0 then
       rcall("DEL", rateLimiterKey)
     end
     local jobCounter = tonumber(rcall("GET", rateLimiterKey) or 0)
     if jobCounter >= maxJobs then
       if pttl > 0 then
         return pttl
       end
```

### Comparing `bullmq-0.5.5/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.5.6/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/obliterate-2.lua` & `bullmq-0.5.6/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/promote-6.lua` & `bullmq-0.5.6/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/removeJob-1.lua` & `bullmq-0.5.6/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.5.6/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/reprocessJob-6.lua` & `bullmq-0.5.6/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/retryJob-8.lua` & `bullmq-0.5.6/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/commands/retryJobs-6.lua` & `bullmq-0.5.6/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/event_emitter.py` & `bullmq-0.5.6/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/job.py` & `bullmq-0.5.6/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/queue.py` & `bullmq-0.5.6/bullmq/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     def trimEvents(self, maxLength: int):
         """
         Trim the event stream to an approximately maxLength.
 
         @param maxLength:
         """
-        return self.client.xtrim(self.opts.get("prefix", f"bull:{self.name}:events"), "MAXLEN", "~", maxLength)
+        return self.client.xtrim(f"{self.prefix}:{self.name}:events", maxlen = maxLength, approximate = "~")
 
     async def getJobCounts(self, *types):
         """
         Returns the job counts for each type specified or every list/set in the queue by default.
 
         @returns: An object, key (type) and value (count)
         """
```

### Comparing `bullmq-0.5.5/bullmq/redis_connection.py` & `bullmq-0.5.6/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/scripts.py` & `bullmq-0.5.6/bullmq/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         result = await self.commands["moveToDelayed"](keys=keys, args=args)
 
         if result is not None:
             if result < 0:
                 raise self.finishedErrors(result, job_id, 'moveToDelayed', 'active')
         return None
 
-    async def remove(self, job_id: str):
+    def remove(self, job_id: str):
         keys = self.getKeys([''])
         args = [job_id]
 
         return self.commands["removeJob"](keys=keys, args=args)
 
     def getCounts(self, types):
         keys = self.getKeys([''])
```

### Comparing `bullmq-0.5.5/bullmq/timer.py` & `bullmq-0.5.6/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/types/job_options.py` & `bullmq-0.5.6/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/types/worker_options.py` & `bullmq-0.5.6/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq/worker.py` & `bullmq-0.5.6/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/bullmq.egg-info/PKG-INFO` & `bullmq-0.5.6/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.5
+Version: 0.5.6
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.5/bullmq.egg-info/SOURCES.txt` & `bullmq-0.5.6/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.5/setup.py` & `bullmq-0.5.6/setup.py`

 * *Files identical despite different names*

