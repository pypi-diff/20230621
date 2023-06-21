# Comparing `tmp/toloka-kit-1.2.0.tar.gz` & `tmp/toloka-kit-1.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toloka-kit-1.2.0.tar", last modified: Mon Jun 19 14:00:13 2023, max compression
+gzip compressed data, was "toloka-kit-1.2.0.post1.tar", last modified: Wed Jun 21 13:44:20 2023, max compression
```

## Comparing `toloka-kit-1.2.0.tar` & `toloka-kit-1.2.0.post1.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-19 13:59:36.000000 toloka-kit-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.131964 toloka-kit-1.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.131964 toloka-kit-1.2.0/src/async_client/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   234034 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/async_client/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.135964 toloka-kit-1.2.0/src/autoquality/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/optimizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/autoquality/scoring.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.155965 toloka-kit-1.2.0/src/client/
--rw-r--r--   0 runner    (1001) docker     (123)   174240 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   241349 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/_converter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/analytics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/analytics_request.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.159965 toloka-kit-1.2.0/src/client/app/
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/app/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/assignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/attachment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/batch_create_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/batch_create_results.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/clone_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/clone_results.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25265 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33104 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/collectors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/error_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/filter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/message_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/message_thread.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operation_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operation_log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/owner.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.159965 toloka-kit-1.2.0/src/client/pool/
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/mixer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/mixer_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.163966 toloka-kit-1.2.0/src/client/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/adapters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/infinite_overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/infinite_overlap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/operators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/parameter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/primitives/retry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.167966 toloka-kit-1.2.0/src/client/project/
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/field_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/field_spec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/localization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/task_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/task_spec.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.175966 toloka-kit-1.2.0/src/client/project/template_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/data.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    47185 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/layouts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    41485 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/template_builder/view.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/view_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/project/view_spec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/quality_control.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/requester.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    46903 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    86035 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_requests.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19042 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/search_results.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/skill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/solution.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_distribution_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_distribution_function.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/task_suite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/training.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_bonus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_bonus.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_restriction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/user_skill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/webhook_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/client/webhook_subscription.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.179967 toloka-kit-1.2.0/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/collector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/jupyter_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/jupyter_dashboard.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23397 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/pool_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/pool_metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/metrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.183967 toloka-kit-1.2.0/src/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/cursor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/locker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/observer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/pipeline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/streaming/storage.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.187967 toloka-kit-1.2.0/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_codegen.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_docstrings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_extendable_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_extendable_enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_managing_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_managing_headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/_typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/async_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/stored.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/src/util/stored.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_aggregated_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_analytics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_deep_clone_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_message_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_operation_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    32761 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_user_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_user_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-19 13:59:37.000000 toloka-kit-1.2.0/tests/test_webhook_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:00:13.195968 toloka-kit-1.2.0/toloka_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 14:00:13.000000 toloka-kit-1.2.0/toloka_kit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.665892 toloka-kit-1.2.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-06-21 13:44:20.665892 toloka-kit-1.2.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:44:20.665892 toloka-kit-1.2.0.post1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3035 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.553891 toloka-kit-1.2.0.post1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.553891 toloka-kit-1.2.0.post1/src/async_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/async_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/async_client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/async_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   233996 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/async_client/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.561891 toloka-kit-1.2.0.post1/src/autoquality/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/autoquality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/autoquality/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/autoquality/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/autoquality/optimizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/autoquality/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/autoquality/scoring.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.593891 toloka-kit-1.2.0.post1/src/client/
+-rw-r--r--   0 runner    (1001) docker     (123)   174232 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241317 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/_converter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/analytics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/analytics_request.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.593891 toloka-kit-1.2.0.post1/src/client/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/app/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/assignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/attachment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/batch_create_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/batch_create_results.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/clone_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/clone_results.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33104 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/collectors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/error_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23876 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28694 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/filter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/message_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/message_thread.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/operation_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/operation_log.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/owner.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.601891 toloka-kit-1.2.0.post1/src/client/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/dynamic_overlap_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/dynamic_overlap_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/dynamic_pricing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/dynamic_pricing_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/mixer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/mixer_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/speed_quality_balance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/pool/speed_quality_balance_config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.613891 toloka-kit-1.2.0.post1/src/client/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/infinite_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/infinite_overlap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/operators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/parameter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/primitives/retry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.613891 toloka-kit-1.2.0.post1/src/client/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/field_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/field_spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/localization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/task_spec.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.629891 toloka-kit-1.2.0.post1/src/client/project/template_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47185 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/layouts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41485 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/template_builder/view.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/view_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/project/view_spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/quality_control.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/requester.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    46900 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/search_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86032 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/search_requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/search_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19042 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/search_results.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/skill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/solution.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/task.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/task_distribution_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/task_distribution_function.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/task_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/task_suite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/training.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user_bonus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user_bonus.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user_restriction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/user_skill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/webhook_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/client/webhook_subscription.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.637892 toloka-kit-1.2.0.post1/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/collector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/jupyter_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/jupyter_dashboard.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20329 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23397 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/pool_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/pool_metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/metrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.645892 toloka-kit-1.2.0.post1/src/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/cursor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/locker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/observer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/pipeline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/streaming/storage.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.653892 toloka-kit-1.2.0.post1/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_codegen.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_docstrings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_extendable_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_extendable_enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_managing_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_managing_headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/_typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/async_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/stored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/src/util/stored.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.661892 toloka-kit-1.2.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_aggregated_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_analytics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_deep_clone_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_message_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_operation_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32761 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_user_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_user_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-21 13:43:42.000000 toloka-kit-1.2.0.post1/tests/test_webhook_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:44:20.665892 toloka-kit-1.2.0.post1/toloka_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-06-21 13:44:20.000000 toloka-kit-1.2.0.post1/toloka_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-21 13:44:20.000000 toloka-kit-1.2.0.post1/toloka_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:44:20.000000 toloka-kit-1.2.0.post1/toloka_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 13:44:20.000000 toloka-kit-1.2.0.post1/toloka_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 13:44:20.000000 toloka-kit-1.2.0.post1/toloka_kit.egg-info/top_level.txt
```

### Comparing `toloka-kit-1.2.0/CONTRIBUTING.md` & `toloka-kit-1.2.0.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/LICENSE` & `toloka-kit-1.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/PKG-INFO` & `toloka-kit-1.2.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: toloka-kit
-Version: 1.2.0
+Version: 1.2.0.post1
 Summary: Toloka API client
 Author: Vladimir Losev
 Author-email: losev@yandex-team.ru
 License: Apache 2.0
-Project-URL: Documentation, https://toloka.ai/en/docs/toloka-kit
+Project-URL: Documentation, https://toloka.ai/docs/toloka-kit
 Project-URL: Source, https://github.com/Toloka/toloka-kit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -41,36 +41,36 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/toloka-kit.svg)](https://pypi.org/project/toloka-kit/)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/toloka-kit.svg)](https://pypi.org/project/toloka-kit)
 [![Downloads](https://pepy.tech/badge/toloka-kit/month)](https://pepy.tech/project/toloka-kit)
 
 [![Coverage](https://codecov.io/gh/Toloka/toloka-kit/branch/main/graph/badge.svg)](https://codecov.io/gh/Toloka/toloka-kit)
 [![GitHub Tests](https://github.com/Toloka/toloka-kit/workflows/Tests/badge.svg?branch=main)](//github.com/Toloka/toloka-kit/actions?query=workflow:Tests)
 
-[Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
+[Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
 
 
 
-Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
+Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 The API allows you to build scalable and fully automated human-in-the-loop ML pipelines, and integrate them into your processes. The toolkit makes integration easier. You can use it with Jupyter notebooks.
 
 * Support for all common Toloka use cases: creating projects, adding pools, uploading tasks, and so on.
 * Toloka entities are represented as Python classes. You can use them instead of accessing the API using JSON representations.
 * There’s no need to validate JSON files and work with them directly.
 * Support of both synchronous and asynchronous (via async/await) executions.
-* Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation. 
+* Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation.
 * [AutoQuality](https://medium.com/toloka/automating-crowdsourcing-quality-control-ad057baf00fd) feature which automatically finds the best fitting quality control rules for your project.
 
 ## Prerequisites
 
 Before you begin, make sure that:
 * You are using [Python](https://www.python.org/) v3.7 or higher.
-* You are [registered](https://toloka.ai/docs/guide/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
-* You have [topped up](https://toloka.ai/docs/guide/concepts/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
-* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
+* You are [registered](https://toloka.ai/docs/guide/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
+* You have [topped up](https://toloka.ai/docs/guide/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
+* You have [set up an OAuth token](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit#overview--accessing-the-api) to access Toloka API.
 
 ## Get Started
 1. Install the Toloka-Kit package. Run the following command in the command shell:
 ```
 $ pip install toloka-kit
 ```
 For production environments, specify the exact package version. For the latest stable version, check the [project page at pypi.org](https://pypi.org/project/toloka-kit/).
@@ -106,17 +106,17 @@
 $ pip install toloka-kit[pandas,autoquality,s3,zookeeper,jupyter-metrics] # remove unnecessary requirements from the list
 ```
 
 ## Usage examples
 [Toloka-kit usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#toloka-kit-usage-examples) - tutorials for specific data labeling tasks. They demonstrate how to work with Toloka API using Toloka-Kit.
 
 ## Documentation
-* [Toloka-Kit documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka API reference](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka-Kit documentation](https://toloka.ai/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka API reference](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka web interface documentation](https://toloka.ai/docs/guide/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
 
 ## Support
 * To suggest a feature or report a bug, go to our [issues page](https://github.com/Toloka/toloka-kit/issues).
 * If you have any questions, feel free to ask our [Slack community](https://toloka.ai/community/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 ## Contributing
 Feel free to contribute to toloka-kit. Right now, we need more [usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#need-more-examples).
```

### Comparing `toloka-kit-1.2.0/README.md` & `toloka-kit-1.2.0.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/toloka-kit.svg)](https://pypi.org/project/toloka-kit/)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/toloka-kit.svg)](https://pypi.org/project/toloka-kit)
 [![Downloads](https://pepy.tech/badge/toloka-kit/month)](https://pepy.tech/project/toloka-kit)
 
 [![Coverage](https://codecov.io/gh/Toloka/toloka-kit/branch/main/graph/badge.svg)](https://codecov.io/gh/Toloka/toloka-kit)
 [![GitHub Tests](https://github.com/Toloka/toloka-kit/workflows/Tests/badge.svg?branch=main)](//github.com/Toloka/toloka-kit/actions?query=workflow:Tests)
 
-[Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
+[Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
 
 
 
-Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
+Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 The API allows you to build scalable and fully automated human-in-the-loop ML pipelines, and integrate them into your processes. The toolkit makes integration easier. You can use it with Jupyter notebooks.
 
 * Support for all common Toloka use cases: creating projects, adding pools, uploading tasks, and so on.
 * Toloka entities are represented as Python classes. You can use them instead of accessing the API using JSON representations.
 * There’s no need to validate JSON files and work with them directly.
 * Support of both synchronous and asynchronous (via async/await) executions.
-* Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation. 
+* Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation.
 * [AutoQuality](https://medium.com/toloka/automating-crowdsourcing-quality-control-ad057baf00fd) feature which automatically finds the best fitting quality control rules for your project.
 
 ## Prerequisites
 
 Before you begin, make sure that:
 * You are using [Python](https://www.python.org/) v3.7 or higher.
-* You are [registered](https://toloka.ai/docs/guide/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
-* You have [topped up](https://toloka.ai/docs/guide/concepts/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
-* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
+* You are [registered](https://toloka.ai/docs/guide/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
+* You have [topped up](https://toloka.ai/docs/guide/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
+* You have [set up an OAuth token](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit#overview--accessing-the-api) to access Toloka API.
 
 ## Get Started
 1. Install the Toloka-Kit package. Run the following command in the command shell:
 ```
 $ pip install toloka-kit
 ```
 For production environments, specify the exact package version. For the latest stable version, check the [project page at pypi.org](https://pypi.org/project/toloka-kit/).
@@ -69,17 +69,17 @@
 $ pip install toloka-kit[pandas,autoquality,s3,zookeeper,jupyter-metrics] # remove unnecessary requirements from the list
 ```
 
 ## Usage examples
 [Toloka-kit usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#toloka-kit-usage-examples) - tutorials for specific data labeling tasks. They demonstrate how to work with Toloka API using Toloka-Kit.
 
 ## Documentation
-* [Toloka-Kit documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka API reference](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka-Kit documentation](https://toloka.ai/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka API reference](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka web interface documentation](https://toloka.ai/docs/guide/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
 
 ## Support
 * To suggest a feature or report a bug, go to our [issues page](https://github.com/Toloka/toloka-kit/issues).
 * If you have any questions, feel free to ask our [Slack community](https://toloka.ai/community/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 ## Contributing
 Feel free to contribute to toloka-kit. Right now, we need more [usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#need-more-examples).
```

### Comparing `toloka-kit-1.2.0/setup.py` & `toloka-kit-1.2.0.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         'simplejson',
         'docstring-parser',
         'tqdm',
     ],
     extras_require=EXTRAS_REQUIRE,
     include_package_data=True,
     project_urls={
-        'Documentation': 'https://toloka.ai/en/docs/toloka-kit',
+        'Documentation': 'https://toloka.ai/docs/toloka-kit',
         'Source': 'https://github.com/Toloka/toloka-kit',
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `toloka-kit-1.2.0/src/async_client/client.py` & `toloka-kit-1.2.0.post1/src/async_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from ..util.async_utils import generate_async_methods_from
 
 logger = logging.getLogger(__name__)
 
 
 @generate_async_methods_from(TolokaClient)
 class AsyncTolokaClient:
-    """Class that implements interaction with [Toloka API](https://toloka.ai/en/docs/api/), in an asynchronous way.
+    """Class that implements interaction with [Toloka API](https://toloka.ai/docs/api/api-reference/), in an asynchronous way.
 
     All methods are wrapped as async. So all methods calls must be awaited.
     All arguments, same as in TolokaClient.
     """
 
     @functools.wraps(TolokaClient.__init__)
     def __init__(
```

### Comparing `toloka-kit-1.2.0/src/async_client/client.pyi` & `toloka-kit-1.2.0.post1/src/async_client/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import toloka.util.async_utils
 import typing
 import urllib3.util.retry
 import uuid
 
 
 class AsyncTolokaClient:
-    """Class that implements interaction with [Toloka API](https://toloka.ai/en/docs/api/), in an asynchronous way.
+    """Class that implements interaction with [Toloka API](https://toloka.ai/docs/api/api-reference/), in an asynchronous way.
 
     All methods are wrapped as async. So all methods calls must be awaited.
     All arguments, same as in TolokaClient.
     """
 
     def __init__(
         self,
@@ -86,15 +86,15 @@
     async def aggregate_solutions_by_pool(self, request: toloka.client.aggregation.PoolAggregatedSolutionRequest) -> toloka.client.operations.AggregatedSolutionOperation:
         """Starts aggregation of responses in all completed tasks in a pool.
 
         The method starts the aggregation process on the Toloka server. To wait for the completion of the operation use the [wait_operation](toloka.client.TolokaClient.wait_operation.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Parameters describing in which pool to aggregate responses and by what rules.
 
         Returns:
@@ -126,15 +126,15 @@
     ) -> toloka.client.operations.AggregatedSolutionOperation:
         """Starts aggregation of responses in all completed tasks in a pool.
 
         The method starts the aggregation process on the Toloka server. To wait for the completion of the operation use the [wait_operation](toloka.client.TolokaClient.wait_operation.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Parameters describing in which pool to aggregate responses and by what rules.
 
         Returns:
@@ -157,15 +157,15 @@
 
     @typing.overload
     async def aggregate_solutions_by_task(self, request: toloka.client.aggregation.WeightedDynamicOverlapTaskAggregatedSolutionRequest) -> toloka.client.aggregation.AggregatedSolution:
         """Aggregates responses to a single task on the Toloka server.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Aggregation parameters.
 
         Returns:
@@ -194,15 +194,15 @@
         answer_weight_skill_id: typing.Optional[str] = None,
         fields: typing.Optional[typing.List[toloka.client.aggregation.WeightedDynamicOverlapTaskAggregatedSolutionRequest.Field]] = None
     ) -> toloka.client.aggregation.AggregatedSolution:
         """Aggregates responses to a single task on the Toloka server.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Aggregation parameters.
 
         Returns:
@@ -324,15 +324,15 @@
 
         `get_aggregated_solutions` returns a generator. You can iterate over all found aggregated responses using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort aggregated responses use the [find_aggregated_solutions](toloka.client.TolokaClient.find_aggregated_solutions.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             operation_id: The ID of the aggregation operation.
             request: Search criteria.
             batch_size: Returned aggregated responses limit for each request. The default batch_size is 50. The maximum allowed limit is 100,000.
@@ -371,15 +371,15 @@
 
         `get_aggregated_solutions` returns a generator. You can iterate over all found aggregated responses using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort aggregated responses use the [find_aggregated_solutions](toloka.client.TolokaClient.find_aggregated_solutions.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             operation_id: The ID of the aggregation operation.
             request: Search criteria.
             batch_size: Returned aggregated responses limit for each request. The default batch_size is 50. The maximum allowed limit is 100,000.
@@ -3794,25 +3794,25 @@
 
     @typing.overload
     async def create_user_bonuses(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         parameters: typing.Optional[toloka.client.user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
-        """Creates rewards for Tolokers.
+        """Creates bonuses for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
             parameters: Parameters for UserBonus creation controlling.
 
         Returns:
-            UserBonusBatchCreateResult: Result of creating rewards. Contains `UserBonus` instances in `items` and
+            UserBonusBatchCreateResult: Result of creating bonuses. Contains `UserBonus` instances in `items` and
                 problems in `validation_errors`.
 
         Example:
             >>> import decimal
             >>> new_bonuses=[
             >>>     UserBonus(
             >>>         user_id='1',
@@ -3851,25 +3851,25 @@
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
         async_mode: typing.Optional[bool] = True,
         skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
-        """Creates rewards for Tolokers.
+        """Creates bonuses for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
             parameters: Parameters for UserBonus creation controlling.
 
         Returns:
-            UserBonusBatchCreateResult: Result of creating rewards. Contains `UserBonus` instances in `items` and
+            UserBonusBatchCreateResult: Result of creating bonuses. Contains `UserBonus` instances in `items` and
                 problems in `validation_errors`.
 
         Example:
             >>> import decimal
             >>> new_bonuses=[
             >>>     UserBonus(
             >>>         user_id='1',
@@ -4015,27 +4015,27 @@
     @typing.overload
     async def find_user_bonuses(
         self,
         request: toloka.client.search_requests.UserBonusSearchRequest,
         sort: typing.Union[typing.List[str], toloka.client.search_requests.UserBonusSortItems, None] = None,
         limit: typing.Optional[int] = None
     ) -> toloka.client.search_results.UserBonusSearchResult:
-        """Finds Tolokers' rewards that match certain criteria.
+        """Finds Tolokers' bonuses that match certain criteria.
 
-        The number of returned rewards is limited. To find remaining rewards call `find_user_bonuses` with updated search criteria.
+        The number of returned bonuses is limited. To find remaining bonuses call `find_user_bonuses` with updated search criteria.
 
-        To iterate over all matching Tolokers' rewards you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
+        To iterate over all matching Tolokers' bonuses you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
-            limit: Returned Tolokers' rewards limit. The maximum allowed limit is 300.
+            limit: Returned Tolokers' bonuses limit. The maximum allowed limit is 300.
 
         Returns:
-            UserBonusSearchResult: Found Tolokers' rewards and a flag showing whether there are more matching rewards exceeding the limit.
+            UserBonusSearchResult: Found Tolokers' bonuses and a flag showing whether there are more matching bonuses exceeding the limit.
 
         Example:
             >>> toloka_client.find_user_bonuses(user_id='1', sort=['-created', '-id'], limit=3)
             ...
         """
         ...
 
@@ -4052,67 +4052,67 @@
         created_lt: typing.Optional[datetime.datetime] = None,
         created_lte: typing.Optional[datetime.datetime] = None,
         created_gt: typing.Optional[datetime.datetime] = None,
         created_gte: typing.Optional[datetime.datetime] = None,
         sort: typing.Union[typing.List[str], toloka.client.search_requests.UserBonusSortItems, None] = None,
         limit: typing.Optional[int] = None
     ) -> toloka.client.search_results.UserBonusSearchResult:
-        """Finds Tolokers' rewards that match certain criteria.
+        """Finds Tolokers' bonuses that match certain criteria.
 
-        The number of returned rewards is limited. To find remaining rewards call `find_user_bonuses` with updated search criteria.
+        The number of returned bonuses is limited. To find remaining bonuses call `find_user_bonuses` with updated search criteria.
 
-        To iterate over all matching Tolokers' rewards you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
+        To iterate over all matching Tolokers' bonuses you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
-            limit: Returned Tolokers' rewards limit. The maximum allowed limit is 300.
+            limit: Returned Tolokers' bonuses limit. The maximum allowed limit is 300.
 
         Returns:
-            UserBonusSearchResult: Found Tolokers' rewards and a flag showing whether there are more matching rewards exceeding the limit.
+            UserBonusSearchResult: Found Tolokers' bonuses and a flag showing whether there are more matching bonuses exceeding the limit.
 
         Example:
             >>> toloka_client.find_user_bonuses(user_id='1', sort=['-created', '-id'], limit=3)
             ...
         """
         ...
 
     async def get_user_bonus(self, user_bonus_id: str) -> toloka.client.user_bonus.UserBonus:
-        """Gets information about a Toloker's reward.
+        """Gets information about a Toloker's bonus.
 
         Args:
-            user_bonus_id: The ID of the reward.
+            user_bonus_id: The ID of the bonus.
 
         Returns:
-            UserBonus: The information about the reward.
+            UserBonus: The information about the bonus.
 
         Example:
             >>> toloka_client.get_user_bonus(user_bonus_id='1')
             ...
         """
         ...
 
     @typing.overload
     def get_user_bonuses(
         self,
         request: toloka.client.search_requests.UserBonusSearchRequest,
         batch_size: typing.Optional[int] = None
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.user_bonus.UserBonus, None]:
-        """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
+        """Finds all Tolokers' bonuses that match certain rules and returns them in an iterable object
 
-        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
+        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' bonuses using the generator. Several requests to the Toloka server are possible while iterating.
 
-        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort bonuses use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
-            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+            batch_size: Returned Tolokers' bonuses limit for each request. The maximum allowed `batch_size` is 300.
 
         Yields:
-            UserBonus: The next matching Toloker's reward.
+            UserBonus: The next matching Toloker's bonus.
 
         Example:
             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
             ...
         """
         ...
 
@@ -4128,26 +4128,26 @@
         id_gte: typing.Optional[str] = None,
         created_lt: typing.Optional[datetime.datetime] = None,
         created_lte: typing.Optional[datetime.datetime] = None,
         created_gt: typing.Optional[datetime.datetime] = None,
         created_gte: typing.Optional[datetime.datetime] = None,
         batch_size: typing.Optional[int] = None
     ) -> toloka.util.async_utils.AsyncGenAdapter[toloka.client.user_bonus.UserBonus, None]:
-        """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
+        """Finds all Tolokers' bonuses that match certain rules and returns them in an iterable object
 
-        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
+        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' bonuses using the generator. Several requests to the Toloka server are possible while iterating.
 
-        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort bonuses use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
-            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+            batch_size: Returned Tolokers' bonuses limit for each request. The maximum allowed `batch_size` is 300.
 
         Yields:
-            UserBonus: The next matching Toloker's reward.
+            UserBonus: The next matching Toloker's bonus.
 
         Example:
             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
             ...
         """
         ...
 
@@ -5409,15 +5409,15 @@
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_item = {
             >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
             >>>     'input_data' : {
-            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'
             >>>     }
             >>> }
             >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
             >>> print(new_item.created_at)
             ...
 
         Args:
@@ -5442,15 +5442,15 @@
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_item = {
             >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
             >>>     'input_data' : {
-            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'
             >>>     }
             >>> }
             >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
             >>> print(new_item.created_at)
             ...
 
         Args:
@@ -5471,16 +5471,16 @@
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
@@ -5498,16 +5498,16 @@
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
@@ -5679,16 +5679,16 @@
         """Creates a batch with task items in an App project in Toloka.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
@@ -5709,16 +5709,16 @@
         """Creates a batch with task items in an App project in Toloka.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
```

### Comparing `toloka-kit-1.2.0/src/autoquality/optimizer.py` & `toloka-kit-1.2.0.post1/src/autoquality/optimizer.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/autoquality/optimizer.pyi` & `toloka-kit-1.2.0.post1/src/autoquality/optimizer.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/autoquality/scoring.py` & `toloka-kit-1.2.0.post1/src/autoquality/scoring.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/autoquality/scoring.pyi` & `toloka-kit-1.2.0.post1/src/autoquality/scoring.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/__init__.py` & `toloka-kit-1.2.0.post1/src/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,27 +166,27 @@
 from ..util._codegen import expand
 from .webhook_subscription import WebhookSubscription
 
 logger = logging.getLogger(__name__)
 
 
 class TolokaClient:
-    """Class that implements interaction with [Toloka API](https://toloka.ai/en/docs/api/).
+    """Class that implements interaction with [Toloka API](https://toloka.ai/docs/api/api-reference/).
 
     Objects of other classes are created and modified only in memory of your computer.
     You can transfer information about these objects to Toloka only by calling one of the `TolokaClient` methods.
 
     For example, creating an instance of `Project` class will not add a project to Toloka right away. It will create a `Project` instance in your local memory.
     You need to call the `TolokaClient.create_project` method and pass the created project instance to it.
     Likewise, if you read a project using the `TolokaClient.get_project` method, you will get an instance of `Project` class.
     But if you change some parameters in this object manually in your code, it will not affect the existing project in Toloka.
     Call `TolokaClient.update_project` and pass the `Project` to apply your changes.
 
     Args:
-        token: Your OAuth token for Toloka. You can learn more about how to get it [here](https://toloka.ai/en/docs/api/concepts/access#token)
+        token: Your OAuth token for Toloka. You can learn more about how to get it [here](https://toloka.ai/docs/api/api-reference/#overview--accessing-the-api)
         environment: There are two environments in Toloka:
             * `SANDBOX` – [Testing environment](https://sandbox.toloka.dev) for Toloka requesters.
             You can test complex projects before assigning tasks to Tolokers. Nobody will see your tasks, and it's free.
             * `PRODUCTION` – [Production environment](https://toloka.dev) for Toloka requesters.
             You spend money there and get the results.
 
             You need to register in each environment separately. OAuth tokens are generated in each environment separately too.
@@ -216,15 +216,15 @@
             * `DAY` - Retry daily quotas. We do not recommend retrying these quotas.
 
             Default value: `MIN`.
         retryer_factory: Factory that creates `Retry` object.
             Fully specified retry policy that will apply to all requests.
             Default value: `None`.
         act_under_account_id: ID of the requester that has been shared access with the current token owner account.
-            All requests will be made using a specified account. See [Shared access to the requester's account](https://toloka.ai/en/docs/guide/concepts/multiple-access)
+            All requests will be made using a specified account. See [Shared access to the requester's account](https://toloka.ai/docs/guide/multiple-access)
             documentation page. ID of the requester can be retrieved using the [get_requester](toloka.client.TolokaClient.get_requester.md)
             method (this method should be called by the account owner using account's token).
         verify: SSL certificates (a.k.a CA bundle) used to
             verify the identity of requested hosts. Either `True` (default CA bundle),
             a path to an SSL certificate file, an `ssl.SSLContext`, or `False`
             (which will disable verification)
 
@@ -331,15 +331,15 @@
             return False
         dot_pos = self.token.find('.')
         return 21 < dot_pos < 25
 
     @property
     def _headers(self):
         headers = {
-            'Authorization': f'ApiKey {self.token}' if self.__is_apikey() else 'OAuth {self.token}',
+            'Authorization': f'ApiKey {self.token}' if self.__is_apikey() else f'OAuth {self.token}',
             'User-Agent': f'python-toloka-client-{__version__}',
         }
         if self.act_under_account_id:
             headers['X-Act-Under-Account-ID'] = self.act_under_account_id
         return headers
 
     def _do_request_with_retries(self, method, path, **kwargs):
@@ -569,15 +569,15 @@
     ) -> operations.AggregatedSolutionOperation:
         """Starts aggregation of responses in all completed tasks in a pool.
 
         The method starts the aggregation process on the Toloka server. To wait for the completion of the operation use the [wait_operation](toloka.client.TolokaClient.wait_operation.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Parameters describing in which pool to aggregate responses and by what rules.
 
         Returns:
@@ -603,15 +603,15 @@
     @expand('request')
     @add_headers('client')
     def aggregate_solutions_by_task(self, request: aggregation.WeightedDynamicOverlapTaskAggregatedSolutionRequest) -> AggregatedSolution:
         """Aggregates responses to a single task on the Toloka server.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Aggregation parameters.
 
         Returns:
@@ -687,15 +687,15 @@
 
         `get_aggregated_solutions` returns a generator. You can iterate over all found aggregated responses using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort aggregated responses use the [find_aggregated_solutions](toloka.client.TolokaClient.find_aggregated_solutions.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             operation_id: The ID of the aggregation operation.
             request: Search criteria.
             batch_size: Returned aggregated responses limit for each request. The default batch_size is 50. The maximum allowed limit is 100,000.
@@ -3033,25 +3033,25 @@
 
     @expand('parameters')
     @add_headers('client')
     def create_user_bonuses(
         self,
         user_bonuses: List[UserBonus], parameters: Optional[user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> batch_create_results.UserBonusBatchCreateResult:
-        """Creates rewards for Tolokers.
+        """Creates bonuses for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
             parameters: Parameters for UserBonus creation controlling.
 
         Returns:
-            UserBonusBatchCreateResult: Result of creating rewards. Contains `UserBonus` instances in `items` and
+            UserBonusBatchCreateResult: Result of creating bonuses. Contains `UserBonus` instances in `items` and
                 problems in `validation_errors`.
 
         Example:
             >>> import decimal
             >>> new_bonuses=[
             >>>     UserBonus(
             >>>         user_id='1',
@@ -3151,45 +3151,45 @@
         )
 
     @expand('request')
     @add_headers('client')
     def find_user_bonuses(self, request: search_requests.UserBonusSearchRequest,
                           sort: Union[List[str], search_requests.UserBonusSortItems, None] = None,
                           limit: Optional[int] = None) -> search_results.UserBonusSearchResult:
-        """Finds Tolokers' rewards that match certain criteria.
+        """Finds Tolokers' bonuses that match certain criteria.
 
-        The number of returned rewards is limited. To find remaining rewards call `find_user_bonuses` with updated search criteria.
+        The number of returned bonuses is limited. To find remaining bonuses call `find_user_bonuses` with updated search criteria.
 
-        To iterate over all matching Tolokers' rewards you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
+        To iterate over all matching Tolokers' bonuses you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
-            limit: Returned Tolokers' rewards limit. The maximum allowed limit is 300.
+            limit: Returned Tolokers' bonuses limit. The maximum allowed limit is 300.
 
         Returns:
-            UserBonusSearchResult: Found Tolokers' rewards and a flag showing whether there are more matching rewards exceeding the limit.
+            UserBonusSearchResult: Found Tolokers' bonuses and a flag showing whether there are more matching bonuses exceeding the limit.
 
         Example:
             >>> toloka_client.find_user_bonuses(user_id='1', sort=['-created', '-id'], limit=3)
             ...
         """
         sort = None if sort is None else structure(sort, search_requests.UserBonusSortItems)
         response = self._search_request('get', '/v1/user-bonuses', request, sort, limit)
         return structure(response, search_results.UserBonusSearchResult)
 
     @add_headers('client')
     def get_user_bonus(self, user_bonus_id: str) -> UserBonus:
-        """Gets information about a Toloker's reward.
+        """Gets information about a Toloker's bonus.
 
         Args:
-            user_bonus_id: The ID of the reward.
+            user_bonus_id: The ID of the bonus.
 
         Returns:
-            UserBonus: The information about the reward.
+            UserBonus: The information about the bonus.
 
         Example:
             >>> toloka_client.get_user_bonus(user_bonus_id='1')
             ...
         """
         response = self._request('get', f'/v1/user-bonuses/{user_bonus_id}')
         return structure(response, UserBonus)
@@ -3197,26 +3197,26 @@
     @expand('request')
     @add_headers('client')
     def get_user_bonuses(
         self,
         request: search_requests.UserBonusSearchRequest,
         batch_size: Optional[int] = None
     ) -> Generator[UserBonus, None, None]:
-        """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
+        """Finds all Tolokers' bonuses that match certain rules and returns them in an iterable object
 
-        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
+        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' bonuses using the generator. Several requests to the Toloka server are possible while iterating.
 
-        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort bonuses use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
-            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+            batch_size: Returned Tolokers' bonuses limit for each request. The maximum allowed `batch_size` is 300.
 
         Yields:
-            UserBonus: The next matching Toloker's reward.
+            UserBonus: The next matching Toloker's bonus.
 
         Example:
             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
             ...
         """
         generator = self._find_all(self.find_user_bonuses, request, batch_size=batch_size)
         yield from generator
@@ -4024,15 +4024,15 @@
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_item = {
             >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
             >>>     'input_data' : {
-            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'
             >>>     }
             >>> }
             >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
             >>> print(new_item.created_at)
             ...
 
         Args:
@@ -4055,16 +4055,16 @@
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
@@ -4171,16 +4171,16 @@
         """Creates a batch with task items in an App project in Toloka.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
```

### Comparing `toloka-kit-1.2.0/src/client/__init__.pyi` & `toloka-kit-1.2.0.post1/src/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -175,27 +175,27 @@
 from toloka.client.user_skill import (
     SetUserSkillRequest,
     UserSkill,
 )
 
 
 class TolokaClient:
-    """Class that implements interaction with [Toloka API](https://toloka.ai/en/docs/api/).
+    """Class that implements interaction with [Toloka API](https://toloka.ai/docs/api/api-reference/).
 
     Objects of other classes are created and modified only in memory of your computer.
     You can transfer information about these objects to Toloka only by calling one of the `TolokaClient` methods.
 
     For example, creating an instance of `Project` class will not add a project to Toloka right away. It will create a `Project` instance in your local memory.
     You need to call the `TolokaClient.create_project` method and pass the created project instance to it.
     Likewise, if you read a project using the `TolokaClient.get_project` method, you will get an instance of `Project` class.
     But if you change some parameters in this object manually in your code, it will not affect the existing project in Toloka.
     Call `TolokaClient.update_project` and pass the `Project` to apply your changes.
 
     Args:
-        token: Your OAuth token for Toloka. You can learn more about how to get it [here](https://toloka.ai/en/docs/api/concepts/access#token)
+        token: Your OAuth token for Toloka. You can learn more about how to get it [here](https://toloka.ai/docs/api/api-reference/#overview--accessing-the-api)
         environment: There are two environments in Toloka:
             * `SANDBOX` – [Testing environment](https://sandbox.toloka.dev) for Toloka requesters.
             You can test complex projects before assigning tasks to Tolokers. Nobody will see your tasks, and it's free.
             * `PRODUCTION` – [Production environment](https://toloka.dev) for Toloka requesters.
             You spend money there and get the results.
 
             You need to register in each environment separately. OAuth tokens are generated in each environment separately too.
@@ -225,15 +225,15 @@
             * `DAY` - Retry daily quotas. We do not recommend retrying these quotas.
 
             Default value: `MIN`.
         retryer_factory: Factory that creates `Retry` object.
             Fully specified retry policy that will apply to all requests.
             Default value: `None`.
         act_under_account_id: ID of the requester that has been shared access with the current token owner account.
-            All requests will be made using a specified account. See [Shared access to the requester's account](https://toloka.ai/en/docs/guide/concepts/multiple-access)
+            All requests will be made using a specified account. See [Shared access to the requester's account](https://toloka.ai/docs/guide/multiple-access)
             documentation page. ID of the requester can be retrieved using the [get_requester](toloka.client.TolokaClient.get_requester.md)
             method (this method should be called by the account owner using account's token).
         verify: SSL certificates (a.k.a CA bundle) used to
             verify the identity of requested hosts. Either `True` (default CA bundle),
             a path to an SSL certificate file, an `ssl.SSLContext`, or `False`
             (which will disable verification)
 
@@ -275,15 +275,15 @@
     def aggregate_solutions_by_pool(self, request: toloka.client.aggregation.PoolAggregatedSolutionRequest) -> toloka.client.operations.AggregatedSolutionOperation:
         """Starts aggregation of responses in all completed tasks in a pool.
 
         The method starts the aggregation process on the Toloka server. To wait for the completion of the operation use the [wait_operation](toloka.client.TolokaClient.wait_operation.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Parameters describing in which pool to aggregate responses and by what rules.
 
         Returns:
@@ -315,15 +315,15 @@
     ) -> toloka.client.operations.AggregatedSolutionOperation:
         """Starts aggregation of responses in all completed tasks in a pool.
 
         The method starts the aggregation process on the Toloka server. To wait for the completion of the operation use the [wait_operation](toloka.client.TolokaClient.wait_operation.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Parameters describing in which pool to aggregate responses and by what rules.
 
         Returns:
@@ -346,15 +346,15 @@
 
     @typing.overload
     def aggregate_solutions_by_task(self, request: toloka.client.aggregation.WeightedDynamicOverlapTaskAggregatedSolutionRequest) -> toloka.client.aggregation.AggregatedSolution:
         """Aggregates responses to a single task on the Toloka server.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Aggregation parameters.
 
         Returns:
@@ -383,15 +383,15 @@
         answer_weight_skill_id: typing.Optional[str] = None,
         fields: typing.Optional[typing.List[toloka.client.aggregation.WeightedDynamicOverlapTaskAggregatedSolutionRequest.Field]] = None
     ) -> toloka.client.aggregation.AggregatedSolution:
         """Aggregates responses to a single task on the Toloka server.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             request: Aggregation parameters.
 
         Returns:
@@ -513,15 +513,15 @@
 
         `get_aggregated_solutions` returns a generator. You can iterate over all found aggregated responses using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort aggregated responses use the [find_aggregated_solutions](toloka.client.TolokaClient.find_aggregated_solutions.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             operation_id: The ID of the aggregation operation.
             request: Search criteria.
             batch_size: Returned aggregated responses limit for each request. The default batch_size is 50. The maximum allowed limit is 100,000.
@@ -560,15 +560,15 @@
 
         `get_aggregated_solutions` returns a generator. You can iterate over all found aggregated responses using the generator. Several requests to the Toloka server are possible while iterating.
 
         If you need to sort aggregated responses use the [find_aggregated_solutions](toloka.client.TolokaClient.find_aggregated_solutions.md) method.
 
         {% note tip %}
 
-        Try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit). It has many aggregation methods and executes on your computer.
+        Try [crowd-kit library](https://toloka.ai/docs/crowd-kit). It has many aggregation methods and executes on your computer.
 
         {% endnote %}
 
         Args:
             operation_id: The ID of the aggregation operation.
             request: Search criteria.
             batch_size: Returned aggregated responses limit for each request. The default batch_size is 50. The maximum allowed limit is 100,000.
@@ -4023,25 +4023,25 @@
 
     @typing.overload
     def create_user_bonuses(
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         parameters: typing.Optional[toloka.client.user_bonus.UserBonusesCreateRequestParameters] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
-        """Creates rewards for Tolokers.
+        """Creates bonuses for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
             parameters: Parameters for UserBonus creation controlling.
 
         Returns:
-            UserBonusBatchCreateResult: Result of creating rewards. Contains `UserBonus` instances in `items` and
+            UserBonusBatchCreateResult: Result of creating bonuses. Contains `UserBonus` instances in `items` and
                 problems in `validation_errors`.
 
         Example:
             >>> import decimal
             >>> new_bonuses=[
             >>>     UserBonus(
             >>>         user_id='1',
@@ -4080,25 +4080,25 @@
         self,
         user_bonuses: typing.List[toloka.client.user_bonus.UserBonus],
         *,
         operation_id: typing.Optional[uuid.UUID] = ...,
         async_mode: typing.Optional[bool] = True,
         skip_invalid_items: typing.Optional[bool] = None
     ) -> toloka.client.batch_create_results.UserBonusBatchCreateResult:
-        """Creates rewards for Tolokers.
+        """Creates bonuses for Tolokers.
 
         Right now it's safer to use asynchronous version: "create_user_bonuses_async"
         You can send a maximum of 10,000 requests of this kind per day.
 
         Args:
             user_bonuses: To whom, how much to pay and for what.
             parameters: Parameters for UserBonus creation controlling.
 
         Returns:
-            UserBonusBatchCreateResult: Result of creating rewards. Contains `UserBonus` instances in `items` and
+            UserBonusBatchCreateResult: Result of creating bonuses. Contains `UserBonus` instances in `items` and
                 problems in `validation_errors`.
 
         Example:
             >>> import decimal
             >>> new_bonuses=[
             >>>     UserBonus(
             >>>         user_id='1',
@@ -4244,27 +4244,27 @@
     @typing.overload
     def find_user_bonuses(
         self,
         request: toloka.client.search_requests.UserBonusSearchRequest,
         sort: typing.Union[typing.List[str], toloka.client.search_requests.UserBonusSortItems, None] = None,
         limit: typing.Optional[int] = None
     ) -> toloka.client.search_results.UserBonusSearchResult:
-        """Finds Tolokers' rewards that match certain criteria.
+        """Finds Tolokers' bonuses that match certain criteria.
 
-        The number of returned rewards is limited. To find remaining rewards call `find_user_bonuses` with updated search criteria.
+        The number of returned bonuses is limited. To find remaining bonuses call `find_user_bonuses` with updated search criteria.
 
-        To iterate over all matching Tolokers' rewards you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
+        To iterate over all matching Tolokers' bonuses you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
-            limit: Returned Tolokers' rewards limit. The maximum allowed limit is 300.
+            limit: Returned Tolokers' bonuses limit. The maximum allowed limit is 300.
 
         Returns:
-            UserBonusSearchResult: Found Tolokers' rewards and a flag showing whether there are more matching rewards exceeding the limit.
+            UserBonusSearchResult: Found Tolokers' bonuses and a flag showing whether there are more matching bonuses exceeding the limit.
 
         Example:
             >>> toloka_client.find_user_bonuses(user_id='1', sort=['-created', '-id'], limit=3)
             ...
         """
         ...
 
@@ -4281,67 +4281,67 @@
         created_lt: typing.Optional[datetime.datetime] = None,
         created_lte: typing.Optional[datetime.datetime] = None,
         created_gt: typing.Optional[datetime.datetime] = None,
         created_gte: typing.Optional[datetime.datetime] = None,
         sort: typing.Union[typing.List[str], toloka.client.search_requests.UserBonusSortItems, None] = None,
         limit: typing.Optional[int] = None
     ) -> toloka.client.search_results.UserBonusSearchResult:
-        """Finds Tolokers' rewards that match certain criteria.
+        """Finds Tolokers' bonuses that match certain criteria.
 
-        The number of returned rewards is limited. To find remaining rewards call `find_user_bonuses` with updated search criteria.
+        The number of returned bonuses is limited. To find remaining bonuses call `find_user_bonuses` with updated search criteria.
 
-        To iterate over all matching Tolokers' rewards you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
+        To iterate over all matching Tolokers' bonuses you may use the [get_user_bonuses](toloka.client.TolokaClient.get_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
             sort: Sorting options. Default: `None`.
-            limit: Returned Tolokers' rewards limit. The maximum allowed limit is 300.
+            limit: Returned Tolokers' bonuses limit. The maximum allowed limit is 300.
 
         Returns:
-            UserBonusSearchResult: Found Tolokers' rewards and a flag showing whether there are more matching rewards exceeding the limit.
+            UserBonusSearchResult: Found Tolokers' bonuses and a flag showing whether there are more matching bonuses exceeding the limit.
 
         Example:
             >>> toloka_client.find_user_bonuses(user_id='1', sort=['-created', '-id'], limit=3)
             ...
         """
         ...
 
     def get_user_bonus(self, user_bonus_id: str) -> toloka.client.user_bonus.UserBonus:
-        """Gets information about a Toloker's reward.
+        """Gets information about a Toloker's bonus.
 
         Args:
-            user_bonus_id: The ID of the reward.
+            user_bonus_id: The ID of the bonus.
 
         Returns:
-            UserBonus: The information about the reward.
+            UserBonus: The information about the bonus.
 
         Example:
             >>> toloka_client.get_user_bonus(user_bonus_id='1')
             ...
         """
         ...
 
     @typing.overload
     def get_user_bonuses(
         self,
         request: toloka.client.search_requests.UserBonusSearchRequest,
         batch_size: typing.Optional[int] = None
     ) -> typing.Generator[toloka.client.user_bonus.UserBonus, None, None]:
-        """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
+        """Finds all Tolokers' bonuses that match certain rules and returns them in an iterable object
 
-        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
+        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' bonuses using the generator. Several requests to the Toloka server are possible while iterating.
 
-        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort bonuses use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
-            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+            batch_size: Returned Tolokers' bonuses limit for each request. The maximum allowed `batch_size` is 300.
 
         Yields:
-            UserBonus: The next matching Toloker's reward.
+            UserBonus: The next matching Toloker's bonus.
 
         Example:
             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
             ...
         """
         ...
 
@@ -4357,26 +4357,26 @@
         id_gte: typing.Optional[str] = None,
         created_lt: typing.Optional[datetime.datetime] = None,
         created_lte: typing.Optional[datetime.datetime] = None,
         created_gt: typing.Optional[datetime.datetime] = None,
         created_gte: typing.Optional[datetime.datetime] = None,
         batch_size: typing.Optional[int] = None
     ) -> typing.Generator[toloka.client.user_bonus.UserBonus, None, None]:
-        """Finds all Tolokers' rewards that match certain rules and returns them in an iterable object
+        """Finds all Tolokers' bonuses that match certain rules and returns them in an iterable object
 
-        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' rewards using the generator. Several requests to the Toloka server are possible while iterating.
+        `get_user_bonuses` returns a generator. You can iterate over all found Tolokers' bonuses using the generator. Several requests to the Toloka server are possible while iterating.
 
-        If you need to sort rewards use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
+        If you need to sort bonuses use the [find_user_bonuses](toloka.client.TolokaClient.find_user_bonuses.md) method.
 
         Args:
             request: Search criteria.
-            batch_size: Returned Tolokers' rewards limit for each request. The maximum allowed batch_size is 300.
+            batch_size: Returned Tolokers' bonuses limit for each request. The maximum allowed `batch_size` is 300.
 
         Yields:
-            UserBonus: The next matching Toloker's reward.
+            UserBonus: The next matching Toloker's bonus.
 
         Example:
             >>> bonuses = list(toloka_client.get_user_bonuses(created_lt='2021-06-01T00:00:00'))
             ...
         """
         ...
 
@@ -5638,15 +5638,15 @@
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_item = {
             >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
             >>>     'input_data' : {
-            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'
             >>>     }
             >>> }
             >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
             >>> print(new_item.created_at)
             ...
 
         Args:
@@ -5671,15 +5671,15 @@
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_item = {
             >>>     'batch_id' : '4Va2BBWKL88S4QyAgVje',
             >>>     'input_data' : {
-            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'
+            >>>         'id':'40', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'
             >>>     }
             >>> }
             >>> new_item = toloka_client.create_app_item(app_project_id = 'Q2d15QBjpwWuDz8Z321g', app_item = new_item)
             >>> print(new_item.created_at)
             ...
 
         Args:
@@ -5700,16 +5700,16 @@
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
@@ -5727,16 +5727,16 @@
         """Creates task items in an App project in Toloka and adds them to an existing batch.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'20', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'21', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_items(app_project_id = 'Q2d15QBjpwWuDz8Z321g', batch_id = '4Va2BBWKL88S4QyAgVje', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the App project.
             request: The request parameters.
@@ -5908,16 +5908,16 @@
         """Creates a batch with task items in an App project in Toloka.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
@@ -5938,16 +5938,16 @@
         """Creates a batch with task items in an App project in Toloka.
 
         Example:
             The following example is suitable for a project
             that requires `query` and `website_url` keys to be present in input data.
 
             >>> new_items = [
-            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/en/docs/toloka-kit'},
-            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/en/docs/crowd-kit'}
+            >>>     {'id':'30', 'query':'toloka kit', 'website_url':'https://toloka.ai/docs/toloka-kit'},
+            >>>     {'id':'31', 'query':'crowd kit', 'website_url':'https://toloka.ai/docs/crowd-kit'}
             >>> ]
             >>> toloka_client.create_app_batch(app_project_id = 'Q2d15QBjpwWuDz8Z321g', items = new_items)
             ...
 
         Args:
             app_project_id: The ID of the project.
             request: The request parameters.
```

### Comparing `toloka-kit-1.2.0/src/client/_converter.py` & `toloka-kit-1.2.0.post1/src/client/_converter.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/actions.py` & `toloka-kit-1.2.0.post1/src/client/actions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/actions.pyi` & `toloka-kit-1.2.0.post1/src/client/actions.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/aggregation.py` & `toloka-kit-1.2.0.post1/src/client/aggregation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for aggregating results
 
 This module has methods to aggregate answers and to estimate confidence in aggregated labels.
 Use it when each task is assigned to several Tolokers.  Note, that aggregation runs on the Toloka server.
 
 If you need advanced aggregation methods or want to run aggregation algorithms locally on your computer,
-try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit).
+try [crowd-kit library](https://toloka.ai/docs/crowd-kit).
 """
 
 __all__ = [
     'AggregatedSolutionType',
     'PoolAggregatedSolutionRequest',
     'TaskAggregatedSolutionRequest',
     'WeightedDynamicOverlapTaskAggregatedSolutionRequest',
@@ -30,16 +30,16 @@
 
 
 class PoolAggregatedSolutionRequest(BaseTolokaObject):
     """Parameters for aggregating results in a pool using the [aggregate_solutions_by_pool](toloka.client.TolokaClient.aggregate_solutions_by_pool.md) method.
 
     Attributes:
         type: Aggregation model:
-            * `WEIGHTED_DYNAMIC_OVERLAP` — [Aggregation](https://toloka.ai/en/docs/guide/concepts/result-aggregation#aggr-by-skill) based on Tolokers' skill in a pool with a dynamic overlap.
-            * `DAWID_SKENE` — [Dawid-Skene aggregation model](https://toloka.ai/en/docs/guide/concepts/result-aggregation#dawid-skene). It is used in pools without a dynamic overlap.
+            * `WEIGHTED_DYNAMIC_OVERLAP` — [Aggregation](https://toloka.ai/docs/guide/result-aggregation#aggr-by-skill) based on Tolokers' skill in a pool with a dynamic overlap.
+            * `DAWID_SKENE` — [Dawid-Skene aggregation model](https://toloka.ai/docs/guide/result-aggregation#dawid-skene). It is used in pools without a dynamic overlap.
         pool_id: The ID of the pool.
         answer_weight_skill_id: The ID of the skill that determines the weight of the Toloker's responses.
         fields: Output data fields to aggregate. For the best results, each of these fields should have limited number of response options.
             If the `DAWID_SKENE` aggregation type is selected, you can only specify one value.
     """
 
     class Field(BaseTolokaObject):
```

### Comparing `toloka-kit-1.2.0/src/client/aggregation.pyi` & `toloka-kit-1.2.0.post1/src/client/aggregation.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for aggregating results
 
 This module has methods to aggregate answers and to estimate confidence in aggregated labels.
 Use it when each task is assigned to several Tolokers.  Note, that aggregation runs on the Toloka server.
 
 If you need advanced aggregation methods or want to run aggregation algorithms locally on your computer,
-try [crowd-kit library](https://toloka.ai/en/docs/crowd-kit).
+try [crowd-kit library](https://toloka.ai/docs/crowd-kit).
 """
 
 __all__ = [
     'AggregatedSolutionType',
     'PoolAggregatedSolutionRequest',
     'TaskAggregatedSolutionRequest',
     'WeightedDynamicOverlapTaskAggregatedSolutionRequest',
@@ -28,16 +28,16 @@
 
 
 class PoolAggregatedSolutionRequest(toloka.client.primitives.base.BaseTolokaObject):
     """Parameters for aggregating results in a pool using the [aggregate_solutions_by_pool](toloka.client.TolokaClient.aggregate_solutions_by_pool.md) method.
 
     Attributes:
         type: Aggregation model:
-            * `WEIGHTED_DYNAMIC_OVERLAP` — [Aggregation](https://toloka.ai/en/docs/guide/concepts/result-aggregation#aggr-by-skill) based on Tolokers' skill in a pool with a dynamic overlap.
-            * `DAWID_SKENE` — [Dawid-Skene aggregation model](https://toloka.ai/en/docs/guide/concepts/result-aggregation#dawid-skene). It is used in pools without a dynamic overlap.
+            * `WEIGHTED_DYNAMIC_OVERLAP` — [Aggregation](https://toloka.ai/docs/guide/result-aggregation#aggr-by-skill) based on Tolokers' skill in a pool with a dynamic overlap.
+            * `DAWID_SKENE` — [Dawid-Skene aggregation model](https://toloka.ai/docs/guide/result-aggregation#dawid-skene). It is used in pools without a dynamic overlap.
         pool_id: The ID of the pool.
         answer_weight_skill_id: The ID of the skill that determines the weight of the Toloker's responses.
         fields: Output data fields to aggregate. For the best results, each of these fields should have limited number of response options.
             If the `DAWID_SKENE` aggregation type is selected, you can only specify one value.
     """
 
     class Field(toloka.client.primitives.base.BaseTolokaObject):
```

### Comparing `toloka-kit-1.2.0/src/client/analytics_request.py` & `toloka-kit-1.2.0.post1/src/client/analytics_request.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/analytics_request.pyi` & `toloka-kit-1.2.0.post1/src/client/analytics_request.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/app/__init__.py` & `toloka-kit-1.2.0.post1/src/client/app/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         name: The solution name.
     """
     id: str
     name: str
 
 
 class AppProject(BaseTolokaObject):
-    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) project.
+    """An [App](https://toloka.ai/docs/api/apps-reference/#tag--app-project) project.
 
     An App project is based on one of App solutions. It is created with a template interface and preconfigured data specification and quality control rules.
 
     To get available App solutions use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
 
     Attributes:
         app_id: The ID of the App solution used to create the project.
@@ -88,15 +88,15 @@
     item_price: decimal.Decimal = attribute(readonly=True)
     errors: List[_AppError] = attribute(readonly=True)
     read_only: bool = attribute(readonly=True)
     app: AppLightestResult = attribute(readonly=True)
 
 
 class App(BaseTolokaObject):
-    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) solution.
+    """An [App](https://toloka.ai/docs/api/apps-reference/#tag--app) solution.
 
     Each App solution targets specific type of tasks which can be solved using Toloka.
 
     Attributes:
         id: The ID of the App solution.
         name: The solution name.
         image: A link to the solution interface preview image.
```

### Comparing `toloka-kit-1.2.0/src/client/app/__init__.pyi` & `toloka-kit-1.2.0.post1/src/client/app/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     id: typing.Optional[str]
     name: typing.Optional[str]
 
 
 class AppProject(toloka.client.primitives.base.BaseTolokaObject):
-    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) project.
+    """An [App](https://toloka.ai/docs/api/apps-reference/#tag--app-project) project.
 
     An App project is based on one of App solutions. It is created with a template interface and preconfigured data specification and quality control rules.
 
     To get available App solutions use the [get_apps](toloka.client.TolokaClient.get_apps.md) method.
 
     Attributes:
         app_id: The ID of the App solution used to create the project.
@@ -130,15 +130,15 @@
     item_price: typing.Optional[decimal.Decimal]
     errors: typing.Optional[typing.List[_AppError]]
     read_only: typing.Optional[bool]
     app: typing.Optional[AppLightestResult]
 
 
 class App(toloka.client.primitives.base.BaseTolokaObject):
-    """An [App](https://toloka.ai/en/docs/toloka-apps/concepts/) solution.
+    """An [App](https://toloka.ai/docs/api/apps-reference/#tag--app) solution.
 
     Each App solution targets specific type of tasks which can be solved using Toloka.
 
     Attributes:
         id: The ID of the App solution.
         name: The solution name.
         image: A link to the solution interface preview image.
```

### Comparing `toloka-kit-1.2.0/src/client/assignment.py` & `toloka-kit-1.2.0.post1/src/client/assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             * `ACTIVE` — The task suite is assigned but it isn't completed yet.
             * `SUBMITTED` — The task suite is completed but it isn't checked.
             * `ACCEPTED` — The task suite is accepted by the requester.
             * `REJECTED` — The task suite is rejected by the requester.
             * `SKIPPED` — The task suite is skipped by the Toloker.
             * `EXPIRED` — Time for completing the tasks has expired.
         reward: Payment received by the Toloker.
-        bonus_ids: IDs of rewards issued for the task.
+        bonus_ids: IDs of bonuses issued for the task.
         tasks: Data for the tasks.
         automerged: Flag of the response received as a result of merging identical tasks. Value:
             * `True` — The response was recorded when identical tasks were merged.
             * `False` — Normal Toloker response.
         created: The date and time when the task suite was assigned to a Toloker.
         submitted: The date and time when the task suite was completed by a Toloker.
         accepted: The date and time when the responses for the task suite were accepted by the requester.
```

### Comparing `toloka-kit-1.2.0/src/client/assignment.pyi` & `toloka-kit-1.2.0.post1/src/client/assignment.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             * `ACTIVE` — The task suite is assigned but it isn't completed yet.
             * `SUBMITTED` — The task suite is completed but it isn't checked.
             * `ACCEPTED` — The task suite is accepted by the requester.
             * `REJECTED` — The task suite is rejected by the requester.
             * `SKIPPED` — The task suite is skipped by the Toloker.
             * `EXPIRED` — Time for completing the tasks has expired.
         reward: Payment received by the Toloker.
-        bonus_ids: IDs of rewards issued for the task.
+        bonus_ids: IDs of bonuses issued for the task.
         tasks: Data for the tasks.
         automerged: Flag of the response received as a result of merging identical tasks. Value:
             * `True` — The response was recorded when identical tasks were merged.
             * `False` — Normal Toloker response.
         created: The date and time when the task suite was assigned to a Toloker.
         submitted: The date and time when the task suite was completed by a Toloker.
         accepted: The date and time when the responses for the task suite were accepted by the requester.
```

### Comparing `toloka-kit-1.2.0/src/client/attachment.py` & `toloka-kit-1.2.0.post1/src/client/attachment.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/attachment.pyi` & `toloka-kit-1.2.0.post1/src/client/attachment.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/batch_create_results.py` & `toloka-kit-1.2.0.post1/src/client/batch_create_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,20 @@
     Attributes:
         items: A dictionary with created task suites. The indexes of a `create_task_suites` input list are used as keys in the dictionary.
         validation_errors: A dictionary with validation errors in input task suites. It is filled if the request parameter `skip_invalid_items` is `True`.
     """
 )
 UserBonusBatchCreateResult = _create_batch_create_result_class_for(
     UserBonus,
-    """The result of issuing rewards for Tolokers.
+    """The result of issuing bonuses for Tolokers.
 
     `UserBonusBatchCreateResult` is returned by the [create_user_bonuses](toloka.client.TolokaClient.create_user_bonuses.md) method.
 
     Attributes:
-        items: A dictionary with created rewards. The indexes of a `create_user_bonuses` input list are used as keys in the dictionary.
+        items: A dictionary with created bonuses. The indexes of a `create_user_bonuses` input list are used as keys in the dictionary.
         validation_errors: A dictionary with validation errors. It is filled if the request parameter `skip_invalid_items` is `True`.
     """
 )
 WebhookSubscriptionBatchCreateResult = _create_batch_create_result_class_for(
     WebhookSubscription,
     """The result of creating webhook subscriptions.
```

### Comparing `toloka-kit-1.2.0/src/client/batch_create_results.pyi` & `toloka-kit-1.2.0.post1/src/client/batch_create_results.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -86,20 +86,20 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     items: typing.Optional[typing.Dict[str, toloka.client.task_suite.TaskSuite]]
     validation_errors: typing.Optional[typing.Dict[str, typing.Dict[str, FieldValidationError]]]
 
 
 class UserBonusBatchCreateResult(toloka.client.primitives.base.BaseTolokaObject):
-    """The result of issuing rewards for Tolokers.
+    """The result of issuing bonuses for Tolokers.
 
     `UserBonusBatchCreateResult` is returned by the [create_user_bonuses](toloka.client.TolokaClient.create_user_bonuses.md) method.
 
     Attributes:
-        items: A dictionary with created rewards. The indexes of a `create_user_bonuses` input list are used as keys in the dictionary.
+        items: A dictionary with created bonuses. The indexes of a `create_user_bonuses` input list are used as keys in the dictionary.
         validation_errors: A dictionary with validation errors. It is filled if the request parameter `skip_invalid_items` is `True`.
     """
 
     def __init__(
         self,
         *,
         items: typing.Optional[typing.Dict[str, toloka.client.user_bonus.UserBonus]] = None,
```

### Comparing `toloka-kit-1.2.0/src/client/clone_results.py` & `toloka-kit-1.2.0.post1/src/client/clone_results.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/clone_results.pyi` & `toloka-kit-1.2.0.post1/src/client/clone_results.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/collectors.py` & `toloka-kit-1.2.0.post1/src/client/collectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'Income',
     'MajorityVote',
     'SkippedInRowAssignments',
     'Training',
     'UsersAssessment'
 ]
 """
-https://toloka.ai/en/docs/guide/concepts/control
+https://toloka.ai/docs/guide/control
 """
 
 import logging
 
 from enum import unique
 from typing import ClassVar, FrozenSet, List, Optional
 from uuid import UUID
```

### Comparing `toloka-kit-1.2.0/src/client/collectors.pyi` & `toloka-kit-1.2.0.post1/src/client/collectors.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/conditions.py` & `toloka-kit-1.2.0.post1/src/client/conditions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/conditions.pyi` & `toloka-kit-1.2.0.post1/src/client/conditions.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/error_codes.py` & `toloka-kit-1.2.0.post1/src/client/error_codes.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/error_codes.pyi` & `toloka-kit-1.2.0.post1/src/client/error_codes.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/exceptions.py` & `toloka-kit-1.2.0.post1/src/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/exceptions.pyi` & `toloka-kit-1.2.0.post1/src/client/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/filter.py` & `toloka-kit-1.2.0.post1/src/client/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 
 
 @inherit_docstrings
 class City(Profile, InclusionConditionMixin, spec_value=Profile.Key.CITY):
     """Filtering Tolokers by a city specified in their profiles.
 
     Attributes:
-        value: The [ID](https://toloka.ai/en/docs/api/concepts/regions) of the city.
+        value: The [ID](https://toloka.ai/docs/api/regions) of the city.
     """
 
     value: int = attribute(required=True)
 
 
 @inherit_docstrings
 class Languages(Profile, InclusionConditionMixin, spec_value=Profile.Key.LANGUAGES):
@@ -485,26 +485,26 @@
 
 
 @inherit_docstrings
 class RegionByPhone(Computed, InclusionConditionMixin, spec_value=Computed.Key.REGION_BY_PHONE):
     """Filtering Tolokers by a region which is determined by their mobile phone number.
 
     Attributes:
-        value: The ID from the [list of regions](https://toloka.ai/en/docs/api/concepts/regions).
+        value: The ID from the [list of regions](https://toloka.ai/docs/api/regions).
     """
 
     value: int = attribute(required=True)
 
 
 @inherit_docstrings
 class RegionByIp(Computed, InclusionConditionMixin, spec_value=Computed.Key.REGION_BY_IP):
     """Filtering Tolokers by a region which is determined by their IP address.
 
     Attributes:
-        value: The ID from the [list of regions](https://toloka.ai/en/docs/api/concepts/regions).
+        value: The ID from the [list of regions](https://toloka.ai/docs/api/regions).
     """
 
     value: int = attribute(required=True)
 
 
 @inherit_docstrings
 class DeviceCategory(Computed, IdentityConditionMixin, spec_value=Computed.Key.DEVICE_CATEGORY):
```

### Comparing `toloka-kit-1.2.0/src/client/filter.pyi` & `toloka-kit-1.2.0.post1/src/client/filter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,15 @@
 
 class City(Profile, toloka.client.primitives.operators.InclusionConditionMixin):
     """Filtering Tolokers by a city specified in their profiles.
 
     Attributes:
         operator: An operator used in a condition.
             Allowed set of operators depends on the filter.
-        value: The [ID](https://toloka.ai/en/docs/api/concepts/regions) of the city.
+        value: The [ID](https://toloka.ai/docs/api/regions) of the city.
     """
 
     def __init__(
         self,
         operator: toloka.client.primitives.operators.InclusionOperator,
         value: int
     ) -> None:
@@ -497,15 +497,15 @@
 
 class RegionByPhone(Computed, toloka.client.primitives.operators.InclusionConditionMixin):
     """Filtering Tolokers by a region which is determined by their mobile phone number.
 
     Attributes:
         operator: An operator used in a condition.
             Allowed set of operators depends on the filter.
-        value: The ID from the [list of regions](https://toloka.ai/en/docs/api/concepts/regions).
+        value: The ID from the [list of regions](https://toloka.ai/docs/api/regions).
     """
 
     def __init__(
         self,
         operator: toloka.client.primitives.operators.InclusionOperator,
         value: int
     ) -> None:
@@ -520,15 +520,15 @@
 
 class RegionByIp(Computed, toloka.client.primitives.operators.InclusionConditionMixin):
     """Filtering Tolokers by a region which is determined by their IP address.
 
     Attributes:
         operator: An operator used in a condition.
             Allowed set of operators depends on the filter.
-        value: The ID from the [list of regions](https://toloka.ai/en/docs/api/concepts/regions).
+        value: The ID from the [list of regions](https://toloka.ai/docs/api/regions).
     """
 
     def __init__(
         self,
         operator: toloka.client.primitives.operators.InclusionOperator,
         value: int
     ) -> None:
```

### Comparing `toloka-kit-1.2.0/src/client/message_thread.py` & `toloka-kit-1.2.0.post1/src/client/message_thread.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/message_thread.pyi` & `toloka-kit-1.2.0.post1/src/client/message_thread.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/operation_log.py` & `toloka-kit-1.2.0.post1/src/client/operation_log.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict
 
 from .primitives.base import BaseTolokaObject
 
 
 # TODO: Add children through spec_field type and success.
 #  Add simple way of getting different objects of interest for every child.
-#  e.g. user_bonus_id for type=USER_BONUS_PERSIST, success=True (https://toloka.ai/docs/api/get-operation-log/)
+#  e.g. user_bonus_id for type=USER_BONUS_PERSIST, success=True (https://toloka.ai/docs/api/api-reference/#get-/operations/-id-/log)
 class OperationLogItem(BaseTolokaObject):
     """Objects of which the operation log consists
 
     Contains information about the validation errors and what sets of objects were created.
 
     Attributes:
         type: Type of action in the operation step.
```

### Comparing `toloka-kit-1.2.0/src/client/operation_log.pyi` & `toloka-kit-1.2.0.post1/src/client/operation_log.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/operations.py` & `toloka-kit-1.2.0.post1/src/client/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,17 +347,17 @@
 class UserBonusCreateBatchOperation(Operation, spec_value=OperationType.USER_BONUS_BATCH_CREATE):
     """Operation returned by the `TolokaClient.create_user_bonuses_async()` method.
 
     All parameters are for reference only and describe the initial parameters of the request that this operation monitors.
 
     Attributes:
         parameters.skip_invalid_items: Validation parameters for JSON objects:
-            * `True` — Create rewards using `UserBonus` instances that passed validation. Skip the rest of the `UserBonus` instances.
+            * `True` — Create bonuses using `UserBonus` instances that passed validation. Skip the rest of the `UserBonus` instances.
             * `False` — If at least one of the `UserBonus` instances didn't pass validation, stop the operation and
-                don't create any rewards.
+                don't create any bonuses.
         details.total_count: The number of bonuses in the request.
         details.valid_count: The number of JSON objects with bonus information that have passed validation.
         details.not_valid_count: The number of JSON objects with bonus information that failed validation.
         details.success_count: Number of bonuses issued.
         details.failed_count: The number of bonuses that were not issued.
     """
```

### Comparing `toloka-kit-1.2.0/src/client/operations.pyi` & `toloka-kit-1.2.0.post1/src/client/operations.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -883,17 +883,17 @@
         submitted: The UTC date and time the request was sent.
         started: The UTC date and time the operation started.
         finished: The UTC date and time the operation finished.
         progress: The percentage of the operation completed.
         parameters: Operation parameters (depending on the operation type).
         details: Details of the operation completion.
         parameters.skip_invalid_items: Validation parameters for JSON objects:
-            * `True` — Create rewards using `UserBonus` instances that passed validation. Skip the rest of the `UserBonus` instances.
+            * `True` — Create bonuses using `UserBonus` instances that passed validation. Skip the rest of the `UserBonus` instances.
             * `False` — If at least one of the `UserBonus` instances didn't pass validation, stop the operation and
-                don't create any rewards.
+                don't create any bonuses.
         details.total_count: The number of bonuses in the request.
         details.valid_count: The number of JSON objects with bonus information that have passed validation.
         details.not_valid_count: The number of JSON objects with bonus information that failed validation.
         details.success_count: Number of bonuses issued.
         details.failed_count: The number of bonuses that were not issued.
     """
```

### Comparing `toloka-kit-1.2.0/src/client/owner.py` & `toloka-kit-1.2.0.post1/src/client/owner.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/owner.pyi` & `toloka-kit-1.2.0.post1/src/client/owner.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/pool/__init__.py` & `toloka-kit-1.2.0.post1/src/client/pool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     """A set of [tasks](toloka.client.task.Task.md) that share the same properties.
 
     In the pool properties, you set the task price, overlap, Toloker selection filters, quality control rules, and so on.
 
     Pool tasks are grouped into [task suites](toloka.client.task_suite.TaskSuite.md). Whole task suites are assigned to Tolokers.
 
     Learn more about:
-    * [Pools](https://toloka.ai/en/docs/guide/concepts/pool-main)
-    * [Pricing](https://toloka.ai/en/docs/guide/concepts/dynamic-pricing)
+    * [Pools](https://toloka.ai/docs/guide/pool-main)
+    * [Pricing](https://toloka.ai/docs/guide/dynamic-pricing)
 
     Attributes:
         project_id: The ID of the project containing the pool.
         private_name: The pool name. It is visible to the requester and is not visible to Tolokers.
         may_contain_adult_content: The presence of adult content.
         reward_per_assignment: Payment in US dollars for a Toloker for completing a task suite. For cents, use the dot as a separator.
             If the pool `type` is `REGULAR`, the minimum payment per task suite is $0.005. For other pool types, you can set the `reward_per_assignment` to zero.
@@ -67,15 +67,15 @@
             * Dynamic overlap is enabled in the pool.
 
             Allowed range: from 0 to 259200 seconds (3 days). The default value is 0.
         dynamic_pricing_config: The dynamic pricing settings.
         auto_accept_solutions:
             * `True` — Responses from Tolokers are accepted or rejected automatically based on some rules.
             * `False` — Responses are checked manually. Time reserved for checking is limited by the `auto_accept_period_day` parameter.
-                Learn more about [non-automatic acceptance](https://toloka.ai/en/docs/guide/concepts/offline-accept).
+                Learn more about [non-automatic acceptance](https://toloka.ai/docs/guide/offline-accept).
         auto_accept_period_day: The number of days reserved for checking responses if the `auto_accept_solutions` parameter is set to `False`.
         assignments_issuing_config: Settings for assigning tasks in the pool.
         priority: The priority of the pool in relation to other pools in the project with the same task price and set of filters.
             Tolokers are assigned tasks with a higher priority first.
 
             Allowed range: from 0 to 100. The default value is 0.
         filter: Settings for Toloker selection filters.
@@ -116,15 +116,15 @@
     class AssignmentsIssuingConfig(BaseTolokaObject, kw_only=False):
         """Settings for assigning task suites in the pool.
 
         Attributes:
             issue_task_suites_in_creation_order:
                 Task suites are assigned in the order in which they were created.
 
-                This parameter is used when tasks are [grouped into suites](https://toloka.ai/en/docs/guide/concepts/distribute-tasks-by-pages)
+                This parameter is used when tasks are [grouped into suites](https://toloka.ai/docs/guide/distribute-tasks-by-pages)
                 manually and the `assignments_issuing_type` project parameter is set to `AUTOMATED`.
         """
 
         issue_task_suites_in_creation_order: bool
 
     @unique
     class CloseReason(ExtendableStrEnum):
```

### Comparing `toloka-kit-1.2.0/src/client/pool/__init__.pyi` & `toloka-kit-1.2.0.post1/src/client/pool/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     """A set of [tasks](toloka.client.task.Task.md) that share the same properties.
 
     In the pool properties, you set the task price, overlap, Toloker selection filters, quality control rules, and so on.
 
     Pool tasks are grouped into [task suites](toloka.client.task_suite.TaskSuite.md). Whole task suites are assigned to Tolokers.
 
     Learn more about:
-    * [Pools](https://toloka.ai/en/docs/guide/concepts/pool-main)
-    * [Pricing](https://toloka.ai/en/docs/guide/concepts/dynamic-pricing)
+    * [Pools](https://toloka.ai/docs/guide/pool-main)
+    * [Pricing](https://toloka.ai/docs/guide/dynamic-pricing)
 
     Attributes:
         project_id: The ID of the project containing the pool.
         private_name: The pool name. It is visible to the requester and is not visible to Tolokers.
         may_contain_adult_content: The presence of adult content.
         reward_per_assignment: Payment in US dollars for a Toloker for completing a task suite. For cents, use the dot as a separator.
             If the pool `type` is `REGULAR`, the minimum payment per task suite is $0.005. For other pool types, you can set the `reward_per_assignment` to zero.
@@ -66,15 +66,15 @@
             * Dynamic overlap is enabled in the pool.
 
             Allowed range: from 0 to 259200 seconds (3 days). The default value is 0.
         dynamic_pricing_config: The dynamic pricing settings.
         auto_accept_solutions:
             * `True` — Responses from Tolokers are accepted or rejected automatically based on some rules.
             * `False` — Responses are checked manually. Time reserved for checking is limited by the `auto_accept_period_day` parameter.
-                Learn more about [non-automatic acceptance](https://toloka.ai/en/docs/guide/concepts/offline-accept).
+                Learn more about [non-automatic acceptance](https://toloka.ai/docs/guide/offline-accept).
         auto_accept_period_day: The number of days reserved for checking responses if the `auto_accept_solutions` parameter is set to `False`.
         assignments_issuing_config: Settings for assigning tasks in the pool.
         priority: The priority of the pool in relation to other pools in the project with the same task price and set of filters.
             Tolokers are assigned tasks with a higher priority first.
 
             Allowed range: from 0 to 100. The default value is 0.
         filter: Settings for Toloker selection filters.
@@ -115,15 +115,15 @@
     class AssignmentsIssuingConfig(toloka.client.primitives.base.BaseTolokaObject):
         """Settings for assigning task suites in the pool.
 
         Attributes:
             issue_task_suites_in_creation_order:
                 Task suites are assigned in the order in which they were created.
 
-                This parameter is used when tasks are [grouped into suites](https://toloka.ai/en/docs/guide/concepts/distribute-tasks-by-pages)
+                This parameter is used when tasks are [grouped into suites](https://toloka.ai/docs/guide/distribute-tasks-by-pages)
                 manually and the `assignments_issuing_type` project parameter is set to `AUTOMATED`.
         """
 
         def __init__(self, issue_task_suites_in_creation_order: typing.Optional[bool] = None) -> None:
             """Method generated by attrs for class Pool.AssignmentsIssuingConfig.
             """
             ...
```

### Comparing `toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.py` & `toloka-kit-1.2.0.post1/src/client/pool/dynamic_overlap_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Dynamic overlap uses the `BASIC` algorithm.
     Each response is assigned a weight depending on the Toloker's skill value.
     The aggregated response confidence is calculated based on the probability algorithm.
     The task overlap increases until it reaches `max_overlap` or until the confidence of the aggregated response exceeds `min_confidence`.
 
     Note, that if you use dynamic overlap, then set the `auto_close_after_complete_delay_seconds` pool parameter to a non zero value.
 
-    Learn more about the [Dynamic overlap](https://toloka.ai/en/docs/guide/concepts/dynamic-overlap) in the guide.
+    Learn more about the [Dynamic overlap](https://toloka.ai/docs/guide/dynamic-overlap) in the guide.
 
     Attributes:
         type: The dynamic overlap algorithm.
         max_overlap: Maximum overlap. The value must be higher than the default overlap value. Allowed range: from 1 to 30,000.
         min_confidence: Minimum required confidence of the aggregated response. Allowed range: from 0 to 1.
         answer_weight_skill_id: A skill that determines the weight of the Toloker's responses.
             For the best results, use a skill calculated as a percentage of correct responses in control tasks.
```

### Comparing `toloka-kit-1.2.0/src/client/pool/dynamic_overlap_config.pyi` & `toloka-kit-1.2.0.post1/src/client/pool/dynamic_overlap_config.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Dynamic overlap uses the `BASIC` algorithm.
     Each response is assigned a weight depending on the Toloker's skill value.
     The aggregated response confidence is calculated based on the probability algorithm.
     The task overlap increases until it reaches `max_overlap` or until the confidence of the aggregated response exceeds `min_confidence`.
 
     Note, that if you use dynamic overlap, then set the `auto_close_after_complete_delay_seconds` pool parameter to a non zero value.
 
-    Learn more about the [Dynamic overlap](https://toloka.ai/en/docs/guide/concepts/dynamic-overlap) in the guide.
+    Learn more about the [Dynamic overlap](https://toloka.ai/docs/guide/dynamic-overlap) in the guide.
 
     Attributes:
         type: The dynamic overlap algorithm.
         max_overlap: Maximum overlap. The value must be higher than the default overlap value. Allowed range: from 1 to 30,000.
         min_confidence: Minimum required confidence of the aggregated response. Allowed range: from 0 to 1.
         answer_weight_skill_id: A skill that determines the weight of the Toloker's responses.
             For the best results, use a skill calculated as a percentage of correct responses in control tasks.
```

### Comparing `toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.py` & `toloka-kit-1.2.0.post1/src/client/pool/dynamic_pricing_config.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/pool/dynamic_pricing_config.pyi` & `toloka-kit-1.2.0.post1/src/client/pool/dynamic_pricing_config.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/pool/mixer_config.py` & `toloka-kit-1.2.0.post1/src/client/pool/mixer_config.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/pool/mixer_config.pyi` & `toloka-kit-1.2.0.post1/src/client/pool/mixer_config.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.py` & `toloka-kit-1.2.0.post1/src/client/pool/speed_quality_balance_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class SpeedQualityBalanceConfig(BaseTolokaObject, spec_enum='Type', spec_field='type'):
     """A configuration of selecting Tolokers based on a personalized quality forecast.
 
     Tolokers are sorted by their quality forecast. You can limit the number of the best Tolokers who have access to your tasks.
     It influences quality of results and speed of getting results.
 
-    Learn more about [Speed/quality balance](https://toloka.ai/en/docs/guide/concepts/adjust).
+    Learn more about [Speed/quality balance](https://toloka.ai/docs/guide/adjust).
     """
 
     @unique
     class Type(ExtendableStrEnum):
         """The type of the filter used in [SpeedQualityBalanceConfig](toloka.client.pool.speed_quality_balance_config.SpeedQualityBalanceConfig.md).
 
         Attributes:
```

### Comparing `toloka-kit-1.2.0/src/client/pool/speed_quality_balance_config.pyi` & `toloka-kit-1.2.0.post1/src/client/pool/speed_quality_balance_config.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class SpeedQualityBalanceConfig(toloka.client.primitives.base.BaseTolokaObject):
     """A configuration of selecting Tolokers based on a personalized quality forecast.
 
     Tolokers are sorted by their quality forecast. You can limit the number of the best Tolokers who have access to your tasks.
     It influences quality of results and speed of getting results.
 
-    Learn more about [Speed/quality balance](https://toloka.ai/en/docs/guide/concepts/adjust).
+    Learn more about [Speed/quality balance](https://toloka.ai/docs/guide/adjust).
     """
 
     class Type(toloka.util._extendable_enum.ExtendableStrEnum):
         """The type of the filter used in [SpeedQualityBalanceConfig](toloka.client.pool.speed_quality_balance_config.SpeedQualityBalanceConfig.md).
 
         Attributes:
             TOP_PERCENTAGE_BY_QUALITY: A percentage of the best Tolokers is configured.
```

### Comparing `toloka-kit-1.2.0/src/client/primitives/adapters.py` & `toloka-kit-1.2.0.post1/src/client/primitives/adapters.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/adapters.pyi` & `toloka-kit-1.2.0.post1/src/client/primitives/adapters.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/base.py` & `toloka-kit-1.2.0.post1/src/client/primitives/base.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/base.pyi` & `toloka-kit-1.2.0.post1/src/client/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/infinite_overlap.py` & `toloka-kit-1.2.0.post1/src/client/primitives/infinite_overlap.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/infinite_overlap.pyi` & `toloka-kit-1.2.0.post1/src/client/primitives/infinite_overlap.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/operators.py` & `toloka-kit-1.2.0.post1/src/client/primitives/operators.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/operators.pyi` & `toloka-kit-1.2.0.post1/src/client/primitives/operators.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/parameter.py` & `toloka-kit-1.2.0.post1/src/client/primitives/parameter.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/parameter.pyi` & `toloka-kit-1.2.0.post1/src/client/primitives/parameter.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 class IdempotentOperationParameters(Parameters):
     """Parameters for idempotent operations such as tasks, task suites and user bonuses creation.
 
     Works only with async_mode = True
 
     Attributes:
         operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+
+            We recommended sending the operation ID in the `POST` requests to avoid accidental errors:
+            when you send several requests with the same `operation_id`, the operation will be performed only once.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally.
             * `False` — The request is processed synchronously.
 
             Default value: `True`.
     """
```

### Comparing `toloka-kit-1.2.0/src/client/primitives/retry.py` & `toloka-kit-1.2.0.post1/src/client/primitives/retry.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/primitives/retry.pyi` & `toloka-kit-1.2.0.post1/src/client/primitives/retry.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/__init__.py` & `toloka-kit-1.2.0.post1/src/client/project/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,37 +60,37 @@
 from ...util._codegen import attribute
 from ...util._extendable_enum import ExtendableStrEnum
 
 
 class Project(BaseTolokaObject):
     """Top-level object in Toloka that describes one requester's objective.
 
-    If your task is complex, consider to [decompose](https://toloka.ai/en/docs/guide/concepts/solution-architecture) it into several projects.
+    If your task is complex, consider to [decompose](https://toloka.ai/docs/guide/solution-architecture) it into several projects.
     For example, one project finds images with some objects, another project describes image segmentation, and the third project checks this segmentation.
 
     In a project, you set properties for tasks and responses:
     * Input data parameters describe what kind of input data you have: images, text, and other.
     * Output data parameters describe Tolokers' responses. They are used to validate a data type, range of values, string length, and so on.
-    * Task interface. To learn how to define the appearance of tasks, see [Task interface](https://toloka.ai/en/docs/en/guide/concepts/spec) in the guide.
+    * Task interface. To learn how to define the appearance of tasks, see [Task interface](https://toloka.ai/docs/guide/spec) in the guide.
 
     You upload [tasks](toloka.client.task.Task.md) to project [pools](toloka.client.pool.Pool.md) and [training pools](toloka.client.training.Training.md).
     They are grouped into [task suites](toloka.client.task_suite.TaskSuite.md) and assigned to Tolokers.
 
     Attributes:
         public_name: The name of the project. Visible to Tolokers.
         public_description: The description of the project. Visible to Tolokers.
         public_instructions: Instructions for Tolokers describe what to do in the tasks. You can use any HTML markup in the instructions.
         private_comment: Comments about the project. Visible only to the requester.
         task_spec: Input and output data specification and the task interface.
-            The interface can be defined with HTML, CSS, and JS or using the [Template Builder](https://toloka.ai/en/docs/template-builder/) components.
+            The interface can be defined with HTML, CSS, and JS or using the [Template Builder](https://toloka.ai/docs/template-builder/) components.
         assignments_issuing_type: Settings for assigning tasks. Default value: `AUTOMATED`.
         assignments_issuing_view_config: The configuration of a task view on a map. Provide it if `assignments_issuing_type=MAP_SELECTOR`.
-        assignments_automerge_enabled: [Merging tasks](https://toloka.ai/en/docs/api/concepts/tasks#task-merge) control.
+        assignments_automerge_enabled: [Merging tasks](https://toloka.ai/docs/api/tasks) control.
         max_active_assignments_count: The number of task suites simultaneously assigned to a Toloker. Note, that Toloka counts assignments having the `ACTIVE` status only.
-        quality_control: [Quality control](https://toloka.ai/en/docs/guide/concepts/project-qa) rules.
+        quality_control: [Quality control](https://toloka.ai/docs/guide/project-qa) rules.
         localization_config: Translations to other languages.
         metadata: Additional information about the project.
         id: The ID of the project. Read-only field.
         status: A project status. Read-only field.
         created: The UTC date and time when the project was created. Read-only field.
 
     Example:
```

### Comparing `toloka-kit-1.2.0/src/client/project/__init__.pyi` & `toloka-kit-1.2.0.post1/src/client/project/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,37 +64,37 @@
     TemplateBuilderViewSpec,
 )
 
 
 class Project(toloka.client.primitives.base.BaseTolokaObject):
     """Top-level object in Toloka that describes one requester's objective.
 
-    If your task is complex, consider to [decompose](https://toloka.ai/en/docs/guide/concepts/solution-architecture) it into several projects.
+    If your task is complex, consider to [decompose](https://toloka.ai/docs/guide/solution-architecture) it into several projects.
     For example, one project finds images with some objects, another project describes image segmentation, and the third project checks this segmentation.
 
     In a project, you set properties for tasks and responses:
     * Input data parameters describe what kind of input data you have: images, text, and other.
     * Output data parameters describe Tolokers' responses. They are used to validate a data type, range of values, string length, and so on.
-    * Task interface. To learn how to define the appearance of tasks, see [Task interface](https://toloka.ai/en/docs/en/guide/concepts/spec) in the guide.
+    * Task interface. To learn how to define the appearance of tasks, see [Task interface](https://toloka.ai/docs/guide/spec) in the guide.
 
     You upload [tasks](toloka.client.task.Task.md) to project [pools](toloka.client.pool.Pool.md) and [training pools](toloka.client.training.Training.md).
     They are grouped into [task suites](toloka.client.task_suite.TaskSuite.md) and assigned to Tolokers.
 
     Attributes:
         public_name: The name of the project. Visible to Tolokers.
         public_description: The description of the project. Visible to Tolokers.
         public_instructions: Instructions for Tolokers describe what to do in the tasks. You can use any HTML markup in the instructions.
         private_comment: Comments about the project. Visible only to the requester.
         task_spec: Input and output data specification and the task interface.
-            The interface can be defined with HTML, CSS, and JS or using the [Template Builder](https://toloka.ai/en/docs/template-builder/) components.
+            The interface can be defined with HTML, CSS, and JS or using the [Template Builder](https://toloka.ai/docs/template-builder/) components.
         assignments_issuing_type: Settings for assigning tasks. Default value: `AUTOMATED`.
         assignments_issuing_view_config: The configuration of a task view on a map. Provide it if `assignments_issuing_type=MAP_SELECTOR`.
-        assignments_automerge_enabled: [Merging tasks](https://toloka.ai/en/docs/api/concepts/tasks#task-merge) control.
+        assignments_automerge_enabled: [Merging tasks](https://toloka.ai/docs/api/tasks) control.
         max_active_assignments_count: The number of task suites simultaneously assigned to a Toloker. Note, that Toloka counts assignments having the `ACTIVE` status only.
-        quality_control: [Quality control](https://toloka.ai/en/docs/guide/concepts/project-qa) rules.
+        quality_control: [Quality control](https://toloka.ai/docs/guide/project-qa) rules.
         localization_config: Translations to other languages.
         metadata: Additional information about the project.
         id: The ID of the project. Read-only field.
         status: A project status. Read-only field.
         created: The UTC date and time when the project was created. Read-only field.
 
     Example:
```

### Comparing `toloka-kit-1.2.0/src/client/project/field_spec.py` & `toloka-kit-1.2.0.post1/src/client/project/field_spec.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/field_spec.pyi` & `toloka-kit-1.2.0.post1/src/client/project/field_spec.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/localization.py` & `toloka-kit-1.2.0.post1/src/client/project/localization.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/localization.pyi` & `toloka-kit-1.2.0.post1/src/client/project/localization.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/task_spec.py` & `toloka-kit-1.2.0.post1/src/client/project/task_spec.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/task_spec.pyi` & `toloka-kit-1.2.0.post1/src/client/project/task_spec.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/__init__.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/__init__.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/actions.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/actions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/actions.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/actions.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/base.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/base.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/base.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/base.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/conditions.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/conditions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/conditions.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/conditions.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/data.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/data.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/data.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/data.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/fields.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/fields.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/fields.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/fields.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/helpers.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/helpers.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/helpers.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/helpers.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/layouts.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/layouts.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/layouts.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/layouts.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/plugins.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/plugins.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/plugins.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/plugins.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/view.py` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/view.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/template_builder/view.pyi` & `toloka-kit-1.2.0.post1/src/client/project/template_builder/view.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/project/view_spec.py` & `toloka-kit-1.2.0.post1/src/client/project/view_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     settings: Settings
 
 
 class ClassicViewSpec(ViewSpec, spec_value=ViewSpec.CLASSIC):
     """A task interface defined with HTML, CSS and JS.
 
-    For more information, see the [guide](https://toloka.ai/en/docs/guide/concepts/spec).
+    For more information, see the [guide](https://toloka.ai/docs/guide/spec).
 
     Attributes:
         markup: HTML markup of the task interface.
         styles: CSS for the task interface.
         script: JavaScript code for the task interface.
         assets: Links to external files.
     """
@@ -87,15 +87,15 @@
 
         You can link:
             * CSS libraries
             * JavaScript libraries
             * Toloka assets — libraries that can be linked using the `$TOLOKA_ASSETS` path:
                 * `$TOLOKA_ASSETS/js/toloka-handlebars-templates.js` — [Handlebars template engine](http://handlebarsjs.com/).
                 * `$TOLOKA_ASSETS/js/image-annotation.js` — Image labeling interface. Note, that this library requires Handlebars and must be linked after it.
-                    For more information, see [Image with area selection](https://toloka.ai/en/docs/guide/concepts/t-components/image-annotation).
+                    For more information, see [Image with area selection](https://toloka.ai/docs/guide/t-components/image-annotation).
 
             Add items in the order they should be linked.
 
         Attributes:
             style_urls: Links to CSS libraries.
             script_urls: Links to JavaScript libraries and Toloka assets.
 
@@ -119,15 +119,15 @@
     styles: str
     assets: Assets
 
 
 class TemplateBuilderViewSpec(ViewSpec, spec_value=ViewSpec.TEMPLATE_BUILDER):
     """A task interface defined with the [TemplateBuilder](toloka.client.project.template_builder.TemplateBuilder.md).
 
-    See also [Template Builder](https://toloka.ai/en/docs/template-builder/) in the guide.
+    See also [Template Builder](https://toloka.ai/docs/template-builder/) in the guide.
 
     Attributes:
         view: A top level component like [SideBySideLayoutV1](toloka.client.project.template_builder.layouts.SideBySideLayoutV1.md).
         plugins: An array of plugins.
         vars: Reusable data. It is referenced with the [RefComponent](toloka.client.project.template_builder.base.RefComponent.md).
         core_version: The default template components version. Most likely, you do not need to change this parameter.
         infer_data_spec:
```

### Comparing `toloka-kit-1.2.0/src/client/project/view_spec.pyi` & `toloka-kit-1.2.0.post1/src/client/project/view_spec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     settings: typing.Optional[Settings]
 
 
 class ClassicViewSpec(ViewSpec):
     """A task interface defined with HTML, CSS and JS.
 
-    For more information, see the [guide](https://toloka.ai/en/docs/guide/concepts/spec).
+    For more information, see the [guide](https://toloka.ai/docs/guide/spec).
 
     Attributes:
         markup: HTML markup of the task interface.
         styles: CSS for the task interface.
         script: JavaScript code for the task interface.
         assets: Links to external files.
     """
@@ -101,15 +101,15 @@
 
         You can link:
             * CSS libraries
             * JavaScript libraries
             * Toloka assets — libraries that can be linked using the `$TOLOKA_ASSETS` path:
                 * `$TOLOKA_ASSETS/js/toloka-handlebars-templates.js` — [Handlebars template engine](http://handlebarsjs.com/).
                 * `$TOLOKA_ASSETS/js/image-annotation.js` — Image labeling interface. Note, that this library requires Handlebars and must be linked after it.
-                    For more information, see [Image with area selection](https://toloka.ai/en/docs/guide/concepts/t-components/image-annotation).
+                    For more information, see [Image with area selection](https://toloka.ai/docs/guide/t-components/image-annotation).
 
             Add items in the order they should be linked.
 
         Attributes:
             style_urls: Links to CSS libraries.
             script_urls: Links to JavaScript libraries and Toloka assets.
 
@@ -160,15 +160,15 @@
     styles: typing.Optional[str]
     assets: typing.Optional[Assets]
 
 
 class TemplateBuilderViewSpec(ViewSpec):
     """A task interface defined with the [TemplateBuilder](toloka.client.project.template_builder.TemplateBuilder.md).
 
-    See also [Template Builder](https://toloka.ai/en/docs/template-builder/) in the guide.
+    See also [Template Builder](https://toloka.ai/docs/template-builder/) in the guide.
 
     Attributes:
         view: A top level component like [SideBySideLayoutV1](toloka.client.project.template_builder.layouts.SideBySideLayoutV1.md).
         plugins: An array of plugins.
         vars: Reusable data. It is referenced with the [RefComponent](toloka.client.project.template_builder.base.RefComponent.md).
         core_version: The default template components version. Most likely, you do not need to change this parameter.
         infer_data_spec:
```

### Comparing `toloka-kit-1.2.0/src/client/quality_control.py` & `toloka-kit-1.2.0.post1/src/client/quality_control.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/quality_control.pyi` & `toloka-kit-1.2.0.post1/src/client/quality_control.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/requester.py` & `toloka-kit-1.2.0.post1/src/client/requester.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/requester.pyi` & `toloka-kit-1.2.0.post1/src/client/requester.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/search_requests.py` & `toloka-kit-1.2.0.post1/src/client/search_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -745,51 +745,51 @@
         >>> result = toloka_client.find_user_restrictions(pool_id=my_pretty_pool_id, sort=sort, limit=10)
         ...
     """
 )
 
 
 class UserBonusSearchRequest(BaseSearchRequest):
-    """Parameters for searching Tolokers' rewards.
+    """Parameters for searching Tolokers' bonuses.
 
     Attributes:
         user_id: The ID of a Toloker.
-        assignment_id: The ID of an assignment a reward was granted for.
-        private_comment: Rewards with specified comment.
-        id_lt: Rewards with IDs less than the specified value.
-        id_lte: Rewards with IDs less than or equal to the specified value.
-        id_gt: Rewards with IDs greater than the specified value.
-        id_gte: Rewards with IDs greater than or equal to the specified value.
-        created_lt: Rewards given before the specified date.
-        created_lte: Rewards given before or on the specified date.
-        created_gt: Rewards given after the specified date.
-        created_gte: Rewards given after or on the specified date.
+        assignment_id: The ID of an assignment a bonus was granted for.
+        private_comment: Bonuses with specified comment.
+        id_lt: Bonuses with IDs less than the specified value.
+        id_lte: Bonuses with IDs less than or equal to the specified value.
+        id_gt: Bonuses with IDs greater than the specified value.
+        id_gte: Bonuses with IDs greater than or equal to the specified value.
+        created_lt: Bonuses given before the specified date.
+        created_lte: Bonuses given before or on the specified date.
+        created_gt: Bonuses given after the specified date.
+        created_gte: Bonuses given after or on the specified date.
     """
 
     class CompareFields:
         id: str
         created: datetime.datetime
 
     user_id: str
     assignment_id: str
     private_comment: str
 
 
 UserBonusSortItems = BaseSortItems.for_fields(
     'UserBonusSortItems', ['id', 'created'],
     # docstring
-    """Keys for sorting rewards in search results.
+    """Keys for sorting bonuses in search results.
 
     Attributes:
         items: A list of sorting keys. Supported values:
-            * `'id'` — The ID of a reward.
-            * `'created'` — The date of granting a reward.
+            * `'id'` — The ID of a bonus.
+            * `'created'` — The date of granting a bonus.
 
     Example:
-        The example shows how to find rewards sorted by granting date in descending order. Rewards with equal granting dates are sorted by IDs in ascending order.
+        The example shows how to find bonuses sorted by granting date in descending order. Bonuses with equal granting dates are sorted by IDs in ascending order.
 
         >>> sort = toloka.client.search_requests.UserBonusSortItems(['-created', 'id'])
         >>> result = toloka_client.find_user_bonuses(user_id=best_toloker_id, sort=sort, limit=10)
         ...
     """
 )
```

### Comparing `toloka-kit-1.2.0/src/client/search_requests.pyi` & `toloka-kit-1.2.0.post1/src/client/search_requests.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1352,28 +1352,28 @@
         ...
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     items: typing.Optional[typing.List[SortItem]]
 
 
 class UserBonusSearchRequest(BaseSearchRequest):
-    """Parameters for searching Tolokers' rewards.
+    """Parameters for searching Tolokers' bonuses.
 
     Attributes:
         user_id: The ID of a Toloker.
-        assignment_id: The ID of an assignment a reward was granted for.
-        private_comment: Rewards with specified comment.
-        id_lt: Rewards with IDs less than the specified value.
-        id_lte: Rewards with IDs less than or equal to the specified value.
-        id_gt: Rewards with IDs greater than the specified value.
-        id_gte: Rewards with IDs greater than or equal to the specified value.
-        created_lt: Rewards given before the specified date.
-        created_lte: Rewards given before or on the specified date.
-        created_gt: Rewards given after the specified date.
-        created_gte: Rewards given after or on the specified date.
+        assignment_id: The ID of an assignment a bonus was granted for.
+        private_comment: Bonuses with specified comment.
+        id_lt: Bonuses with IDs less than the specified value.
+        id_lte: Bonuses with IDs less than or equal to the specified value.
+        id_gt: Bonuses with IDs greater than the specified value.
+        id_gte: Bonuses with IDs greater than or equal to the specified value.
+        created_lt: Bonuses given before the specified date.
+        created_lte: Bonuses given before or on the specified date.
+        created_gt: Bonuses given after the specified date.
+        created_gte: Bonuses given after or on the specified date.
     """
 
     class CompareFields:
         id: str
         created: datetime.datetime
 
     def __init__(
@@ -1405,23 +1405,23 @@
     created_lt: typing.Optional[datetime.datetime]
     created_lte: typing.Optional[datetime.datetime]
     created_gt: typing.Optional[datetime.datetime]
     created_gte: typing.Optional[datetime.datetime]
 
 
 class UserBonusSortItems(BaseSortItems):
-    """Keys for sorting rewards in search results.
+    """Keys for sorting bonuses in search results.
 
     Attributes:
         items: A list of sorting keys. Supported values:
-            * `'id'` — The ID of a reward.
-            * `'created'` — The date of granting a reward.
+            * `'id'` — The ID of a bonus.
+            * `'created'` — The date of granting a bonus.
 
     Example:
-        The example shows how to find rewards sorted by granting date in descending order. Rewards with equal granting dates are sorted by IDs in ascending order.
+        The example shows how to find bonuses sorted by granting date in descending order. Bonuses with equal granting dates are sorted by IDs in ascending order.
 
         >>> sort = toloka.client.search_requests.UserBonusSortItems(['-created', 'id'])
         >>> result = toloka_client.find_user_bonuses(user_id=best_toloker_id, sort=sort, limit=10)
         ...
     """
 
     class SortItem(BaseSortItem):
```

### Comparing `toloka-kit-1.2.0/src/client/search_results.py` & `toloka-kit-1.2.0.post1/src/client/search_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 )
 TrainingSearchResult = _create_search_result_class_for(
     Training,
     _create_search_result_docstring('training pools')
 )
 UserBonusSearchResult = _create_search_result_class_for(
     UserBonus,
-    _create_search_result_docstring("rewards", "Tolokers' rewards")
+    _create_search_result_docstring("bonuses", "Tolokers' bonuses")
 )
 UserRestrictionSearchResult = _create_search_result_class_for(
     UserRestriction,
     _create_search_result_docstring('Toloker restrictions')
 )
 UserSkillSearchResult = _create_search_result_class_for(
     UserSkill,
```

### Comparing `toloka-kit-1.2.0/src/client/search_results.pyi` & `toloka-kit-1.2.0.post1/src/client/search_results.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -286,21 +286,21 @@
 
     _unexpected: typing.Optional[typing.Dict[str, typing.Any]]
     items: typing.Optional[typing.List[toloka.client.training.Training]]
     has_more: typing.Optional[bool]
 
 
 class UserBonusSearchResult(toloka.client.primitives.base.BaseTolokaObject):
-    """The result of searching Tolokers' rewards.
+    """The result of searching Tolokers' bonuses.
 
     Attributes:
-        items: A list with found rewards.
-        has_more: A flag showing whether there are more matching rewards.
-            * `True` — There are more matching rewards, not included in `items` due to the limit set in the search request.
-            * `False` — `items` contains all matching rewards.
+        items: A list with found bonuses.
+        has_more: A flag showing whether there are more matching bonuses.
+            * `True` — There are more matching bonuses, not included in `items` due to the limit set in the search request.
+            * `False` — `items` contains all matching bonuses.
     """
 
     def __init__(
         self,
         *,
         items: typing.Optional[typing.List[toloka.client.user_bonus.UserBonus]] = None,
         has_more: typing.Optional[bool] = None
```

### Comparing `toloka-kit-1.2.0/src/client/skill.py` & `toloka-kit-1.2.0.post1/src/client/skill.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/skill.pyi` & `toloka-kit-1.2.0.post1/src/client/skill.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/solution.py` & `toloka-kit-1.2.0.post1/src/client/solution.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/solution.pyi` & `toloka-kit-1.2.0.post1/src/client/solution.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/task.py` & `toloka-kit-1.2.0.post1/src/client/task.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/task.pyi` & `toloka-kit-1.2.0.post1/src/client/task.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,16 @@
     """Parameters used with the [create_task](toloka.client.TolokaClient.create_task.md) method.
 
     If the operation is started in an asynchronous mode,
     we recommend that you send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
 
     Attributes:
         operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+            We recommended sending the operation ID in the `POST` requests to avoid accidental errors:
+            when you send several requests with the same `operation_id`, the operation will be performed only once.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally and `create_tasks` waits for the completion of it. It is recommended to create no more than 10,000 tasks per request in this mode.
             * `False` — The request is processed synchronously. A maximum of 5000 tasks can be added in a single request in this mode.
             Default value: `True`.
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_tasks` pool parameter.
             * `False` — Use the overlap that is set in the `overlap` task parameter.
@@ -214,14 +216,16 @@
     and [create_tasks_async](toloka.client.TolokaClient.create_tasks_async.md) methods.
 
     If the operation is started in an asynchronous mode,
     we recommend that you send the `operation_id` to avoid creating the same tasks multiple times. You can use this ID later to get information about the operation.
 
     Attributes:
         operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+            We recommended sending the operation ID in the `POST` requests to avoid accidental errors:
+            when you send several requests with the same `operation_id`, the operation will be performed only once.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally and `create_tasks` waits for the completion of it. It is recommended to create no more than 10,000 tasks per request in this mode.
             * `False` — The request is processed synchronously. A maximum of 5000 tasks can be added in a single request in this mode.
             Default value: `True`.
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_tasks` pool parameter.
             * `False` — Use the overlap that is set in the `overlap` task parameter.
```

### Comparing `toloka-kit-1.2.0/src/client/task_distribution_function.py` & `toloka-kit-1.2.0.post1/src/client/task_distribution_function.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/task_distribution_function.pyi` & `toloka-kit-1.2.0.post1/src/client/task_distribution_function.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/task_suite.py` & `toloka-kit-1.2.0.post1/src/client/task_suite.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,28 +27,28 @@
         pool_id: The ID of a pool that the task suite belongs to.
         tasks: The tasks.
         reserved_for: IDs of Tolokers who have access to the task suite.
         unavailable_for: IDs of Tolokers who don't have access to the task suite.
         issuing_order_override: The priority of a task suite.
             It influences the order of assigning task suites to Tolokers in pools with the `issue_task_suites_in_creation_order` parameter set to `True`.
             Allowed range: from -99999.99999 to 99999.99999.
-        mixed: [The way of grouping tasks](https://toloka.ai/en/docs/guide/concepts/distribute-tasks-by-pages) to create the task suite.
+        mixed: [The way of grouping tasks](https://toloka.ai/docs/guide/distribute-tasks-by-pages) to create the task suite.
             * `True` — The tasks are mixed automatically using the smart mixing approach.
             * `False` — The tasks are grouped manually.
 
             Default value: `False`.
         traits_all_of: The task suite can be assigned to Tolokers who have all of the specified traits.
         traits_any_of: The task suite can be assigned to Tolokers who have any of the specified traits.
         traits_none_of_any: The task suite can not be assigned to Tolokers who have any of the specified traits.
         longitude: The longitude of the point on the map for the task suite.
         latitude: The latitude of the point on the map for the task suite.
         id: The ID of the task suite. Read-only field.
         remaining_overlap: The number of times left for this task suite to be assigned to Tolokers. Read-only field.
         automerged:
-            * `True` — The task suite was created after [merging tasks](https://toloka.ai/en/docs/api/concepts/tasks#task-merge).
+            * `True` — The task suite was created after [merging tasks](https://toloka.ai/docs/api/tasks).
             * `False` — There are no merged tasks in the task suite.
         created: The UTC date and time when the task suite was created. Read-only field.
     """
 
     pool_id: str
     tasks: List[BaseTask] = attr.attrib(factory=list)
```

### Comparing `toloka-kit-1.2.0/src/client/task_suite.pyi` & `toloka-kit-1.2.0.post1/src/client/task_suite.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,28 @@
         pool_id: The ID of a pool that the task suite belongs to.
         tasks: The tasks.
         reserved_for: IDs of Tolokers who have access to the task suite.
         unavailable_for: IDs of Tolokers who don't have access to the task suite.
         issuing_order_override: The priority of a task suite.
             It influences the order of assigning task suites to Tolokers in pools with the `issue_task_suites_in_creation_order` parameter set to `True`.
             Allowed range: from -99999.99999 to 99999.99999.
-        mixed: [The way of grouping tasks](https://toloka.ai/en/docs/guide/concepts/distribute-tasks-by-pages) to create the task suite.
+        mixed: [The way of grouping tasks](https://toloka.ai/docs/guide/distribute-tasks-by-pages) to create the task suite.
             * `True` — The tasks are mixed automatically using the smart mixing approach.
             * `False` — The tasks are grouped manually.
 
             Default value: `False`.
         traits_all_of: The task suite can be assigned to Tolokers who have all of the specified traits.
         traits_any_of: The task suite can be assigned to Tolokers who have any of the specified traits.
         traits_none_of_any: The task suite can not be assigned to Tolokers who have any of the specified traits.
         longitude: The longitude of the point on the map for the task suite.
         latitude: The latitude of the point on the map for the task suite.
         id: The ID of the task suite. Read-only field.
         remaining_overlap: The number of times left for this task suite to be assigned to Tolokers. Read-only field.
         automerged:
-            * `True` — The task suite was created after [merging tasks](https://toloka.ai/en/docs/api/concepts/tasks#task-merge).
+            * `True` — The task suite was created after [merging tasks](https://toloka.ai/docs/api/tasks).
             * `False` — There are no merged tasks in the task suite.
         created: The UTC date and time when the task suite was created. Read-only field.
     """
 
     @typing.overload
     def add_base_task(self, base_task: toloka.client.task.BaseTask) -> 'TaskSuite': ...
 
@@ -103,14 +103,16 @@
 
 
 class TaskSuiteCreateRequestParameters(toloka.client.primitives.parameter.IdempotentOperationParameters):
     """Parameters for creating task suite.
 
     Attributes:
         operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+            We recommended sending the operation ID in the `POST` requests to avoid accidental errors:
+            when you send several requests with the same `operation_id`, the operation will be performed only once.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally.
             * `False` — The request is processed synchronously.
 
             Default value: `True`.
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_task_suites` pool parameter.
@@ -140,14 +142,16 @@
 
 
 class TaskSuitesCreateRequestParameters(TaskSuiteCreateRequestParameters):
     """Parameters for creating task suites.
 
     Attributes:
         operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+            We recommended sending the operation ID in the `POST` requests to avoid accidental errors:
+            when you send several requests with the same `operation_id`, the operation will be performed only once.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally.
             * `False` — The request is processed synchronously. A maximum of 5000 task suites can be added in a single request in this mode.
             Default value: `True`.
         allow_defaults: Active overlap setting:
             * `True` — Use the overlap that is set in the `defaults.default_overlap_for_new_task_suites` pool parameter.
             * `False` — Use the overlap that is set in the `overlap` task suite parameter.
```

### Comparing `toloka-kit-1.2.0/src/client/training.py` & `toloka-kit-1.2.0.post1/src/client/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - To train Tolokers so they solve general tasks better.
     - To select Tolokers who successfully completed training tasks and to give them access to a general pool.
 
     To link a training to a general pool set the
     [Pool](toloka.client.pool.Pool.md).[quality_control](toloka.client.quality_control.QualityControl.md).[training_requirement](toloka.client.quality_control.QualityControl.TrainingRequirement.md)
     parameter.
 
-    For more information, see [Adding a training](https://toloka.ai/en/docs/guide/concepts/train).
+    For more information, see [Adding a training](https://toloka.ai/docs/guide/train).
 
     Attributes:
         project_id: The ID of the project containing the training.
         private_name: The training name. It is visible to the requester only.
         may_contain_adult_content: The presence of adult content.
         assignment_max_duration_seconds: Time limit to complete a task suite.
             Take into account loading a page with a task suite and sending responses to the server. It is recommended that you set at least 60 seconds.
```

### Comparing `toloka-kit-1.2.0/src/client/training.pyi` & `toloka-kit-1.2.0.post1/src/client/training.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     - To train Tolokers so they solve general tasks better.
     - To select Tolokers who successfully completed training tasks and to give them access to a general pool.
 
     To link a training to a general pool set the
     [Pool](toloka.client.pool.Pool.md).[quality_control](toloka.client.quality_control.QualityControl.md).[training_requirement](toloka.client.quality_control.QualityControl.TrainingRequirement.md)
     parameter.
 
-    For more information, see [Adding a training](https://toloka.ai/en/docs/guide/concepts/train).
+    For more information, see [Adding a training](https://toloka.ai/docs/guide/train).
 
     Attributes:
         project_id: The ID of the project containing the training.
         private_name: The training name. It is visible to the requester only.
         may_contain_adult_content: The presence of adult content.
         assignment_max_duration_seconds: Time limit to complete a task suite.
             Take into account loading a page with a task suite and sending responses to the server. It is recommended that you set at least 60 seconds.
```

### Comparing `toloka-kit-1.2.0/src/client/user.py` & `toloka-kit-1.2.0.post1/src/client/user.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/user.pyi` & `toloka-kit-1.2.0.post1/src/client/user.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/user_bonus.py` & `toloka-kit-1.2.0.post1/src/client/user_bonus.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             (the message will come in the Toloker's language). Format {'language': 'title', ... }.
             The language can be RU/EN/TR/ID/FR.
         public_message: Message text for the Toloker. You can provide text in several languages
             (the message will come in the Toloker's language). Format {'language': 'message', ... }.
             The language can be RU/EN/TR/ID/FR.
         without_message: Do not send a bonus message to the Toloker. To award a bonus without a message, specify null
             for `public_title` and `public_message` and `True` for `without_message`.
-        assignment_id: ID of the Toloker's response to the task a reward is issued for.
+        assignment_id: ID of the Toloker's response to the task a bonus is issued for.
         id: Internal ID of the issued bonus. Read-only field.
         created: Date the bonus was awarded, in UTC. Read-only field.
 
     Example:
         How to create bonus with message for specific assignment.
 
         >>> new_bonus = toloka_client.create_user_bonus(
```

### Comparing `toloka-kit-1.2.0/src/client/user_bonus.pyi` & `toloka-kit-1.2.0.post1/src/client/user_bonus.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             (the message will come in the Toloker's language). Format {'language': 'title', ... }.
             The language can be RU/EN/TR/ID/FR.
         public_message: Message text for the Toloker. You can provide text in several languages
             (the message will come in the Toloker's language). Format {'language': 'message', ... }.
             The language can be RU/EN/TR/ID/FR.
         without_message: Do not send a bonus message to the Toloker. To award a bonus without a message, specify null
             for `public_title` and `public_message` and `True` for `without_message`.
-        assignment_id: ID of the Toloker's response to the task a reward is issued for.
+        assignment_id: ID of the Toloker's response to the task a bonus is issued for.
         id: Internal ID of the issued bonus. Read-only field.
         created: Date the bonus was awarded, in UTC. Read-only field.
 
     Example:
         How to create bonus with message for specific assignment.
 
         >>> new_bonus = toloka_client.create_user_bonus(
@@ -101,14 +101,16 @@
 class UserBonusCreateRequestParameters(toloka.client.primitives.parameter.IdempotentOperationParameters):
     """Parameters for creating bonus for Toloker.
 
     Used in methods 'create_user_bonus' of the class TolokaClient.
 
     Attributes:
         operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+            We recommended sending the operation ID in the `POST` requests to avoid accidental errors:
+            when you send several requests with the same `operation_id`, the operation will be performed only once.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally.
             * `False` — The request is processed synchronously.
 
             Default value: `True`.
     """
 
@@ -131,14 +133,16 @@
     """Parameters for creating bonuses for Tolokers.
 
     Used in methods 'create_user_bonuses' и 'create_user_bonuses_async' of the class TolokaClient,
     to clarify the behavior when creating bonuses.
 
     Attributes:
         operation_id: The ID of the operation conforming to the [RFC4122 standard](https://tools.ietf.org/html/rfc4122).
+            We recommended sending the operation ID in the `POST` requests to avoid accidental errors:
+            when you send several requests with the same `operation_id`, the operation will be performed only once.
         async_mode: Request processing mode:
             * `True` — Asynchronous operation is started internally.
             * `False` — The request is processed synchronously.
 
             Default value: `True`.
         skip_invalid_items: Validation parameters of objects:
             * `True` — Award a bonus if the object with bonus information passed validation. Otherwise, skip the bonus.
```

### Comparing `toloka-kit-1.2.0/src/client/user_restriction.py` & `toloka-kit-1.2.0.post1/src/client/user_restriction.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/user_restriction.pyi` & `toloka-kit-1.2.0.post1/src/client/user_restriction.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/user_skill.py` & `toloka-kit-1.2.0.post1/src/client/user_skill.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/user_skill.pyi` & `toloka-kit-1.2.0.post1/src/client/user_skill.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/webhook_subscription.py` & `toloka-kit-1.2.0.post1/src/client/webhook_subscription.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/client/webhook_subscription.pyi` & `toloka-kit-1.2.0.post1/src/client/webhook_subscription.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/__init__.py` & `toloka-kit-1.2.0.post1/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/__init__.pyi` & `toloka-kit-1.2.0.post1/src/metrics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/collector.py` & `toloka-kit-1.2.0.post1/src/metrics/collector.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/collector.pyi` & `toloka-kit-1.2.0.post1/src/metrics/collector.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/jupyter_dashboard.py` & `toloka-kit-1.2.0.post1/src/metrics/jupyter_dashboard.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/jupyter_dashboard.pyi` & `toloka-kit-1.2.0.post1/src/metrics/jupyter_dashboard.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/metrics.py` & `toloka-kit-1.2.0.post1/src/metrics/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         requester: Requester = await self.atoloka_client.get_requester()
         result = {self.balance_name: [(datetime.datetime.now(datetime.timezone.utc), requester.balance)]}
         return result
 
 
 @attr.s(auto_attribs=True)
 class NewUserBonuses(BaseMetric):
-    """Tracking rewards for Tolokers: reward count or money amount.
+    """Tracking bonuses for Tolokers: bonus count or money amount.
 
     Args:
         cursor_time_lag: Time lag for cursor. This controls time lag between user bonuses being added and this metric
             being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new bonuses.
         money_name: Metric name for amount of money in new bonuses.
         join_events: Count all events in one point.  Default `False`.
```

### Comparing `toloka-kit-1.2.0/src/metrics/metrics.pyi` & `toloka-kit-1.2.0.post1/src/metrics/metrics.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     toloka_client: toloka.client.TolokaClient
     atoloka_client: toloka.async_client.client.AsyncTolokaClient
     timeout: datetime.timedelta
     balance_name: typing.Optional[str]
 
 
 class NewUserBonuses(BaseMetric):
-    """Tracking rewards for Tolokers: reward count or money amount.
+    """Tracking bonuses for Tolokers: bonus count or money amount.
 
     Args:
         cursor_time_lag: Time lag for cursor. This controls time lag between user bonuses being added and this metric
             being updated. See BaseCursor.time_lag for details and reasoning behind this.
         count_name: Metric name for a count of new bonuses.
         money_name: Metric name for amount of money in new bonuses.
         join_events: Count all events in one point.  Default `False`.
```

### Comparing `toloka-kit-1.2.0/src/metrics/pool_metrics.py` & `toloka-kit-1.2.0.post1/src/metrics/pool_metrics.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/metrics/pool_metrics.pyi` & `toloka-kit-1.2.0.post1/src/metrics/pool_metrics.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/__init__.py` & `toloka-kit-1.2.0.post1/src/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/__init__.pyi` & `toloka-kit-1.2.0.post1/src/streaming/__init__.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/cursor.py` & `toloka-kit-1.2.0.post1/src/streaming/cursor.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/cursor.pyi` & `toloka-kit-1.2.0.post1/src/streaming/cursor.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/event.py` & `toloka-kit-1.2.0.post1/src/streaming/event.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/event.pyi` & `toloka-kit-1.2.0.post1/src/streaming/event.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/locker.py` & `toloka-kit-1.2.0.post1/src/streaming/locker.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/locker.pyi` & `toloka-kit-1.2.0.post1/src/streaming/locker.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/observer.py` & `toloka-kit-1.2.0.post1/src/streaming/observer.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/observer.pyi` & `toloka-kit-1.2.0.post1/src/streaming/observer.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/pipeline.py` & `toloka-kit-1.2.0.post1/src/streaming/pipeline.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/pipeline.pyi` & `toloka-kit-1.2.0.post1/src/streaming/pipeline.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/streaming/storage.py` & `toloka-kit-1.2.0.post1/src/streaming/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,17 +177,17 @@
     Examples:
         Create new instance.
 
         >>> !pip install toloka-kit[s3]
         >>> import boto3
         >>> import os
         >>> session = boto3.Session(
-        ...     aws_access_key_id=os.getenv('AWS_ACCESS_KEY_ID'),
-        ...     aws_secret_access_key=os.getenv('AWS_SECRET_ACCESS_KEY')
-        ... )
+        >>>     aws_access_key_id=os.getenv('AWS_ACCESS_KEY_ID'),
+        >>>     aws_secret_access_key=os.getenv('AWS_SECRET_ACCESS_KEY')
+        >>> )
         >>> resource = session.resource('s3', region_name=os.getenv('AWS_DEFAULT_REGION', 'us-east-2'))
         >>> bucket = resource.Bucket('my-bucket')
         >>> storage = S3Storage(bucket)
         ...
 
         Use with pipelines.
```

### Comparing `toloka-kit-1.2.0/src/streaming/storage.pyi` & `toloka-kit-1.2.0.post1/src/streaming/storage.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -171,17 +171,17 @@
     Examples:
         Create new instance.
 
         >>> !pip install toloka-kit[s3]
         >>> import boto3
         >>> import os
         >>> session = boto3.Session(
-        ...     aws_access_key_id=os.getenv('AWS_ACCESS_KEY_ID'),
-        ...     aws_secret_access_key=os.getenv('AWS_SECRET_ACCESS_KEY')
-        ... )
+        >>>     aws_access_key_id=os.getenv('AWS_ACCESS_KEY_ID'),
+        >>>     aws_secret_access_key=os.getenv('AWS_SECRET_ACCESS_KEY')
+        >>> )
         >>> resource = session.resource('s3', region_name=os.getenv('AWS_DEFAULT_REGION', 'us-east-2'))
         >>> bucket = resource.Bucket('my-bucket')
         >>> storage = S3Storage(bucket)
         ...
 
         Use with pipelines.
```

### Comparing `toloka-kit-1.2.0/src/util/__init__.py` & `toloka-kit-1.2.0.post1/src/util/__init__.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_codegen.py` & `toloka-kit-1.2.0.post1/src/util/_codegen.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_codegen.pyi` & `toloka-kit-1.2.0.post1/src/util/_codegen.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_docstrings.py` & `toloka-kit-1.2.0.post1/src/util/_docstrings.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_docstrings.pyi` & `toloka-kit-1.2.0.post1/src/util/_docstrings.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_extendable_enum.py` & `toloka-kit-1.2.0.post1/src/util/_extendable_enum.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_extendable_enum.pyi` & `toloka-kit-1.2.0.post1/src/util/_extendable_enum.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_managing_headers.py` & `toloka-kit-1.2.0.post1/src/util/_managing_headers.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_managing_headers.pyi` & `toloka-kit-1.2.0.post1/src/util/_managing_headers.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/_typing.py` & `toloka-kit-1.2.0.post1/src/util/_typing.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/async_utils.py` & `toloka-kit-1.2.0.post1/src/util/async_utils.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/async_utils.pyi` & `toloka-kit-1.2.0.post1/src/util/async_utils.pyi`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/src/util/stored.py` & `toloka-kit-1.2.0.post1/src/util/stored.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_aggregated_solution.py` & `toloka-kit-1.2.0.post1/tests/test_aggregated_solution.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_analytics_request.py` & `toloka-kit-1.2.0.post1/tests/test_analytics_request.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_assignment.py` & `toloka-kit-1.2.0.post1/tests/test_assignment.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_attachment.py` & `toloka-kit-1.2.0.post1/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_client.py` & `toloka-kit-1.2.0.post1/tests/test_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -100,15 +100,17 @@
     return request.param
 
 
 def test_client_act_as(respx_mock, client_act_under_account, shared_account_id, requester_mapping):
 
     def get_requester(request):
         expected_headers = {
-            'X-Caller-Context': 'client' if isinstance(client_act_under_account, client.TolokaClient) else 'async_client',
+            'X-Caller-Context': 'client' if isinstance(
+                client_act_under_account, client.TolokaClient
+            ) else 'async_client',
             'X-Top-Level-Method': 'get_requester',
             'X-Low-Level-Method': 'get_requester',
             'X-Act-Under-Account-ID': shared_account_id
         }
         check_headers(request, expected_headers)
 
         return httpx.Response(text=simplejson.dumps(requester_mapping), status_code=200)
@@ -129,7 +131,35 @@
         (False, ssl.CERT_NONE),
     ]
 )
 def test_client_ssl_verify(toloka_client, verify, expected_ssl_context):
     client = copy.deepcopy(toloka_client)
     client.verify = verify
     assert get_verify_mode(client) == expected_ssl_context
+
+
+@pytest.mark.parametrize(
+    'token,is_apikey', [
+        ('fake-token', False),
+        (
+            # api-key like fake token
+            'LrB_oHKYMtXeD-BoVFWTwi.nfNC.vcRjfXLoJtfWAExAizBKrsBlbfLQJFSFDEnoUODffGsyPjpOlfyAIkFlgZBloBQJHxkjMtAohTTCm-sVtAnNueMVEGqiyBPxz-elOp-hEpA',
+            True
+        )
+    ]
+)
+def test_client_auth_headers(respx_mock, token, is_apikey):
+    client = TolokaClient(environment='SANDBOX', token=token)
+
+    def get_requester(request):
+        expected_headers = {
+            'X-Caller-Context': 'client',
+            'X-Top-Level-Method': 'get_requester',
+            'X-Low-Level-Method': 'get_requester',
+            'authorization': f'ApiKey {token}' if is_apikey else f'OAuth {token}',
+        }
+        check_headers(request, expected_headers)
+
+        return httpx.Response(text=simplejson.dumps({}), status_code=200)
+
+    respx_mock.get(f'{client.url}/api/v1/requester').mock(side_effect=get_requester)
+    client.get_requester()
```

### Comparing `toloka-kit-1.2.0/tests/test_deep_clone_project.py` & `toloka-kit-1.2.0.post1/tests/test_deep_clone_project.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_exceptions.py` & `toloka-kit-1.2.0.post1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_filter.py` & `toloka-kit-1.2.0.post1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_message_thread.py` & `toloka-kit-1.2.0.post1/tests/test_message_thread.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_operation.py` & `toloka-kit-1.2.0.post1/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_operation_log.py` & `toloka-kit-1.2.0.post1/tests/test_operation_log.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_project.py` & `toloka-kit-1.2.0.post1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_requester.py` & `toloka-kit-1.2.0.post1/tests/test_requester.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_serialization.py` & `toloka-kit-1.2.0.post1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_skill.py` & `toloka-kit-1.2.0.post1/tests/test_skill.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_training.py` & `toloka-kit-1.2.0.post1/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_user.py` & `toloka-kit-1.2.0.post1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_user_restriction.py` & `toloka-kit-1.2.0.post1/tests/test_user_restriction.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_user_skill.py` & `toloka-kit-1.2.0.post1/tests/test_user_skill.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/tests/test_webhook_subscription.py` & `toloka-kit-1.2.0.post1/tests/test_webhook_subscription.py`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/toloka_kit.egg-info/PKG-INFO` & `toloka-kit-1.2.0.post1/toloka_kit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: toloka-kit
-Version: 1.2.0
+Version: 1.2.0.post1
 Summary: Toloka API client
 Author: Vladimir Losev
 Author-email: losev@yandex-team.ru
 License: Apache 2.0
-Project-URL: Documentation, https://toloka.ai/en/docs/toloka-kit
+Project-URL: Documentation, https://toloka.ai/docs/toloka-kit
 Project-URL: Source, https://github.com/Toloka/toloka-kit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -41,36 +41,36 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/toloka-kit.svg)](https://pypi.org/project/toloka-kit/)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/toloka-kit.svg)](https://pypi.org/project/toloka-kit)
 [![Downloads](https://pepy.tech/badge/toloka-kit/month)](https://pepy.tech/project/toloka-kit)
 
 [![Coverage](https://codecov.io/gh/Toloka/toloka-kit/branch/main/graph/badge.svg)](https://codecov.io/gh/Toloka/toloka-kit)
 [![GitHub Tests](https://github.com/Toloka/toloka-kit/workflows/Tests/badge.svg?branch=main)](//github.com/Toloka/toloka-kit/actions?query=workflow:Tests)
 
-[Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
+[Toloka website](https://toloka.ai/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Documentation](https://toloka.ai/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) | [Issue tracker](https://github.com/Toloka/toloka-kit/issues)
 
 
 
-Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit). 
+Toloka-Kit is a Python library for working with [Toloka API](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 The API allows you to build scalable and fully automated human-in-the-loop ML pipelines, and integrate them into your processes. The toolkit makes integration easier. You can use it with Jupyter notebooks.
 
 * Support for all common Toloka use cases: creating projects, adding pools, uploading tasks, and so on.
 * Toloka entities are represented as Python classes. You can use them instead of accessing the API using JSON representations.
 * There’s no need to validate JSON files and work with them directly.
 * Support of both synchronous and asynchronous (via async/await) executions.
-* Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation. 
+* Streaming support: build complex pipelines which send and receive data in real time. For example, you can [pass data between two related projects](https://github.com/Toloka/toloka-kit/blob/main/examples/6.streaming_pipelines/streaming_pipelines.ipynb): one for data labeling, and another for its validation.
 * [AutoQuality](https://medium.com/toloka/automating-crowdsourcing-quality-control-ad057baf00fd) feature which automatically finds the best fitting quality control rules for your project.
 
 ## Prerequisites
 
 Before you begin, make sure that:
 * You are using [Python](https://www.python.org/) v3.7 or higher.
-* You are [registered](https://toloka.ai/docs/guide/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
-* You have [topped up](https://toloka.ai/docs/guide/concepts/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
-* You have [set up an OAuth token](https://toloka.ai/docs/api/concepts/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) to access Toloka API.
+* You are [registered](https://toloka.ai/docs/guide/access/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) in Toloka as a requester.
+* You have [topped up](https://toloka.ai/docs/guide/refill/?utm_source=github&utm_medium=site&utm_campaign=tolokakit) your Toloka account.
+* You have [set up an OAuth token](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit#overview--accessing-the-api) to access Toloka API.
 
 ## Get Started
 1. Install the Toloka-Kit package. Run the following command in the command shell:
 ```
 $ pip install toloka-kit
 ```
 For production environments, specify the exact package version. For the latest stable version, check the [project page at pypi.org](https://pypi.org/project/toloka-kit/).
@@ -106,17 +106,17 @@
 $ pip install toloka-kit[pandas,autoquality,s3,zookeeper,jupyter-metrics] # remove unnecessary requirements from the list
 ```
 
 ## Usage examples
 [Toloka-kit usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#toloka-kit-usage-examples) - tutorials for specific data labeling tasks. They demonstrate how to work with Toloka API using Toloka-Kit.
 
 ## Documentation
-* [Toloka-Kit documentation](https://toloka.ai/en/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka API reference](https://toloka.ai/docs/api/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
-* [Toloka web interface documentation](https://toloka.ai/docs/guide/concepts/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka-Kit documentation](https://toloka.ai/docs/toloka-kit/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka API reference](https://toloka.ai/docs/api/api-reference/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
+* [Toloka web interface documentation](https://toloka.ai/docs/guide/overview/?utm_source=github&utm_medium=site&utm_campaign=tolokakit)
 
 ## Support
 * To suggest a feature or report a bug, go to our [issues page](https://github.com/Toloka/toloka-kit/issues).
 * If you have any questions, feel free to ask our [Slack community](https://toloka.ai/community/?utm_source=github&utm_medium=site&utm_campaign=tolokakit).
 
 ## Contributing
 Feel free to contribute to toloka-kit. Right now, we need more [usage examples](https://github.com/Toloka/toloka-kit/tree/main/examples#need-more-examples).
```

### Comparing `toloka-kit-1.2.0/toloka_kit.egg-info/SOURCES.txt` & `toloka-kit-1.2.0.post1/toloka_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toloka-kit-1.2.0/toloka_kit.egg-info/requires.txt` & `toloka-kit-1.2.0.post1/toloka_kit.egg-info/requires.txt`

 * *Files identical despite different names*

