# Comparing `tmp/lume-0.9.5rc0.tar.gz` & `tmp/lume-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lume-0.9.5rc0.tar", last modified: Wed Feb 15 15:54:20 2023, max compression
+gzip compressed data, was "lume-0.9.6.tar", last modified: Wed Jun 21 21:40:05 2023, max compression
```

## Comparing `lume-0.9.5rc0.tar` & `lume-0.9.6.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-15 15:54:10.000000 lume-0.9.5rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-15 15:54:10.000000 lume-0.9.5rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-02-15 15:54:20.460193 lume-0.9.5rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-02-15 15:54:10.000000 lume-0.9.5rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.452193 lume-0.9.5rc0/lume/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-15 15:54:12.000000 lume-0.9.5rc0/lume/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.456194 lume-0.9.5rc0/lume/config/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/check_list_or_str_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/check_os_list_or_str_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/config_file_not_found_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/config_file_not_valid_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/dependency_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/get_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/install_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/required_env_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/setup_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/step_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/config/uninstall_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.456194 lume-0.9.5rc0/lume/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.456194 lume-0.9.5rc0/lume/src/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.456194 lume-0.9.5rc0/lume/src/application/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/cli/lume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.456194 lume-0.9.5rc0/lume/src/application/use_cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/use_cases/env_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/use_cases/lume_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/use_cases/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/application/use_cases/use_case_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.456194 lume-0.9.5rc0/lume/src/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/lume/src/domain/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/domain/services/executor_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/domain/services/killer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/domain/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/domain/services/setup_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/lume/src/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/lume/src/infrastructure/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/lume/src/infrastructure/services/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/executor/detach_popen_executor_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/executor/fake_executor_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/executor/popen_executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/lume/src/infrastructure/services/killer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/killer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/killer/fake_killer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/killer/popen_killer_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/lume/src/infrastructure/services/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/logger/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/logger/emojis_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/logger/fake_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/logger/not_implemented_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/logger/print_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/lume/src/infrastructure/services/setup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/fake_setup_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_item_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_item_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-02-15 15:54:10.000000 lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.456194 lume-0.9.5rc0/lume.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-02-15 15:54:20.000000 lume-0.9.5rc0/lume.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-02-15 15:54:20.000000 lume-0.9.5rc0/lume.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 15:54:20.000000 lume-0.9.5rc0/lume.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-15 15:54:20.000000 lume-0.9.5rc0/lume.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 15:54:20.000000 lume-0.9.5rc0/lume.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-15 15:54:20.000000 lume-0.9.5rc0/lume.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-15 15:54:20.000000 lume-0.9.5rc0/lume.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:54:20.460193 lume-0.9.5rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-15 15:54:10.000000 lume-0.9.5rc0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-15 15:54:20.464194 lume-0.9.5rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-15 15:54:10.000000 lume-0.9.5rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 21:40:03.000000 lume-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 21:40:03.000000 lume-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-21 21:40:05.927133 lume-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-21 21:40:03.000000 lume-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 21:40:03.000000 lume-0.9.6/lume/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 21:40:03.000000 lume-0.9.6/lume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/check_list_or_str_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/check_os_list_or_str_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/config_file_not_found_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/config_file_not_valid_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/dependency_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/get_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/install_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/required_env_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/setup_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/step_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-21 21:40:03.000000 lume-0.9.6/lume/config/uninstall_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume/src/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume/src/application/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/cli/lume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume/src/application/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/use_cases/env_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/use_cases/lume_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/use_cases/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/application/use_cases/use_case_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume/src/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/lume/src/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/domain/services/executor_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/domain/services/killer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/domain/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/domain/services/setup_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/lume/src/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/lume/src/infrastructure/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/lume/src/infrastructure/services/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/executor/detach_popen_executor_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/executor/fake_executor_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/executor/popen_executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/lume/src/infrastructure/services/killer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/killer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/killer/fake_killer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/killer/popen_killer_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/lume/src/infrastructure/services/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/logger/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/logger/emojis_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/logger/fake_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/logger/not_implemented_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/logger/print_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/lume/src/infrastructure/services/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/fake_setup_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/setup_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/setup_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/setup_item_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/setup_item_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/setup_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-21 21:40:03.000000 lume-0.9.6/lume/src/infrastructure/services/setup/setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.923133 lume-0.9.6/lume.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-21 21:40:05.000000 lume-0.9.6/lume.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-21 21:40:05.000000 lume-0.9.6/lume.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:40:05.000000 lume-0.9.6/lume.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 21:40:05.000000 lume-0.9.6/lume.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:40:05.000000 lume-0.9.6/lume.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 21:40:05.000000 lume-0.9.6/lume.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 21:40:05.000000 lume-0.9.6/lume.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 21:40:03.000000 lume-0.9.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-21 21:40:05.927133 lume-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-21 21:40:03.000000 lume-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:05.927133 lume-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:40:03.000000 lume-0.9.6/tests/__init__.py
```

### Comparing `lume-0.9.5rc0/LICENSE` & `lume-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/PKG-INFO` & `lume-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lume
-Version: 0.9.5rc0
+Version: 0.9.6
 Summary: Lume
 Home-page: https://github.com/alice-biometrics/lume
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: lume
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: lume Version: 0.9.5rc0 Summary: Lume Home-page:
-https://github.com/alice-biometrics/lume Author: Alice Biometrics Author-email:
+Metadata-Version: 2.1 Name: lume Version: 0.9.6 Summary: Lume Home-page: https:
+//github.com/alice-biometrics/lume Author: Alice Biometrics Author-email:
 support@alicebiometrics.com License: MIT Keywords: lume Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
```

### Comparing `lume-0.9.5rc0/README.md` & `lume-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/config/check_list_or_str_item.py` & `lume-0.9.6/lume/config/check_list_or_str_item.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/config/check_os_list_or_str_item.py` & `lume-0.9.6/lume/config/check_os_list_or_str_item.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/config/config.py` & `lume-0.9.6/lume/config/config.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/config/get_envs.py` & `lume-0.9.6/lume/config/get_envs.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/config/install_config.py` & `lume-0.9.6/lume/config/uninstall_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pydantic import BaseModel
 
 from lume.config.check_os_list_or_str_item import check_os_list_or_str_item
 from lume.config.get_envs import get_envs
 
 
-class InstallConfig(BaseModel):
+class UninstallConfig(BaseModel):
     run: List[str]
     cwd: Optional[str] = None
     envs: Dict[str, str] = dict()
     overwrote_envs: List[str] = list()
 
     def add_shared_env(self, shared_envs: Dict[str, str]):
         if shared_envs and self.envs:
@@ -18,8 +18,8 @@
                 set(shared_envs.keys()).intersection(set(self.envs))
             )
 
     @staticmethod
     def from_dict(kdict):
         run = check_os_list_or_str_item(kdict, "run")
         envs = get_envs(kdict)
-        return InstallConfig(run=run if run else [], cwd=kdict.get("cwd"), envs=envs)
+        return UninstallConfig(run=run if run else [], cwd=kdict.get("cwd"), envs=envs)
```

### Comparing `lume-0.9.5rc0/lume/config/step_config.py` & `lume-0.9.6/lume/config/step_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel
 
 from lume.config.check_list_or_str_item import check_list_or_str_item
 from lume.config.check_os_list_or_str_item import check_os_list_or_str_item
 from lume.config.get_envs import get_envs
 
 
 class StepConfig(BaseModel):
     run: List[str]
     cwd: Optional[str] = None
-    envs: Dict[str, str] = dict()
+    envs: Dict[str, Any] = dict()
     setup: Optional[List[str]] = None
     teardown: Optional[List[str]] = None
     setup_detach: Optional[Dict] = None
     wait_seconds: Optional[int] = None
     wait_http_200: Optional[str] = None
     overwrote_envs: List[str] = list()
```

### Comparing `lume-0.9.5rc0/lume/config/uninstall_config.py` & `lume-0.9.6/lume/config/install_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Dict, List, Optional
+from typing import Dict, List, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from lume.config.check_os_list_or_str_item import check_os_list_or_str_item
 from lume.config.get_envs import get_envs
 
 
-class UninstallConfig(BaseModel):
-    run: List[str]
-    cwd: Optional[str] = None
-    envs: Dict[str, str] = dict()
-    overwrote_envs: List[str] = list()
+class InstallConfig(BaseModel):
+    run: List[str] = Field()
+    cwd: Union[str, None] = Field(default=None)
+    envs: Dict[str, str] = Field(default=dict())
+    overwrote_envs: List[str] = Field(default=list())
 
     def add_shared_env(self, shared_envs: Dict[str, str]):
         if shared_envs and self.envs:
             self.overwrote_envs = list(
                 set(shared_envs.keys()).intersection(set(self.envs))
             )
 
     @staticmethod
     def from_dict(kdict):
         run = check_os_list_or_str_item(kdict, "run")
         envs = get_envs(kdict)
-        return UninstallConfig(run=run if run else [], cwd=kdict.get("cwd"), envs=envs)
+        return InstallConfig(run=run if run else [], cwd=kdict.get("cwd"), envs=envs)
```

### Comparing `lume-0.9.5rc0/lume/src/application/cli/lume.py` & `lume-0.9.6/lume/src/application/cli/lume.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/application/use_cases/env_manager.py` & `lume-0.9.6/lume/src/application/use_cases/env_manager.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/application/use_cases/lume_use_case.py` & `lume-0.9.6/lume/src/application/use_cases/lume_use_case.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from __future__ import annotations
 
 import os
 import time
 from typing import List, Tuple, Union
 
 import requests
-from meiga import Error, Failure, Result, Success, isFailure, isSuccess
+from meiga import (
+    Error,
+    Failure,
+    OnFailureHandler,
+    Result,
+    Success,
+    isFailure,
+    isSuccess,
+)
 from meiga.decorators import meiga
 
 from lume.config import Config
 from lume.src.application.use_cases.env_manager import EnvManager
 from lume.src.application.use_cases.messages import get_colored_command_message
 from lume.src.domain.services.executor_service import ExecutorService
 from lume.src.domain.services.killer_service import KillerService
@@ -80,28 +88,40 @@
                 result = self.setup_service.execute()
                 if result.is_failure:
                     self.logger.log(ERROR, f"Setup: {result.value.message}")
                 result.unwrap_or_return()
             else:
                 cwd = (
                     self._get_cwd(step)
-                    .handle(on_failure=on_error_with_cwd, failure_args=(self, step))
+                    .handle(
+                        on_failure_handler=OnFailureHandler(
+                            func=on_error_with_cwd, args=(self, step)
+                        )
+                    )
                     .unwrap_or_return()
                 )
 
                 self._set_env(step)
                 processes: List = (
                     self._run_setup_detach(step, cwd)
-                    .handle(on_failure=self._run_teardown, failure_args=(cwd, step))
+                    .handle(
+                        on_failure_handler=OnFailureHandler(
+                            func=self._run_teardown, args=(cwd, step)
+                        )
+                    )
                     .unwrap_or([])
                 )
                 self._run_setup(step, cwd).handle(
-                    on_failure=self._run_teardown_detach, failure_args=processes
+                    on_failure_handler=OnFailureHandler(
+                        func=self._run_teardown_detach, args=processes
+                    )
                 ).handle(
-                    on_failure=self._run_teardown, failure_args=(cwd, step)
+                    on_failure_handler=OnFailureHandler(
+                        func=self._run_teardown, args=(cwd, step)
+                    )
                 ).unwrap_or_return()
                 self._run_commands(step, cwd, processes).unwrap_or_return()
                 self._run_teardown_detach(processes)
                 self._run_teardown(cwd, step)
                 self._unset_env(step)
 
         self.env_manager.unset(self.config.shared_envs)
@@ -223,24 +243,32 @@
         return
 
     @meiga
     def _run_commands(self, step, cwd, processes) -> Result:
         self._wait_if_necessary(step)
         commands: List[str] = (
             self._get_commands(step)
-            .handle(on_failure=on_empty_config, failure_args=(self, step))
+            .handle(
+                on_failure_handler=OnFailureHandler(
+                    func=on_empty_config, args=(self, step)
+                )
+            )
             .unwrap_or([])
         )
         for command in commands:
             message = get_colored_command_message(command, cwd, step)
             self.logger.log(COMMAND, message)
             self.executor_service.execute(command, cwd).handle(
-                on_failure=self._run_teardown_detach, failure_args=processes
+                on_failure_handler=OnFailureHandler(
+                    func=self._run_teardown_detach, args=processes
+                )
             ).handle(
-                on_failure=self._run_teardown, failure_args=(cwd, step)
+                on_failure_handler=OnFailureHandler(
+                    func=self._run_teardown, args=(cwd, step)
+                )
             ).unwrap_or_return()
 
         return isSuccess
 
     def _run_teardown(self, cwd, step):
         teardown_commands = self._get_teardown_commands(step).unwrap_or([])
         for teardown_command in teardown_commands:
```

### Comparing `lume-0.9.5rc0/lume/src/application/use_cases/use_case_builder.py` & `lume-0.9.6/lume/src/application/use_cases/use_case_builder.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/executor/detach_popen_executor_service.py` & `lume-0.9.6/lume/src/infrastructure/services/executor/detach_popen_executor_service.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/executor/popen_executor_service.py` & `lume-0.9.6/lume/src/infrastructure/services/executor/popen_executor_service.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/killer/popen_killer_service.py` & `lume-0.9.6/lume/src/infrastructure/services/killer/popen_killer_service.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/logger/emojis_logger.py` & `lume-0.9.6/lume/src/infrastructure/services/logger/emojis_logger.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/setup/fake_setup_service.py` & `lume-0.9.6/lume/src/infrastructure/services/setup/fake_setup_service.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_errors.py` & `lume-0.9.6/lume/src/infrastructure/services/setup/setup_errors.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_item_bucket.py` & `lume-0.9.6/lume/src/infrastructure/services/setup/setup_item_bucket.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_item_file.py` & `lume-0.9.6/lume/src/infrastructure/services/setup/setup_item_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import Union
 from zipfile import BadZipFile
 
 import requests
 from meiga import Failure, Result, Success
 from requests.auth import HTTPBasicAuth
 
 from lume.config import DependencyConfig
@@ -43,12 +44,12 @@
                 unzip_file(dependency_path, dependency_config.url)
             except BadZipFile:
                 return Failure(BadZipFileError(name))
 
         return Success()
 
     @staticmethod
-    def __download_file(dst: str, url: str, auth: HTTPBasicAuth = None):
+    def __download_file(dst: str, url: str, auth: Union[HTTPBasicAuth, None] = None):
         r = requests.get(url, auth=auth, stream=True)
         dst_filename = os.path.split(url)[-1]
         with open(os.path.join(dst, dst_filename), "wb") as f:
             f.write(r.content)
```

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_service.py` & `lume-0.9.6/lume/src/infrastructure/services/setup/setup_service.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume/src/infrastructure/services/setup/setup_utils.py` & `lume-0.9.6/lume/src/infrastructure/services/setup/setup_utils.py`

 * *Files identical despite different names*

### Comparing `lume-0.9.5rc0/lume.egg-info/PKG-INFO` & `lume-0.9.6/lume.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lume
-Version: 0.9.5rc0
+Version: 0.9.6
 Summary: Lume
 Home-page: https://github.com/alice-biometrics/lume
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: lume
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: lume Version: 0.9.5rc0 Summary: Lume Home-page:
-https://github.com/alice-biometrics/lume Author: Alice Biometrics Author-email:
+Metadata-Version: 2.1 Name: lume Version: 0.9.6 Summary: Lume Home-page: https:
+//github.com/alice-biometrics/lume Author: Alice Biometrics Author-email:
 support@alicebiometrics.com License: MIT Keywords: lume Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
```

### Comparing `lume-0.9.5rc0/lume.egg-info/SOURCES.txt` & `lume-0.9.6/lume.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,8 +59,9 @@
 lume/src/infrastructure/services/setup/fake_setup_service.py
 lume/src/infrastructure/services/setup/setup_errors.py
 lume/src/infrastructure/services/setup/setup_item.py
 lume/src/infrastructure/services/setup/setup_item_bucket.py
 lume/src/infrastructure/services/setup/setup_item_file.py
 lume/src/infrastructure/services/setup/setup_service.py
 lume/src/infrastructure/services/setup/setup_utils.py
-requirements/requirements.txt
+requirements/requirements.txt
+tests/__init__.py
```

### Comparing `lume-0.9.5rc0/setup.py` & `lume-0.9.6/setup.py`

 * *Files identical despite different names*

