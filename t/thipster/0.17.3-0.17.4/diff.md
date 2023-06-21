# Comparing `tmp/thipster-0.17.3.tar.gz` & `tmp/thipster-0.17.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.17.3.tar", last modified: Wed Jun 21 13:17:38 2023, max compression
+gzip compressed data, was "thipster-0.17.4.tar", last modified: Wed Jun 21 13:44:00 2023, max compression
```

## Comparing `thipster-0.17.3.tar` & `thipster-0.17.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.940759 thipster-0.17.3/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 13:17:34.000000 thipster-0.17.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-21 13:17:34.000000 thipster-0.17.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 13:17:38.940759 thipster-0.17.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-21 13:17:34.000000 thipster-0.17.3/README.md
--rw-r--r--   0 root         (0) root         (0)      995 2023-06-21 13:17:34.000000 thipster-0.17.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-21 13:17:34.000000 thipster-0.17.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:17:38.940759 thipster-0.17.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-21 13:17:35.000000 thipster-0.17.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.932759 thipster-0.17.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.932759 thipster-0.17.3/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     5390 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.932759 thipster-0.17.3/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.932759 thipster-0.17.3/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    15280 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    13619 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     4697 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3235 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4379 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/parser/test_yamlparser.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-06-21 13:17:34.000000 thipster-0.17.3/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.932759 thipster-0.17.3/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.936759 thipster-0.17.3/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.936759 thipster-0.17.3/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.936759 thipster-0.17.3/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.936759 thipster-0.17.3/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9180 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13507 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17026 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    20074 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6370 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.940759 thipster-0.17.3/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4669 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.940759 thipster-0.17.3/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20583 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-06-21 13:17:34.000000 thipster-0.17.3/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:17:38.932759 thipster-0.17.3/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 13:17:38.000000 thipster-0.17.3/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-21 13:17:38.000000 thipster-0.17.3/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:17:38.000000 thipster-0.17.3/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-21 13:17:38.000000 thipster-0.17.3/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-21 13:17:38.000000 thipster-0.17.3/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.502878 thipster-0.17.4/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 13:43:56.000000 thipster-0.17.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-21 13:43:56.000000 thipster-0.17.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 13:44:00.502878 thipster-0.17.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-21 13:43:56.000000 thipster-0.17.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      995 2023-06-21 13:43:56.000000 thipster-0.17.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-21 13:43:56.000000 thipster-0.17.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:44:00.502878 thipster-0.17.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-21 13:43:57.000000 thipster-0.17.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.490878 thipster-0.17.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.494878 thipster-0.17.4/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.494878 thipster-0.17.4/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.494878 thipster-0.17.4/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    15280 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    13619 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/parser/test_yamlparser.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-06-21 13:43:56.000000 thipster-0.17.4/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.494878 thipster-0.17.4/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.494878 thipster-0.17.4/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.498878 thipster-0.17.4/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.498878 thipster-0.17.4/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.498878 thipster-0.17.4/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9180 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13507 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17026 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    20074 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6370 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.498878 thipster-0.17.4/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.502878 thipster-0.17.4/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20630 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-06-21 13:43:56.000000 thipster-0.17.4/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:44:00.494878 thipster-0.17.4/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 13:44:00.000000 thipster-0.17.4/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-21 13:44:00.000000 thipster-0.17.4/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:44:00.000000 thipster-0.17.4/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-21 13:44:00.000000 thipster-0.17.4/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-21 13:44:00.000000 thipster-0.17.4/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.17.3/LICENSE` & `thipster-0.17.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/PKG-INFO` & `thipster-0.17.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.3
+Version: 0.17.4
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.3 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.4 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.3/README.md` & `thipster-0.17.4/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/pyproject.toml` & `thipster-0.17.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/setup.py` & `thipster-0.17.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.17.3'
+__version__ = '0.17.4'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.17.3/tests/engine/test_engine.py` & `thipster-0.17.4/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/engine/test_generation.py` & `thipster-0.17.4/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/dsl_parser/test_ast.py` & `thipster-0.17.4/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.17.4/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.17.4/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/dsl_parser/test_token.py` & `thipster-0.17.4/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.17.4/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/test_parsedfile.py` & `thipster-0.17.4/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/test_parserfactory.py` & `thipster-0.17.4/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/parser/test_yamlparser.py` & `thipster-0.17.4/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/test_e2e.py` & `thipster-0.17.4/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/tests/test_tools.py` & `thipster-0.17.4/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/auth/google.py` & `thipster-0.17.4/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/engine/engine.py` & `thipster-0.17.4/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/engine/i_parser.py` & `thipster-0.17.4/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/engine/i_repository.py` & `thipster-0.17.4/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/engine/i_terraform.py` & `thipster-0.17.4/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/engine/parsed_file.py` & `thipster-0.17.4/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/engine/resource_model.py` & `thipster-0.17.4/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/helpers.py` & `thipster-0.17.4/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/ast.py` & `thipster-0.17.4/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.17.4/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.17.4/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/lexer.py` & `thipster-0.17.4/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.17.4/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/parser.py` & `thipster-0.17.4/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/token.py` & `thipster-0.17.4/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.17.4/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/exceptions.py` & `thipster-0.17.4/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/parser_factory.py` & `thipster-0.17.4/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/parser/yaml_parser.py` & `thipster-0.17.4/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/repository/github.py` & `thipster-0.17.4/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/repository/json.py` & `thipster-0.17.4/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster/terraform/cdk.py` & `thipster-0.17.4/thipster/terraform/cdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 import thipster.terraform.exceptions as cdk_exceptions
 from thipster.engine import AuthPort, TerraformPort
 from thipster.helpers import create_logger
 
 
-class ResourceCreationContext():
+class ResourceCreationContext:
     def __init__(
         self,
         stack_self: TerraformStack,
         resource_name: str | None = None,
         resource_type: str | None = None,
         resource_class: type | None = None,
         parent_name: str | None = None,
@@ -288,17 +288,19 @@
         else:
             attributes[a.name] = rm.ModelAttribute(
                 cdk_name=a.name,
                 default=rm.ModelLiteral(a.value),
             )
 
     # Checks that all attributes have a default value
-    if ctx.no_modif and not all(x.default is not None for x in attributes.values()):
+    if ctx.no_modif and not all(
+        x.optional or (x.default is not None) for x in attributes.values()
+    ):
         missing_atributes = [
-            k for k, v in attributes.items() if v.default is None
+            k for k, v in attributes.items() if not v.optional and v.default is None
         ]
 
         raise cdk_exceptions.CDKMissingAttributeInDependencyError(
             ctx.resource_type,
             missing_atributes,
         )
```

### Comparing `thipster-0.17.3/thipster/terraform/exceptions.py` & `thipster-0.17.4/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.3/thipster.egg-info/PKG-INFO` & `thipster-0.17.4/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.3
+Version: 0.17.4
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.17.3 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.4 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.3/thipster.egg-info/SOURCES.txt` & `thipster-0.17.4/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

