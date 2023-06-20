# Comparing `tmp/mindflow-0.5.1.tar.gz` & `tmp/mindflow-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindflow-0.5.1.tar", last modified: Tue Jun 20 21:55:15 2023, max compression
+gzip compressed data, was "mindflow-0.5.2.tar", last modified: Tue Jun 20 23:53:23 2023, max compression
```

## Comparing `mindflow-0.5.1.tar` & `mindflow-0.5.2.tar`

### file list

```diff
@@ -1,109 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 21:55:02.000000 mindflow-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 21:55:02.000000 mindflow-0.5.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:55:02.000000 mindflow-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 21:55:02.000000 mindflow-0.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:55:15.304136 mindflow-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-20 21:55:02.000000 mindflow-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 21:55:02.000000 mindflow-0.5.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow/cli/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/command_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/file_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/file_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/file_processing/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/file_processing/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/prompt_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/resolving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/resolving/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolvers/document_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/resolving/resolvers/file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.300136 mindflow-0.5.1/mindflow/core/text_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/text_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/text_processing/utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/text_processing/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/token_counting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/core/types/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/mind_flow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/definitions/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/mindflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/core/types/store_traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/core/types/store_traits/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.304136 mindflow-0.5.1/mindflow/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/unit_tests/dummy_diff.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-20 21:55:02.000000 mindflow-0.5.1/mindflow/unit_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:15.296136 mindflow-0.5.1/mindflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:55:15.000000 mindflow-0.5.1/mindflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 21:55:02.000000 mindflow-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:55:15.304136 mindflow-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 21:55:02.000000 mindflow-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 23:53:13.000000 mindflow-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 23:53:13.000000 mindflow-0.5.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:53:13.000000 mindflow-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 23:53:13.000000 mindflow-0.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 23:53:23.307656 mindflow-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-20 23:53:13.000000 mindflow-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 23:53:13.000000 mindflow-0.5.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/command_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/file_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/file_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/file_processing/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/file_processing/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/prompt_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/resolving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/resolving/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolvers/document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolvers/file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/text_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/text_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/text_processing/utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/text_processing/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/token_counting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/core/types/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/mind_flow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/mindflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/core/types/store_traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/unit_tests/dummy_diff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 23:53:13.000000 mindflow-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:53:23.307656 mindflow-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 23:53:13.000000 mindflow-0.5.2/setup.py
```

### Comparing `mindflow-0.5.1/.gitignore` & `mindflow-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/Makefile` & `mindflow-0.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/PKG-INFO` & `mindflow-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.1
+Version: 0.5.2
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.5.1/README.md` & `mindflow-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/cli_main.py` & `mindflow-0.5.2/mindflow/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/commands/chat.py` & `mindflow-0.5.2/mindflow/cli/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/commands/config.py` & `mindflow-0.5.2/mindflow/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/commands/git/commit.py` & `mindflow-0.5.2/mindflow/cli/commands/git/commit.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/commands/git/diff.py` & `mindflow-0.5.2/mindflow/cli/commands/git/diff.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/commands/git/mr.py` & `mindflow-0.5.2/mindflow/cli/commands/git/mr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/commands/git/pr.py` & `mindflow-0.5.2/mindflow/cli/commands/git/pr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/cli/util.py` & `mindflow-0.5.2/mindflow/cli/util.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/chat.py` & `mindflow-0.5.2/mindflow/core/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/delete.py` & `mindflow-0.5.2/mindflow/core/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/gen.py` & `mindflow-0.5.2/mindflow/core/commands/gen.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/git/commit.py` & `mindflow-0.5.2/mindflow/core/commands/git/commit.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/git/diff.py` & `mindflow-0.5.2/mindflow/core/commands/git/diff.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/git/mr.py` & `mindflow-0.5.2/mindflow/core/commands/git/mr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/git/pr.py` & `mindflow-0.5.2/mindflow/core/commands/git/pr.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/index.py` & `mindflow-0.5.2/mindflow/core/commands/index.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/inspect.py` & `mindflow-0.5.2/mindflow/core/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/login.py` & `mindflow-0.5.2/mindflow/core/commands/login.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/commands/query.py` & `mindflow-0.5.2/mindflow/core/commands/query.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/errors.py` & `mindflow-0.5.2/mindflow/core/errors.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/file_processing/extract.py` & `mindflow-0.5.2/mindflow/core/file_processing/extract.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/file_processing/git.py` & `mindflow-0.5.2/mindflow/core/file_processing/git.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/prompt_builders.py` & `mindflow-0.5.2/mindflow/core/prompt_builders.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/prompts.py` & `mindflow-0.5.2/mindflow/core/prompts.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/resolving/resolve.py` & `mindflow-0.5.2/mindflow/core/resolving/resolve.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/resolving/resolvers/file_resolver.py` & `mindflow-0.5.2/mindflow/core/resolving/resolvers/file_resolver.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/token_counting.py` & `mindflow-0.5.2/mindflow/core/token_counting.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/types/definitions/mind_flow_model.py` & `mindflow-0.5.2/mindflow/core/types/definitions/mind_flow_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,21 +63,7 @@
     MindFlowModelID.EMBEDDING.value: {
         MindFlowModelParameterKey.ID.value: MindFlowModelID.EMBEDDING.value,
         MindFlowModelParameterKey.NAME.value: MindFlowModelName.EMBEDDING.value,
         MindFlowModelParameterKey.DEFAULTS.value: MindFlowModelDefaults.EMBEDDING.value,
         MindFlowModelParameterKey.DESCRIPTION.value: MindFlowModelDescription.EMBEDDING.value,
     },
 }
-
-# MindFlowModelUnion = Union[
-#     MindFlowModelID,
-#     MindFlowModelDefaults,
-#     MindFlowModelName,
-#     MindFlowModelType,
-#     MindFlowModelDescription,
-# ]
-
-
-# def get_mind_flow_model_static(
-#     static: Type[MindFlowModelUnion], key: MindFlowModelUnion
-# ) -> MindFlowModelUnion:
-#     return static.__members__[key.name]
```

### Comparing `mindflow-0.5.1/mindflow/core/types/definitions/model.py` & `mindflow-0.5.2/mindflow/core/types/definitions/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,20 +278,7 @@
         ModelParameterKey.SOFT_TOKEN_LIMIT.value: ModelSoftTokenLimit.TEXT_EMBEDDING_ADA_002.value,
         ModelParameterKey.HARD_TOKEN_LIMIT.value: ModelHardTokenLimit.TEXT_EMBEDDING_ADA_002.value,
         ModelParameterKey.TOKEN_COST.value: ModelTokenCost.TEXT_EMBEDDING_ADA_002.value,
         ModelParameterKey.TOKEN_COST_UNIT.value: ModelTokenCostUnit.THOUSAND.value,
         ModelParameterKey.CONFIG_DESCRIPTION.value: ModelConfigDescription.TEXT_EMBEDDING_ADA_002.value,
     },
 }
-
-
-# ModelUnion = Union[
-#     ModelID,
-#     ModelParameterKey,
-#     ModelName,
-#     ModelHardTokenLimit,
-#     ModelDescription,
-# ]
-
-
-# def get_model_static(static: Type[ModelUnion], key: ModelUnion) -> ModelUnion:
-#     return static.__members__[key.name]
```

### Comparing `mindflow-0.5.1/mindflow/core/types/definitions/service.py` & `mindflow-0.5.2/mindflow/core/types/definitions/service.py`

 * *Files 13% similar despite different names*

```diff
@@ -114,23 +114,7 @@
     ServiceID.PINECONE.value: {
         ServiceParameterKey.ID.value: ServiceID.PINECONE.value,
         ServiceParameterKey.NAME.value: ServiceName.PINECONE.value,
         ServiceParameterKey.URL.value: ServiceURL.PINECONE.value,
         ServiceParameterKey.API_URL.value: ServiceURL.PINECONE.value,
     },
 }
-
-
-# ServiceUnion = Union[
-#     ServiceID,
-#     ServiceParameterKey,
-#     ServiceConfigParameterKey,
-#     ServiceName,
-#     ServiceURL,
-#     ServiceModel,
-#     ServiceModelTypeTextEmbedding,
-#     ServiceModelTypeTextCompletion,
-# ]
-
-
-# def get_service_static(static: Type[ServiceUnion], key: ServiceUnion) -> ServiceUnion:
-#     return static.__members__[key.name]
```

### Comparing `mindflow-0.5.1/mindflow/core/types/document.py` & `mindflow-0.5.2/mindflow/core/types/document.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/types/mindflow_model.py` & `mindflow-0.5.2/mindflow/core/types/mindflow_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import sys
-from typing import Dict
+from typing import Dict, Generic, TypeVar, cast
+from mindflow.core.types.definitions.model import ModelID
 from mindflow.core.types.store_traits.static import StaticStore
 from mindflow.core.types.store_traits.json import JsonStore
 
-from mindflow.core.types.model import ConfiguredModel
+from mindflow.core.types.model import (
+    ConfiguredModel,
+    ConfiguredOpenAIChatCompletionModel,
+    ConfiguredAnthropicChatCompletionModel,
+    ConfiguredOpenAITextEmbeddingModel,
+)
 from mindflow.core.types.service import ConfiguredServices
 from mindflow.core.types.definitions.mind_flow_model import MindFlowModelID
 from mindflow.core.types.definitions.service import (
     ServiceConfigParameterKey,
     ServiceID,
 )
 
@@ -20,19 +26,22 @@
 
 
 class MindFlowModelConfig(JsonStore):
     id: str
     model: str
 
 
-class ConfiguredMindFlowModel:
+T = TypeVar("T", bound="ConfiguredModel")
+
+
+class ConfiguredMindFlowModel(Generic[T]):
     id: str  # index, query, embedding
     name: str
     defaults: Dict[str, str]
-    model: ConfiguredModel
+    model: T
 
     def __init__(self, mindflow_model_id: str, configured_services: ConfiguredServices):
         self.id = mindflow_model_id
 
         if mind_flow_model := MindFlowModel.load(mindflow_model_id):
             for key, value in mind_flow_model.__dict__.items():
                 setattr(self, key, value)
@@ -40,15 +49,22 @@
         if (
             model_id := getattr(
                 MindFlowModelConfig.load(f"{mindflow_model_id}_config"), "model", None
             )
         ) is None:
             model_id = self.get_default_model_id(mindflow_model_id, configured_services)
 
-        self.model = ConfiguredModel(model_id)
+        if model_id in [ModelID.GPT_3_5_TURBO.value, ModelID.GPT_4.value]:
+            self.model = cast(T, ConfiguredOpenAIChatCompletionModel(model_id))
+        elif model_id in [ModelID.CLAUDE_INSTANT_V1.value, ModelID.CLAUDE_V1.value]:
+            self.model = cast(T, ConfiguredAnthropicChatCompletionModel(model_id))
+        elif model_id == ModelID.TEXT_EMBEDDING_ADA_002.value:
+            self.model = cast(T, ConfiguredOpenAITextEmbeddingModel(model_id))
+        else:
+            raise Exception("Unsupported model: " + model_id)
 
     def get_default_model_id(
         self, mindflow_model_id: str, configured_services: ConfiguredServices
     ) -> str:
         services = {
             ServiceID.OPENAI.value: configured_services.openai,
             ServiceID.ANTHROPIC.value: configured_services.anthropic,
```

### Comparing `mindflow-0.5.1/mindflow/core/types/model.py` & `mindflow-0.5.2/mindflow/core/types/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+from abc import ABC, abstractmethod
 import time
 from typing import Optional, Union
 
 import openai
 import anthropic
 
 import numpy as np
 from traitlets import Callable
-
-from mindflow.core.types.definitions.model_type import ModelType
-
 import tiktoken
 
 from mindflow.core.types.store_traits.json import JsonStore
 from mindflow.core.types.store_traits.static import StaticStore
 from mindflow.core.types.service import ServiceConfig
 from mindflow.core.types.definitions.model import ModelID
 from mindflow.core.types.definitions.service import ServiceID
@@ -36,15 +34,15 @@
 
 
 class ModelConfig(JsonStore):
     id: str
     soft_token_limit: int
 
 
-class ConfiguredModel(Callable):
+class ConfiguredModel(ABC, Callable):
     id: str
     name: str
     service: str
     model_type: str
 
     tokenizer: tiktoken.Encoding
 
@@ -76,15 +74,36 @@
                         ModelID.GPT_3_5_TURBO.value
                     )
                 else:
                     self.tokenizer = tiktoken.encoding_for_model(self.id)
         except NameError:
             pass
 
-    def openai_chat_completion(
+    @abstractmethod
+    def __call__(self, *args, **kwargs):
+        pass
+
+
+class ConfiguredOpenAIChatCompletionModel(ConfiguredModel):
+    id: str
+    name: str
+    service: str
+    model_type: str
+
+    tokenizer: tiktoken.Encoding
+
+    hard_token_limit: int
+    token_cost: int
+    token_cost_unit: str
+
+    # Config
+    soft_token_limit: int
+    api_key: str
+
+    def __call__(
         self,
         messages: list,
         temperature: float = 0.0,
         max_tokens: Optional[int] = None,
         stop: Optional[list] = None,
     ) -> Union[str, ModelError]:
         try_count = 0
@@ -102,15 +121,32 @@
             except Exception as e:
                 try_count += 1
                 error_message = f"Error: {str(e)}"
                 time.sleep(5)
 
         return ModelError(error_message)
 
-    def anthropic_chat_completion(
+
+class ConfiguredAnthropicChatCompletionModel(ConfiguredModel):
+    id: str
+    name: str
+    service: str
+    model_type: str
+
+    tokenizer: tiktoken.Encoding
+
+    hard_token_limit: int
+    token_cost: int
+    token_cost_unit: str
+
+    # Config
+    soft_token_limit: int
+    api_key: str
+
+    def __call__(
         self,
         prompt: str,
         temperature: float = 0.0,
         max_tokens: Optional[int] = 100,
     ) -> Union[str, ModelError]:
         try_count = 0
         error_message = ""
@@ -127,43 +163,39 @@
             except Exception as e:
                 try_count += 1
                 error_message = f"Error: {str(e)}"
                 time.sleep(5)
 
         return ModelError(error_message)
 
-    def openai_embedding(self, text: str) -> Union[np.ndarray, ModelError]:
+
+class ConfiguredOpenAITextEmbeddingModel(ConfiguredModel):
+    id: str
+    name: str
+    service: str
+    model_type: str
+
+    tokenizer: tiktoken.Encoding
+
+    hard_token_limit: int
+    token_cost: int
+    token_cost_unit: str
+
+    # Config
+    soft_token_limit: int
+    api_key: str
+
+    def __call__(self, text: str) -> Union[np.ndarray, ModelError]:
         try_count = 0
         error_message = ""
         while try_count < 5:
             try:
                 openai.api_key = self.api_key
                 return openai.Embedding.create(engine=self.id, input=text)["data"][0][
                     "embedding"
                 ]
             except Exception as e:
                 try_count += 1
                 error_message = f"Error: {str(e)}"
                 time.sleep(5)
 
         return ModelError(error_message)
-
-    def __call__(self, prompt, *args, **kwargs):
-        service_model_mapping = {
-            (
-                ServiceID.OPENAI.value,
-                ModelType.TEXT_COMPLETION.value,
-            ): self.openai_chat_completion,
-            (
-                ServiceID.OPENAI.value,
-                ModelType.TEXT_EMBEDDING.value,
-            ): self.openai_embedding,
-            (
-                ServiceID.ANTHROPIC.value,
-                ModelType.TEXT_COMPLETION.value,
-            ): self.anthropic_chat_completion,
-        }
-        if (
-            func := service_model_mapping.get((self.service, self.model_type))
-        ) is not None:
-            return func(prompt, *args, **kwargs)
-        raise NotImplementedError(f"Service {self.service} not implemented.")
```

### Comparing `mindflow-0.5.1/mindflow/core/types/service.py` & `mindflow-0.5.2/mindflow/core/types/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/types/store_traits/json.py` & `mindflow-0.5.2/mindflow/core/types/store_traits/json.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/types/store_traits/pinecone.py` & `mindflow-0.5.2/mindflow/core/types/store_traits/pinecone.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/core/types/store_traits/static.py` & `mindflow-0.5.2/mindflow/core/types/store_traits/static.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/unit_tests/dummy_diff.txt` & `mindflow-0.5.2/mindflow/unit_tests/dummy_diff.txt`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow/unit_tests/test_utils.py` & `mindflow-0.5.2/mindflow/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.1/mindflow.egg-info/PKG-INFO` & `mindflow-0.5.2/mindflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.1
+Version: 0.5.2
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.5.1/mindflow.egg-info/SOURCES.txt` & `mindflow-0.5.2/mindflow.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 mindflow/core/types/service.py
 mindflow/core/types/definitions/__init__.py
 mindflow/core/types/definitions/conversation.py
 mindflow/core/types/definitions/document.py
 mindflow/core/types/definitions/mind_flow_model.py
 mindflow/core/types/definitions/model.py
 mindflow/core/types/definitions/model_type.py
-mindflow/core/types/definitions/object.py
 mindflow/core/types/definitions/service.py
 mindflow/core/types/store_traits/__init__.py
 mindflow/core/types/store_traits/json.py
 mindflow/core/types/store_traits/pinecone.py
 mindflow/core/types/store_traits/static.py
 mindflow/unit_tests/dummy_diff.txt
 mindflow/unit_tests/test_cli.py
```

### Comparing `mindflow-0.5.1/setup.py` & `mindflow-0.5.2/setup.py`

 * *Files identical despite different names*

