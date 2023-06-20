# Comparing `tmp/circlecigen-0.0.5.tar.gz` & `tmp/circlecigen-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circlecigen-0.0.5.tar", last modified: Tue Jun 20 04:07:01 2023, max compression
+gzip compressed data, was "circlecigen-0.0.6.tar", last modified: Tue Jun 20 22:32:03 2023, max compression
```

## Comparing `circlecigen-0.0.5.tar` & `circlecigen-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.712526 circlecigen-0.0.5/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3975 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.codeclimate.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-20 04:06:42.000000 circlecigen-0.0.5/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-20 04:06:42.000000 circlecigen-0.0.5/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22357 2023-06-20 04:07:01.712526 circlecigen-0.0.5/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-20 04:06:42.000000 circlecigen-0.0.5/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21721 2023-06-20 04:06:42.000000 circlecigen-0.0.5/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:06:42.000000 circlecigen-0.0.5/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/circlecigen.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22357 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-20 04:07:01.000000 circlecigen-0.0.5/circlecigen.egg-info/top_level.txt
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/env_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/default.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/dev.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/multi.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/nonprod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/post-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/pre-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-20 04:06:42.000000 circlecigen-0.0.5/env_test/prod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-20 04:06:42.000000 circlecigen-0.0.5/notes.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-20 04:06:42.000000 circlecigen-0.0.5/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-20 04:06:42.000000 circlecigen-0.0.5/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-20 04:06:42.000000 circlecigen-0.0.5/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-20 04:07:01.712526 circlecigen-0.0.5/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      760 2023-06-20 04:06:42.000000 circlecigen-0.0.5/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.708527 circlecigen-0.0.5/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-20 04:07:01.000000 circlecigen-0.0.5/src/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5805 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-20 04:06:42.000000 circlecigen-0.0.5/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 04:07:01.712526 circlecigen-0.0.5/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/generated_config_setup.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2266 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-20 04:06:42.000000 circlecigen-0.0.5/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.161690 circlecigen-0.0.6/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3975 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.codeclimate.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-20 22:31:57.000000 circlecigen-0.0.6/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-20 22:31:57.000000 circlecigen-0.0.6/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-20 22:32:03.165690 circlecigen-0.0.6/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-20 22:31:57.000000 circlecigen-0.0.6/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21721 2023-06-20 22:31:57.000000 circlecigen-0.0.6/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:31:57.000000 circlecigen-0.0.6/__init__.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.161690 circlecigen-0.0.6/circlecigen.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-20 22:32:03.000000 circlecigen-0.0.6/circlecigen.egg-info/top_level.txt
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/env_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/default.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/dev.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/multi.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/nonprod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-20 22:31:57.000000 circlecigen-0.0.6/env_test/prod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-20 22:31:57.000000 circlecigen-0.0.6/notes.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-20 22:31:57.000000 circlecigen-0.0.6/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-20 22:31:57.000000 circlecigen-0.0.6/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-20 22:31:57.000000 circlecigen-0.0.6/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-20 22:32:03.165690 circlecigen-0.0.6/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-20 22:31:57.000000 circlecigen-0.0.6/setup.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-20 22:32:03.000000 circlecigen-0.0.6/src/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5805 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-20 22:31:57.000000 circlecigen-0.0.6/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 22:32:03.165690 circlecigen-0.0.6/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5543 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/generated_config_setup.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2266 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-20 22:31:57.000000 circlecigen-0.0.6/test/test_utils.py
```

### Comparing `circlecigen-0.0.5/.circleci/config.yml` & `circlecigen-0.0.6/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/.pre-commit-config.yaml` & `circlecigen-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/.pylintrc` & `circlecigen-0.0.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/LICENSE` & `circlecigen-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/PKG-INFO` & `circlecigen-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.5
+Version: 0.0.6
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.5 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.6 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
```

### Comparing `circlecigen-0.0.5/README.md` & `circlecigen-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/circlecigen.egg-info/PKG-INFO` & `circlecigen-0.0.6/circlecigen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.5
+Version: 0.0.6
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.5 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.6 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
```

### Comparing `circlecigen-0.0.5/circlecigen.egg-info/SOURCES.txt` & `circlecigen-0.0.6/circlecigen.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 requirements.txt
 setup.py
 .circleci/config.yml
 circlecigen.egg-info/PKG-INFO
 circlecigen.egg-info/SOURCES.txt
 circlecigen.egg-info/dependency_links.txt
 circlecigen.egg-info/entry_points.txt
+circlecigen.egg-info/requires.txt
 circlecigen.egg-info/top_level.txt
 env_test/config.yml
 env_test/default.json
 env_test/dev.json
 env_test/generated_config.yml
 env_test/multi.json
 env_test/nonprod-us-east-2.tfvars.json
```

### Comparing `circlecigen-0.0.5/env_test/config.yml` & `circlecigen-0.0.6/env_test/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/env_test/generated_config.yml` & `circlecigen-0.0.6/env_test/generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/env_test/multi.json` & `circlecigen-0.0.6/env_test/multi.json`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/env_test/post-approve.yml` & `circlecigen-0.0.6/env_test/post-approve.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/pyproject.toml` & `circlecigen-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/setup.py` & `circlecigen-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,13 +13,18 @@
     url="https://github.com/ThoughtWorks-DPS/circlecigen",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     packages=setuptools.find_packages(),
     include_package_data=True,
-    python_requires=">=3.10",
+    install_requires=[
+        "click",
+        "pathvalidate",
+        "jinja2"
+    ],
+    python_requires=">=3.7",
     entry_points='''
         [console_scripts]
         circlecigen=src.circlecigen:cli
     '''
 )
```

### Comparing `circlecigen-0.0.5/src/circlecigen.py` & `circlecigen-0.0.6/src/circlecigen.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/src/template.py` & `circlecigen-0.0.6/src/template.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/src/tfvars.py` & `circlecigen-0.0.6/src/tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/src/utils.py` & `circlecigen-0.0.6/src/utils.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/test/generated_config.yml` & `circlecigen-0.0.6/test/generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/test/generated_config_setup.yml` & `circlecigen-0.0.6/test/generated_config_setup.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/test/test_circlecigen.py` & `circlecigen-0.0.6/test/test_circlecigen.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/test/test_template.py` & `circlecigen-0.0.6/test/test_template.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/test/test_tfvars.py` & `circlecigen-0.0.6/test/test_tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.5/test/test_utils.py` & `circlecigen-0.0.6/test/test_utils.py`

 * *Files identical despite different names*

