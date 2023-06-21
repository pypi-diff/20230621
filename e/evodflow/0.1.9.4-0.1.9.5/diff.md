# Comparing `tmp/evodflow-0.1.9.4.tar.gz` & `tmp/evodflow-0.1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodflow-0.1.9.4.tar", last modified: Mon Jun 12 05:30:05 2023, max compression
+gzip compressed data, was "evodflow-0.1.9.5.tar", last modified: Wed Jun 21 11:40:35 2023, max compression
```

## Comparing `evodflow-0.1.9.4.tar` & `evodflow-0.1.9.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.478440 evodflow-0.1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-12 05:30:05.478440 evodflow-0.1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.466440 evodflow-0.1.9.4/evodflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-12 05:30:05.000000 evodflow-0.1.9.4/evodflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-12 05:30:05.000000 evodflow-0.1.9.4/evodflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 05:30:05.000000 evodflow-0.1.9.4/evodflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 05:30:05.000000 evodflow-0.1.9.4/evodflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-12 05:30:05.000000 evodflow-0.1.9.4/evodflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 05:30:05.000000 evodflow-0.1.9.4/evodflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.466440 evodflow-0.1.9.4/evoflow/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/common_step_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/controller/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/data_manipulate/PdfFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/data_manipulate/PptxFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/data_manipulate/data_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/data_manipulate/excel_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/data_manipulate/file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/data_manipulate/image_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/log_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/controller/visualize_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/entities/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/entities/common/step/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/common/step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/entities/common/step/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/common/step/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/common/step/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/entities/common/step/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/common/step/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/common/step/open_excel_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/entities/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/step_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.470440 evodflow-0.1.9.4/evoflow/entities/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/abstract_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/pdf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/pptx_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/evoflow/entities/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/exceptions/base_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/exceptions/evo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/entities/global_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/evoflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/operators/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/operators/empty_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/operators/python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/evoflow/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/abstract_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/evoflow/services/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/ocr/easy_ocr_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/ocr/ocr_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/ocr/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/ocr/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/service_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/evoflow/services/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/services/templates/item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/evoflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/utils/create_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/utils/ultilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/evoflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 05:30:05.478440 evodflow-0.1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 05:30:05.474440 evodflow-0.1.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-12 05:29:53.000000 evodflow-0.1.9.4/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evodflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-21 11:40:35.000000 evodflow-0.1.9.5/evodflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-21 11:40:35.000000 evodflow-0.1.9.5/evodflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:40:35.000000 evodflow-0.1.9.5/evodflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 11:40:35.000000 evodflow-0.1.9.5/evodflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 11:40:35.000000 evodflow-0.1.9.5/evodflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 11:40:35.000000 evodflow-0.1.9.5/evodflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/common_step_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/controller/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/data_manipulate/data_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/data_manipulate/excel_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/data_manipulate/file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/data_manipulate/image_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/data_manipulate/pdf_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/data_manipulate/pptx_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/log_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/controller/visualize_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/entities/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/entities/common/step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/common/step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/entities/common/step/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/common/step/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/common/step/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.075230 evodflow-0.1.9.5/evoflow/entities/common/step/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/common/step/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/common/step/open_excel_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/entities/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/step_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/entities/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/abstract_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/pdf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/pptx_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/entities/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/exceptions/base_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/exceptions/evo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/entities/global_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/operators/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/operators/empty_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/operators/python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/abstract_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/services/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/ocr/easy_ocr_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/ocr/ocr_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/ocr/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/ocr/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/service_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/services/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/services/templates/item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/evoflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/utils/create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/utils/ultilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/evoflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:35.079230 evodflow-0.1.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 11:40:23.000000 evodflow-0.1.9.5/tests/test_base.py
```

### Comparing `evodflow-0.1.9.4/LICENSE` & `evodflow-0.1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/PKG-INFO` & `evodflow-0.1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.9.4
+Version: 0.1.9.5
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.9.4/README.md` & `evodflow-0.1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evodflow.egg-info/PKG-INFO` & `evodflow-0.1.9.5/evodflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.9.4
+Version: 0.1.9.5
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.9.4/evodflow.egg-info/SOURCES.txt` & `evodflow-0.1.9.5/evodflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 evoflow/cli.py
 evoflow/params.py
 evoflow/version.py
 evoflow/controller/__init__.py
 evoflow/controller/common_step_controller.py
 evoflow/controller/log_controller.py
 evoflow/controller/visualize_controller.py
-evoflow/controller/data_manipulate/PdfFileOperator.py
-evoflow/controller/data_manipulate/PptxFileOperator.py
 evoflow/controller/data_manipulate/__init__.py
 evoflow/controller/data_manipulate/data_manipulate.py
 evoflow/controller/data_manipulate/excel_file_operator.py
 evoflow/controller/data_manipulate/file_operator.py
 evoflow/controller/data_manipulate/image_file_operator.py
+evoflow/controller/data_manipulate/pdf_file_operator.py
+evoflow/controller/data_manipulate/pptx_file_operator.py
 evoflow/entities/__init__.py
 evoflow/entities/global_vars.py
 evoflow/entities/common/__init__.py
 evoflow/entities/common/step/__init__.py
 evoflow/entities/common/step/downloader.py
 evoflow/entities/common/step/open_excel_file.py
 evoflow/entities/common/step/browser/__init__.py
```

### Comparing `evodflow-0.1.9.4/evoflow/__init__.py` & `evodflow-0.1.9.5/evoflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         for key in setting.__dict__:
             if str(key).startswith("__"):
                 continue
             value = setting.__dict__[key]
             os.environ[key] = str(value)
     except Exception as e:
         logger.debug(e)
-        logger.info("Can't import setting.py")
+        logger.debug("Can't import setting.py")
 
 
 def versioning(version_module):
     try:
         repo = git.Repo(search_parent_directories=True)
         sha = repo.head.object.hexsha
         if version_module.__sha__ != sha:
@@ -61,15 +61,15 @@
 
 def bot_versioning():
     try:
         import version
 
         versioning(version)
     except:
-        logger.error("Can't versioning For Bot")
+        logger.debug("Can't versioning For Bot")
 
 
 init_setting()
 # framework_versioning()
 bot_versioning()
 
 IS_DEBUG = sys.gettrace() is not None
```

### Comparing `evodflow-0.1.9.4/evoflow/cli.py` & `evodflow-0.1.9.5/evoflow/cli.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/controller/data_manipulate/PdfFileOperator.py` & `evodflow-0.1.9.5/evoflow/controller/data_manipulate/pdf_file_operator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pdfplumber
 
-from evoflow.Controller.DataManipulate.FileOperator import FileOperator
-from evoflow.Entities.DataManipulate.FileOperator.File import File
-from evoflow.Entities.DataManipulate.FileOperator.PdfFile import PdfFile
+from evoflow.controller.data_manipulate.file_operator import FileOperator
+from evoflow.entities.data_manipulate.file_operator.file import File
+from evoflow.entities.data_manipulate.file_operator.pdf_file import PdfFile
 
 
 class PdfFileOperator(FileOperator):
     """
     Read and write file PDF
     """
```

### Comparing `evodflow-0.1.9.4/evoflow/controller/data_manipulate/PptxFileOperator.py` & `evodflow-0.1.9.5/evoflow/controller/data_manipulate/pptx_file_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pptx import Presentation
 
-from evoflow.Controller.DataManipulate.FileOperator import FileOperator
-from evoflow.Entities.DataManipulate.FileOperator.File import File
-from evoflow.Entities.DataManipulate.FileOperator.PPTXFile import PPTXFile
+from evoflow.controller.data_manipulate.file_operator import FileOperator
+from evoflow.entities.data_manipulate.file_operator.file import File
+from evoflow.entities.data_manipulate.file_operator.pptx_file import PPTXFile
 
 
 class PptxFileOperator(FileOperator):
     def save(self, file: File, file_path) -> bool:
         file.data: Presentation
         file.data.save(file_path)
         return True
```

### Comparing `evodflow-0.1.9.4/evoflow/controller/data_manipulate/excel_file_operator.py` & `evodflow-0.1.9.5/evoflow/controller/data_manipulate/image_file_operator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 #  Copyright (c) 2021. Copyright belongs to evoflow team
 
-import pandas as pd
+import os
 
-from evoflow.controller.data_manipulate.FileOperator import FileOperator
-from evoflow.Entities.DataManipulate.FileOperator.DataFrameFile import DataFrameFile
-from evoflow.Entities.DataManipulate.FileOperator.File import File
-
-
-class ExcelFileOperator(FileOperator):
-    def read(self, file_path, **args) -> File:
-        """
-        read file excel
-        :param file_path:
-        :return:
-        """
+import cv2
+import numpy as np
+
+from evoflow import logger
+from evoflow.controller.data_manipulate.file_operator import FileOperator
+from evoflow.entities.data_manipulate.file_operator.file import File
+from evoflow.entities.data_manipulate.file_operator.image_file import ImageFile
+
+
+def imread(path, flags: int = -1):
+    """
+    :flags: Default=  cv2.IMREAD_UNCHANGED
+    """
+    normed_path = os.path.normpath(path)
+    mat = cv2.imdecode(np.fromfile(normed_path, dtype=np.uint8), flags)
+    if mat is None:
+        logger.error(f"Can't read image: {path}")
+        raise Exception
+    return mat
+
+
+def imwrite(path, mat):
+    image_type = path.split(".")[-1]
+    is_success, im_buf_arr = cv2.imencode(".{}".format(image_type), mat)
+    im_buf_arr.tofile(path)
+    return is_success
 
-        file = DataFrameFile(file_path=file_path)
-        file.data = pd.read_excel(file_path, **args)
-        return file
+
+cv2.imwrite = imwrite
+cv2.imread = imread
+
+
+class ImageFileOperator(FileOperator):
+    """
+    File operator with images
+    """
 
     def save(self, file: File, file_path) -> bool:
-        """
-        save excel file
-        :param file:
-        :param file_path:
-        :return:
-        """
-        file.data: pd.DataFrame
-        file.data.to_excel(file_path)
-        return file_path
+        return cv2.imwrite(file_path, file.data)
+
+    def read(self, file_path, **args):
+        data = cv2.imread(file_path, **args)
+        file = ImageFile(file_path=file_path, data=data)
+        return file
 
     @staticmethod
     def supported_file_types():
-        return ["xlsx", "csv", "xls"]
+        return ["jpg", "png", "tiff", "tif"]
```

### Comparing `evodflow-0.1.9.4/evoflow/controller/data_manipulate/file_operator.py` & `evodflow-0.1.9.5/evoflow/controller/data_manipulate/file_operator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-#  Copyright (c) 2021. Copyright belongs to evoflow team
-
 import abc
 
 from tqdm import tqdm
 
-from evoflow.Controller.DataManipulate.DataManipulate import DataManipulate
-from evoflow.Entities.DataManipulate.FileOperator.File import File
+from evoflow.controller.data_manipulate.data_manipulate import DataManipulate
+from evoflow.entities.data_manipulate.file_operator.file import File
 
 
 def get_reader(file_type):
     """
     Trả về reader thỏa vãn mới file_type này
     """
     readers = FileOperator.__subclasses__()
```

### Comparing `evodflow-0.1.9.4/evoflow/controller/log_controller.py` & `evodflow-0.1.9.5/evoflow/controller/log_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/common/step/__init__.py` & `evodflow-0.1.9.5/evoflow/entities/common/step/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/common/step/browser/__init__.py` & `evodflow-0.1.9.5/evoflow/entities/common/step/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/common/step/downloader.py` & `evodflow-0.1.9.5/evoflow/entities/common/step/downloader.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/common/step/open_excel_file.py` & `evodflow-0.1.9.5/evoflow/entities/common/step/open_excel_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/core/base_object.py` & `evodflow-0.1.9.5/evoflow/entities/core/base_object.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/core/condition.py` & `evodflow-0.1.9.5/evoflow/entities/core/condition.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/core/job.py` & `evodflow-0.1.9.5/evoflow/entities/core/job.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/core/step.py` & `evodflow-0.1.9.5/evoflow/entities/core/step.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/core/step_list.py` & `evodflow-0.1.9.5/evoflow/entities/core/step_list.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/core/transaction.py` & `evodflow-0.1.9.5/evoflow/entities/core/transaction.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/core/workflow.py` & `evodflow-0.1.9.5/evoflow/entities/core/workflow.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/data_manipulate/abstract_data.py` & `evodflow-0.1.9.5/evoflow/entities/data_manipulate/abstract_data.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/dataframe_file.py` & `evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/dataframe_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/file.py` & `evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from evoflow.entities.data_manipulate.abstract_data import AbstractData
 
 
 class File(AbstractData):
     def __init__(self, file_path: str = None, **args):
         self.file_path = file_path
+        self.file_path = os.path.abspath(self.file_path)
 
         self.file_name = os.path.split(file_path)[1].replace(
             "." + self.get_file_type(), ""
         )
         self.data = args.get("data")
         self.__meta_data__ = None
         super().__init__()
```

### Comparing `evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/image_file.py` & `evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/image_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 import cv2
 import PIL
 from PIL import Image, ImageDraw, ImageFont
 
 from evoflow.entities.data_manipulate.file_operator.file import File
-from evoflow.entities.Global import Global
-from evoflow.Services.OCR.EasyOCREngine import EasyOCREngine
-from evoflow.Services.OCR.Result import OCRResult
+from evoflow.entities.global_vars import Global
+from evoflow.services.ocr.easy_ocr_engine import EasyOCREngine
+from evoflow.services.ocr.result import OCRResult
 
 
 class ImageFile(File):
     """
     Read and write image files
     """
 
@@ -37,14 +37,19 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def to_pil(self):
         return PIL.Image.fromarray(self.data)
 
+    def __array__(self):
+        """
+        Convert to numpy array: np.array(image_file)
+        """
+        return self.data
     def draw(self, ocr_results):
         user_path = f'{os.getenv("userprofile")}/.evoflow/fonts/Noto_Sans_JP/NotoSansJP-Regular.otf'
         data_path = "./data/.evoflow/fonts/Noto_Sans_JP/NotoSansJP-Regular.otf"
 
         if os.path.isfile(user_path):
             font_file = user_path
         else:
```

### Comparing `evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/pdf_file.py` & `evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/pdf_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import glob
 import json
 import os
 import pathlib
 import urllib
 from typing import Iterator
+from urllib.request import URLopener
 
 import cv2
 import numpy as np
+import pdfplumber
 from tqdm import tqdm
 
-import evoflow.Params
+import evoflow.params
 from evoflow import logger
 from evoflow.controller.data_manipulate.image_file_operator import ImageFileOperator
 from evoflow.entities.data_manipulate.file_operator.file import File
 from evoflow.entities.data_manipulate.file_operator.image_file import ImageFile
 
 
 def download_poppler():
@@ -22,29 +24,34 @@
     except ImportError:
         logger.error(
             "Can't import pyunpack. Try to install with:\npip install pyunpack"
         )
 
     poppler_path = f"{os.getenv('userprofile')}/.evoflow/poppler"
     pathlib.Path(poppler_path).mkdir(parents=True, exist_ok=True)
-    poppler_file_name = evoflow.Params.POPPLER_URL.rsplit("/", maxsplit=-1)
-    opener = urllib.request.URLopener()
+    poppler_file_name = evoflow.params.POPPLER_URL.rsplit("/", maxsplit=-1)[-1]
+    opener = URLopener()
     opener.addheader("User-Agent", "evoflow")
     filename, _ = opener.retrieve(
-        evoflow.Params.POPPLER_URL, f"{poppler_path}/{poppler_file_name}"
+        evoflow.params.POPPLER_URL, f"{poppler_path}/{poppler_file_name}"
     )
     Archive(filename).extractall(poppler_path)
     os.remove(filename)
     poppler_path = glob.glob(f"{poppler_path}/*/bin")[0]
     return os.path.normpath(poppler_path)
 
 
 class PdfFile(File):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.data = pdfplumber.open(self.file_path)
+
+    @property
+    def pages(self):
+        return self.data.pages
 
     def get_texts(self):
         page_count = len(self.data.pages)
         texts = []
         for i in range(page_count):
             page = self.data.pages[i]
             text = page.extract_text()
@@ -72,15 +79,15 @@
                 if str(value_error) == "patool not found! Please install patool!":
                     raise ValueError(
                         "patool not found! Please install patool!. \n"
                         "Try to install with: pip install patool"
                     ) from value_error
         else:
             poppler_path = poppler_paths[0]
-
+        poppler_path = os.path.abspath(poppler_path)
         pages = convert_from_path(self.file_path, dpi, poppler_path=poppler_path)
         images = []
         for i, page in tqdm(
             enumerate(pages),
             total=len(pages),
             desc=f"Extract image from file: {self.file_path}",
         ):
```

### Comparing `evodflow-0.1.9.4/evoflow/entities/data_manipulate/file_operator/pptx_file.py` & `evodflow-0.1.9.5/evoflow/entities/data_manipulate/file_operator/pptx_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/entities/global_vars.py` & `evodflow-0.1.9.5/evoflow/entities/global_vars.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/operators/base_operator.py` & `evodflow-0.1.9.5/evoflow/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/operators/empty_operator.py` & `evodflow-0.1.9.5/evoflow/operators/empty_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/operators/python_operator.py` & `evodflow-0.1.9.5/evoflow/operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/services/ocr/easy_ocr_engine.py` & `evodflow-0.1.9.5/evoflow/services/ocr/easy_ocr_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import os.path
 from typing import Iterator
 from urllib.error import URLError
 
 import numpy as np
 
 from evoflow import logger
-from evoflow.Services.ocr.result import OCRResult
+from evoflow.services.ocr.result import OCRResult
 
 try:
     import easyocr
 except ImportError:
-    logger.error("Can't import easyocr. Try to install with: pip install easyocr")
+    logger.debug("Can't import easyocr. Try to install with: pip install easyocr")
 
 MODEL_PATH = "/ocr"
 
 
 class EasyOCREngine:
     """
     Engine OCR sử dụng thư viện easyocr
```

### Comparing `evodflow-0.1.9.4/evoflow/services/ocr/ocr_service.py` & `evodflow-0.1.9.5/evoflow/services/ocr/ocr_service.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/services/ocr/result.py` & `evodflow-0.1.9.5/evoflow/services/ocr/result.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/services/service_controller.py` & `evodflow-0.1.9.5/evoflow/services/service_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/evoflow/utils/ultilities.py` & `evodflow-0.1.9.5/evoflow/utils/ultilities.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.4/setup.py` & `evodflow-0.1.9.5/setup.py`

 * *Files identical despite different names*

