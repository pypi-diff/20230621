# Comparing `tmp/hrflow-2.1.0.tar.gz` & `tmp/hrflow-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrflow-2.1.0.tar", last modified: Fri Mar 10 09:03:13 2023, max compression
+gzip compressed data, was "dist/hrflow-3.0.0.tar", last modified: Wed Jun 21 10:58:13 2023, max compression
```

## Comparing `hrflow-2.1.0.tar` & `hrflow-3.0.0.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.812633 hrflow-2.1.0/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     2454 2023-03-07 10:18:45.000000 hrflow-2.1.0/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      202 2023-03-07 10:18:45.000000 hrflow-2.1.0/.gitmodules
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18309 2023-03-09 13:39:22.000000 hrflow-2.1.0/Documentation.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-07 10:18:45.000000 hrflow-2.1.0/LICENSE.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      255 2023-03-10 09:03:13.812633 hrflow-2.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3899 2023-03-09 13:39:22.000000 hrflow-2.1.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-03-07 10:18:45.000000 hrflow-2.1.0/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.796633 hrflow-2.1.0/examples/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.804633 hrflow-2.1.0/examples/colab/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24398 2023-03-07 10:18:45.000000 hrflow-2.1.0/examples/colab/build_personalized_ai_hr_models.ipynb
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19481 2023-03-07 10:18:45.000000 hrflow-2.1.0/examples/colab/implement_hrflow_in_5min.ipynb
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.804633 hrflow-2.1.0/hrflow/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      176 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2023-03-10 09:03:02.000000 hrflow-2.1.0/hrflow/__version__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.804633 hrflow-2.1.0/hrflow/hrflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.804633 hrflow-2.1.0/hrflow/hrflow/board/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/board/__init__.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5929 2023-03-09 14:29:43.000000 hrflow-2.1.0/hrflow/hrflow/hrflow.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.804633 hrflow-2.1.0/hrflow/hrflow/job/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/job/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      852 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/job/embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3497 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/job/indexing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/job/parsing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      183 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/job/reasoning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2397 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/job/scoring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1700 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/job/searching.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5277 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/job/storing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.808633 hrflow-2.1.0/hrflow/hrflow/profile/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1155 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/profile/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1195 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      832 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/exporter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/importer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3107 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/profile/indexing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4582 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/parsing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      187 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/reasoning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/revealing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2387 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/scoring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1720 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/profile/searching.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5628 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/profile/storing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.808633 hrflow-2.1.0/hrflow/hrflow/source/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1723 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/source/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.812633 hrflow-2.1.0/hrflow/hrflow/text/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      917 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      603 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      966 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/imaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/linking.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      841 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/ocr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/parsing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/revealing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/text/tagging.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.812633 hrflow-2.1.0/hrflow/hrflow/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3688 2023-03-09 13:39:22.000000 hrflow-2.1.0/hrflow/hrflow/utils/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.812633 hrflow-2.1.0/hrflow/hrflow/webhook/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6155 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/webhook/__init__.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      418 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/webhook/base64Wrapper.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      469 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/webhook/bytesutils.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      391 2023-03-07 10:18:45.000000 hrflow-2.1.0/hrflow/hrflow/webhook/hmacutils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.804633 hrflow-2.1.0/hrflow.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      255 2023-03-10 09:03:13.000000 hrflow-2.1.0/hrflow.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1678 2023-03-10 09:03:13.000000 hrflow-2.1.0/hrflow.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-10 09:03:13.000000 hrflow-2.1.0/hrflow.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-07 21:41:14.000000 hrflow-2.1.0/hrflow.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-03-10 09:03:13.000000 hrflow-2.1.0/hrflow.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-03-10 09:03:13.000000 hrflow-2.1.0/hrflow.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.812633 hrflow-2.1.0/libs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 10:18:45.000000 hrflow-2.1.0/libs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    76494 2023-03-09 13:39:22.000000 hrflow-2.1.0/poetry.lock
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      471 2023-03-09 13:39:22.000000 hrflow-2.1.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-10 09:03:13.812633 hrflow-2.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-03-09 13:39:22.000000 hrflow-2.1.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-10 09:03:13.812633 hrflow-2.1.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 10:18:45.000000 hrflow-2.1.0/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      145 2023-03-07 10:18:45.000000 hrflow-2.1.0/tests/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7977 2023-03-07 10:18:45.000000 hrflow-2.1.0/tests/test_api.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.662356 hrflow-3.0.0/
+-rwxrwxr-x   0 parsing   (1000) parsing   (1000)     2490 2023-06-21 09:07:18.000000 hrflow-3.0.0/.gitignore
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      202 2023-06-20 08:34:01.000000 hrflow-3.0.0/.gitmodules
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)    18309 2023-06-20 08:34:01.000000 hrflow-3.0.0/Documentation.md
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1069 2023-06-20 08:34:01.000000 hrflow-3.0.0/LICENSE.txt
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      382 2023-06-21 10:57:45.000000 hrflow-3.0.0/Makefile
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      255 2023-06-21 10:58:13.662356 hrflow-3.0.0/PKG-INFO
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     3899 2023-06-20 08:34:01.000000 hrflow-3.0.0/README.md
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)       25 2023-06-20 08:34:01.000000 hrflow-3.0.0/README.rst
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.626357 hrflow-3.0.0/examples/
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.634357 hrflow-3.0.0/examples/colab/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)    24398 2023-06-20 08:34:01.000000 hrflow-3.0.0/examples/colab/build_personalized_ai_hr_models.ipynb
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)    19481 2023-06-20 08:34:01.000000 hrflow-3.0.0/examples/colab/implement_hrflow_in_5min.ipynb
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.634357 hrflow-3.0.0/examples/job/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)    11668 2023-06-21 10:29:02.000000 hrflow-3.0.0/examples/job/job_endpoints_examples.ipynb
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.638357 hrflow-3.0.0/examples/profile/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)    56140 2023-06-21 10:29:13.000000 hrflow-3.0.0/examples/profile/profile_endpoints_examples.ipynb
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.638357 hrflow-3.0.0/hrflow/
+-rwxrwxr-x   0 parsing   (1000) parsing   (1000)      176 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/__init__.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      232 2023-06-21 10:22:09.000000 hrflow-3.0.0/hrflow/__version__.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.642357 hrflow-3.0.0/hrflow/hrflow/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)        0 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/__init__.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.642357 hrflow-3.0.0/hrflow/hrflow/board/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1702 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/board/__init__.py
+-rwxrwxr-x   0 parsing   (1000) parsing   (1000)     5943 2023-06-21 10:10:40.000000 hrflow-3.0.0/hrflow/hrflow/hrflow.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.642357 hrflow-3.0.0/hrflow/hrflow/job/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      572 2023-06-20 15:36:38.000000 hrflow-3.0.0/hrflow/hrflow/job/__init__.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      850 2023-06-20 09:17:44.000000 hrflow-3.0.0/hrflow/hrflow/job/embedding.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      206 2023-06-20 09:17:20.000000 hrflow-3.0.0/hrflow/hrflow/job/parsing.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      183 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/job/reasoning.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     2397 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/job/scoring.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1731 2023-06-20 09:17:40.000000 hrflow-3.0.0/hrflow/hrflow/job/searching.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     8309 2023-06-20 15:35:54.000000 hrflow-3.0.0/hrflow/hrflow/job/storing.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.646357 hrflow-3.0.0/hrflow/hrflow/profile/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1064 2023-06-20 15:07:08.000000 hrflow-3.0.0/hrflow/hrflow/profile/__init__.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1013 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/attachment.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1195 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/embedding.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      832 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/exporter.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1059 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/importer.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     4582 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/parsing.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      187 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/reasoning.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      984 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/revealing.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     2387 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/scoring.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1720 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/profile/searching.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     8125 2023-06-20 14:51:48.000000 hrflow-3.0.0/hrflow/hrflow/profile/storing.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.646357 hrflow-3.0.0/hrflow/hrflow/rating/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     5516 2023-06-21 10:19:05.000000 hrflow-3.0.0/hrflow/hrflow/rating/__init__.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.650357 hrflow-3.0.0/hrflow/hrflow/source/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1723 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/source/__init__.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.654357 hrflow-3.0.0/hrflow/hrflow/text/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      917 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/__init__.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      603 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/embedding.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      966 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/imaging.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      728 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/linking.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      841 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/ocr.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      594 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/parsing.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      576 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/revealing.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     2131 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/text/tagging.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.654357 hrflow-3.0.0/hrflow/hrflow/tracking/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     5807 2023-06-20 16:49:05.000000 hrflow-3.0.0/hrflow/hrflow/tracking/__init__.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.654357 hrflow-3.0.0/hrflow/hrflow/utils/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     3688 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/utils/__init__.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.658357 hrflow-3.0.0/hrflow/hrflow/webhook/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     6155 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/webhook/__init__.py
+-rwxrwxr-x   0 parsing   (1000) parsing   (1000)      418 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/webhook/base64Wrapper.py
+-rwxrwxr-x   0 parsing   (1000) parsing   (1000)      469 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/webhook/bytesutils.py
+-rwxrwxr-x   0 parsing   (1000) parsing   (1000)      391 2023-06-20 08:34:01.000000 hrflow-3.0.0/hrflow/hrflow/webhook/hmacutils.py
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.638357 hrflow-3.0.0/hrflow.egg-info/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      255 2023-06-21 10:58:13.000000 hrflow-3.0.0/hrflow.egg-info/PKG-INFO
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     1746 2023-06-21 10:58:13.000000 hrflow-3.0.0/hrflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)        1 2023-06-21 10:58:13.000000 hrflow-3.0.0/hrflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)        1 2023-06-21 10:58:13.000000 hrflow-3.0.0/hrflow.egg-info/not-zip-safe
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)       22 2023-06-21 10:58:13.000000 hrflow-3.0.0/hrflow.egg-info/requires.txt
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)       13 2023-06-21 10:58:13.000000 hrflow-3.0.0/hrflow.egg-info/top_level.txt
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)       38 2023-06-21 10:58:13.662356 hrflow-3.0.0/setup.cfg
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      790 2023-06-20 08:34:01.000000 hrflow-3.0.0/setup.py
+-rwxrwxr-x   0 parsing   (1000) parsing   (1000)     1001 2023-06-21 09:49:51.000000 hrflow-3.0.0/tag.sh
+drwxrwxr-x   0 parsing   (1000) parsing   (1000)        0 2023-06-21 10:58:13.658357 hrflow-3.0.0/tests/
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)        0 2023-06-20 08:34:01.000000 hrflow-3.0.0/tests/__init__.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)      145 2023-06-20 08:34:01.000000 hrflow-3.0.0/tests/config.py
+-rw-rw-r--   0 parsing   (1000) parsing   (1000)     7977 2023-06-20 08:34:01.000000 hrflow-3.0.0/tests/test_api.py
```

### Comparing `hrflow-2.1.0/.gitignore` & `hrflow-3.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -179,7 +179,13 @@
 *.pyc
 __pycache__/
 local_settings.py
 db.sqlite3
 media
 
 deploy/*.zip
+
+
+# Pyre type checker
+.pyre/
+
+.envrc
```

### Comparing `hrflow-2.1.0/Documentation.md` & `hrflow-3.0.0/Documentation.md`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/LICENSE.txt` & `hrflow-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/README.md` & `hrflow-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/examples/colab/build_personalized_ai_hr_models.ipynb` & `hrflow-3.0.0/examples/colab/build_personalized_ai_hr_models.ipynb`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/examples/colab/implement_hrflow_in_5min.ipynb` & `hrflow-3.0.0/examples/colab/implement_hrflow_in_5min.ipynb`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/board/__init__.py` & `hrflow-3.0.0/hrflow/hrflow/board/__init__.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/hrflow.py` & `hrflow-3.0.0/hrflow/hrflow/hrflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from .board import Board
 from .job import Job
 from .text import Text
 from .profile import Profile
 from .webhook import Webhook
 from .source import Source
+from .tracking import Tracking
+from .rating import Rating
 
 
 CLIENT_API_URL = "https://api.hrflow.ai/v1/"
 
 
 class Hrflow(object):
     """client api wrapper client."""
@@ -42,18 +44,19 @@
         """
         self.api_url = api_url
         self.auth_header = {"X-API-KEY": api_secret, "X-USER-EMAIL": api_user}
         self.webhook_secret = webhook_secret
         self.job = Job(self)
         self.profile = Profile(self)
         self.text = Text(self)
-        self.document = Text(self) # This is a patch to avoid breaking changes in the API. Will be in future release.
         self.webhooks = Webhook(self)
         self.source = Source(self)
         self.board = Board(self)
+        self.tracking = Tracking(self)
+        self.rating = Rating(self)
 
     def _create_request_url(self, resource_url):
         return "{api_endpoint}{resource_url}".format(
             api_endpoint=self.api_url, resource_url=resource_url
         )
 
     def _fill_headers(self, header, base={}):
```

### Comparing `hrflow-2.1.0/hrflow/hrflow/job/__init__.py` & `hrflow-3.0.0/hrflow/hrflow/job/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from .parsing import JobParsing
-from .indexing import JobIndexing
 from .embedding import JobEmbedding
 from .searching import JobSearching
 from .scoring import JobScoring
 from .reasoning import JobReasoning
 from .storing import JobStoring
 
 
-class Job(object):
+class Job:
     def __init__(self, client):
         self.client = client
         self.parsing = JobParsing(self.client)
-        self.indexing = JobIndexing(self.client)
         self.embedding = JobEmbedding(self.client)
         self.searching = JobSearching(self.client)
         self.scoring = JobScoring(self.client)
         self.reasoning = JobReasoning(self.client)
         self.storing = JobStoring(self.client)
```

### Comparing `hrflow-2.1.0/hrflow/hrflow/job/embedding.py` & `hrflow-3.0.0/hrflow/hrflow/job/embedding.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..utils import format_item_payload, validate_response
 
 
-class JobEmbedding():
+class JobEmbedding:
     """Manage embedding related job calls."""
 
     def __init__(self, api):
         """Init."""
         self.client = api
 
     def get(self, board_key, key=None, reference=None):
@@ -20,10 +20,10 @@
             reference:              <string>
                                     job_reference
 
         Returns
             parsing information
 
         """
-        query_params = format_item_payload('job', board_key, key, reference)
-        response = self.client.get('job/embedding', query_params)
+        query_params = format_item_payload("job", board_key, key, reference)
+        response = self.client.get("job/embedding", query_params)
         return validate_response(response)
```

### Comparing `hrflow-2.1.0/hrflow/hrflow/job/scoring.py` & `hrflow-3.0.0/hrflow/hrflow/job/scoring.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/job/searching.py` & `hrflow-3.0.0/hrflow/hrflow/profile/searching.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import json
 
 from ..utils import validate_provider_keys, validate_limit, validate_page, validate_value, validate_response
 
 from ..utils import ORDER_BY_VALUES, SORT_BY_VALUES, STAGE_VALUES
 
 
-class JobSearching():
+class ProfileSearching():
     """Manage stage related profile calls."""
 
     def __init__(self, api):
         """Init."""
         self.client = api
 
-    def list(self, board_keys=None, stage=None, page=1, limit=30, sort_by='created_at', order_by=None, **kwargs):
+    def list(self, source_keys=None, stage=None, page=1, limit=30, sort_by='created_at', order_by=None, **kwargs):
         """
         Retrieve the scoring information.
 
         Args:
-            board_keys:         <list>
-                                board_keys
+            source_keys:        <list>
+                                source_keys
             stage:              <string>
                                 stage
             limit:              <int> (default to 30)
                                 number of fetched profiles/page
             page:               <int> REQUIRED default to 1
                                 number of the page associated to the pagination
             sort_by:            <string>
             order_by:           <string>
 
         Returns
             parsing information
 
         """
 
-        query_params = {'board_keys': json.dumps(validate_provider_keys(board_keys)),
-                        'stage': validate_value(stage, STAGE_VALUES),
+        query_params = {'source_keys': json.dumps(validate_provider_keys(source_keys)),
+                        'stage': validate_value(stage, STAGE_VALUES, "stage"),
                         'limit': validate_limit(limit),
                         'page': validate_page(page),
                         'sort_by': validate_value(sort_by, SORT_BY_VALUES, "sort by"),
-                        'order_by': validate_value(order_by, ORDER_BY_VALUES, "order by")
+                        'order_by': validate_value(order_by, ORDER_BY_VALUES, "oder by")
                         }
 
         params = {**query_params, **kwargs}
-        response = self.client.get('jobs/searching', params)
+        response = self.client.get('profiles/searching', params)
         return validate_response(response)
```

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/__init__.py` & `hrflow-3.0.0/hrflow/hrflow/profile/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Profile related calls."""
 from .attachment import ProfileAttachments
 from .parsing import ProfileParsing
-from .indexing import ProfileIndexing
+from .storing import ProfileStoring
 from .revealing import ProfileRevealing
 from .embedding import ProfileEmbedding
 from .searching import ProfileSearching
 from .scoring import ProfileScoring
 from .reasoning import ProfileReasoning
-from .storing import ProfileStoring
 
 
 class Profile(object):
     def __init__(self, client):
         """
         Initialize Profile object with hrflow client.
 
@@ -21,14 +20,13 @@
         Returns
             Profile instance object.
 
         """
         self.client = client
         self.attachment = ProfileAttachments(self.client)
         self.parsing = ProfileParsing(self.client)
-        self.indexing = ProfileIndexing(self.client)
+        self.storing = ProfileStoring(self.client)
         self.embedding = ProfileEmbedding(self.client)
         self.revealing = ProfileRevealing(self.client)
         self.scoring = ProfileScoring(self.client)
         self.searching = ProfileSearching(self.client)
         self.reasoning = ProfileReasoning(self.client)
-        self.storing = ProfileStoring(self.client)
```

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/attachment.py` & `hrflow-3.0.0/hrflow/hrflow/profile/attachment.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/embedding.py` & `hrflow-3.0.0/hrflow/hrflow/profile/embedding.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/exporter.py` & `hrflow-3.0.0/hrflow/hrflow/profile/exporter.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/importer.py` & `hrflow-3.0.0/hrflow/hrflow/profile/importer.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/parsing.py` & `hrflow-3.0.0/hrflow/hrflow/profile/parsing.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/revealing.py` & `hrflow-3.0.0/hrflow/hrflow/profile/revealing.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/scoring.py` & `hrflow-3.0.0/hrflow/hrflow/profile/scoring.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/searching.py` & `hrflow-3.0.0/hrflow/hrflow/job/searching.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 import json
 
-from ..utils import validate_provider_keys, validate_limit, validate_page, validate_value, validate_response
+from ..utils import (
+    validate_provider_keys,
+    validate_limit,
+    validate_page,
+    validate_value,
+    validate_response,
+)
 
 from ..utils import ORDER_BY_VALUES, SORT_BY_VALUES, STAGE_VALUES
 
 
-class ProfileSearching():
+class JobSearching:
     """Manage stage related profile calls."""
 
     def __init__(self, api):
         """Init."""
         self.client = api
 
-    def list(self, source_keys=None, stage=None, page=1, limit=30, sort_by='created_at', order_by=None, **kwargs):
+    def list(
+        self,
+        board_keys=None,
+        stage=None,
+        page=1,
+        limit=30,
+        sort_by="created_at",
+        order_by=None,
+        **kwargs
+    ):
         """
         Retrieve the scoring information.
 
         Args:
-            source_keys:        <list>
-                                source_keys
+            board_keys:         <list>
+                                board_keys
             stage:              <string>
                                 stage
             limit:              <int> (default to 30)
                                 number of fetched profiles/page
             page:               <int> REQUIRED default to 1
                                 number of the page associated to the pagination
             sort_by:            <string>
             order_by:           <string>
 
         Returns
             parsing information
 
         """
 
-        query_params = {'source_keys': json.dumps(validate_provider_keys(source_keys)),
-                        'stage': validate_value(stage, STAGE_VALUES, "stage"),
-                        'limit': validate_limit(limit),
-                        'page': validate_page(page),
-                        'sort_by': validate_value(sort_by, SORT_BY_VALUES, "sort by"),
-                        'order_by': validate_value(order_by, ORDER_BY_VALUES, "oder by")
-                        }
+        query_params = {
+            "board_keys": json.dumps(validate_provider_keys(board_keys)),
+            "stage": validate_value(stage, STAGE_VALUES),
+            "limit": validate_limit(limit),
+            "page": validate_page(page),
+            "sort_by": validate_value(sort_by, SORT_BY_VALUES, "sort by"),
+            "order_by": validate_value(order_by, ORDER_BY_VALUES, "order by"),
+        }
 
         params = {**query_params, **kwargs}
-        response = self.client.get('profiles/searching', params)
+        response = self.client.get("jobs/searching", params)
         return validate_response(response)
```

### Comparing `hrflow-2.1.0/hrflow/hrflow/profile/storing.py` & `hrflow-3.0.0/hrflow/hrflow/profile/storing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,94 @@
 import json
 from ..utils import (
+    format_item_payload,
     validate_boolean,
     validate_key,
     validate_limit,
     validate_page,
     validate_provider_keys,
     validate_response,
     validate_reference,
     ORDER_BY_VALUES,
     SORT_BY_VALUES,
     validate_value,
 )
 
 
 class ProfileStoring:
-    """
-    This class manages Profiles storing endpoint (https://api.hrflow.ai/v1/storing/profiles).
-    This endpoint allows you to retrieve the list of profiles stored in a Source.
-    """
+    """Manage Storing related profile calls."""
 
     def __init__(self, api):
         """Init."""
         self.client = api
 
-    # Params list
-    """
-    source_keys:["{{source_key}}"]
-    name:
-    key:
-    reference:
-    location_lat:
-    location_lon:
-    location_dist:
-    return_profile:
-    page:
-    limit:
-    order_by:
-    sort_by:
-    created_at_min:
-    created_at_max:
-    """
+    def add_json(self, source_key, profile_json):
+        """Use the api to add a new profile using profile_data."""
+        profile_json["source_key"] = validate_key("Source", source_key)
+        response = self.client.post("profile/indexing", json=profile_json)
+        return validate_response(response)
+
+    def edit(self, source_key, key, profile_json):
+        """Use the api to add a new profile using profile_data."""
+        profile_json["source_key"] = validate_key("Source", source_key)
+        profile_json["key"] = validate_key("Profile", key)
+        response = self.client.put("profile/indexing", json=profile_json)
+        return validate_response(response)
+
+    def get(self, source_key, key=None, reference=None):
+        """
+        💾 Get a Profile indexed in a Source (https://api.hrflow.ai/v1/profile/indexing).
+        Profiles can either be retrieved using this method by their key or their reference.
+        One of the two values must be provided.
+
+        Args:
+            source_key:             <string>
+                                    The key of the Source where the profile is indexed.
+            key:                    <string>
+                                    The Profile unique identifier.
+            reference:              <string>
+                                    The Profile reference chosen by the customer.
+
+        Returns
+            Get information
+
+        """
+        query_params = format_item_payload("profile", source_key, key, reference)
+        response = self.client.get("profile/indexing", query_params)
+        return validate_response(response)
+
+    def archive(self, source_key, key=None, reference=None, is_archive=1, email=None):
+        """
+        This method allows to archive (is_archive=1) or unarchive (is_archive=0)a profile
+        in HrFlow.ai.
+        The profile is identified by either its key or its reference,
+        at least one of the two values must be provided.
+
+        Args:
+            source_key:             <string>
+                                    source identifier
+            key:                    <string>
+                                    profile identifier (key)
+            reference:              <string>
+                                    profile identifier (reference)
+            is_archive:             <integer>
+                                    default = 1
+                                    {0, 1} to indicate archive/unarchive action
+            email:                  <string>
+                                    profile_email
+
+        Returns
+            Archive/unarchive profile response
+
+        """
+
+        payload = format_item_payload("profile", source_key, key, reference, email)
+        payload["is_archive"] = is_archive
+        response = self.client.patch("profile/indexing/archive", json=payload)
+        return validate_response(response)
 
     def list(
         self,
         source_keys,
         name=None,
         key=None,
         reference=None,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hrflow-2.1.0/hrflow/hrflow/source/__init__.py` & `hrflow-3.0.0/hrflow/hrflow/source/__init__.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/__init__.py` & `hrflow-3.0.0/hrflow/hrflow/text/__init__.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/embedding.py` & `hrflow-3.0.0/hrflow/hrflow/text/embedding.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/imaging.py` & `hrflow-3.0.0/hrflow/hrflow/text/imaging.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/linking.py` & `hrflow-3.0.0/hrflow/hrflow/text/linking.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/ocr.py` & `hrflow-3.0.0/hrflow/hrflow/text/ocr.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/parsing.py` & `hrflow-3.0.0/hrflow/hrflow/text/parsing.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/revealing.py` & `hrflow-3.0.0/hrflow/hrflow/text/revealing.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/text/tagging.py` & `hrflow-3.0.0/hrflow/hrflow/text/tagging.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/utils/__init__.py` & `hrflow-3.0.0/hrflow/hrflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow/hrflow/webhook/__init__.py` & `hrflow-3.0.0/hrflow/hrflow/webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/hrflow.egg-info/SOURCES.txt` & `hrflow-3.0.0/hrflow.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 .gitignore
 .gitmodules
 Documentation.md
 LICENSE.txt
+Makefile
 README.md
 README.rst
-poetry.lock
-pyproject.toml
 setup.py
+tag.sh
 examples/colab/build_personalized_ai_hr_models.ipynb
 examples/colab/implement_hrflow_in_5min.ipynb
+examples/job/job_endpoints_examples.ipynb
+examples/profile/profile_endpoints_examples.ipynb
 hrflow/__init__.py
 hrflow/__version__.py
 hrflow.egg-info/PKG-INFO
 hrflow.egg-info/SOURCES.txt
 hrflow.egg-info/dependency_links.txt
 hrflow.egg-info/not-zip-safe
 hrflow.egg-info/requires.txt
 hrflow.egg-info/top_level.txt
 hrflow/hrflow/__init__.py
 hrflow/hrflow/hrflow.py
 hrflow/hrflow/board/__init__.py
 hrflow/hrflow/job/__init__.py
 hrflow/hrflow/job/embedding.py
-hrflow/hrflow/job/indexing.py
 hrflow/hrflow/job/parsing.py
 hrflow/hrflow/job/reasoning.py
 hrflow/hrflow/job/scoring.py
 hrflow/hrflow/job/searching.py
 hrflow/hrflow/job/storing.py
 hrflow/hrflow/profile/__init__.py
 hrflow/hrflow/profile/attachment.py
 hrflow/hrflow/profile/embedding.py
 hrflow/hrflow/profile/exporter.py
 hrflow/hrflow/profile/importer.py
-hrflow/hrflow/profile/indexing.py
 hrflow/hrflow/profile/parsing.py
 hrflow/hrflow/profile/reasoning.py
 hrflow/hrflow/profile/revealing.py
 hrflow/hrflow/profile/scoring.py
 hrflow/hrflow/profile/searching.py
 hrflow/hrflow/profile/storing.py
+hrflow/hrflow/rating/__init__.py
 hrflow/hrflow/source/__init__.py
 hrflow/hrflow/text/__init__.py
 hrflow/hrflow/text/embedding.py
 hrflow/hrflow/text/imaging.py
 hrflow/hrflow/text/linking.py
 hrflow/hrflow/text/ocr.py
 hrflow/hrflow/text/parsing.py
 hrflow/hrflow/text/revealing.py
 hrflow/hrflow/text/tagging.py
+hrflow/hrflow/tracking/__init__.py
 hrflow/hrflow/utils/__init__.py
 hrflow/hrflow/webhook/__init__.py
 hrflow/hrflow/webhook/base64Wrapper.py
 hrflow/hrflow/webhook/bytesutils.py
 hrflow/hrflow/webhook/hmacutils.py
-libs/__init__.py
 tests/__init__.py
 tests/config.py
 tests/test_api.py
```

### Comparing `hrflow-2.1.0/setup.py` & `hrflow-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `hrflow-2.1.0/tests/test_api.py` & `hrflow-3.0.0/tests/test_api.py`

 * *Files identical despite different names*

